# Comparing `tmp/ts_task_script_utils-1.5.0.tar.gz` & `tmp/ts_task_script_utils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_task_script_utils-1.5.0.tar", max compression
+gzip compressed data, was "ts_task_script_utils-1.6.0.tar", max compression
```

## Comparing `ts_task_script_utils-1.5.0.tar` & `ts_task_script_utils-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-03-28 19:46:22.484027 ts_task_script_utils-1.5.0/LICENSE
--rw-r--r--   0        0        0     4833 2023-03-28 19:46:22.484027 ts_task_script_utils-1.5.0/README.md
--rw-r--r--   0        0        0     1155 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/__init__.py
--rw-r--r--   0        0        0     1123 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/check_file_type.py
--rw-r--r--   0        0        0     2454 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/convert_datetime_to_ts_format.py
--rw-r--r--   0        0        0    24970 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/README.md
--rw-r--r--   0        0        0       96 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/__init__.py
--rw-r--r--   0        0        0     2680 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/datetime_config.py
--rw-r--r--   0        0        0    30200 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/datetime_info.py
--rw-r--r--   0        0        0    88298 2023-03-28 19:46:22.488028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/flowcharts/parse.png
--rw-r--r--   0        0        0    70421 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
--rw-r--r--   0        0        0     1827 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
--rw-r--r--   0        0        0   104888 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parse-white.png
--rw-r--r--   0        0        0     2248 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parser.py
--rw-r--r--   0        0        0      841 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parser_exceptions.py
--rw-r--r--   0        0        0     3999 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/ts_datetime.py
--rw-r--r--   0        0        0      178 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/tz_dicts.py
--rw-r--r--   0        0        0     2357 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/tz_list.py
--rw-r--r--   0        0        0     3710 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/utils/manipulation.py
--rw-r--r--   0        0        0     4558 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/utils/parsing.py
--rw-r--r--   0        0        0     7486 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/extract_to_decorate.py
--rw-r--r--   0        0        0      424 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/is_number.py
--rw-r--r--   0        0        0     4227 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/parse.py
--rw-r--r--   0        0        0     2795 2023-03-28 19:46:22.492028 ts_task_script_utils-1.5.0/task_script_utils/random.py
--rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 ts_task_script_utils-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 20:01:25.929169 ts_task_script_utils-1.6.0/LICENSE
+-rw-r--r--   0        0        0     5183 2023-04-13 20:01:25.929169 ts_task_script_utils-1.6.0/README.md
+-rw-r--r--   0        0        0     1238 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/check_file_type.py
+-rw-r--r--   0        0        0     2454 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/convert_datetime_to_ts_format.py
+-rw-r--r--   0        0        0     3596 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datacubes/README.md
+-rw-r--r--   0        0        0     5309 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datacubes/parquet.py
+-rw-r--r--   0        0        0    24970 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/README.md
+-rw-r--r--   0        0        0       96 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/__init__.py
+-rw-r--r--   0        0        0     2680 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_config.py
+-rw-r--r--   0        0        0    30200 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_info.py
+-rw-r--r--   0        0        0    88298 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/parse.png
+-rw-r--r--   0        0        0    70421 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
+-rw-r--r--   0        0        0     1827 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
+-rw-r--r--   0        0        0   104888 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parse-white.png
+-rw-r--r--   0        0        0     2248 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser.py
+-rw-r--r--   0        0        0      841 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser_exceptions.py
+-rw-r--r--   0        0        0     3999 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/ts_datetime.py
+-rw-r--r--   0        0        0      178 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_dicts.py
+-rw-r--r--   0        0        0     2357 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_list.py
+-rw-r--r--   0        0        0     3710 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/manipulation.py
+-rw-r--r--   0        0        0     4558 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/parsing.py
+-rw-r--r--   0        0        0     7486 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/extract_to_decorate.py
+-rw-r--r--   0        0        0      424 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/is_number.py
+-rw-r--r--   0        0        0     4227 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/parse.py
+-rw-r--r--   0        0        0     2795 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/random.py
+-rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 ts_task_script_utils-1.6.0/PKG-INFO
```

### Comparing `ts_task_script_utils-1.5.0/LICENSE` & `ts_task_script_utils-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/README.md` & `ts_task_script_utils-1.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # ts-task-script-utils <!-- omit in toc -->
 
 [![Build Status](https://travis-ci.com/tetrascience/ts-task-script-utils.svg?branch=master)](https://travis-ci.com/tetrascience/ts-task-script-utils)
 
 ## Version <!-- omit in toc -->
 
-v1.5.0
+v1.6.0
 
 ## Table of Contents <!-- omit in toc -->
 
+- [Summary](#summary)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Parsing Numbers](#parsing-numbers)
   - [Parsing Datetimes](#parsing-datetimes)
     - [`parse` Usage](#parse-usage)
-  - [Generating Random Values](#generating-random-values)
+  - [Generating Random UUIDs for Task Scripts](#generating-random-uuids-for-task-scripts)
+  - [Creating datacube Parquet files](#creating-datacube-parquet-files)
 - [Changelog](#changelog)
+  - [v1.6.0](#v160)
   - [v1.5.0](#v150)
   - [v1.4.0](#v140)
   - [v1.3.1](#v131)
   - [v1.3.0](#v130)
   - [v1.2.0](#v120)
   - [v1.1.1](#v111)
   - [v1.1.0](#v110)
@@ -132,17 +135,24 @@
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 
 rand2 = TaskScriptUUIDGenerator.get_last_created()
 
 assert rand1 is rand2
 ```
 
+### Creating datacube Parquet files
+
+[See the docs](task_script_utils/datacubes/README.md).
 
 ## Changelog
 
+### v1.6.0
+
+- Add `task_script_utils.datacubes.parquet` for creating Parquet file representations of datacubes
+
 ### v1.5.0
 
 - Add `TaskScriptUUIDGenerator` class for generating random UUIDs and random bytes.
 
 ### v1.4.0
 
 - Add `extract-to-decorate` functions
```

### Comparing `ts_task_script_utils-1.5.0/pyproject.toml` & `ts_task_script_utils-1.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,35 +7,39 @@
 line-length = 88
 target-version = ['py37', 'py38', 'py39']
 include = '\.pyi?$'
 extend-exclude = 'snapshots'
 
 [tool.poetry]
 name = "ts-task-script-utils"
-version = "1.5.0"
+version = "1.6.0"
 description = "Python utility for Tetra Task Scripts"
 authors = ["Tetrascience <developers@tetrascience.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["LICENSE"]
 classifiers =[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 packages = [{ include = 'task_script_utils'}]
 
 [tool.poetry.dependencies]
 # python version is restricted to less than 3.11 to allow numpy to resolve correctly
-python = "^3.7.1,<3.11"
+python = "^3.7.2,<3.11"
 python-dateutil = "^2.8.2"
 dateparser = "^1.1.1"
 arrow = "^1.2.2"
 pendulum = "^2.1.2"
 pydash = "^5.1.0"
+pandas = ">=1.3.5"
+fastparquet = ">=0.8.1"
+numpy = "^1.17.0"
+fsspec = "<=2023.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 black = "^22.3.0"
 ipdb = "^0.13.9"
```

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/check_file_type.py` & `ts_task_script_utils-1.6.0/task_script_utils/check_file_type.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/convert_datetime_to_ts_format.py` & `ts_task_script_utils-1.6.0/task_script_utils/convert_datetime_to_ts_format.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/README.md` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/README.md`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/datetime_config.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_config.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/datetime_info.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_info.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/flowcharts/parse.png` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/parse.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parse-white.png` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parse-white.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parser.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/parser_exceptions.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser_exceptions.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/ts_datetime.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/ts_datetime.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/tz_list.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_list.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/utils/manipulation.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/manipulation.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/datetime_parser/utils/parsing.py` & `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/extract_to_decorate.py` & `ts_task_script_utils-1.6.0/task_script_utils/extract_to_decorate.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/parse.py` & `ts_task_script_utils-1.6.0/task_script_utils/parse.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/task_script_utils/random.py` & `ts_task_script_utils-1.6.0/task_script_utils/random.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.5.0/PKG-INFO` & `ts_task_script_utils-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 Metadata-Version: 2.1
 Name: ts-task-script-utils
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python utility for Tetra Task Scripts
 License: Apache-2.0
 Author: Tetrascience
 Author-email: developers@tetrascience.com
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.7.2,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
 Requires-Dist: dateparser (>=1.1.1,<2.0.0)
+Requires-Dist: fastparquet (>=0.8.1)
+Requires-Dist: fsspec (<=2023.1.0)
+Requires-Dist: numpy (>=1.17.0,<2.0.0)
+Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydash (>=5.1.0,<6.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ts-task-script-utils <!-- omit in toc -->
 
 [![Build Status](https://travis-ci.com/tetrascience/ts-task-script-utils.svg?branch=master)](https://travis-ci.com/tetrascience/ts-task-script-utils)
 
 ## Version <!-- omit in toc -->
 
-v1.5.0
+v1.6.0
 
 ## Table of Contents <!-- omit in toc -->
 
+- [Summary](#summary)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Parsing Numbers](#parsing-numbers)
   - [Parsing Datetimes](#parsing-datetimes)
     - [`parse` Usage](#parse-usage)
-  - [Generating Random Values](#generating-random-values)
+  - [Generating Random UUIDs for Task Scripts](#generating-random-uuids-for-task-scripts)
+  - [Creating datacube Parquet files](#creating-datacube-parquet-files)
 - [Changelog](#changelog)
+  - [v1.6.0](#v160)
   - [v1.5.0](#v150)
   - [v1.4.0](#v140)
   - [v1.3.1](#v131)
   - [v1.3.0](#v130)
   - [v1.2.0](#v120)
   - [v1.1.1](#v111)
   - [v1.1.0](#v110)
@@ -154,17 +161,24 @@
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 
 rand2 = TaskScriptUUIDGenerator.get_last_created()
 
 assert rand1 is rand2
 ```
 
+### Creating datacube Parquet files
+
+[See the docs](task_script_utils/datacubes/README.md).
 
 ## Changelog
 
+### v1.6.0
+
+- Add `task_script_utils.datacubes.parquet` for creating Parquet file representations of datacubes
+
 ### v1.5.0
 
 - Add `TaskScriptUUIDGenerator` class for generating random UUIDs and random bytes.
 
 ### v1.4.0
 
 - Add `extract-to-decorate` functions
```

