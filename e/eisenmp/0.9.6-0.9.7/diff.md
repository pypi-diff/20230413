# Comparing `tmp/eisenmp-0.9.6.tar.gz` & `tmp/eisenmp-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp-0.9.6.tar", last modified: Thu Apr 13 16:35:11 2023, max compression
+gzip compressed data, was "eisenmp-0.9.7.tar", last modified: Thu Apr 13 20:59:19 2023, max compression
```

## Comparing `eisenmp-0.9.6.tar` & `eisenmp-0.9.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.950544 eisenmp-0.9.6/
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.6/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.6/LICENSE.rst
--rw-rw-rw-   0        0        0      187 2023-04-13 16:26:07.000000 eisenmp-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0     9965 2023-04-13 16:35:11.951524 eisenmp-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2023-04-13 16:26:07.000000 eisenmp-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.785710 eisenmp-0.9.6/docs/
--rw-rw-rw-   0        0        0      756 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/Makefile
--rwxrwxrwx   0        0        0      804 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.861812 eisenmp-0.9.6/docs/source/
--rw-rw-rw-   0        0        0     6979 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.869612 eisenmp-0.9.6/docs/source/_static/
--rw-rw-rw-   0        0        0      458 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/_static/css-style.css
--rw-rw-rw-   0        0        0     3283 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/conf.py
--rw-rw-rw-   0        0        0     2504 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.rst
--rw-rw-rw-   0        0        0      747 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.utils.rst
--rw-rw-rw-   0        0        0      806 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.utils_exa.rst
--rw-rw-rw-   0        0        0    27208 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp_logo.png
--rw-rw-rw-   0        0        0      237 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/index.rst
--rw-rw-rw-   0        0        0       65 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.893994 eisenmp-0.9.6/eisenmp/
--rw-rw-rw-   0        0        0     4471 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/__init__.py
--rw-rw-rw-   0        0        0     7399 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_procenv.py
--rw-rw-rw-   0        0        0    10522 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_q_coll.py
--rw-rw-rw-   0        0        0     5401 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_worker_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.949568 eisenmp-0.9.6/eisenmp/utils/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_constants.py
--rw-rw-rw-   0        0        0     3918 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_info.py
--rw-rw-rw-   0        0        0     1434 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.934937 eisenmp-0.9.6/eisenmp.egg-info/
--rw-rw-rw-   0        0        0     9965 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 16:35:10.000000 eisenmp-0.9.6/eisenmp.egg-info/zip-safe
--rw-rw-rw-   0        0        0      921 2023-04-13 16:26:07.000000 eisenmp-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0      392 2023-04-13 16:35:11.954448 eisenmp-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.419350 eisenmp-0.9.7/
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.7/LICENSE.rst
+-rw-rw-rw-   0        0        0      187 2023-04-13 16:26:07.000000 eisenmp-0.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     9965 2023-04-13 20:59:19.420325 eisenmp-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7437 2023-04-13 16:26:07.000000 eisenmp-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.353025 eisenmp-0.9.7/docs/
+-rw-rw-rw-   0        0        0      756 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.371565 eisenmp-0.9.7/docs/source/
+-rw-rw-rw-   0        0        0     6979 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.373508 eisenmp-0.9.7/docs/source/_static/
+-rw-rw-rw-   0        0        0      458 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/_static/css-style.css
+-rw-rw-rw-   0        0        0     3283 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2504 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.rst
+-rw-rw-rw-   0        0        0      747 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.utils.rst
+-rw-rw-rw-   0        0        0      806 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.utils_exa.rst
+-rw-rw-rw-   0        0        0    27208 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp_logo.png
+-rw-rw-rw-   0        0        0      237 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0       65 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.381313 eisenmp-0.9.7/eisenmp/
+-rw-rw-rw-   0        0        0     4471 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/__init__.py
+-rw-rw-rw-   0        0        0     7459 2023-04-13 20:24:29.000000 eisenmp-0.9.7/eisenmp/eisenmp_procenv.py
+-rw-rw-rw-   0        0        0    10522 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/eisenmp_q_coll.py
+-rw-rw-rw-   0        0        0     5401 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/eisenmp_worker_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.418374 eisenmp-0.9.7/eisenmp/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_constants.py
+-rw-rw-rw-   0        0        0     3918 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_info.py
+-rw-rw-rw-   0        0        0     1434 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.405694 eisenmp-0.9.7/eisenmp.egg-info/
+-rw-rw-rw-   0        0        0     9965 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 20:59:18.000000 eisenmp-0.9.7/eisenmp.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      921 2023-04-13 20:55:32.000000 eisenmp-0.9.7/pyproject.toml
+-rw-rw-rw-   0        0        0      392 2023-04-13 20:59:19.428127 eisenmp-0.9.7/setup.cfg
```

### Comparing `eisenmp-0.9.6/LICENSE` & `eisenmp-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/LICENSE.rst` & `eisenmp-0.9.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/PKG-INFO` & `eisenmp-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.6
+Version: 0.9.7
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
```

### Comparing `eisenmp-0.9.6/README.md` & `eisenmp-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/Makefile` & `eisenmp-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/make.bat` & `eisenmp-0.9.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/README.rst` & `eisenmp-0.9.7/docs/source/README.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/conf.py` & `eisenmp-0.9.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/eisenmp.rst` & `eisenmp-0.9.7/docs/source/eisenmp.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/eisenmp.utils.rst` & `eisenmp-0.9.7/docs/source/eisenmp.utils.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/eisenmp.utils_exa.rst` & `eisenmp-0.9.7/docs/source/eisenmp.utils_exa.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/docs/source/eisenmp_logo.png` & `eisenmp-0.9.7/docs/source/eisenmp_logo.png`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/__init__.py` & `eisenmp-0.9.7/eisenmp/__init__.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/eisenmp_procenv.py` & `eisenmp-0.9.7/eisenmp/eisenmp_procenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 import multiprocessing as mp
 from multiprocessing import Queue
 
 import eisenmp.eisenmp_worker_loader as loader
 import eisenmp.utils.eisenmp_utils as e_utils
 import eisenmp.utils.eisenmp_constants as const
 
+mp.set_start_method('spawn', force=True)  # override in ProcEnv.run_proc
+
 
 class ProcEnv:
     """Create the environment for worker processes on CPUs.
     All queues shared among processes.
     'maxsize=1' can be altered, should be tested and documented.
 
-    - **Queues ONLY** in this version
+    - **Queues ONLY**
     - custom Queue builder with a queue in a dict to show a name
     - another Queue builder can add a category name, dict in dict
 
     """
 
     def __init__(self):
         # CPU - process
```

### Comparing `eisenmp-0.9.6/eisenmp/eisenmp_q_coll.py` & `eisenmp-0.9.7/eisenmp/eisenmp_q_coll.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/eisenmp_worker_loader.py` & `eisenmp-0.9.7/eisenmp/eisenmp_worker_loader.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/utils/eisenmp_constants.py` & `eisenmp-0.9.7/eisenmp/utils/eisenmp_constants.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/utils/eisenmp_info.py` & `eisenmp-0.9.7/eisenmp/utils/eisenmp_info.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp/utils/eisenmp_utils.py` & `eisenmp-0.9.7/eisenmp/utils/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/eisenmp.egg-info/PKG-INFO` & `eisenmp-0.9.7/eisenmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.6
+Version: 0.9.7
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
```

### Comparing `eisenmp-0.9.6/eisenmp.egg-info/SOURCES.txt` & `eisenmp-0.9.7/eisenmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.6/pyproject.toml` & `eisenmp-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp"
-version = "0.9.6"
+version = "0.9.7"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,"
 keywords = ['multiprocess framework', 'python multiprocessor framework']
 license = {file = "LICENSE.rst"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

