# Comparing `tmp/uvw-0.5.0.tar.gz` & `tmp/uvw-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvw-0.5.0.tar", last modified: Fri Nov 25 13:07:57 2022, max compression
+gzip compressed data, was "uvw-0.5.1.tar", last modified: Thu Apr 13 09:02:03 2023, max compression
```

## Comparing `uvw-0.5.0.tar` & `uvw-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:07:57.107330 uvw-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-11-25 13:07:45.000000 uvw-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-11-25 13:07:45.000000 uvw-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2022-11-25 13:07:57.107330 uvw-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2022-11-25 13:07:45.000000 uvw-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-11-25 13:07:57.107330 uvw-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2022-11-25 13:07:45.000000 uvw-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:07:57.107330 uvw-0.5.0/uvw/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-11-25 13:07:57.107330 uvw-0.5.0/uvw/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/data_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:07:57.107330 uvw-0.5.0/uvw/dropin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/dropin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14613 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/dropin/hl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/vtk_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2022-11-25 13:07:45.000000 uvw-0.5.0/uvw/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:07:57.107330 uvw-0.5.0/uvw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2022-11-25 13:07:57.000000 uvw-0.5.0/uvw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-11-25 13:07:57.000000 uvw-0.5.0/uvw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 13:07:57.000000 uvw-0.5.0/uvw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-11-25 13:07:57.000000 uvw-0.5.0/uvw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-11-25 13:07:57.000000 uvw-0.5.0/uvw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2022-11-25 13:07:45.000000 uvw-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 09:01:53.000000 uvw-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 09:01:53.000000 uvw-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-13 09:02:03.407386 uvw-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-13 09:01:53.000000 uvw-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 09:02:03.407386 uvw-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 09:01:53.000000 uvw-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/data_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/dropin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/dropin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/dropin/hl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/vtk_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-13 09:01:53.000000 uvw-0.5.1/versioneer.py
```

### Comparing `uvw-0.5.0/LICENSE.md` & `uvw-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/PKG-INFO` & `uvw-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvw
-Version: 0.5.0
+Version: 0.5.1
 Summary: Universal VTK Writer for Numpy Arrays
 Home-page: https://github.com/prs513rosewood/uvw
 Author: Lucas Frérot
 Author-email: lucas.frerot@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uvw-0.5.0/README.md` & `uvw-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/setup.py` & `uvw-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/__init__.py` & `uvw-0.5.1/uvw/__init__.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/data_array.py` & `uvw-0.5.1/uvw/data_array.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/dropin/hl.py` & `uvw-0.5.1/uvw/dropin/hl.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/parallel.py` & `uvw-0.5.1/uvw/parallel.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/unstructured.py` & `uvw-0.5.1/uvw/unstructured.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @unique
 class CellType(Enum):
     """
     Enumerates the VTK cell types.
 
-    See https://lorensen.github.io/VTKExamples/site/VTKFileFormats/
+    See https://kitware.github.io/vtk-examples/site/VTKFileFormats/#legacy-file-examples
     """
 
     VERTEX = 1
     POLY_VERTEX = 2
     LINE = 3
     POLY_LINE = 4
     TRIANGLE = 5
@@ -60,15 +60,15 @@
     CellType.TRIANGLE: 3,
     CellType.TRIANGLE_STRIP: -1,
     CellType.POLYGON: -1,
     CellType.PIXEL: 4,
     CellType.QUAD: 4,
     CellType.TETRA: 4,
     CellType.VOXEL: 8,
-    CellType.HEXAHEDRON: 9,
+    CellType.HEXAHEDRON: 8,
     CellType.WEDGE: 6,
     CellType.PYRAMID: 5,
     CellType.PENTAGONAL_PRISM: 10,
     CellType.HEXAGONAL_PRISM: 12,
     CellType.QUADRATIC_EDGE: 3,
     CellType.QUADRATIC_TRIANGLE: 6,
     CellType.QUADRATIC_QUAD: 8,
```

### Comparing `uvw-0.5.0/uvw/vtk_files.py` & `uvw-0.5.1/uvw/vtk_files.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw/writer.py` & `uvw-0.5.1/uvw/writer.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.0/uvw.egg-info/PKG-INFO` & `uvw-0.5.1/uvw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvw
-Version: 0.5.0
+Version: 0.5.1
 Summary: Universal VTK Writer for Numpy Arrays
 Home-page: https://github.com/prs513rosewood/uvw
 Author: Lucas Frérot
 Author-email: lucas.frerot@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uvw-0.5.0/versioneer.py` & `uvw-0.5.1/versioneer.py`

 * *Files identical despite different names*

