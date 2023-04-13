# Comparing `tmp/triqler-0.7.0-py3-none-any.whl.zip` & `tmp/triqler-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 62571 bytes, number of entries: 28
+Zip file size: 62937 bytes, number of entries: 28
 -rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 triqler/__init__.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 triqler/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 triqler/convert/__init__.py
--rw-r--r--  2.0 unx     2041 b- defN 80-Jan-01 00:00 triqler/convert/diann.py
+-rw-r--r--  2.0 unx     3406 b- defN 80-Jan-01 00:00 triqler/convert/diann.py
 -rw-r--r--  2.0 unx     6505 b- defN 80-Jan-01 00:00 triqler/convert/dinosaur.py
 -rw-r--r--  2.0 unx     6022 b- defN 80-Jan-01 00:00 triqler/convert/helpers.py
 -rw-r--r--  2.0 unx     6372 b- defN 80-Jan-01 00:00 triqler/convert/maxquant.py
 -rw-r--r--  2.0 unx     5245 b- defN 80-Jan-01 00:00 triqler/convert/normalize_intensities.py
 -rwxr-xr-x  2.0 unx     2902 b- defN 80-Jan-01 00:00 triqler/convert/percolator.py
 -rw-r--r--  2.0 unx     6447 b- defN 80-Jan-01 00:00 triqler/convert/quandenser.py
 -rw-r--r--  2.0 unx     1127 b- defN 80-Jan-01 00:00 triqler/convolution_dp.py
@@ -18,13 +18,13 @@
 -rw-r--r--  2.0 unx    17329 b- defN 80-Jan-01 00:00 triqler/hyperparameters.py
 -rw-r--r--  2.0 unx     1735 b- defN 80-Jan-01 00:00 triqler/multiprocessing_pool.py
 -rw-r--r--  2.0 unx    11469 b- defN 80-Jan-01 00:00 triqler/parsers.py
 -rwxr-xr-x  2.0 unx     9551 b- defN 80-Jan-01 00:00 triqler/pgm.py
 -rw-r--r--  2.0 unx    16130 b- defN 80-Jan-01 00:00 triqler/qvality.py
 -rw-r--r--  2.0 unx    23827 b- defN 80-Jan-01 00:00 triqler/triqler.py
 -rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 triqler/version.py
-?rw-r--r--  2.0 unx      368 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 triqler-0.7.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    10942 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     2279 b- defN 16-Jan-01 00:00 triqler-0.7.0.dist-info/RECORD
-28 files, 195836 bytes uncompressed, 58937 bytes compressed:  69.9%
+?rw-r--r--  2.0 unx      368 b- defN 16-Jan-01 00:00 triqler-0.7.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 triqler-0.7.1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 triqler-0.7.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    10942 b- defN 16-Jan-01 00:00 triqler-0.7.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     2279 b- defN 16-Jan-01 00:00 triqler-0.7.1.dist-info/RECORD
+28 files, 197201 bytes uncompressed, 59303 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: triqler/triqler.py
 Comment: 
 
 Filename: triqler/version.py
 Comment: 
 
-Filename: triqler-0.7.0.dist-info/entry_points.txt
+Filename: triqler-0.7.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: triqler-0.7.0.dist-info/LICENSE
+Filename: triqler-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: triqler-0.7.0.dist-info/WHEEL
+Filename: triqler-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: triqler-0.7.0.dist-info/METADATA
+Filename: triqler-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: triqler-0.7.0.dist-info/RECORD
+Filename: triqler-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## triqler/convert/diann.py

```diff
@@ -7,63 +7,94 @@
 import glob
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 
 from ..triqler import __version__, __copyright__
+from .. import parsers
 
 
 def main():
   print('triqler.convert.diann version %s\n%s' % (__version__, __copyright__))
   print('Issued command:', os.path.basename(__file__) + " " + " ".join(map(str, sys.argv[1:])))
   
   args, params = parseArgs()
   
   # hack for windows
   if len(args.in_file) == 1 and '*' in args.in_file[0]:
     args.in_file = glob.glob(args.in_file[0])
   
-  diann_to_triqler(args.in_file, args.out_file, params)
+  diann_to_triqler(args.in_file, args.file_list_file, args.out_file, params)
 
 
 def parseArgs():
   import argparse
   apars = argparse.ArgumentParser(
       description='Converts DIA-NN output files to Triqler input format.',
       formatter_class=argparse.ArgumentDefaultsHelpFormatter)
   
+  requiredNamed = apars.add_argument_group('required arguments')
+  
   apars.add_argument('in_file', default=None, metavar = "IN_FILE",
                      help='''DIA-NN output file
                           ''')
   
+  requiredNamed.add_argument('--file_list_file', metavar='L', 
+                     help='''Simple tab separated file with run names in first column and condition in second column. 
+                             The run names should be identical to the entries in the "Run" column of the DIA-NN output file.
+                             ''',
+                     required = True)
+
   apars.add_argument('--out_file', default = "triqler_input.tsv", metavar='OUT', 
                      help='''Path to triqler input file (writing in TSV format).
                           ''')
   
   # ------------------------------------------------
   args = apars.parse_args()
   
   params = dict()
   return args, params
 
 
-def diann_to_triqler(diann_file_path: str, triqler_input_file: str, params: Dict):
-  df = pd.read_csv(diann_file_path, sep='\t')
+def diann_to_triqler(diann_file_path: str, file_list_file: str, triqler_input_file: str, params: Dict):
+  file_list_df = parse_file_list(file_list_file)
   
-  run_mapper = lambda x : x.split("_")[5]
-  condition_mapper = lambda x : x.split("_")[8]
+  sample_mapper = dict(zip(file_list_df["run"], file_list_df["sample"]))
+  condition_mapper = dict(zip(file_list_df["run"], file_list_df["condition"]))
   
-  df["run"] = df["Run"].map(run_mapper)
+  df = pd.read_csv(diann_file_path, sep='\t')
+  
+  df["run"] = df["Run"].map(sample_mapper)
   df["condition"] = df["Run"].map(condition_mapper)
   df["charge"] = df["Precursor.Charge"]
   df["searchScore"] = -np.log(df["Q.Value"])
   df["intensity"] = df['Precursor.Quantity']
   df["peptide"] = df["Stripped.Sequence"]
   df["proteins"] = df["Protein.Ids"]
   triqler_input_df = df[["run", "condition", "charge", "searchScore", "intensity", "peptide", "proteins"]]
 
   triqler_input_df.to_csv(triqler_input_file, sep='\t', index=False)
 
 
+def parse_file_list(file_list_file: str):
+  file_list_df = pd.read_csv(file_list_file, sep='\t', header=None)
+  
+  if len(file_list_df.columns) < 2:
+    raise ValueError("Too few columns present in file list mapping, need at least 2 columns: run, condition")
+  
+  if len(file_list_df.columns) > 4:
+    raise ValueError("Too many columns present in file list mapping, can at most have 4 columns: run, condition, sample, fraction")
+  
+  file_list_df.columns = ["run", "condition", "sample", "fraction"][:len(file_list_df.columns)]
+  
+  if "sample" not in file_list_df.columns:
+    file_list_df["sample"] = file_list_df["run"]
+  
+  if "fraction" not in file_list_df.columns:
+    file_list_df["fraction"] = -1
+  
+  return file_list_df
+  
+
 if __name__ == "__main__":
    main()
```

## Comparing `triqler-0.7.0.dist-info/LICENSE` & `triqler-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triqler-0.7.0.dist-info/METADATA` & `triqler-0.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triqler
-Version: 0.7.0
+Version: 0.7.1
 Summary: Triqler: TRansparent Identification-Quantification-Linked Error Rates
 Home-page: https://github.com/statisticalbiotechnology/triqler
 License: Apache-2.0
 Keywords: mass spectrometry,missing values,proteomics,quantification
 Author: Matthew The
 Author-email: matthew.the@tum.de
 Requires-Python: >=3.8,<3.12
```

## Comparing `triqler-0.7.0.dist-info/RECORD` & `triqler-0.7.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 triqler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 triqler/__main__.py,sha256=4KsrTa5I-Sx5SYo9dkAxVahQ3tXNMxun_xhbfEdfOGE,140
 triqler/convert/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triqler/convert/diann.py,sha256=rpG7yaB7eEBRUvs4oXiQO8BIuyLLiXXDs9pngYoWU-c,2041
+triqler/convert/diann.py,sha256=n0wcC8EUGuflZXqP1Pn183cYrdncYfGhRz4nAsRRekI,3406
 triqler/convert/dinosaur.py,sha256=SlLUbw02sTjWi6DfRBG8d_5IFJKmu0xneyF4aA_eeis,6505
 triqler/convert/helpers.py,sha256=EpQhQ7QcICU1itp44yrAFzUu9allkItAFNQka5axkf4,6022
 triqler/convert/maxquant.py,sha256=ErLgH6Ccg2rtZW0suImfxSHbJUYYp2SL9ldHzrj12C0,6372
 triqler/convert/normalize_intensities.py,sha256=EWpuYIWhVEuAtej-_398IAk4PqMPNo2oUGZoWsEA7mI,5245
 triqler/convert/percolator.py,sha256=S_topa6Upt1Z4JX8vlR-zQhyHnqFSbXj7LLLrEtJGJY,2902
 triqler/convert/quandenser.py,sha256=c_eivM7K_hUldOgjs6A3dV1Hmr6_vGSBvcNB0wI3jGc,6447
 triqler/convolution_dp.py,sha256=kkrkXzFoo_qyiaYhFe-eL-cWsIqXexC8O2VSvbn2390,1127
@@ -17,12 +17,12 @@
 triqler/hyperparameters.py,sha256=cynq1MiULviVRelkus1CUYjEDdMKQvCORPzWBsiD2UY,17329
 triqler/multiprocessing_pool.py,sha256=7-WLPbe4oGxDCBsXXt6liHvWqLTHqpbnBo8csL7GMms,1735
 triqler/parsers.py,sha256=1P5u_XGIzFXmDzVUPguCJNWNP5HC7IixaZ-NS56Is8M,11469
 triqler/pgm.py,sha256=K8ahgtkXJBvfRGR8Dlw6DOV3uWRgQ3Pkfar_0sj5YjY,9551
 triqler/qvality.py,sha256=OKUBqN33ueQZXcwNfCFvsTCkSsvb2CsokBCfOraqXVo,16130
 triqler/triqler.py,sha256=ViKI3oR06mGsSLOQL9E8574GXmDdnWztjpXBqElOm_I,23827
 triqler/version.py,sha256=zzbjDF36eHFnDr1FmWabpC8EPDbZ16N5ExMFhM1smPQ,1018
-triqler-0.7.0.dist-info/entry_points.txt,sha256=BjsG9Dsy4s82N-4fVE_AymOkM3HhvbjU5rovQmj4oQE,368
-triqler-0.7.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-triqler-0.7.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-triqler-0.7.0.dist-info/METADATA,sha256=PZI4uxGV2fCyVD2_IM3-tmeNTD1ViqGSIhnr8EugCXc,10942
-triqler-0.7.0.dist-info/RECORD,,
+triqler-0.7.1.dist-info/entry_points.txt,sha256=BjsG9Dsy4s82N-4fVE_AymOkM3HhvbjU5rovQmj4oQE,368
+triqler-0.7.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+triqler-0.7.1.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+triqler-0.7.1.dist-info/METADATA,sha256=qsmb0n7_GqOfZfPWWttxen-HHLUR02UTKj394pB7WJk,10942
+triqler-0.7.1.dist-info/RECORD,,
```

