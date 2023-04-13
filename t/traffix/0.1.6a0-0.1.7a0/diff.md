# Comparing `tmp/traffix-0.1.6a0.tar.gz` & `tmp/traffix-0.1.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffix-0.1.6a0.tar", last modified: Thu Apr 13 18:32:33 2023, max compression
+gzip compressed data, was "traffix-0.1.7a0.tar", last modified: Thu Apr 13 18:55:37 2023, max compression
```

## Comparing `traffix-0.1.6a0.tar` & `traffix-0.1.7a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:32:33.026791 traffix-0.1.6a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 traffix-0.1.6a0/LICENSE
--rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 traffix-0.1.6a0/MANIFEST.in
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 18:32:33.026042 traffix-0.1.6a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 traffix-0.1.6a0/README.md
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 18:32:33.027081 traffix-0.1.6a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 18:32:12.000000 traffix-0.1.6a0/setup.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:32:33.020390 traffix-0.1.6a0/traffix/
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.6a0/traffix/.___init__.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.6a0/traffix/.__api.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.6a0/traffix/.__version.py
--rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 traffix-0.1.6a0/traffix/OD.py
--rw-r--r--   0 maman      (501) staff       (20)      543 2023-04-13 18:26:24.000000 traffix-0.1.6a0/traffix/__init__.py
--rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 18:29:59.000000 traffix-0.1.6a0/traffix/_version.py
--rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 traffix-0.1.6a0/traffix/add.py
--rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 traffix-0.1.6a0/traffix/flow.py
--rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 traffix-0.1.6a0/traffix/lpr.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:32:33.025074 traffix-0.1.6a0/traffix/traffix.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 18:32:32.000000 traffix-0.1.6a0/traffix/traffix.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      408 2023-04-13 18:32:32.000000 traffix-0.1.6a0/traffix/traffix.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 18:32:32.000000 traffix-0.1.6a0/traffix/traffix.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 18:32:32.000000 traffix-0.1.6a0/traffix/traffix.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)       37 2023-04-13 18:32:32.000000 traffix-0.1.6a0/traffix/traffix.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 traffix-0.1.6a0/traffix/ue.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:55:37.485759 traffix-0.1.7a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 traffix-0.1.7a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 traffix-0.1.7a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 18:55:37.485183 traffix-0.1.7a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 traffix-0.1.7a0/README.md
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 18:55:37.485946 traffix-0.1.7a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 18:54:58.000000 traffix-0.1.7a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:55:37.477088 traffix-0.1.7a0/traffix/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.7a0/traffix/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.7a0/traffix/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 traffix-0.1.7a0/traffix/OD.py
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 18:53:38.000000 traffix-0.1.7a0/traffix/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 18:55:16.000000 traffix-0.1.7a0/traffix/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 traffix-0.1.7a0/traffix/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 traffix-0.1.7a0/traffix/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 traffix-0.1.7a0/traffix/lpr.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 18:55:37.483757 traffix-0.1.7a0/traffix/traffix.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 18:55:37.000000 traffix-0.1.7a0/traffix/traffix.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      409 2023-04-13 18:55:37.000000 traffix-0.1.7a0/traffix/traffix.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 18:55:37.000000 traffix-0.1.7a0/traffix/traffix.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 18:55:37.000000 traffix-0.1.7a0/traffix/traffix.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       45 2023-04-13 18:55:37.000000 traffix-0.1.7a0/traffix/traffix.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)      542 2023-04-13 18:53:35.000000 traffix-0.1.7a0/traffix/traffix.py
+-rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 traffix-0.1.7a0/traffix/ue.py
```

### Comparing `traffix-0.1.6a0/LICENSE` & `traffix-0.1.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/PKG-INFO` & `traffix-0.1.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffix
-Version: 0.1.6a0
+Version: 0.1.7a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `traffix-0.1.6a0/README.md` & `traffix-0.1.7a0/README.md`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/setup.py` & `traffix-0.1.7a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import setup
 
 
 setup(
     name="traffix", 
-    version = "0.1.6-alpha",
+    version = "0.1.7-alpha",
     description = "A package for macroscopic transportation assignment.",
     package_dir = {"":"traffix"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Ultios/traffix",
```

### Comparing `traffix-0.1.6a0/traffix/.___init__.py` & `traffix-0.1.7a0/traffix/.___init__.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/.__api.py` & `traffix-0.1.7a0/traffix/.__version.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/OD.py` & `traffix-0.1.7a0/traffix/OD.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/__init__.py` & `traffix-0.1.7a0/traffix/traffix.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 from .OD import OD_nodes_list
 from .OD import OD_shortest_path
 from .ue import line_search
 from .ue import bisection
 from .ue import update
 from .ue import update_mainflow
 from .ue import CCA
-from ._version import __version__
+from ._version import __version__
```

### Comparing `traffix-0.1.6a0/traffix/add.py` & `traffix-0.1.7a0/traffix/add.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/flow.py` & `traffix-0.1.7a0/traffix/flow.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/lpr.py` & `traffix-0.1.7a0/traffix/lpr.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.6a0/traffix/traffix.egg-info/PKG-INFO` & `traffix-0.1.7a0/traffix/traffix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffix
-Version: 0.1.6a0
+Version: 0.1.7a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `traffix-0.1.6a0/traffix/ue.py` & `traffix-0.1.7a0/traffix/ue.py`

 * *Files identical despite different names*

