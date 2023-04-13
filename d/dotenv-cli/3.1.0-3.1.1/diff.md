# Comparing `tmp/dotenv-cli-3.1.0.tar.gz` & `tmp/dotenv-cli-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenv-cli-3.1.0.tar", last modified: Wed Sep  7 18:17:23 2022, max compression
+gzip compressed data, was "dotenv-cli-3.1.1.tar", last modified: Thu Apr 13 08:38:24 2023, max compression
```

## Comparing `dotenv-cli-3.1.0.tar` & `dotenv-cli-3.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-07 18:17:23.530356 dotenv-cli-3.1.0/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.1.0/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.1.0/MANIFEST.in
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2896 2022-09-07 18:17:23.530356 dotenv-cli-3.1.0/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2347 2019-08-03 12:37:48.000000 dotenv-cli-3.1.0/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-07 18:17:23.526353 dotenv-cli-3.1.0/completion/
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-07 18:17:23.526353 dotenv-cli-3.1.0/completion/bash/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.1.0/completion/bash/dotenv
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-07 18:17:23.526353 dotenv-cli-3.1.0/dotenv_cli/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       65 2022-09-07 18:14:49.000000 dotenv-cli-3.1.0/dotenv_cli/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1162 2022-09-07 18:14:49.000000 dotenv-cli-3.1.0/dotenv_cli/cli.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2758 2022-09-07 18:14:49.000000 dotenv-cli-3.1.0/dotenv_cli/core.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2022-09-07 18:16:42.000000 dotenv-cli-3.1.0/dotenv_cli/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-07 18:17:23.530356 dotenv-cli-3.1.0/dotenv_cli.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2896 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      359 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       48 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       44 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2022-09-07 18:17:23.000000 dotenv-cli-3.1.0/dotenv_cli.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2022-09-07 18:17:23.530356 dotenv-cli-3.1.0/setup.cfg
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1076 2022-05-31 18:04:39.000000 dotenv-cli-3.1.0/setup.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.1.1/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.1.1/MANIFEST.in
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2876 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2347 2019-08-03 12:37:48.000000 dotenv-cli-3.1.1/README.md
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.987097 dotenv-cli-3.1.1/completion/
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.987097 dotenv-cli-3.1.1/completion/bash/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.1.1/completion/bash/dotenv
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/dotenv_cli/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       65 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/__init__.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1162 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/cli.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2758 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/core.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-04-13 08:20:01.000000 dotenv-cli-3.1.1/dotenv_cli/version.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/dotenv_cli.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2876 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      359 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       47 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/entry_points.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       44 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/requires.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/top_level.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/setup.cfg
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1076 2022-05-31 18:04:39.000000 dotenv-cli-3.1.1/setup.py
```

### Comparing `dotenv-cli-3.1.0/LICENSE` & `dotenv-cli-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.0/PKG-INFO` & `dotenv-cli-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple dotenv CLI.
 Home-page: https://github.com/venthur/dotenv-cli
 Author: Bastian Venthur
 Author-email: mail@venthur.de
 License: MIT
 Keywords: dotenv cli .env
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -119,9 +118,7 @@
 TRIM_WHITESPACE=foo
 KEEP_WHITESPACE=  foo
 MULTILINE_DQ=multi
 line
 MULTILINE_SQ=multi\nline
 MULTILINE_NQ=multi\nline
 ```
-
-
```

### Comparing `dotenv-cli-3.1.0/README.md` & `dotenv-cli-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.0/completion/bash/dotenv` & `dotenv-cli-3.1.1/completion/bash/dotenv`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.0/dotenv_cli/cli.py` & `dotenv-cli-3.1.1/dotenv_cli/cli.py`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.0/dotenv_cli/core.py` & `dotenv-cli-3.1.1/dotenv_cli/core.py`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.0/dotenv_cli.egg-info/PKG-INFO` & `dotenv-cli-3.1.1/dotenv_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple dotenv CLI.
 Home-page: https://github.com/venthur/dotenv-cli
 Author: Bastian Venthur
 Author-email: mail@venthur.de
 License: MIT
 Keywords: dotenv cli .env
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -119,9 +118,7 @@
 TRIM_WHITESPACE=foo
 KEEP_WHITESPACE=  foo
 MULTILINE_DQ=multi
 line
 MULTILINE_SQ=multi\nline
 MULTILINE_NQ=multi\nline
 ```
-
-
```

### Comparing `dotenv-cli-3.1.0/setup.py` & `dotenv-cli-3.1.1/setup.py`

 * *Files identical despite different names*

