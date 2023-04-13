# Comparing `tmp/aicsimageprocessing-0.8.2.tar.gz` & `tmp/aicsimageprocessing-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicsimageprocessing-0.8.2.tar", last modified: Wed Sep 29 23:53:07 2021, max compression
+gzip compressed data, was "aicsimageprocessing-0.8.3.tar", last modified: Thu Apr 13 19:51:51 2023, max compression
```

## Comparing `aicsimageprocessing-0.8.2.tar` & `aicsimageprocessing-0.8.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.423387 aicsimageprocessing-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-09-29 23:53:07.423387 aicsimageprocessing-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.419386 aicsimageprocessing-0.8.2/aicsimageprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7047 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/alignMajor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/backgroundCrop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/backgroundSub.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.419386 aicsimageprocessing-0.8.2/aicsimageprocessing/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/bin/make_atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/bin/make_thumbnail.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      345 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/crop_img.py
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/flip.py
--rw-r--r--   0 runner    (1001) docker     (121)     6037 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/imgCenter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3180 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/imgToCoords.py
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/imgToProjection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      987 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/imshow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/isosurfaceGenerator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3145 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/resize.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5722 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/rigidAlignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9413 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/sdfGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.419386 aicsimageprocessing-0.8.2/aicsimageprocessing/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6220 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/segmentation/nucleusSegmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)    10875 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/textureAtlas.py
--rw-r--r--   0 runner    (1001) docker     (121)    17742 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/thumbnailGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/aicsimageprocessing/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.419386 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-29 23:53:07.000000 aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 23:53:07.423387 aicsimageprocessing-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (121)     5423 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      458 2021-09-29 23:53:07.423387 aicsimageprocessing-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2021-09-29 23:53:03.000000 aicsimageprocessing-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.966014 aicsimageprocessing-0.8.3/aicsimageprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/alignMajor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/backgroundCrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/backgroundSub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/aicsimageprocessing/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/bin/make_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/bin/make_thumbnail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/crop_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/diagnosticsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/imgCenter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/imgToCoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/imgToProjection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/imshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/isosurfaceGenerator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3145 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/resize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5722 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/rigidAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/sdfGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/aicsimageprocessing/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/segmentation/nucleusSegmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/textureAtlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/thumbnailGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/aicsimageprocessing/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 19:51:51.000000 aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5423 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-13 19:51:51.970014 aicsimageprocessing-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-13 19:51:47.000000 aicsimageprocessing-0.8.3/setup.py
```

### Comparing `aicsimageprocessing-0.8.2/CONTRIBUTING.md` & `aicsimageprocessing-0.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/LICENSE` & `aicsimageprocessing-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/PKG-INFO` & `aicsimageprocessing-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsimageprocessing
-Version: 0.8.2
+Version: 0.8.3
 Summary: A generalized scientific image processing module from the Allen Institute for Cell Science.
 Home-page: https://github.com/AllenCellModeling/aicsimageprocessing
 Author: AICS
 Author-email: !AICS_SW@alleninstitute.org
 License: Allen Institute Software License
 Description: # aicsimageprocessing
```

### Comparing `aicsimageprocessing-0.8.2/README.md` & `aicsimageprocessing-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/__init__.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Top-level package for aicsimageprocessing."""
 
 __author__ = "AICS"
 __email__ = "!AICS_SW@alleninstitute.org"
 # Do not edit this string manually, always use bumpversion
 # Details in CONTRIBUTING.md
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 
 def get_module_version():
     return __version__
 
 
 from .alignMajor import *  # noqa
@@ -23,7 +23,8 @@
 from .imgToProjection import *  # noqa
 from .imshow import *  # noqa
 from .isosurfaceGenerator import *  # noqa
 from .normalization import *  # noqa
 from .resize import *  # noqa
 from .rigidAlignment import *  # noqa
 from .thumbnailGenerator import *  # noqa
+from .diagnosticsheet import *  # noqa
```

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/alignMajor.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/alignMajor.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/backgroundCrop.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/backgroundCrop.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/backgroundSub.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/backgroundSub.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/bin/make_atlas.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/bin/make_atlas.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/bin/make_thumbnail.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/bin/make_thumbnail.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/flip.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/flip.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/imgCenter.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/imgCenter.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/imgToCoords.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/imgToCoords.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/imgToProjection.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/imgToProjection.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/imshow.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/imshow.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/isosurfaceGenerator.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/isosurfaceGenerator.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/normalization.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/resize.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/resize.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/rigidAlignment.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/rigidAlignment.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/sdfGenerator.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/sdfGenerator.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/segmentation/nucleusSegmentation.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/segmentation/nucleusSegmentation.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/textureAtlas.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/textureAtlas.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/thumbnailGenerator.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/thumbnailGenerator.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing/transformation.py` & `aicsimageprocessing-0.8.3/aicsimageprocessing/transformation.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/PKG-INFO` & `aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsimageprocessing
-Version: 0.8.2
+Version: 0.8.3
 Summary: A generalized scientific image processing module from the Allen Institute for Cell Science.
 Home-page: https://github.com/AllenCellModeling/aicsimageprocessing
 Author: AICS
 Author-email: !AICS_SW@alleninstitute.org
 License: Allen Institute Software License
 Description: # aicsimageprocessing
```

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/SOURCES.txt` & `aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 aicsimageprocessing/__init__.py
 aicsimageprocessing/alignMajor.py
 aicsimageprocessing/backgroundCrop.py
 aicsimageprocessing/backgroundSub.py
 aicsimageprocessing/crop_img.py
+aicsimageprocessing/diagnosticsheet.py
 aicsimageprocessing/flip.py
 aicsimageprocessing/imgCenter.py
 aicsimageprocessing/imgToCoords.py
 aicsimageprocessing/imgToProjection.py
 aicsimageprocessing/imshow.py
 aicsimageprocessing/isosurfaceGenerator.py
 aicsimageprocessing/normalization.py
```

### Comparing `aicsimageprocessing-0.8.2/aicsimageprocessing.egg-info/requires.txt` & `aicsimageprocessing-0.8.3/aicsimageprocessing.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 numpy>=1.16.4
 Pillow>=5.2.0
 PyMCubes
 scikit-image>=0.15.0
 scikit-learn
 scikit-fmm>=2021.7.8
 scipy>=1.3.0
-vtk>=9.0.1
+vtk
+aics_dask_utils
+ome-zarr
+universal_pathlib==0.0.19
 
 [all]
 aicsimageio[all]>=4.1.0
 matplotlib>=3.1.1
 numpy>=1.16.4
 Pillow>=5.2.0
 PyMCubes
 scikit-image>=0.15.0
 scikit-learn
 scikit-fmm>=2021.7.8
 scipy>=1.3.0
-vtk>=9.0.1
+vtk
+aics_dask_utils
+ome-zarr
+universal_pathlib==0.0.19
 codecov
 flake8
 black
 pytest
 pytest-cov
 pytest-raises
 pytest-runner
```

### Comparing `aicsimageprocessing-0.8.2/docs/Makefile` & `aicsimageprocessing-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/docs/conf.py` & `aicsimageprocessing-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/docs/installation.rst` & `aicsimageprocessing-0.8.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/docs/make.bat` & `aicsimageprocessing-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicsimageprocessing-0.8.2/setup.py` & `aicsimageprocessing-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,19 @@
     "numpy>=1.16.4",
     "Pillow>=5.2.0",
     "PyMCubes",
     "scikit-image>=0.15.0",
     "scikit-learn",
     "scikit-fmm>=2021.7.8",
     "scipy>=1.3.0",
-    "vtk>=9.0.1",
+    "vtk",
+    "aics_dask_utils",
+    "ome-zarr",
+    "universal_pathlib==0.0.19",
+    
 ]
 
 extra_requirements = {
     "test": test_requirements,
     "setup": setup_requirements,
     "dev": dev_requirements,
     "interactive": interactive_requirements,
@@ -108,10 +112,10 @@
     setup_requires=setup_requirements,
     test_suite="aicsimageprocessing/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCellModeling/aicsimageprocessing",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.8.2",
+    version="0.8.3",
     zip_safe=False,
 )
```

