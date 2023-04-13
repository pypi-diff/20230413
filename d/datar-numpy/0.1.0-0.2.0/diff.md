# Comparing `tmp/datar_numpy-0.1.0.tar.gz` & `tmp/datar_numpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datar_numpy-0.1.0.tar", max compression
+gzip compressed data, was "datar_numpy-0.2.0.tar", max compression
```

## Comparing `datar_numpy-0.1.0.tar` & `datar_numpy-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1063 2022-12-15 18:20:53.630499 datar_numpy-0.1.0/LICENSE
--rw-r--r--   0        0        0      373 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/README.md
--rw-r--r--   0        0        0       54 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/__init__.py
--rw-r--r--   0        0        0     5520 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/arithm.py
--rw-r--r--   0        0        0     3971 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/asis.py
--rw-r--r--   0        0        0     1909 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/bessel.py
--rw-r--r--   0        0        0      481 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/complex.py
--rw-r--r--   0        0        0      345 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/constants.py
--rw-r--r--   0        0        0      464 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/cum.py
--rw-r--r--   0        0        0     2963 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/date.py
--rw-r--r--   0        0        0     1595 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/random.py
--rw-r--r--   0        0        0     5343 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/seq.py
--rw-r--r--   0        0        0     2950 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/sets.py
--rw-r--r--   0        0        0     1575 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/special.py
--rw-r--r--   0        0        0     8127 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/string.py
--rw-r--r--   0        0        0     1513 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/trig.py
--rw-r--r--   0        0        0      359 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/api/which.py
--rw-r--r--   0        0        0     1325 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/plugin.py
--rw-r--r--   0        0        0     2682 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/utils.py
--rw-r--r--   0        0        0       22 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/datar_numpy/version.py
--rw-r--r--   0        0        0      729 2022-12-15 18:20:53.634499 datar_numpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 datar_numpy-0.1.0/setup.py
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 datar_numpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/README.md
+-rw-r--r--   0        0        0       54 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/__init__.py
+-rw-r--r--   0        0        0     5520 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/arithm.py
+-rw-r--r--   0        0        0     3971 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/asis.py
+-rw-r--r--   0        0        0     1909 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/bessel.py
+-rw-r--r--   0        0        0      481 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/complex.py
+-rw-r--r--   0        0        0      345 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/constants.py
+-rw-r--r--   0        0        0      464 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/cum.py
+-rw-r--r--   0        0        0     2963 2023-04-13 07:21:14.736516 datar_numpy-0.2.0/datar_numpy/api/date.py
+-rw-r--r--   0        0        0     1595 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/random.py
+-rw-r--r--   0        0        0     5343 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/seq.py
+-rw-r--r--   0        0        0     2950 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/sets.py
+-rw-r--r--   0        0        0     1575 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/special.py
+-rw-r--r--   0        0        0     8127 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/string.py
+-rw-r--r--   0        0        0     1513 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/trig.py
+-rw-r--r--   0        0        0      359 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/api/which.py
+-rw-r--r--   0        0        0     1325 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/plugin.py
+-rw-r--r--   0        0        0     2682 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/datar_numpy/version.py
+-rw-r--r--   0        0        0      727 2023-04-13 07:21:14.740516 datar_numpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 datar_numpy-0.2.0/PKG-INFO
```

### Comparing `datar_numpy-0.1.0/LICENSE` & `datar_numpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/arithm.py` & `datar_numpy-0.2.0/datar_numpy/api/arithm.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/asis.py` & `datar_numpy-0.2.0/datar_numpy/api/asis.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/bessel.py` & `datar_numpy-0.2.0/datar_numpy/api/bessel.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/date.py` & `datar_numpy-0.2.0/datar_numpy/api/date.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/random.py` & `datar_numpy-0.2.0/datar_numpy/api/random.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/seq.py` & `datar_numpy-0.2.0/datar_numpy/api/seq.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/sets.py` & `datar_numpy-0.2.0/datar_numpy/api/sets.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/special.py` & `datar_numpy-0.2.0/datar_numpy/api/special.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/string.py` & `datar_numpy-0.2.0/datar_numpy/api/string.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/api/trig.py` & `datar_numpy-0.2.0/datar_numpy/api/trig.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/plugin.py` & `datar_numpy-0.2.0/datar_numpy/plugin.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/datar_numpy/utils.py` & `datar_numpy-0.2.0/datar_numpy/utils.py`

 * *Files identical despite different names*

### Comparing `datar_numpy-0.1.0/pyproject.toml` & `datar_numpy-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "datar-numpy"
-version = "0.1.0"
+version = "0.2.0"
 description = "The numpy backend for datar"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "datar_numpy"}]
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-datar = "^0.11"
-numpy = "^1.17"
+python = "^3.8"
+datar = "^0.12"
+numpy = "^1.20"
 
 [tool.poetry.plugins.datar]
 numpy = "datar_numpy:plugin"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
```

### Comparing `datar_numpy-0.1.0/PKG-INFO` & `datar_numpy-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datar-numpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: The numpy backend for datar
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: datar (>=0.11,<0.12)
-Requires-Dist: numpy (>=1.17,<2.0)
+Requires-Dist: datar (>=0.12,<0.13)
+Requires-Dist: numpy (>=1.20,<2.0)
 Description-Content-Type: text/markdown
 
 # datar-numpy
 
 The numpy backend for [datar][1].
 
 Note that only `base` APIs are implemented.
```

