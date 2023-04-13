# Comparing `tmp/simplepush-2.2.2.tar.gz` & `tmp/simplepush-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepush-2.2.2.tar", last modified: Fri Mar 24 11:18:33 2023, max compression
+gzip compressed data, was "simplepush-2.2.3.tar", last modified: Thu Apr 13 18:48:48 2023, max compression
```

## Comparing `simplepush-2.2.2.tar` & `simplepush-2.2.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-03-24 11:18:33.471512 simplepush-2.2.2/
--rw-r--r--   0 tymm       (501) staff       (20)     1079 2023-03-21 16:52:39.000000 simplepush-2.2.2/LICENSE.txt
--rw-r--r--   0 tymm       (501) staff       (20)     2288 2023-03-24 11:18:33.471391 simplepush-2.2.2/PKG-INFO
--rw-r--r--   0 tymm       (501) staff       (20)     1780 2023-03-21 16:52:09.000000 simplepush-2.2.2/README.md
--rw-r--r--   0 tymm       (501) staff       (20)      631 2023-03-24 11:17:09.000000 simplepush-2.2.2/pyproject.toml
--rw-r--r--   0 tymm       (501) staff       (20)       38 2023-03-24 11:18:33.471559 simplepush-2.2.2/setup.cfg
-drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-03-24 11:18:33.470166 simplepush-2.2.2/src/
-drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-03-24 11:18:33.470739 simplepush-2.2.2/src/simplepush/
--rw-r--r--   0 tymm       (501) staff       (20)      131 2023-03-22 22:17:04.000000 simplepush-2.2.2/src/simplepush/__init__.py
--rw-r--r--   0 tymm       (501) staff       (20)    13272 2023-03-23 19:23:30.000000 simplepush-2.2.2/src/simplepush/simplepush.py
-drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-03-24 11:18:33.471205 simplepush-2.2.2/src/simplepush.egg-info/
--rw-r--r--   0 tymm       (501) staff       (20)     2288 2023-03-24 11:18:33.000000 simplepush-2.2.2/src/simplepush.egg-info/PKG-INFO
--rw-r--r--   0 tymm       (501) staff       (20)      244 2023-03-24 11:18:33.000000 simplepush-2.2.2/src/simplepush.egg-info/SOURCES.txt
--rw-r--r--   0 tymm       (501) staff       (20)        1 2023-03-24 11:18:33.000000 simplepush-2.2.2/src/simplepush.egg-info/dependency_links.txt
--rw-r--r--   0 tymm       (501) staff       (20)       11 2023-03-24 11:18:33.000000 simplepush-2.2.2/src/simplepush.egg-info/top_level.txt
+drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-04-13 18:48:48.441871 simplepush-2.2.3/
+-rw-r--r--   0 tymm       (501) staff       (20)     1079 2023-04-13 18:46:30.000000 simplepush-2.2.3/LICENSE.txt
+-rw-r--r--   0 tymm       (501) staff       (20)     2288 2023-04-13 18:48:48.441768 simplepush-2.2.3/PKG-INFO
+-rw-r--r--   0 tymm       (501) staff       (20)     1780 2023-04-13 18:46:30.000000 simplepush-2.2.3/README.md
+-rw-r--r--   0 tymm       (501) staff       (20)      637 2023-04-13 18:46:52.000000 simplepush-2.2.3/pyproject.toml
+-rw-r--r--   0 tymm       (501) staff       (20)       38 2023-04-13 18:48:48.441905 simplepush-2.2.3/setup.cfg
+drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-04-13 18:48:48.440501 simplepush-2.2.3/src/
+drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-04-13 18:48:48.441052 simplepush-2.2.3/src/simplepush/
+-rw-r--r--   0 tymm       (501) staff       (20)      131 2023-04-13 18:46:30.000000 simplepush-2.2.3/src/simplepush/__init__.py
+-rw-r--r--   0 tymm       (501) staff       (20)    13272 2023-04-13 18:46:30.000000 simplepush-2.2.3/src/simplepush/simplepush.py
+drwxr-xr-x   0 tymm       (501) staff       (20)        0 2023-04-13 18:48:48.441604 simplepush-2.2.3/src/simplepush.egg-info/
+-rw-r--r--   0 tymm       (501) staff       (20)     2288 2023-04-13 18:48:48.000000 simplepush-2.2.3/src/simplepush.egg-info/PKG-INFO
+-rw-r--r--   0 tymm       (501) staff       (20)      281 2023-04-13 18:48:48.000000 simplepush-2.2.3/src/simplepush.egg-info/SOURCES.txt
+-rw-r--r--   0 tymm       (501) staff       (20)        1 2023-04-13 18:48:48.000000 simplepush-2.2.3/src/simplepush.egg-info/dependency_links.txt
+-rw-r--r--   0 tymm       (501) staff       (20)       30 2023-04-13 18:48:48.000000 simplepush-2.2.3/src/simplepush.egg-info/requires.txt
+-rw-r--r--   0 tymm       (501) staff       (20)       11 2023-04-13 18:48:48.000000 simplepush-2.2.3/src/simplepush.egg-info/top_level.txt
```

### Comparing `simplepush-2.2.2/LICENSE.txt` & `simplepush-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simplepush-2.2.2/PKG-INFO` & `simplepush-2.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepush
-Version: 2.2.2
+Version: 2.2.3
 Summary: Simplepush Python Library
 Author-email: Timm Schaeuble <contact@simplepush.io>
 Project-URL: Homepage, https://github.com/simplepush/simplepush-python
 Project-URL: Bug Tracker, https://github.com/simplepush/simplepush-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplepush-2.2.2/README.md` & `simplepush-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `simplepush-2.2.2/pyproject.toml` & `simplepush-2.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
-requires = [
-    "setuptools>=61.0",
-    "requests",
-    "cryptography",
-    "aiohttp"
-]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplepush"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
   { name="Timm Schaeuble", email="contact@simplepush.io" },
 ]
 description = "Simplepush Python Library"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "requests",
+  "cryptography",
+  "aiohttp"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/simplepush/simplepush-python"
 "Bug Tracker" = "https://github.com/simplepush/simplepush-python/issues"
```

### Comparing `simplepush-2.2.2/src/simplepush/simplepush.py` & `simplepush-2.2.3/src/simplepush/simplepush.py`

 * *Files identical despite different names*

### Comparing `simplepush-2.2.2/src/simplepush.egg-info/PKG-INFO` & `simplepush-2.2.3/src/simplepush.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepush
-Version: 2.2.2
+Version: 2.2.3
 Summary: Simplepush Python Library
 Author-email: Timm Schaeuble <contact@simplepush.io>
 Project-URL: Homepage, https://github.com/simplepush/simplepush-python
 Project-URL: Bug Tracker, https://github.com/simplepush/simplepush-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

