# Comparing `tmp/data_cliff-0.1.0.tar.gz` & `tmp/data_cliff-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_cliff-0.1.0.tar", last modified: Sat Mar 25 18:23:46 2023, max compression
+gzip compressed data, was "data_cliff-0.1.2.tar", last modified: Thu Apr 13 12:07:20 2023, max compression
```

## Comparing `data_cliff-0.1.0.tar` & `data_cliff-0.1.2.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)      165 2023-03-25 18:23:38.000000 data_cliff-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3553 2023-03-25 18:23:38.000000 data_cliff-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)       89 2023-03-25 18:23:38.000000 data_cliff-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)      583 2023-03-25 18:23:38.000000 data_cliff-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      262 2023-03-25 18:23:38.000000 data_cliff-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3414 2023-03-25 18:23:46.070165 data_cliff-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2562 2023-03-25 18:23:38.000000 data_cliff-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.066165 data_cliff-0.1.0/data_cliff/
--rw-r--r--   0 runner    (1001) docker     (116)      137 2023-03-25 18:23:38.000000 data_cliff-0.1.0/data_cliff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1490 2023-03-25 18:23:38.000000 data_cliff-0.1.0/data_cliff/arg_parse.py
--rw-r--r--   0 runner    (1001) docker     (116)      444 2023-03-25 18:23:38.000000 data_cliff-0.1.0/data_cliff/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     3209 2023-03-25 18:23:38.000000 data_cliff-0.1.0/data_cliff/data_cliff.py
--rw-r--r--   0 runner    (1001) docker     (116)      462 2023-03-25 18:23:38.000000 data_cliff-0.1.0/data_cliff/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/data_cliff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3414 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       11 2023-03-25 18:23:46.000000 data_cliff-0.1.0/data_cliff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      611 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     4814 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)      620 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/data_cliff.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      307 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)      808 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       67 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)       27 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)      381 2023-03-25 18:23:38.000000 data_cliff-0.1.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)      614 2023-03-25 18:23:46.070165 data_cliff-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1598 2023-03-25 18:23:43.000000 data_cliff-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       40 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      410 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     1463 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_arg_parse.py
--rw-r--r--   0 runner    (1001) docker     (116)     1274 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     4276 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_data_cliff.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/
--rw-r--r--   0 runner    (1001) docker     (116)       39 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/local_data/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/local_data/dir.dvc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.066165 data_cliff-0.1.0/tests/test_dvc_data/remote_data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/remote_data/4c/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/remote_data/4c/4885c2fcf398194990138a70dfd826
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/remote_data/61/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/remote_data/61/2420ac8c564d2bf1cb65de08322a15
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/remote_data/bd/
--rw-r--r--   0 runner    (1001) docker     (116)      145 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/remote_data/bd/7bc28baf5816c0404f8adbad51e0bc.dir
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-25 18:23:46.070165 data_cliff-0.1.0/tests/test_dvc_data/remote_data/f9/
--rw-r--r--   0 runner    (1001) docker     (116)       69 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_dvc_data/remote_data/f9/2164d14b41244ade9045a5736a1054.dir
--rw-r--r--   0 runner    (1001) docker     (116)      592 2023-03-25 18:23:38.000000 data_cliff-0.1.0/tests/test_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 12:07:13.000000 data_cliff-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-13 12:07:13.000000 data_cliff-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 12:07:13.000000 data_cliff-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 12:07:13.000000 data_cliff-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 12:07:13.000000 data_cliff-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 12:07:20.668955 data_cliff-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-13 12:07:13.000000 data_cliff-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/data_cliff/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/arg_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/data_cliff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:13.000000 data_cliff-0.1.2/data_cliff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/data_cliff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:07:20.000000 data_cliff-0.1.2/data_cliff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4814 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/data_cliff.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 12:07:13.000000 data_cliff-0.1.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-13 12:07:20.668955 data_cliff-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-13 12:07:18.000000 data_cliff-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_arg_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_data_cliff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/local_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/local_data/dir.dvc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.660955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/38/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/38/9af16f6ea3dd642636ebd29745313e.dir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.664955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/4c/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/4c/4885c2fcf398194990138a70dfd826
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/61/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/61/2420ac8c564d2bf1cb65de08322a15
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/bd/7bc28baf5816c0404f8adbad51e0bc.dir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/dc/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/dc/84b0d741e5beae8070013addcc8c28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:07:20.668955 data_cliff-0.1.2/tests/test_dvc_data/remote_data/f9/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_dvc_data/remote_data/f9/2164d14b41244ade9045a5736a1054.dir
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 12:07:13.000000 data_cliff-0.1.2/tests/test_getter.py
```

### Comparing `data_cliff-0.1.0/CONTRIBUTING.rst` & `data_cliff-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/LICENSE` & `data_cliff-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/PKG-INFO` & `data_cliff-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_cliff
-Version: 0.1.0
+Version: 0.1.2
 Summary: CLI tool to show differences on text data tracked by dvc.
 Home-page: https://github.com/ruizdesotto/data_cliff
 Author: Miguel Ruiz
 Author-email: miguel.ruizdesotto@gmail.com
 License: Apache Software License 2.0
 Keywords: data_cliff
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `data_cliff-0.1.0/README.rst` & `data_cliff-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/data_cliff/arg_parse.py` & `data_cliff-0.1.2/data_cliff/arg_parse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import argparse
 from dataclasses import dataclass
+from typing import Optional
 
 from pygit2 import Repository, RevSpec
 
 
 class CLIException(Exception):
     pass
 
 
 @dataclass(frozen=True)
 class _Args:
     a_rev: str
-    b_rev: str | None
+    b_rev: Optional[str]
     data_path: str
 
 
 def parse_args(args: list[str]) -> _Args:
     raw_args = parse_command_line_raw_args(args)
     a_rev = raw_args.pos_1 if _is_git_rev(raw_args.pos_1) else "HEAD"
     b_rev = raw_args.pos_2 if _is_git_rev(raw_args.pos_2) else None
@@ -27,19 +28,19 @@
     raw_parser = _cli_parse_factory()
     try:
         return raw_parser.parse_args(args)
     except SystemExit:
         raise CLIException(raw_parser.usage)
 
 
-def _is_git_rev(rev: str | None) -> bool:
+def _is_git_rev(rev: Optional[str]) -> bool:
     if rev is None:
         return False
     try:
-        return isinstance(Repository(".").revparse(rev), RevSpec)
+        return isinstance(Repository(".").revparse(rev.rstrip("/")), RevSpec)
     except KeyError:
         return False
 
 
 def _get_data_path(raw_args: argparse.Namespace):
     for arg in [raw_args.pos_1, raw_args.pos_2, raw_args.pos_3]:
         if arg is not None and not _is_git_rev(arg):
```

### Comparing `data_cliff-0.1.0/data_cliff/data_cliff.py` & `data_cliff-0.1.2/data_cliff/data_cliff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from difflib import unified_diff
 from hashlib import md5
 from pathlib import Path
 from tempfile import TemporaryDirectory
+from typing import Optional
 
 from data_cliff.getter import get_data
 
 
-def compare(a_rev: str, b_rev: str | None, data_path: str) -> int:
+def compare(a_rev: str, b_rev: Optional[str], data_path: str) -> int:
     with TemporaryDirectory() as tmp_path:
         a_path = tmp_path + "a"
         b_path = tmp_path + "b"
         success = get_data(a_rev, data_path, local_path=a_path)
         success |= get_data(b_rev, data_path, local_path=b_path)
 
         if not success:
@@ -33,15 +34,26 @@
             b_path=f"{b_path}/{file}",
             data_path=f"{data_path}/{file}",
         )
 
 
 def _diff_file(a_file_path: str, b_file_path: str, file_name: str) -> None:
     _assert_files_exist(a_file_path, b_file_path)
+    try:
+        _diff_text_file(a_file_path, b_file_path, file_name)
+    except UnicodeDecodeError:
+        _diff_binary_file(a_file_path, b_file_path, file_name)
 
+
+def _assert_files_exist(a_file_path: str, b_file_path: str) -> None:
+    _touch_if_does_not_exist(Path(a_file_path))
+    _touch_if_does_not_exist(Path(b_file_path))
+
+
+def _diff_text_file(a_file_path: str, b_file_path: str, file_name: str) -> None:
     with open(a_file_path) as a, open(b_file_path) as b:
         diff_list = [
             _format_line(line)
             for line in unified_diff(
                 a.read().splitlines(),
                 b.read().splitlines(),
                 fromfile=f"a/{file_name}",
@@ -49,17 +61,20 @@
             )
         ]
 
         header = _get_header(a_file_path, b_file_path, file_name)
         _display(diff_list, header)
 
 
-def _assert_files_exist(a_file_path: str, b_file_path: str) -> None:
-    _touch_if_does_not_exist(Path(a_file_path))
-    _touch_if_does_not_exist(Path(b_file_path))
+def _diff_binary_file(a_file_path: str, b_file_path: str, file_name: str) -> None:
+    a_hash = _hash_file(a_file_path)
+    b_hash = _hash_file(b_file_path)
+    if a_hash != b_hash:
+        header = _get_header(a_file_path, b_file_path, file_name)
+        _display([f"Binary files a/{file_name} and b/{file_name} differ"], header)
 
 
 def _touch_if_does_not_exist(file_path: Path) -> None:
     if not file_path.exists():
         file_path.touch()
```

### Comparing `data_cliff-0.1.0/data_cliff.egg-info/PKG-INFO` & `data_cliff-0.1.2/data_cliff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-cliff
-Version: 0.1.0
+Version: 0.1.2
 Summary: CLI tool to show differences on text data tracked by dvc.
 Home-page: https://github.com/ruizdesotto/data_cliff
 Author: Miguel Ruiz
 Author-email: miguel.ruizdesotto@gmail.com
 License: Apache Software License 2.0
 Keywords: data_cliff
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `data_cliff-0.1.0/data_cliff.egg-info/SOURCES.txt` & `data_cliff-0.1.2/data_cliff.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 data_cliff/__init__.py
 data_cliff/arg_parse.py
 data_cliff/cli.py
 data_cliff/data_cliff.py
 data_cliff/getter.py
+data_cliff/py.typed
 data_cliff.egg-info/PKG-INFO
 data_cliff.egg-info/SOURCES.txt
 data_cliff.egg-info/dependency_links.txt
 data_cliff.egg-info/entry_points.txt
 data_cliff.egg-info/not-zip-safe
 data_cliff.egg-info/top_level.txt
 docs/Makefile
@@ -33,11 +34,13 @@
 tests/conftest.py
 tests/test_arg_parse.py
 tests/test_cli.py
 tests/test_data_cliff.py
 tests/test_getter.py
 tests/test_dvc_data/.gitignore
 tests/test_dvc_data/local_data/dir.dvc
+tests/test_dvc_data/remote_data/38/9af16f6ea3dd642636ebd29745313e.dir
 tests/test_dvc_data/remote_data/4c/4885c2fcf398194990138a70dfd826
 tests/test_dvc_data/remote_data/61/2420ac8c564d2bf1cb65de08322a15
 tests/test_dvc_data/remote_data/bd/7bc28baf5816c0404f8adbad51e0bc.dir
+tests/test_dvc_data/remote_data/dc/84b0d741e5beae8070013addcc8c28
 tests/test_dvc_data/remote_data/f9/2164d14b41244ade9045a5736a1054.dir
```

### Comparing `data_cliff-0.1.0/docs/Makefile` & `data_cliff-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/docs/conf.py` & `data_cliff-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/docs/data_cliff.rst` & `data_cliff-0.1.2/docs/data_cliff.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/docs/installation.rst` & `data_cliff-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/docs/make.bat` & `data_cliff-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/setup.cfg` & `data_cliff-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/setup.py` & `data_cliff-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,13 +40,14 @@
     install_requires=requirements,
     license="Apache Software License 2.0",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="data_cliff",
     name="data_cliff",
     packages=find_packages(include=["data_cliff", "data_cliff.*"]),
+    package_data={"data_cliff": ["py.typed"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ruizdesotto/data_cliff",
-    version="0.1.0",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `data_cliff-0.1.0/tests/test_arg_parse.py` & `data_cliff-0.1.2/tests/test_arg_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @pytest.mark.parametrize(
     "args, a_rev, b_rev, data_path",
     [
         ([], "HEAD", None, ""),
         (["origin/main"], "origin/main", None, ""),
-        (["some/path"], "HEAD", None, "some/path"),
+        (["some/path/"], "HEAD", None, "some/path/"),
         (["origin/main", "some/path"], "origin/main", None, "some/path"),
         (["origin/main", "HEAD", "some/path"], "origin/main", "HEAD", "some/path"),
     ],
 )
 def test_parse_args(args: list[str], a_rev: str, b_rev: str, data_path: str) -> None:
     # Given
     from data_cliff.arg_parse import _Args, parse_args
```

### Comparing `data_cliff-0.1.0/tests/test_cli.py` & `data_cliff-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `data_cliff-0.1.0/tests/test_data_cliff.py` & `data_cliff-0.1.2/tests/test_data_cliff.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from struct import pack
 
 import pytest
 
 
 def test_retrieves_file(dvc_path: Path, tmp_path: Path) -> None:
     # Given
     from dvc.api import DVCFileSystem
@@ -15,15 +16,15 @@
     # When
     a_fs.get(str(file), str(out_file))
 
     # Then
     assert out_file.is_file()
 
 
-def test_compare_staged_change_on_single_file(dvc_path, capsys) -> None:
+def test_compare_staged_change_on_text_file(dvc_path, capsys) -> None:
     # Given
     from dvc.api import DVCFileSystem
 
     from data_cliff.data_cliff import compare
 
     file = dvc_path / "dir" / "file.json"
     _add_key_to_json(file)
@@ -49,14 +50,42 @@
 
         # Then
         assert stdout == expected_output
     finally:
         DVCFileSystem(rev="HEAD").get(str(file), str(file))
 
 
+def test_compare_staged_change_on_binary_file(dvc_path, capsys) -> None:
+    # Given
+    from dvc.api import DVCFileSystem
+
+    from data_cliff.data_cliff import compare
+
+    file = dvc_path / "dir" / "binary"
+    _modify_binary_file(file)
+
+    expected_output = (
+        "cliff a/tests/test_dvc_data/local_data/dir/binary "
+        "b/tests/test_dvc_data/local_data/dir/binary\n"
+        "index dc84b0d..dd0695e 100644\n"
+        "Binary files a/tests/test_dvc_data/local_data/dir/binary and "
+        "b/tests/test_dvc_data/local_data/dir/binary differ\n"
+    )
+
+    try:
+        # When
+        compare("HEAD", None, str(file))
+        stdout, _ = capsys.readouterr()
+
+        # Then
+        assert stdout == expected_output
+    finally:
+        DVCFileSystem(rev="HEAD").get(str(file), str(file))
+
+
 def test_compare_staged_change_on_folder(
     dvc_path: Path, capsys: pytest.CaptureFixture
 ) -> None:
     # Given
     from dvc.api import DVCFileSystem
 
     from data_cliff.data_cliff import compare
@@ -81,25 +110,26 @@
         # When
         compare("HEAD", None, str(folder))
         stdout, _ = capsys.readouterr()
 
         # Then
         assert stdout == expected_output
     finally:
-        DVCFileSystem(rev="HEAD").get(str(folder), str(folder), recursive=True)
+        DVCFileSystem(rev="HEAD").get(str(folder), str(folder.parent), recursive=True)
 
 
 def test_compare_staged_change_on_new_file(
     dvc_path: Path, capsys: pytest.CaptureFixture
 ) -> None:
     # Given
 
     from data_cliff.data_cliff import compare
 
-    new_file = dvc_path / "dir" / "new_file.txt"
+    folder = dvc_path / "dir"
+    new_file = folder / "new_file.txt"
     new_file.touch()
     _add_line_to_file(new_file)
 
     expected_output = (
         "cliff a/tests/test_dvc_data/local_data/dir/new_file.txt"
         " b/tests/test_dvc_data/local_data/dir/new_file.txt\n"
         "index d41d8cd..426d316 100644\n"
@@ -107,15 +137,15 @@
         "+++ b/tests/test_dvc_data/local_data/dir/new_file.txt\n"
         "@@ -0,0 +1 @@\n"
         "\x1b[92m+new line\x1b[00m\n"
     )
 
     try:
         # When
-        compare("HEAD", None, str(new_file))
+        compare("HEAD", None, str(folder))
         stdout, _ = capsys.readouterr()
 
         # Then
         assert stdout == expected_output
     finally:
         new_file.unlink()
 
@@ -148,14 +178,19 @@
 
     data.append("new line\n")
 
     with open(file, "w") as outid:
         outid.write("".join(data))
 
 
+def _modify_binary_file(file: Path) -> None:
+    with open(file, "ab") as fid:
+        fid.write(pack("i", 255))
+
+
 def _add_key_to_json(file: Path) -> None:
     with open(file) as fid:
         parsed_json = json.load(fid)
 
     parsed_json["new_key"] = "new_value"
 
     with open(file, "w") as outid:
```

### Comparing `data_cliff-0.1.0/tests/test_getter.py` & `data_cliff-0.1.2/tests/test_getter.py`

 * *Files identical despite different names*

