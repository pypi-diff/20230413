# Comparing `tmp/tdfextractor-0.1.3.tar.gz` & `tmp/tdfextractor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfextractor-0.1.3.tar", last modified: Mon Nov 21 00:06:50 2022, max compression
+gzip compressed data, was "tdfextractor-0.1.4.tar", last modified: Thu Apr 13 16:27:30 2023, max compression
```

## Comparing `tdfextractor-0.1.3.tar` & `tdfextractor-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 00:06:50.214887 tdfextractor-0.1.3/
--rw-rw-rw-   0        0        0      453 2022-11-21 00:06:50.214887 tdfextractor-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2022-11-21 00:06:50.214887 tdfextractor-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      625 2022-11-20 23:11:01.000000 tdfextractor-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-21 00:06:50.185675 tdfextractor-0.1.3/tdfextractor/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.3/tdfextractor/__init__.py
--rw-rw-rw-   0        0        0       50 2022-09-29 06:07:39.000000 tdfextractor-0.1.3/tdfextractor/constants.py
--rw-rw-rw-   0        0        0     4064 2022-11-20 23:53:51.000000 tdfextractor-0.1.3/tdfextractor/ms2_extractor.py
--rw-rw-rw-   0        0        0     1498 2022-11-19 18:06:55.000000 tdfextractor-0.1.3/tdfextractor/string_templates.py
--rw-rw-rw-   0        0        0     1602 2022-11-20 23:14:32.000000 tdfextractor-0.1.3/tdfextractor/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-21 00:06:50.208681 tdfextractor-0.1.3/tdfextractor.egg-info/
--rw-rw-rw-   0        0        0      453 2022-11-21 00:06:50.000000 tdfextractor-0.1.3/tdfextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2022-11-21 00:06:50.000000 tdfextractor-0.1.3/tdfextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-21 00:06:50.000000 tdfextractor-0.1.3/tdfextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-11-21 00:06:50.000000 tdfextractor-0.1.3/tdfextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-21 00:06:50.000000 tdfextractor-0.1.3/tdfextractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-21 00:06:50.208681 tdfextractor-0.1.3/test/
--rw-rw-rw-   0        0        0     2444 2022-11-19 19:23:32.000000 tdfextractor-0.1.3/test/test_ms2_extractor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.336149 tdfextractor-0.1.4/
+-rw-rw-rw-   0        0        0      453 2023-04-13 16:27:30.335958 tdfextractor-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:27:30.336149 tdfextractor-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-13 16:25:55.000000 tdfextractor-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.322522 tdfextractor-0.1.4/tdfextractor/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.4/tdfextractor/__init__.py
+-rw-rw-rw-   0        0        0       50 2022-09-29 06:07:39.000000 tdfextractor-0.1.4/tdfextractor/constants.py
+-rw-rw-rw-   0        0        0     5365 2023-04-13 16:11:10.000000 tdfextractor-0.1.4/tdfextractor/ms2_extractor.py
+-rw-rw-rw-   0        0        0     1498 2022-11-21 00:49:16.000000 tdfextractor-0.1.4/tdfextractor/string_templates.py
+-rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.4/tdfextractor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.333536 tdfextractor-0.1.4/tdfextractor.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 16:27:30.000000 tdfextractor-0.1.4/tdfextractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 16:27:30.334522 tdfextractor-0.1.4/test/
+-rw-rw-rw-   0        0        0     2440 2023-04-12 23:55:45.000000 tdfextractor-0.1.4/test/test_ms2_extractor.py
```

### Comparing `tdfextractor-0.1.3/setup.py` & `tdfextractor-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='tdfextractor',
-    version='0.1.3',
+    version='0.1.4',
     description='extract mass spec files from bruker d folder',
     url='https://github.com/pgarrett-scripps/tdfextractor.git',
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     license='MIT',
     packages=['tdfextractor'],
-    install_requires=['tdfpy==0.1.2', 'serenipy==0.1.2'],
+    install_requires=['tdfpy==0.1.2', 'serenipy==0.2.6'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

### Comparing `tdfextractor-0.1.3/tdfextractor/ms2_extractor.py` & `tdfextractor-0.1.4/tdfextractor/ms2_extractor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,32 @@
+import logging
+import time
 from datetime import datetime
 from pathlib import Path
+from typing import List
 
 from tdfpy import timsdata
 from tdfpy.pandas_tdf import PandasTdf
 from serenipy.ms2 import Ms2Spectra, to_ms2
 
 from .constants import MS2_VERSION
 from .string_templates import header_ms2_template
 from .utils import calculate_mass, map_precursor_to_ip2_scan_number
 
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-def get_ms2_content(analysis_dir: str, include_spectra=True):
+
+def batch_iterator(input_list: List, batch_size: int):
+    for i in range(0, len(input_list), batch_size):
+        yield input_list[i:i + batch_size]
+
+
+def get_ms2_content(analysis_dir: str, include_spectra: bool = True, batch_size: int = 100,
+                    remove_charge1: bool = True, remove_empty_spectra: bool = True):
+    logging.info(f'Starting to process {analysis_dir}')
 
     with timsdata.timsdata_connect(analysis_dir) as td:
 
         pd_tdf = PandasTdf(str(Path(analysis_dir) / 'analysis.tdf'))
         precursors_df = pd_tdf.precursors
         frames_df = pd_tdf.frames
         precursor_to_scan_number = map_precursor_to_ip2_scan_number(precursors_df, frames_df)
@@ -22,50 +34,65 @@
 
         parent_id_to_rt = {int(frame_id): rt for frame_id, rt in frames_df[['Id', 'Time']].values}
         precursor_id_to_collision_energy = {int(prec_id): ce for prec_id, ce in
                                             pasef_frames_msms_info_df[['Precursor', 'CollisionEnergy']].values}
 
         precursors_df.dropna(subset=['MonoisotopicMz', 'Charge'], inplace=True)
 
-        for _, precursor_row in precursors_df.iterrows():
-
-            precursor_id = int(precursor_row['Id'])
-            parent_id = int(precursor_row['Parent'])
-            charge = int(precursor_row['Charge'])
-            ip2_scan_number = precursor_to_scan_number[precursor_id]
-            ook0 = td.scanNumToOneOverK0(parent_id, [precursor_row['ScanNumber']])[0]
-            ccs = timsdata.oneOverK0ToCCSforMz(ook0, charge, precursor_row['MonoisotopicMz'])
-            mz = precursor_row['MonoisotopicMz']
-            prec_intensity = precursor_row['Intensity']
-            mass = calculate_mass(mz, charge)
-
-            ms2_spectra = Ms2Spectra(low_scan=ip2_scan_number,
-                                     high_scan=ip2_scan_number,
-                                     mz=mz,
-                                     mass=mass,
-                                     charge=charge,
-                                     info={},
-                                     mz_spectra=[],
-                                     intensity_spectra=[],
-                                     charge_spectra=[])
-
-            ms2_spectra.parent_id = parent_id
-            ms2_spectra.precursor_id = precursor_id
-            ms2_spectra.prec_intensity = round(prec_intensity, 1)
-            ms2_spectra.ook0 = round(ook0, 4)
-            ms2_spectra.ccs = round(ccs, 4)
-            ms2_spectra.rt = round(parent_id_to_rt[parent_id], 4)
-            ms2_spectra.ce = round(precursor_id_to_collision_energy[precursor_id], 1)
+        for precursor_rows in batch_iterator(input_list=list(precursors_df.iterrows()), batch_size=batch_size):
+            logging.info(f'Processing batch of {batch_size} precursors')
 
+            pasef_ms_ms = None
             if include_spectra:
-                mz_arr, int_arr = td.readPasefMsMs([precursor_id])[precursor_id]
-                ms2_spectra.mz_spectra = mz_arr
-                ms2_spectra.intensity_spectra = int_arr
+                pasef_ms_ms = td.readPasefMsMs([int(row['Id']) for _, row in precursor_rows])
+
+            for _, precursor_row in precursor_rows:
 
-            yield ms2_spectra
+                precursor_id = int(precursor_row['Id'])
+                parent_id = int(precursor_row['Parent'])
+                charge = int(precursor_row['Charge'])
+
+                if remove_charge1 is True and charge == 1:
+                    continue
+
+                ip2_scan_number = precursor_to_scan_number[precursor_id]
+                ook0 = td.scanNumToOneOverK0(parent_id, [precursor_row['ScanNumber']])[0]
+                ccs = timsdata.oneOverK0ToCCSforMz(ook0, charge, precursor_row['MonoisotopicMz'])
+                mz = precursor_row['MonoisotopicMz']
+                prec_intensity = precursor_row['Intensity']
+                mass = calculate_mass(mz, charge)
+
+                ms2_spectra = Ms2Spectra(low_scan=ip2_scan_number,
+                                         high_scan=ip2_scan_number,
+                                         mz=mz,
+                                         mass=mass,
+                                         charge=charge,
+                                         info={},
+                                         mz_spectra=[],
+                                         intensity_spectra=[],
+                                         charge_spectra=[])
+
+                ms2_spectra.parent_id = parent_id
+                ms2_spectra.precursor_id = precursor_id
+                ms2_spectra.prec_intensity = round(prec_intensity, 1)
+                ms2_spectra.ook0 = round(ook0, 4)
+                ms2_spectra.ccs = round(ccs, 4)
+                ms2_spectra.rt = round(parent_id_to_rt[parent_id], 4)
+                ms2_spectra.ce = round(precursor_id_to_collision_energy[precursor_id], 1)
+
+                if include_spectra:
+                    ms2_spectra.mz_spectra = pasef_ms_ms[precursor_id][0]
+                    ms2_spectra.intensity_spectra = pasef_ms_ms[precursor_id][1]
+
+                    assert len(ms2_spectra.mz_spectra) == len(ms2_spectra.intensity_spectra)
+
+                    if remove_empty_spectra is True and len(ms2_spectra.mz_spectra) == 0:
+                        continue
+
+                yield ms2_spectra
 
 
 def generate_header(analysis_dir: str):
     pd_tdf = PandasTdf(str(Path(analysis_dir) / 'analysis.tdf'))
     precursors_df = pd_tdf.precursors
     frames_df = pd_tdf.frames
     precursor_to_scan_number = map_precursor_to_ip2_scan_number(precursors_df, frames_df)
@@ -74,18 +101,17 @@
                                             date_of_creation=str(datetime.now().strftime("%B %d, %Y %H:%M")),
                                             first_scan=list(precursor_to_scan_number.values())[0],
                                             last_scan=list(precursor_to_scan_number.values())[-1])
 
     return ms2_header
 
 
-def write_ms2_file(analysis_dir: str, include_spectra=True, output_file=None):
+def write_ms2_file(analysis_dir: str, include_spectra: bool = True, output_file: str = None, batch_size: int = 1000):
     if output_file is None:
         output_file = str(Path(analysis_dir) / Path(analysis_dir).stem) + '.ms2'
 
     ms2_header = generate_header(analysis_dir)
-    ms2_spectra = list(get_ms2_content(analysis_dir, include_spectra))
-
+    ms2_spectra = get_ms2_content(analysis_dir=analysis_dir, include_spectra=include_spectra, batch_size=batch_size)
     ms2_content = to_ms2([ms2_header], ms2_spectra)
 
     with open(output_file, 'w') as file:
         file.write(ms2_content)
```

### Comparing `tdfextractor-0.1.3/tdfextractor/string_templates.py` & `tdfextractor-0.1.4/tdfextractor/string_templates.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.3/tdfextractor/utils.py` & `tdfextractor-0.1.4/tdfextractor/utils.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.3/test/test_ms2_extractor.py` & `tdfextractor-0.1.4/test/test_ms2_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,9 +58,7 @@
         for spectra in get_ms2_content(d_folder, include_spectra=False):
             ms2_spectra = spectra
             break
 
         self.assertEqual(len(ms2_spectra.mz_spectra), 0)
         self.assertEqual(len(ms2_spectra.intensity_spectra), 0)
         self.assertEqual(len(ms2_spectra.charge_spectra), 0)
-
-
```

