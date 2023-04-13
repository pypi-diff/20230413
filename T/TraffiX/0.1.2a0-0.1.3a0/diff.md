# Comparing `tmp/TraffiX-0.1.2a0.tar.gz` & `tmp/TraffiX-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TraffiX-0.1.2a0.tar", last modified: Thu Apr 13 16:19:12 2023, max compression
+gzip compressed data, was "TraffiX-0.1.3a0.tar", last modified: Thu Apr 13 17:00:24 2023, max compression
```

## Comparing `TraffiX-0.1.2a0.tar` & `TraffiX-0.1.3a0.tar`

### file list

```diff
@@ -1,14 +1,26 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 16:19:12.484125 TraffiX-0.1.2a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.2a0/LICENSE
--rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.2a0/MANIFEST.in
--rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 16:19:12.483551 TraffiX-0.1.2a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.2a0/README.md
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 16:19:12.476716 TraffiX-0.1.2a0/TraffiX/
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 16:19:12.482532 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 16:19:12.000000 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      232 2023-04-13 16:19:12.000000 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 16:19:12.000000 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 16:19:12.000000 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 16:19:12.000000 TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 16:19:12.484326 TraffiX-0.1.2a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1181 2023-04-13 16:18:45.000000 TraffiX-0.1.2a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.240562 TraffiX-0.1.3a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.3a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.3a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 17:00:24.239907 TraffiX-0.1.3a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.3a0/README.md
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.229366 TraffiX-0.1.3a0/TraffiX/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.__api.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      519 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/OD.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.237082 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      439 2023-04-13 17:00:24.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       46 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)       75 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)      622 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/_api.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5245 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1322 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      670 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/lpr.py
+-rw-r--r--   0 maman      (501) staff       (20)      228 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/me2.py
+-rw-r--r--   0 maman      (501) staff       (20)     2123 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/ue.py
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 17:00:24.240702 TraffiX-0.1.3a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1181 2023-04-13 16:59:32.000000 TraffiX-0.1.3a0/setup.py
```

### Comparing `TraffiX-0.1.2a0/LICENSE` & `TraffiX-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.2a0/PKG-INFO` & `TraffiX-0.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/StraPy
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TraffiX-0.1.2a0/README.md` & `TraffiX-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.2a0/TraffiX/TraffiX.egg-info/PKG-INFO` & `TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/StraPy
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TraffiX-0.1.2a0/setup.py` & `TraffiX-0.1.3a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import setup
 
 
 setup(
     name="TraffiX", 
-    version = "0.1.2-alpha",
+    version = "0.1.3-alpha",
     description = "A package for macroscopic transportation assignment.",
     package_dir = {"":"TraffiX"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Ultios/StraPy",
```

