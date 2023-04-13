# Comparing `tmp/plink_pipelines-0.1.5a0.tar.gz` & `tmp/plink_pipelines-0.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plink_pipelines-0.1.5a0.tar", max compression
+gzip compressed data, was "plink_pipelines-0.1.6a0.tar", max compression
```

## Comparing `plink_pipelines-0.1.5a0.tar` & `plink_pipelines-0.1.6a0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    34523 2021-06-10 12:58:24.376189 plink_pipelines-0.1.5a0/LICENSE
--rw-r--r--   0        0        0        0 2021-06-10 12:58:24.383042 plink_pipelines-0.1.5a0/plink_pipelines/__init__.py
--rw-r--r--   0        0        0    14616 2023-02-06 07:27:50.346566 plink_pipelines-0.1.5a0/plink_pipelines/make_dataset.py
--rw-r--r--   0        0        0      418 2021-06-10 12:58:24.382729 plink_pipelines-0.1.5a0/plink_pipelines/validation_functions.py
--rw-r--r--   0        0        0      846 2023-02-06 07:32:59.381686 plink_pipelines-0.1.5a0/pyproject.toml
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 plink_pipelines-0.1.5a0/setup.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plink_pipelines-0.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/__init__.py
+-rw-r--r--   0        0        0    15580 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/make_dataset.py
+-rw-r--r--   0        0        0      417 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/validation_functions.py
+-rw-r--r--   0        0        0      845 2023-04-13 15:40:12.495581 plink_pipelines-0.1.6a0/pyproject.toml
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plink_pipelines-0.1.6a0/PKG-INFO
```

### Comparing `plink_pipelines-0.1.5a0/LICENSE` & `plink_pipelines-0.1.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `plink_pipelines-0.1.5a0/plink_pipelines/make_dataset.py` & `plink_pipelines-0.1.6a0/plink_pipelines/make_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import subprocess
 import warnings
 from pathlib import Path
-from shutil import copyfile, rmtree
+from shutil import copyfile, rmtree, which
 from typing import Generator, Tuple, Literal, Optional, Sequence
 
 import deeplake
 import luigi
 import numpy as np
 import torch
 from torch.nn.functional import one_hot
@@ -129,14 +129,16 @@
 
     def requires(self):
         if self.extract_snp_file:
             return self.clone(PlinkExtractAlleles)
         return self.clone(ExternalRawData)
 
     def run(self):
+        _validate_plink_exists_in_path()
+
         input_path = Path(self.input().path)
         output_path = Path(self.output().path)
         ensure_path_exists(output_path)
 
         plink_input = input_path.parent / input_path.stem
         plink_output = output_path.parent / output_path.stem
         cmd = [
@@ -162,25 +164,34 @@
 
         if self.autosome_only:
             cmd += ["--autosome"]
 
         subprocess.call(cmd)
 
 
+def _validate_plink_exists_in_path():
+    if which("plink") is None:
+        raise RuntimeError(
+            "plink is not installed or is not in the path. "
+            "Please install plink and try again."
+        )
+
+
 @inherits(ExternalRawData, PlinkExtractAlleles, PlinkQC)
 class OneHotSNPs(Config):
     """
     Generates one hot encodings from a individuals x SNPs file.
     """
 
     output_folder = luigi.Parameter()
     output_format = luigi.Parameter()
     output_name = luigi.Parameter()
     qc = luigi.BoolParameter()
     extract_snp_file = luigi.Parameter()
+    array_chunk_size = luigi.IntParameter()
     file_name = "processed/encoded_outputs"
 
     def requires(self):
         """
         Here we can return any of:
 
             - [raw.bed]             # no QC, no extract
@@ -203,15 +214,15 @@
         input_path = Path(self.input()[-1].path)
         assert input_path.suffix == ".bed"
 
         output_path = Path(self.output().path)
         ensure_path_exists(output_path, is_folder=True)
 
         chunk_generator = get_sample_generator_from_bed(
-            bed_path=input_path, chunk_size=1000
+            bed_path=input_path, chunk_size=int(self.array_chunk_size)
         )
         sample_id_one_hot_array_generator = _get_one_hot_encoded_generator(
             chunked_sample_generator=chunk_generator
         )
 
         write_one_hot_outputs(
             id_array_generator=sample_id_one_hot_array_generator,
@@ -223,15 +234,14 @@
 
 def write_one_hot_outputs(
     id_array_generator: Generator[Tuple[str, np.ndarray], None, None],
     output_folder: Path,
     output_format: Literal["disk", "deeplake"],
     output_name: Optional[str] = None,
 ) -> None:
-
     if output_format == "disk":
         _write_one_hot_arrays_to_disk(
             id_array_generator=id_array_generator, output_folder=output_folder
         )
     elif output_format == "deeplake":
         assert output_name is not None
         _write_one_hot_arrays_to_deeplake_ds(
@@ -271,15 +281,14 @@
             sample = {"ID": id_, output_name: array}
             ds.append(sample)
 
 
 def _get_one_hot_encoded_generator(
     chunked_sample_generator: Generator[Tuple[Sequence[str], np.ndarray], None, None]
 ) -> Generator[Tuple[str, np.ndarray], None, None]:
-
     for id_chunk, array_chunk in chunked_sample_generator:
         array_tensor = torch.from_numpy(array_chunk).to(dtype=torch.long)
         one_hot_encoded = one_hot(array_tensor, num_classes=4)
 
         # convert (n_samples, n_snps, 4) -> (n_samples, 4, n_snps)
         one_hot_encoded = one_hot_encoded.transpose(2, 1)
         one_hot_encoded = one_hot_encoded.numpy().astype(np.int8)
@@ -299,30 +308,33 @@
     (which should be individuals), it actually indexes SNPs. So we need to
     explicitly index both dimensions.
     """
     with open_bed(bed_path) as bed_handle:
         n_samples = bed_handle.iid_count
 
         for index in range(0, n_samples, chunk_size):
-            ids = bed_handle.iid[index : index + chunk_size]
+            samples_idx_start = index
+            samples_idx_end = index + chunk_size
+            ids = bed_handle.iid[samples_idx_start:samples_idx_end]
             arrays = bed_handle.read(
-                index=np.s_[index : index + chunk_size, :],
+                index=np.s_[samples_idx_start:samples_idx_end, :],
                 dtype=np.int8,
             )
             arrays[arrays == -127] = 3  # NA is encoded as -127
             yield ids, arrays
             logger.info("Processed %s samples.", index + chunk_size)
 
 
 @inherits(OneHotSNPs)
 class FinalizeParsing(luigi.Task):
     output_folder = luigi.Parameter()
     output_format = luigi.Parameter()
     output_name = luigi.Parameter()
     qc = luigi.BoolParameter()
+    array_chunk_size = luigi.IntParameter()
     extract_snp_file = luigi.Parameter()
 
     def requires(self):
         base = [self.clone(OneHotSNPs)]
 
         last_plink_task = [self.clone(ExternalRawData)]
         if self.extract_snp_file:
@@ -353,19 +365,19 @@
         )
         one_hot_outputs = self.input()
         return [luigi.LocalTarget(str(output_path)), one_hot_outputs]
 
 
 @requires(FinalizeParsing)
 class CleanupIntermediateTaskOutputs(luigi.Task):
-
     raw_data_path = luigi.Parameter()
     output_folder = luigi.Parameter()
     output_format = luigi.Parameter()
     qc = luigi.BoolParameter()
+    array_chunk_size = luigi.IntParameter()
     indiv_sample_size = luigi.IntParameter()
     chr_sample = luigi.Parameter()
     autosome_only = luigi.BoolParameter()
     extract_snp_file = luigi.Parameter()
 
     @property
     def interim_folder(self):
@@ -402,15 +414,15 @@
 
     config = luigi.DictParameter()
 
     def requires(self):
         yield CleanupIntermediateTaskOutputs(**self.config)
 
 
-def get_cl_args():
+def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--raw_data_path",
         type=str,
         default="",
         help="Path to raw data folder to be processed (containing data.bed, data.fam, "
         "data.bim)",
@@ -446,40 +458,57 @@
     )
     parser.add_argument(
         "--no_qc", dest="qc", action="store_false", help="Skip QC on plink data."
     )
     parser.set_defaults(qc=False)
 
     parser.add_argument(
+        "--array_chunk_size",
+        type=int,
+        default=1000,
+        help="How many individuals to process at a time. "
+        "Useful to avoid running out of memory.",
+    )
+
+    parser.add_argument(
         "--indiv_sample_size",
         type=int,
         default=None,
-        help="How many individuals to randomly sample.",
+        help="How many individuals to randomly sample."
+        " Only applicable if do_qc is set.",
     )
 
     parser.add_argument(
         "--chr_sample",
         type=str,
         default="",
-        help="Which chromosomes to sample, follows plink notation.",
+        help="Which chromosomes to sample, follows plink notation."
+        " Only applicable if do_qc is set.",
     )
 
     parser.add_argument(
-        "--autosome_only", action="store_true", help="Whether to only use autosomes."
+        "--autosome_only",
+        action="store_true",
+        help="Whether to only use autosomes. " "Only applicable if do_qc is set.",
     )
 
     parser.add_argument(
         "--extract_snp_file",
         type=str,
         default=None,
         help=".bim file to use if generating only the "
         "intersection between the data and the "
         "specified .bim file.",
     )
 
+    return parser
+
+
+def get_cl_args():
+    parser = get_parser()
     cl_args = parser.parse_args()
     validate_cl_args(cl_args)
 
     return cl_args
 
 
 def main():
```

### Comparing `plink_pipelines-0.1.5a0/pyproject.toml` & `plink_pipelines-0.1.6a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plink_pipelines"
-version = "0.1.5-alpha"
+version = "0.1.6-alpha"
 description = ""
 authors = ["Arnor Sigurdsson <arnor-sigurdsson@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.2.4"
 py = "^1.10.0"
@@ -27,12 +27,12 @@
 Sphinx = "^4.0.2"
 coverage = "^6.1.1"
 snakeviz = "^2.1.0"
 pytest-cov = "^3.0.0"
 pynvim = "^0.4.3"
 visidata = "^2.4"
 pre-commit = "^2.13.0"
-black = "^22.12.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plink_pipelines-0.1.5a0/PKG-INFO` & `plink_pipelines-0.1.6a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plink-pipelines
-Version: 0.1.5a0
+Version: 0.1.6a0
 Summary: 
 Author: Arnor Sigurdsson
 Author-email: arnor-sigurdsson@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

