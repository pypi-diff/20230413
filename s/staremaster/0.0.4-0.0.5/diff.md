# Comparing `tmp/staremaster-0.0.4.tar.gz` & `tmp/staremaster-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staremaster-0.0.4.tar", last modified: Thu Nov 24 01:27:52 2022, max compression
+gzip compressed data, was "staremaster-0.0.5.tar", last modified: Wed Apr 12 22:08:07 2023, max compression
```

## Comparing `staremaster-0.0.4.tar` & `staremaster-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:27:52.364172 staremaster-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-24 01:27:37.000000 staremaster-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-11-24 01:27:52.364172 staremaster-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-11-24 01:27:37.000000 staremaster-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-24 01:27:37.000000 staremaster-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-11-24 01:27:52.364172 staremaster-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-24 01:27:37.000000 staremaster-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:27:52.364172 staremaster-0.0.4/staremaster/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-24 01:27:52.364172 staremaster-0.0.4/staremaster/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/conversions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6544 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/create_sidecar_files.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3639 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/find_missing_sidecars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:27:52.360172 staremaster-0.0.4/staremaster/products/
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/amsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/atms.py
--rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/goes_abi_fixed_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/hdfeos.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/imerg.py
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/mod05.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/mod09.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/modis_tilegrid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/satcorps.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/ssmis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2633 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/viirsL2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/products/xcal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6109 2022-11-24 01:27:37.000000 staremaster-0.0.4/staremaster/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:27:52.360172 staremaster-0.0.4/staremaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-24 01:27:52.000000 staremaster-0.0.4/staremaster.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:27:52.364172 staremaster-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-24 01:27:37.000000 staremaster-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_atms.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_cldmsk.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_mod05.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_mod09.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_parallel_files.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_ssmis.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-11-24 01:27:38.000000 staremaster-0.0.4/tests/test_vnp03.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-11-24 01:27:38.000000 staremaster-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:07.214841 staremaster-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 22:07:53.000000 staremaster-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-12 22:08:07.214841 staremaster-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-12 22:07:53.000000 staremaster-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 22:07:53.000000 staremaster-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 22:08:07.214841 staremaster-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 22:07:53.000000 staremaster-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:07.214841 staremaster-0.0.5/staremaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 22:08:07.214841 staremaster-0.0.5/staremaster/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/conversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6544 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/create_sidecar_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3639 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/find_missing_sidecars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:07.210840 staremaster-0.0.5/staremaster/products/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/amsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/atms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/goes_abi_fixed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/hdfeos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/imerg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/mod05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/mod09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/modis_tilegrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/satcorps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/ssmis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/viirsL2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/products/xcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-12 22:07:53.000000 staremaster-0.0.5/staremaster/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:07.210840 staremaster-0.0.5/staremaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:08:07.000000 staremaster-0.0.5/staremaster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:07.214841 staremaster-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:07:53.000000 staremaster-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_atms.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_cldmsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_mod05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_mod09.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_parallel_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_ssmis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 22:07:54.000000 staremaster-0.0.5/tests/test_vnp03.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-12 22:07:54.000000 staremaster-0.0.5/versioneer.py
```

### Comparing `staremaster-0.0.4/PKG-INFO` & `staremaster-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staremaster
-Version: 0.0.4
+Version: 0.0.5
 Summary: STARE sidecar creator
 Home-page: https://github.com/SpatioTemporal/STAREMaster_py
 Author: Niklas Griessbaum
 Author-email: griessbaum@ucsb.edu
 Project-URL: Bug Tracker, https://github.com/SpatioTemporal/STAREMaster_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `staremaster-0.0.4/README.md` & `staremaster-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/setup.cfg` & `staremaster-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/conversions.py` & `staremaster-0.0.5/staremaster/conversions.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/create_sidecar_files.py` & `staremaster-0.0.5/staremaster/create_sidecar_files.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/find_missing_sidecars.py` & `staremaster-0.0.5/staremaster/find_missing_sidecars.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/__init__.py` & `staremaster-0.0.5/staremaster/products/__init__.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/goes_abi_fixed_grid.py` & `staremaster-0.0.5/staremaster/products/goes_abi_fixed_grid.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/hdfeos.py` & `staremaster-0.0.5/staremaster/products/hdfeos.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/imerg.py` & `staremaster-0.0.5/staremaster/products/imerg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     
     def __init__(self):
         ## IMERG is a gridded dataset on a 0.05 degree grid
         self.lats = None
         self.lons = None
         self.nom_res = ''
         self.sids = []
+        self.make_latlon()
         
-    def get_latlon(self):
+    def make_latlon(self):
         self.lats = numpy.ascontiguousarray(numpy.tile(numpy.arange(-89.95, 90, 0.1), (3600, 1)).transpose())
         self.lons = numpy.tile(numpy.arange(-179.95, 180, 0.1), (1800, 1))
 
     def get_cover_sids(self):
         cover_sids = numpy.array([0x0000000000000000, 0x0800000000000000, 0x1000000000000000, 0x1800000000000000,
                                   0x2000000000000000, 0x2800000000000000, 0x3000000000000000, 0x3800000000000000])
         return cover_sids
@@ -38,15 +39,15 @@
         pickle_name = 'imerg_sids.pickle'
         if os.path.exists(pickle_name):
             self.load_sids_pickle(pickle_name)
         else:
             self.make_sids()
         return self.sids
 
-    def create_sidecar(self, out_path):
+    def create_sidecar(self, out_path, n_workers):
         sids = self.get_sids()
         cover_sids = self.get_cover_sids()
         
         i = self.lats.shape[0]
         j = self.lats.shape[1]
         l = cover_sids.size
```

### Comparing `staremaster-0.0.4/staremaster/products/mod05.py` & `staremaster-0.0.5/staremaster/products/mod05.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/mod09.py` & `staremaster-0.0.5/staremaster/products/mod09.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/modis_tilegrid.py` & `staremaster-0.0.5/staremaster/products/modis_tilegrid.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/satcorps.py` & `staremaster-0.0.5/staremaster/products/satcorps.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/viirsL2.py` & `staremaster-0.0.5/staremaster/products/viirsL2.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/products/xcal.py` & `staremaster-0.0.5/staremaster/products/xcal.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster/sidecar.py` & `staremaster-0.0.5/staremaster/sidecar.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/staremaster.egg-info/PKG-INFO` & `staremaster-0.0.5/staremaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staremaster
-Version: 0.0.4
+Version: 0.0.5
 Summary: STARE sidecar creator
 Home-page: https://github.com/SpatioTemporal/STAREMaster_py
 Author: Niklas Griessbaum
 Author-email: griessbaum@ucsb.edu
 Project-URL: Bug Tracker, https://github.com/SpatioTemporal/STAREMaster_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `staremaster-0.0.4/staremaster.egg-info/SOURCES.txt` & `staremaster-0.0.5/staremaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/tests/test_mod05.py` & `staremaster-0.0.5/tests/test_mod05.py`

 * *Files identical despite different names*

### Comparing `staremaster-0.0.4/versioneer.py` & `staremaster-0.0.5/versioneer.py`

 * *Files identical despite different names*

