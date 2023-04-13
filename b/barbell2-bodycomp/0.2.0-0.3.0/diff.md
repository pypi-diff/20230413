# Comparing `tmp/barbell2_bodycomp-0.2.0.tar.gz` & `tmp/barbell2_bodycomp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_bodycomp-0.2.0.tar", last modified: Thu Apr 13 10:44:28 2023, max compression
+gzip compressed data, was "dist/barbell2_bodycomp-0.3.0.tar", last modified: Thu Apr 13 11:39:22 2023, max compression
```

## Comparing `barbell2_bodycomp-0.2.0.tar` & `barbell2_bodycomp-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 10:44:28.337581 barbell2_bodycomp-0.2.0/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 10:44:28.337397 barbell2_bodycomp-0.2.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 10:44:28.334753 barbell2_bodycomp-0.2.0/barbell2_bodycomp/
--rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-13 10:44:23.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/__init__.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 10:44:28.337151 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/
--rw-r--r--   0 ralph      (501) staff       (20)       55 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/tag2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 10:44:28.335848 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      653 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       32 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-13 10:44:28.000000 barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-13 10:44:28.337637 barbell2_bodycomp-0.2.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1399 2023-04-13 10:40:57.000000 barbell2_bodycomp-0.2.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.294780 barbell2_bodycomp-0.3.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 11:39:22.294564 barbell2_bodycomp-0.3.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.290507 barbell2_bodycomp-0.3.0/barbell2_bodycomp/
+-rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-13 11:39:07.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4456 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.293900 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 ralph      (501) staff       (20)       55 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2npy.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6046 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1374 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5788 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.291948 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      804 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       40 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-13 11:39:22.294844 barbell2_bodycomp-0.3.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1414 2023-04-13 11:38:29.000000 barbell2_bodycomp-0.3.0/setup.py
```

### Comparing `barbell2_bodycomp-0.2.0/PKG-INFO` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2_bodycomp
-Version: 0.2.0
+Name: barbell2-bodycomp
+Version: 0.3.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2-bodycomp
-Version: 0.2.0
+Name: barbell2_bodycomp
+Version: 0.3.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.2.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 setup.py
 barbell2_bodycomp/__init__.py
+barbell2_bodycomp/calculator.py
+barbell2_bodycomp/seg.py
+barbell2_bodycomp/selectroi.py
+barbell2_bodycomp/selectslice.py
+barbell2_bodycomp/totalseg.py
 barbell2_bodycomp/utils.py
 barbell2_bodycomp.egg-info/PKG-INFO
 barbell2_bodycomp.egg-info/SOURCES.txt
 barbell2_bodycomp.egg-info/dependency_links.txt
 barbell2_bodycomp.egg-info/entry_points.txt
 barbell2_bodycomp.egg-info/not-zip-safe
 barbell2_bodycomp.egg-info/requires.txt
```

### Comparing `barbell2_bodycomp-0.2.0/setup.py` & `barbell2_bodycomp-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'numpy',
     'pydicom',
     'pynrrd',
     'matplotlib',
+    'nibabel',
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
```

