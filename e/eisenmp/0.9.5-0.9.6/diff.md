# Comparing `tmp/eisenmp-0.9.5.tar.gz` & `tmp/eisenmp-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp-0.9.5.tar", last modified: Thu Apr 13 09:03:18 2023, max compression
+gzip compressed data, was "eisenmp-0.9.6.tar", last modified: Thu Apr 13 16:35:11 2023, max compression
```

## Comparing `eisenmp-0.9.5.tar` & `eisenmp-0.9.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.427952 eisenmp-0.9.5/
--rw-rw-rw-   0        0        0     1525 2023-04-06 10:49:51.000000 eisenmp-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-06 10:49:51.000000 eisenmp-0.9.5/LICENSE.rst
--rw-rw-rw-   0        0        0      187 2023-04-06 10:49:51.000000 eisenmp-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9965 2023-04-13 09:03:18.427952 eisenmp-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2023-04-13 00:15:44.000000 eisenmp-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.265143 eisenmp-0.9.5/docs/
--rw-rw-rw-   0        0        0      756 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/Makefile
--rwxrwxrwx   0        0        0      804 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.349815 eisenmp-0.9.5/docs/source/
--rw-rw-rw-   0        0        0     6979 2023-04-12 21:34:45.000000 eisenmp-0.9.5/docs/source/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.349815 eisenmp-0.9.5/docs/source/_static/
--rw-rw-rw-   0        0        0      458 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/source/_static/css-style.css
--rw-rw-rw-   0        0        0     3283 2023-04-12 21:37:25.000000 eisenmp-0.9.5/docs/source/conf.py
--rw-rw-rw-   0        0        0     2504 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.rst
--rw-rw-rw-   0        0        0      747 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.utils.rst
--rw-rw-rw-   0        0        0      806 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/eisenmp.utils_exa.rst
--rw-rw-rw-   0        0        0    27208 2023-04-12 20:01:06.000000 eisenmp-0.9.5/docs/source/eisenmp_logo.png
--rw-rw-rw-   0        0        0      237 2023-04-12 20:26:08.000000 eisenmp-0.9.5/docs/source/index.rst
--rw-rw-rw-   0        0        0       65 2023-04-12 20:08:53.000000 eisenmp-0.9.5/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.381082 eisenmp-0.9.5/eisenmp/
--rw-rw-rw-   0        0        0     4471 2023-04-12 16:40:53.000000 eisenmp-0.9.5/eisenmp/__init__.py
--rw-rw-rw-   0        0        0     7399 2023-04-12 19:09:27.000000 eisenmp-0.9.5/eisenmp/eisenmp_procenv.py
--rw-rw-rw-   0        0        0    10522 2023-04-11 18:12:16.000000 eisenmp-0.9.5/eisenmp/eisenmp_q_coll.py
--rw-rw-rw-   0        0        0     5401 2023-04-12 09:25:01.000000 eisenmp-0.9.5/eisenmp/eisenmp_worker_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.427952 eisenmp-0.9.5/eisenmp/utils/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:49:51.000000 eisenmp-0.9.5/eisenmp/utils/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-10 16:30:06.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_constants.py
--rw-rw-rw-   0        0        0     3918 2023-04-10 10:29:05.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_info.py
--rw-rw-rw-   0        0        0     1434 2023-04-11 11:41:34.000000 eisenmp-0.9.5/eisenmp/utils/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:03:18.412341 eisenmp-0.9.5/eisenmp.egg-info/
--rw-rw-rw-   0        0        0     9965 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 09:03:18.000000 eisenmp-0.9.5/eisenmp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 09:03:17.000000 eisenmp-0.9.5/eisenmp.egg-info/zip-safe
--rw-rw-rw-   0        0        0      921 2023-04-12 20:36:14.000000 eisenmp-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0      392 2023-04-13 09:03:18.443591 eisenmp-0.9.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.950544 eisenmp-0.9.6/
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.6/LICENSE.rst
+-rw-rw-rw-   0        0        0      187 2023-04-13 16:26:07.000000 eisenmp-0.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     9965 2023-04-13 16:35:11.951524 eisenmp-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7437 2023-04-13 16:26:07.000000 eisenmp-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.785710 eisenmp-0.9.6/docs/
+-rw-rw-rw-   0        0        0      756 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.861812 eisenmp-0.9.6/docs/source/
+-rw-rw-rw-   0        0        0     6979 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.869612 eisenmp-0.9.6/docs/source/_static/
+-rw-rw-rw-   0        0        0      458 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/_static/css-style.css
+-rw-rw-rw-   0        0        0     3283 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2504 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.rst
+-rw-rw-rw-   0        0        0      747 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.utils.rst
+-rw-rw-rw-   0        0        0      806 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp.utils_exa.rst
+-rw-rw-rw-   0        0        0    27208 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/eisenmp_logo.png
+-rw-rw-rw-   0        0        0      237 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0       65 2023-04-13 16:26:07.000000 eisenmp-0.9.6/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.893994 eisenmp-0.9.6/eisenmp/
+-rw-rw-rw-   0        0        0     4471 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/__init__.py
+-rw-rw-rw-   0        0        0     7399 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_procenv.py
+-rw-rw-rw-   0        0        0    10522 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_q_coll.py
+-rw-rw-rw-   0        0        0     5401 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/eisenmp_worker_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.949568 eisenmp-0.9.6/eisenmp/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_constants.py
+-rw-rw-rw-   0        0        0     3918 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_info.py
+-rw-rw-rw-   0        0        0     1434 2023-04-13 16:26:07.000000 eisenmp-0.9.6/eisenmp/utils/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:35:11.934937 eisenmp-0.9.6/eisenmp.egg-info/
+-rw-rw-rw-   0        0        0     9965 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 16:35:11.000000 eisenmp-0.9.6/eisenmp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 16:35:10.000000 eisenmp-0.9.6/eisenmp.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      921 2023-04-13 16:26:07.000000 eisenmp-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0      392 2023-04-13 16:35:11.954448 eisenmp-0.9.6/setup.cfg
```

### Comparing `eisenmp-0.9.5/LICENSE` & `eisenmp-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/LICENSE.rst` & `eisenmp-0.9.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/PKG-INFO` & `eisenmp-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.5
+Version: 0.9.6
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
```

### Comparing `eisenmp-0.9.5/README.md` & `eisenmp-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/Makefile` & `eisenmp-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/make.bat` & `eisenmp-0.9.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/README.rst` & `eisenmp-0.9.6/docs/source/README.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/conf.py` & `eisenmp-0.9.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/eisenmp.rst` & `eisenmp-0.9.6/docs/source/eisenmp.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/eisenmp.utils.rst` & `eisenmp-0.9.6/docs/source/eisenmp.utils.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/eisenmp.utils_exa.rst` & `eisenmp-0.9.6/docs/source/eisenmp.utils_exa.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/docs/source/eisenmp_logo.png` & `eisenmp-0.9.6/docs/source/eisenmp_logo.png`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/__init__.py` & `eisenmp-0.9.6/eisenmp/__init__.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/eisenmp_procenv.py` & `eisenmp-0.9.6/eisenmp/eisenmp_procenv.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/eisenmp_q_coll.py` & `eisenmp-0.9.6/eisenmp/eisenmp_q_coll.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/eisenmp_worker_loader.py` & `eisenmp-0.9.6/eisenmp/eisenmp_worker_loader.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/utils/eisenmp_constants.py` & `eisenmp-0.9.6/eisenmp/utils/eisenmp_constants.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/utils/eisenmp_info.py` & `eisenmp-0.9.6/eisenmp/utils/eisenmp_info.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp/utils/eisenmp_utils.py` & `eisenmp-0.9.6/eisenmp/utils/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/eisenmp.egg-info/PKG-INFO` & `eisenmp-0.9.6/eisenmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp
-Version: 0.9.5
+Version: 0.9.6
 Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, René Horn
```

### Comparing `eisenmp-0.9.5/eisenmp.egg-info/SOURCES.txt` & `eisenmp-0.9.6/eisenmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.5/pyproject.toml` & `eisenmp-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp"
-version = "0.9.5"
+version = "0.9.6"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,"
 keywords = ['multiprocess framework', 'python multiprocessor framework']
 license = {file = "LICENSE.rst"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

