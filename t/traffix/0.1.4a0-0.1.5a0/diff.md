# Comparing `tmp/TraffiX-0.1.4a0.tar.gz` & `tmp/traffix-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TraffiX-0.1.4a0.tar", last modified: Thu Apr 13 17:36:42 2023, max compression
+gzip compressed data, was "traffix-0.1.5a0.tar", last modified: Thu Apr 13 17:50:50 2023, max compression
```

## Comparing `TraffiX-0.1.4a0.tar` & `traffix-0.1.5a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.756472 TraffiX-0.1.4a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.4a0/LICENSE
--rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.4a0/MANIFEST.in
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:36:42.755790 TraffiX-0.1.4a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.4a0/README.md
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 17:36:42.756669 TraffiX-0.1.4a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 17:26:03.000000 TraffiX-0.1.4a0/setup.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.750972 TraffiX-0.1.4a0/traffix/
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.___init__.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.__api.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.__version.py
--rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 TraffiX-0.1.4a0/traffix/OD.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.754903 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      424 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)       42 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)       75 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/__init__.py
--rw-r--r--   0 maman      (501) staff       (20)      567 2023-04-13 17:35:20.000000 TraffiX-0.1.4a0/traffix/_api.py
--rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 17:25:45.000000 TraffiX-0.1.4a0/traffix/_version.py
--rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 TraffiX-0.1.4a0/traffix/add.py
--rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 TraffiX-0.1.4a0/traffix/flow.py
--rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 TraffiX-0.1.4a0/traffix/lpr.py
--rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 TraffiX-0.1.4a0/traffix/ue.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:50:50.061578 traffix-0.1.5a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 traffix-0.1.5a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 traffix-0.1.5a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:50:50.061163 traffix-0.1.5a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 traffix-0.1.5a0/README.md
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 17:50:50.061765 traffix-0.1.5a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 17:49:08.000000 traffix-0.1.5a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:50:50.056529 traffix-0.1.5a0/traffix/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.5a0/traffix/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.5a0/traffix/.__api.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.5a0/traffix/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 traffix-0.1.5a0/traffix/OD.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:50:50.059538 traffix-0.1.5a0/traffix/TraffiX.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:50:49.000000 traffix-0.1.5a0/traffix/TraffiX.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      584 2023-04-13 17:50:49.000000 traffix-0.1.5a0/traffix/TraffiX.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 17:50:49.000000 traffix-0.1.5a0/traffix/TraffiX.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 17:50:49.000000 traffix-0.1.5a0/traffix/TraffiX.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       42 2023-04-13 17:50:49.000000 traffix-0.1.5a0/traffix/TraffiX.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)       75 2023-04-13 16:58:26.000000 traffix-0.1.5a0/traffix/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)      567 2023-04-13 17:35:20.000000 traffix-0.1.5a0/traffix/_api.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 17:49:45.000000 traffix-0.1.5a0/traffix/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 traffix-0.1.5a0/traffix/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 traffix-0.1.5a0/traffix/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 traffix-0.1.5a0/traffix/lpr.py
+-rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 traffix-0.1.5a0/traffix/ue.py
```

### Comparing `TraffiX-0.1.4a0/LICENSE` & `traffix-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/PKG-INFO` & `traffix-0.1.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TraffiX
-Version: 0.1.4a0
+Name: traffix
+Version: 0.1.5a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TraffiX-0.1.4a0/README.md` & `traffix-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/setup.py` & `traffix-0.1.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import setup
 
 
 setup(
-    name="TraffiX", 
-    version = "0.1.4-alpha",
+    name="traffix", 
+    version = "0.1.5-alpha",
     description = "A package for macroscopic transportation assignment.",
     package_dir = {"":"traffix"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Ultios/traffix",
```

### Comparing `TraffiX-0.1.4a0/traffix/.___init__.py` & `traffix-0.1.5a0/traffix/.___init__.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/.__api.py` & `traffix-0.1.5a0/traffix/.__api.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/.__version.py` & `traffix-0.1.5a0/traffix/.__version.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/OD.py` & `traffix-0.1.5a0/traffix/OD.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/TraffiX.egg-info/PKG-INFO` & `traffix-0.1.5a0/traffix/TraffiX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TraffiX
-Version: 0.1.4a0
+Name: traffix
+Version: 0.1.5a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TraffiX-0.1.4a0/traffix/_api.py` & `traffix-0.1.5a0/traffix/_api.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/add.py` & `traffix-0.1.5a0/traffix/add.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/flow.py` & `traffix-0.1.5a0/traffix/flow.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/lpr.py` & `traffix-0.1.5a0/traffix/lpr.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.4a0/traffix/ue.py` & `traffix-0.1.5a0/traffix/ue.py`

 * *Files identical despite different names*

