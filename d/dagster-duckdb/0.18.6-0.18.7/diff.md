# Comparing `tmp/dagster-duckdb-0.18.6.tar.gz` & `tmp/dagster-duckdb-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.18.6.tar", last modified: Thu Apr  6 00:28:43 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.18.7.tar", last modified: Thu Apr 13 15:15:13 2023, max compression
```

## Comparing `dagster-duckdb-0.18.6.tar` & `dagster-duckdb-0.18.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:43.256440 dagster-duckdb-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-06 00:28:43.256440 dagster-duckdb-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:43.256440 dagster-duckdb-0.18.6/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6874 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:43.256440 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-06 00:28:43.000000 dagster-duckdb-0.18.6/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-04-06 00:28:43.260439 dagster-duckdb-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1544 2023-04-05 23:51:52.000000 dagster-duckdb-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:13.553774 dagster-duckdb-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-13 15:15:13.553774 dagster-duckdb-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:13.553774 dagster-duckdb-0.18.7/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9446 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:13.553774 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 15:15:13.000000 dagster-duckdb-0.18.7/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-04-13 15:15:13.557774 dagster-duckdb-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-04-13 15:03:07.000000 dagster-duckdb-0.18.7/setup.py
```

### Comparing `dagster-duckdb-0.18.6/LICENSE` & `dagster-duckdb-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.18.6/PKG-INFO` & `dagster-duckdb-0.18.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.18.6/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.18.7/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.18.6/setup.py` & `dagster-duckdb-0.18.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.2.6",
+        "dagster==1.2.7",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

