# Comparing `tmp/test_data_visualization-0.0.1.tar.gz` & `tmp/test_data_visualization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_data_visualization-0.0.1.tar", last modified: Wed Apr 12 19:29:50 2023, max compression
+gzip compressed data, was "test_data_visualization-0.0.2.tar", last modified: Thu Apr 13 06:15:54 2023, max compression
```

## Comparing `test_data_visualization-0.0.1.tar` & `test_data_visualization-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-12 19:29:50.679806 test_data_visualization-0.0.1/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-11 05:15:17.000000 test_data_visualization-0.0.1/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-11 05:15:17.000000 test_data_visualization-0.0.1/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      296 2023-04-12 19:29:50.679410 test_data_visualization-0.0.1/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-11 05:15:17.000000 test_data_visualization-0.0.1/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-12 19:29:50.676405 test_data_visualization-0.0.1/data_visualization/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2013 2023-04-12 19:20:09.000000 test_data_visualization-0.0.1/data_visualization/__init__.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-11 05:42:08.000000 test_data_visualization-0.0.1/data_visualization/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-12 19:29:50.679965 test_data_visualization-0.0.1/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      630 2023-04-12 19:26:20.000000 test_data_visualization-0.0.1/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-12 19:29:50.678815 test_data_visualization-0.0.1/test_data_visualization.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      296 2023-04-12 19:29:50.000000 test_data_visualization-0.0.1/test_data_visualization.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      334 2023-04-12 19:29:50.000000 test_data_visualization-0.0.1/test_data_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-12 19:29:50.000000 test_data_visualization-0.0.1/test_data_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-12 19:29:50.000000 test_data_visualization-0.0.1/test_data_visualization.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-12 19:29:50.000000 test_data_visualization-0.0.1/test_data_visualization.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.724725 test_data_visualization-0.0.2/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 06:13:34.000000 test_data_visualization-0.0.2/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-13 06:15:17.000000 test_data_visualization-0.0.2/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      296 2023-04-13 06:15:54.724449 test_data_visualization-0.0.2/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-13 06:13:34.000000 test_data_visualization-0.0.2/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.715390 test_data_visualization-0.0.2/data_visualization/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2013 2023-04-13 06:13:34.000000 test_data_visualization-0.0.2/data_visualization/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.712918 test_data_visualization-0.0.2/data_visualization/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.716382 test_data_visualization-0.0.2/data_visualization/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.721958 test_data_visualization-0.0.2/data_visualization/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1950083 2023-04-12 19:17:22.000000 test_data_visualization-0.0.2/data_visualization/frontend/dist/assets/index-8b489cec.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-12 19:17:22.000000 test_data_visualization-0.0.2/data_visualization/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-12 19:17:32.000000 test_data_visualization-0.0.2/data_visualization/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-12 19:17:21.000000 test_data_visualization-0.0.2/data_visualization/frontend/dist/vite.svg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-13 06:13:34.000000 test_data_visualization-0.0.2/data_visualization/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 06:15:54.724823 test_data_visualization-0.0.2/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      630 2023-04-13 06:15:15.000000 test_data_visualization-0.0.2/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 06:15:54.723926 test_data_visualization-0.0.2/test_data_visualization.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      296 2023-04-13 06:15:54.000000 test_data_visualization-0.0.2/test_data_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      537 2023-04-13 06:15:54.000000 test_data_visualization-0.0.2/test_data_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 06:15:54.000000 test_data_visualization-0.0.2/test_data_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 06:15:54.000000 test_data_visualization-0.0.2/test_data_visualization.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-13 06:15:54.000000 test_data_visualization-0.0.2/test_data_visualization.egg-info/top_level.txt
```

### Comparing `test_data_visualization-0.0.1/LICENSE` & `test_data_visualization-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test_data_visualization-0.0.1/data_visualization/__init__.py` & `test_data_visualization-0.0.2/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `test_data_visualization-0.0.1/data_visualization/register.py` & `test_data_visualization-0.0.2/data_visualization/register.py`

 * *Files identical despite different names*

### Comparing `test_data_visualization-0.0.1/setup.py` & `test_data_visualization-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_data_visualization",
-    version="0.0.1",
+    version="0.0.2",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Show data in charts",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

