# Comparing `tmp/taipy-2.1.0.tar.gz` & `tmp/taipy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.1.0.tar", last modified: Tue Jan 31 19:44:24 2023, max compression
+gzip compressed data, was "taipy-2.2.0.tar", last modified: Thu Apr 13 18:52:50 2023, max compression
```

## Comparing `taipy-2.1.0.tar` & `taipy-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 19:44:24.944095 taipy-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)    11353 2023-01-31 19:44:08.000000 taipy-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-01-31 19:44:08.000000 taipy-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3236 2023-01-31 19:44:24.944095 taipy-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2366 2023-01-31 19:44:08.000000 taipy-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-31 19:44:24.944095 taipy-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2546 2023-01-31 19:44:08.000000 taipy-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 19:44:24.940095 taipy-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 19:44:24.944095 taipy-2.1.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (116)     2644 2023-01-31 19:44:08.000000 taipy-2.1.0/src/taipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1914 2023-01-31 19:44:08.000000 taipy-2.1.0/src/taipy/_run.py
--rw-r--r--   0 runner    (1001) docker     (116)       37 2023-01-31 19:44:08.000000 taipy-2.1.0/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (116)      997 2023-01-31 19:44:08.000000 taipy-2.1.0/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 19:44:24.944095 taipy-2.1.0/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3236 2023-01-31 19:44:24.000000 taipy-2.1.0/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      318 2023-01-31 19:44:24.000000 taipy-2.1.0/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-31 19:44:24.000000 taipy-2.1.0/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-31 19:44:18.000000 taipy-2.1.0/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      233 2023-01-31 19:44:24.000000 taipy-2.1.0/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-01-31 19:44:24.000000 taipy-2.1.0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.221018 taipy-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-13 18:52:40.000000 taipy-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 18:52:40.000000 taipy-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 18:52:50.217018 taipy-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-13 18:52:40.000000 taipy-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:52:50.221018 taipy-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-13 18:52:40.000000 taipy-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:43.000000 taipy-2.2.0/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-13 18:52:40.000000 taipy-2.2.0/tests/test_run.py
```

### Comparing `taipy-2.1.0/LICENSE` & `taipy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.1.0/PKG-INFO` & `taipy-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.1.0
+Version: 2.2.0
 Summary: The Python application builder. Turns Data and AI algorithms into full web apps in no time.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-2.1.0/README.md` & `taipy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-2.1.0/setup.py` & `taipy-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 with open(f"src{os.sep}taipy{os.sep}version.json") as version_file:
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
-    "taipy-gui>=2.1,<2.2",
-    "taipy-rest>=2.1,<2.2",
+    "taipy-gui>=2.2,<2.3",
+    "taipy-rest>=2.2,<2.3",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "ngrok": ["pyngrok>=5"],
     "image": ["python-magic;platform_system!='Windows'", "python-magic-bin;platform_system=='Windows'"],
```

### Comparing `taipy-2.1.0/src/taipy/__init__.py` & `taipy-2.2.0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-2.1.0/src/taipy/_run.py` & `taipy-2.2.0/src/taipy/_run.py`

 * *Files identical despite different names*

### Comparing `taipy-2.1.0/src/taipy/version.py` & `taipy-2.2.0/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.1.0/src/taipy.egg-info/PKG-INFO` & `taipy-2.2.0/src/taipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy
-Version: 2.1.0
+Version: 2.2.0
 Summary: The Python application builder. Turns Data and AI algorithms into full web apps in no time.
 Home-page: https://github.com/avaiga/taipy
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy
 Classifier: Intended Audience :: Developers
```

