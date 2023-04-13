# Comparing `tmp/alfred5-1.1.1.tar.gz` & `tmp/alfred5-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.1.1.tar", last modified: Tue Apr 11 01:04:37 2023, max compression
+gzip compressed data, was "alfred5-1.1.2.tar", last modified: Thu Apr 13 21:31:33 2023, max compression
```

## Comparing `alfred5-1.1.1.tar` & `alfred5-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-11 01:04:28.000000 alfred5-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 01:04:28.000000 alfred5-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-11 01:04:37.079642 alfred5-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:04:36.000000 alfred5-1.1.1/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-11 01:04:28.000000 alfred5-1.1.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:04:37.079642 alfred5-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-11 01:04:28.000000 alfred5-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:28.000000 alfred5-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 01:04:28.000000 alfred5-1.1.1/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 21:31:22.000000 alfred5-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 21:31:22.000000 alfred5-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-13 21:31:33.867080 alfred5-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:31:22.000000 alfred5-1.1.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:31:33.867080 alfred5-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 21:31:22.000000 alfred5-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:22.000000 alfred5-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 21:31:22.000000 alfred5-1.1.2/tests/test_snippets.py
```

### Comparing `alfred5-1.1.1/LICENSE` & `alfred5-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.1/PKG-INFO` & `alfred5-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
```

### Comparing `alfred5-1.1.1/alfred5/client.py` & `alfred5-1.1.2/alfred5/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         with self.db_results.open("r") as f:
             data = yaml_load(f) or {}
         data[self.bare_query] = [
             {
                 "title": result.title,
                 "subtitle": result.subtitle,
                 "icon_path": result.icon.path if result.icon else None,
+                "arg": result.arg,
             }
             for result in self.results
         ]
         with self.db_results.open("w") as f:
             yaml_dump(data, f)
             self.log(f"cached response to {self.db_results}")
 
@@ -165,14 +166,15 @@
                     self.results = [
                         Result(
                             title=result["title"],
                             subtitle=result["subtitle"],
                             icon=Result.Icon(result["icon_path"])
                             if result["icon_path"]
                             else None,
+                            arg=result["arg"],
                         )
                         for result in data[self.bare_query]
                     ]
                     self.log(f"found: {self.bare_query} in {self.db_results}")
                     return True
         self.log(f"not found `{self.bare_query}` in `{self.db_results}`")
         return False
```

### Comparing `alfred5-1.1.1/alfred5/icons/download.png` & `alfred5-1.1.2/alfred5/icons/download.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.1/alfred5/icons/error.png` & `alfred5-1.1.2/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.1/alfred5/models.py` & `alfred5-1.1.2/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.1/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.2/alfred5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
```

### Comparing `alfred5-1.1.1/docs/README.md` & `alfred5-1.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.1/setup.py` & `alfred5-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 DESCRIPTION = "Simple python wrapper for alfred5 workflow / snippets"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 KEYWORDS = [
     "alfred",
     "alfred5",
```

