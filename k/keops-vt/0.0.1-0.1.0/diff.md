# Comparing `tmp/keops-vt-0.0.1.tar.gz` & `tmp/keops-vt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keops-vt-0.0.1.tar", last modified: Thu Apr 13 15:59:20 2023, max compression
+gzip compressed data, was "keops-vt-0.1.0.tar", last modified: Thu Apr 13 16:31:19 2023, max compression
```

## Comparing `keops-vt-0.0.1.tar` & `keops-vt-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:20.192977 keops-vt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-13 15:59:09.000000 keops-vt-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-13 15:59:20.192977 keops-vt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 15:59:09.000000 keops-vt-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:20.188977 keops-vt-0.0.1/keops/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/erase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/shrink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:20.188977 keops-vt-0.0.1/keops/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/mvt_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/mvt_eraser.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/mvt_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/mvt_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-13 15:59:09.000000 keops-vt-0.0.1/keops/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:20.192977 keops-vt-0.0.1/keops_vt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:59:20.000000 keops-vt-0.0.1/keops_vt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-13 15:59:09.000000 keops-vt-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:59:20.192977 keops-vt-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:20.192977 keops-vt-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-13 15:59:09.000000 keops-vt-0.0.1/tests/test_erase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 15:59:09.000000 keops-vt-0.0.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 15:59:09.000000 keops-vt-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:19.002165 keops-vt-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-13 16:31:07.000000 keops-vt-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-13 16:31:19.002165 keops-vt-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-13 16:31:07.000000 keops-vt-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:19.002165 keops-vt-0.1.0/keops/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/erase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/shrink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:19.002165 keops-vt-0.1.0/keops/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/mvt_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/mvt_eraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/mvt_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/mvt_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-13 16:31:07.000000 keops-vt-0.1.0/keops/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:19.002165 keops-vt-0.1.0/keops_vt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:31:18.000000 keops-vt-0.1.0/keops_vt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 16:31:07.000000 keops-vt-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:31:19.002165 keops-vt-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:31:19.002165 keops-vt-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-13 16:31:07.000000 keops-vt-0.1.0/tests/test_erase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 16:31:07.000000 keops-vt-0.1.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 16:31:07.000000 keops-vt-0.1.0/tests/test_utils.py
```

### Comparing `keops-vt-0.0.1/LICENSE.md` & `keops-vt-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/PKG-INFO` & `keops-vt-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: keops-vt
-Version: 0.0.1
+Version: 0.1.0
 Summary: CLI tool for custom edition and management of Mapbox Vector Tiles in MBTiles format
 Author-email: Fran Martín <fmartinrivas2@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fmariv/keops-vt
 Project-URL: Bug Tracker, https://github.com/fmariv/keops-vt/issues
 Keywords: mbtiles,python,vector-tiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Keops
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#wip)
 ![CI](https://github.com/fmariv/keops-vt/actions/workflows/test_lint.yaml/badge.svg)
 
 <p align="center">
     <img src="favicon.png" alt="Keops logo">
 </p>
 
 Keops is a CLI tool that allows you to apply some logic to vector tiles in a MBTiles file, such as removing or getting the size of a given tile, obtaining the vector layers that conform the MBTiles or shrinking the vector data, in order to reduce the data size.
```

### Comparing `keops-vt-0.0.1/README.md` & `keops-vt-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Keops
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#wip)
 ![CI](https://github.com/fmariv/keops-vt/actions/workflows/test_lint.yaml/badge.svg)
 
 <p align="center">
     <img src="favicon.png" alt="Keops logo">
 </p>
 
 Keops is a CLI tool that allows you to apply some logic to vector tiles in a MBTiles file, such as removing or getting the size of a given tile, obtaining the vector layers that conform the MBTiles or shrinking the vector data, in order to reduce the data size.
```

### Comparing `keops-vt-0.0.1/keops/debug.py` & `keops-vt-0.1.0/keops/debug.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/info.py` & `keops-vt-0.1.0/keops/info.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/main.py` & `keops-vt-0.1.0/keops/main.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/shrink.py` & `keops-vt-0.1.0/keops/shrink.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/size.py` & `keops-vt-0.1.0/keops/size.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/src/mvt_debugger.py` & `keops-vt-0.1.0/keops/src/mvt_debugger.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/src/mvt_eraser.py` & `keops-vt-0.1.0/keops/src/mvt_eraser.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/src/mvt_printer.py` & `keops-vt-0.1.0/keops/src/mvt_printer.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/src/mvt_reader.py` & `keops-vt-0.1.0/keops/src/mvt_reader.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops/src/utils.py` & `keops-vt-0.1.0/keops/src/utils.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/keops_vt.egg-info/PKG-INFO` & `keops-vt-0.1.0/keops_vt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: keops-vt
-Version: 0.0.1
+Version: 0.1.0
 Summary: CLI tool for custom edition and management of Mapbox Vector Tiles in MBTiles format
 Author-email: Fran Martín <fmartinrivas2@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fmariv/keops-vt
 Project-URL: Bug Tracker, https://github.com/fmariv/keops-vt/issues
 Keywords: mbtiles,python,vector-tiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Keops
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#wip)
 ![CI](https://github.com/fmariv/keops-vt/actions/workflows/test_lint.yaml/badge.svg)
 
 <p align="center">
     <img src="favicon.png" alt="Keops logo">
 </p>
 
 Keops is a CLI tool that allows you to apply some logic to vector tiles in a MBTiles file, such as removing or getting the size of a given tile, obtaining the vector layers that conform the MBTiles or shrinking the vector data, in order to reduce the data size.
```

### Comparing `keops-vt-0.0.1/keops_vt.egg-info/SOURCES.txt` & `keops-vt-0.1.0/keops_vt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/pyproject.toml` & `keops-vt-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 [build-system]
 requires = ["setuptools>=59.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keops-vt"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Fran Martín", email="fmartinrivas2@gmail.com" },
 ]
 description = "CLI tool for custom edition and management of Mapbox Vector Tiles in MBTiles format"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["mbtiles", "python", "vector-tiles"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "Click",
     "mapbox-vector-tile==1.2.1",
     "protobuf==3.19.4",
+    "geopandas==0.12.1",
+    "click==8.1.3",
+    "geojson==2.5.0",
+    "setuptools==58.1.0",
+    "docker==6.0.1",
+    "mkdocs==1.4.1",
+    "mkdocs-material==9.1.0",
+    "prettytable==3.6.0",
+    "halo==0.0.31"
 ]
 
 [project.scripts]
 keops = "keops.main:main_group"
 
 [project.urls]
 "Homepage" = "https://github.com/fmariv/keops-vt"
```

### Comparing `keops-vt-0.0.1/tests/test_erase.py` & `keops-vt-0.1.0/tests/test_erase.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/tests/test_reader.py` & `keops-vt-0.1.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `keops-vt-0.0.1/tests/test_utils.py` & `keops-vt-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

