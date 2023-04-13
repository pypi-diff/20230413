# Comparing `tmp/simepy-0.1.0.tar.gz` & `tmp/simepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simepy-0.1.0.tar", max compression
+gzip compressed data, was "simepy-0.2.0.tar", max compression
```

## Comparing `simepy-0.1.0.tar` & `simepy-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      866 2023-04-11 13:37:56.489001 simepy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-11 13:37:56.489001 simepy-0.1.0/simepy/__init__.py
--rw-r--r--   0        0        0    24244 2023-04-11 13:37:56.489001 simepy-0.1.0/simepy/extract_meta_data.py
--rw-r--r--   0        0        0     1133 2023-04-11 13:37:56.489001 simepy-0.1.0/simepy/extract_scans.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 simepy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-04-13 20:25:23.860283 simepy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-13 20:25:23.860283 simepy-0.2.0/simepy/__init__.py
+-rw-r--r--   0        0        0    23675 2023-04-13 20:25:01.919963 simepy-0.2.0/simepy/extract_meta_data.py
+-rw-r--r--   0        0        0     1098 2023-04-13 20:25:01.919963 simepy-0.2.0/simepy/extract_scans.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 simepy-0.2.0/PKG-INFO
```

### Comparing `simepy-0.1.0/pyproject.toml` & `simepy-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "simepy"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Gavain Sweetman, Manuel Kösters, Artyom Vlasov, Tristan Ranff, Christian Fufezan"]
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pymzml = "2.5.2"
 pydantic = "^1.10.7"
 pandas = "^1.5.3"
```

### Comparing `simepy-0.1.0/simepy/extract_meta_data.py` & `simepy-0.2.0/simepy/extract_meta_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Spectrum Meta Data resource."""
-import argparse
-import csv
 import logging
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Optional
 
+import pandas as pd
 import pymzml
 from dateutil import parser as dparser
 from pydantic import BaseModel, Field
 
 try:
     import czxcalibur
 
@@ -493,37 +492,32 @@
         raise ModuleNotFoundError
     else:
         return extract_function(input_file, object_name, lineage_root, time_format)
 
 
 def extract_meta_data(
     input_file,
-    run_output_file,
-    spec_output_file,
-    noise_output_file,
-    unit_output_file,
     time_format="%Y-%m-%d %H:%M:%S",
     object_name=None,
     lineage_root=None,
 ):
     """
     Extract Run and Spectrum metadata from MS data.
 
     Args:
         input_file (PosixPath/str): path to ms data input file (mzml|raw|mgf)
-        run_output_file (PosixPath/str): path to run metadata output_file
-        spec_output_file (PosixPath/str): path to spectrum metadata output_file
-        noise_output_file (PosixPath/str): path to spectrum noise output_file
-        units_output_file (PosixPath/str): path to instrument units output_file
         time_format (str): string defining the time_format to format into
         object_name (str/NoneType): string to be used as file identifier
         lineage_root (str/NoneType): name of the root file associated to the one, from which metadata is queried
 
     Returns:
-        None
+        rmd_df (pandas.DataFrame): df containing run metadata
+        imu_df (pandas.DataFrame): df containing instrument unit info
+        smd_df (pandas.DataFrame): df containing spectrum metadata
+        sn_df (pandas.DataFrame): df containing spectrum noise info
     """
     if isinstance(input_file, str):
         input_file = Path(input_file)
 
     if object_name is None:
         object_name = Path(input_file).resolve().name
 
@@ -531,80 +525,86 @@
         lineage_root = Path(input_file).resolve().name
 
     file_type = "".join(Path(input_file).suffixes).lower()[1:]
     logging.info(
         f"Identified file type is '{file_type}'. Proceeding with metadata extraction..."
     )
     # 1. RunInfoMetaData
-    fieldnames = [x for x in RunInfoMetaData.schema()["properties"].keys()]
-    with open(run_output_file, "w") as fobj:
-        writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-        writer.writeheader()
-        for meta_data_line in extract_data(
+    rmd_rows = []
+    for meta_data_line in extract_data(
+        input_file,
+        object_name,
+        lineage_root,
+        file_type,
+        time_format,
+        mode="run_metadata",
+    ):
+        rmd_rows.append(
+            pd.DataFrame(meta_data_line.dict(exclude_unset=True), index=[0])
+        )
+    rmd_df = pd.concat(rmd_rows, ignore_index=True)
+    logging.info("Finished run metadata info extraction!")
+
+    # 2. InstrumentUnit
+    gex_lookup = {}
+    if input_file.suffix.lower() == ".raw":
+        imu_rows = []
+        for unit_data_line in extract_data(
             input_file,
             object_name,
             lineage_root,
             file_type,
             time_format,
-            mode="run_metadata",
+            mode="instrument_unit",
         ):
-            writer.writerow(meta_data_line.dict())
+            imu_rows.append(
+                pd.DataFrame(unit_data_line.dict(exclude_unset=True), index=[0])
+            )
+            gex_lookup[unit_data_line.faims_cv] = unit_data_line.gex_id
+        imu_df = pd.concat(imu_rows, ignore_index=True)
+        logging.info("Finished instrument unit info extraction!")
 
-    # 2. InstrumentUnit
-    gex_lookup = {}
-    if input_file.suffix.lower() == ".raw" and unit_output_file is not None:
-        fieldnames = [x for x in InstrumentMetaUnit.schema()["properties"].keys()]
-        with open(unit_output_file, "w") as fobj:
-            writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-            writer.writeheader()
-            for unit_data_line in extract_data(
-                input_file,
-                object_name,
-                lineage_root,
-                file_type,
-                time_format,
-                mode="instrument_unit",
-            ):
-                writer.writerow(unit_data_line.dict())
-                gex_lookup[unit_data_line.faims_cv] = unit_data_line.gex_id
     elif "".join(input_file.suffixes).lower() in [".mzml", ".mzml.gz"]:
-        fieldnames = [x for x in InstrumentMetaUnit.schema()["properties"].keys()]
-        with open(unit_output_file, "w") as fobj:
-            writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-            writer.writeheader()
+        imu_df = pd.DataFrame(
+            [], columns=[x for x in InstrumentMetaUnit.schema()["properties"].keys()]
+        )
 
     # 3. SpectrumMetaData
-    fieldnames = [x for x in SpectrumMetaData.schema()["properties"].keys()]
-    with open(spec_output_file, "w") as fobj:
-        writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-        writer.writeheader()
-        for meta_data_line in extract_data(
+    smd_rows = []
+    for meta_data_line in extract_data(
+        input_file,
+        object_name,
+        lineage_root,
+        file_type,
+        time_format,
+        mode="spectrum_metadata",
+        gex_lookup=gex_lookup,
+    ):
+        smd_rows.append(
+            pd.DataFrame(meta_data_line.dict(exclude_unset=True), index=[0])
+        )
+    smd_df = pd.concat(smd_rows, ignore_index=True)
+    logging.info("Finished spectrum metadata info extraction!")
+
+    # 4. SpectrumNoise
+    if input_file.suffix.lower() == ".raw":
+        sn_rows = []
+        for noise_data_line in extract_data(
             input_file,
             object_name,
             lineage_root,
             file_type,
             time_format,
-            mode="spectrum_metadata",
-            gex_lookup=gex_lookup,
+            mode="run_noise",
         ):
-            writer.writerow(meta_data_line.dict())
+            sn_rows.append(
+                pd.DataFrame(noise_data_line.dict(exclude_unset=True), index=[0])
+            )
+        sn_df = pd.concat(sn_rows, ignore_index=True)
+        logging.info("Finished spectrum noise extraction!")
 
-    # 4. SpectrumNoise
-    if input_file.suffix.lower() == ".raw":
-        fieldnames = [x for x in SpectrumNoise.schema()["properties"].keys()]
-        with open(noise_output_file, "w") as fobj:
-            writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-            writer.writeheader()
-            for noise_data_line in extract_data(
-                input_file,
-                object_name,
-                lineage_root,
-                file_type,
-                time_format,
-                mode="run_noise",
-            ):
-                writer.writerow(noise_data_line.dict())
     elif "".join(input_file.suffixes).lower() in [".mzml", ".mzml.gz"]:
-        fieldnames = [x for x in SpectrumNoise.schema()["properties"].keys()]
-        with open(noise_output_file, "w") as fobj:
-            writer = csv.DictWriter(fobj, fieldnames=fieldnames)
-            writer.writeheader()
+        sn_df = pd.DataFrame(
+            [], columns=[x for x in SpectrumNoise.schema()["properties"].keys()]
+        )
+
+    return rmd_df, imu_df, smd_df, sn_df
```

### Comparing `simepy-0.1.0/simepy/extract_scans.py` & `simepy-0.2.0/simepy/extract_scans.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 import logging
 from pathlib import Path
 
 import pandas as pd
 import pymzml
 
 
-def extract_scan_data(input_file, output_file):
+def extract_scan_data(input_file):
     """
     Extract scan info like mass, intensity, id and filename from an input mzml file.
 
     Args:
         input_file (PosixPath): path to input file
-        output_file (PosixPath): path to scans output file
 
     Returns:
-        None
+        scans_out (pandas.DataFrame): Dataframe containing scans information
     """
     logging.info("Starting scan info extraction!")
     with pymzml.run.Reader(str(input_file)) as reader:
         scans = []
         for spectrum in reader:
             scans_df = pd.DataFrame()
             scans_df["mz"] = spectrum.get_array("m/z array")
             scans_df["intensity"] = spectrum.get_array("intensity array")
             scans_df["spectrum_id"] = spectrum.ID
             scans_df["retention_time_seconds"] = spectrum.scan_time_in_minutes() * 60.0
             scans_df["filename"] = Path(input_file).resolve().name
             scans.append(scans_df)
 
     scans_out = pd.concat(scans)
-    scans_out.to_csv(output_file, index=False)
-
     logging.info("Scans info extraction completed!")
+    return scans_out
```

### Comparing `simepy-0.1.0/PKG-INFO` & `simepy-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simepy
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Gavain Sweetman, Manuel Kösters, Artyom Vlasov, Tristan Ranff, Christian Fufezan
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

