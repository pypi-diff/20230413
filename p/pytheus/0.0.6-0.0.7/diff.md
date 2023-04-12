# Comparing `tmp/pytheus-0.0.6.tar.gz` & `tmp/pytheus-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.6.tar", last modified: Wed Apr 12 19:37:37 2023, max compression
+gzip compressed data, was "pytheus-0.0.7.tar", last modified: Wed Apr 12 22:38:58 2023, max compression
```

## Comparing `pytheus-0.0.6.tar` & `pytheus-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.113518 pytheus-0.0.6/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.6/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 19:37:37.113332 pytheus-0.0.6/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.6/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1070 2023-04-12 19:37:03.000000 pytheus-0.0.6/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.110728 pytheus-0.0.6/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.6/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.112212 pytheus-0.0.6/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.6/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.6/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.6/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.6/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-11 21:40:44.000000 pytheus-0.0.6/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    18563 2023-04-12 19:31:40.000000 pytheus-0.0.6/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.6/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      173 2023-04-01 23:52:48.000000 pytheus-0.0.6/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.111532 pytheus-0.0.6/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      164 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-12 19:37:37.113564 pytheus-0.0.6/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.6/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.112750 pytheus-0.0.6/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-03-30 23:54:35.000000 pytheus-0.0.6/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    22327 2023-04-12 19:31:40.000000 pytheus-0.0.6/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.6/tests/test_registry.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.914042 pytheus-0.0.7/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.7/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 22:38:58.913841 pytheus-0.0.7/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.7/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-12 22:38:15.000000 pytheus-0.0.7/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.912402 pytheus-0.0.7/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.7/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.913302 pytheus-0.0.7/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.7/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.7/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.7/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.7/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.7/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    18563 2023-04-12 19:31:40.000000 pytheus-0.0.7/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.7/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      230 2023-04-12 22:36:32.000000 pytheus-0.0.7/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.912937 pytheus-0.0.7/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-12 22:38:58.914089 pytheus-0.0.7/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.7/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.913673 pytheus-0.0.7/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-04-12 22:30:37.000000 pytheus-0.0.7/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    22327 2023-04-12 19:31:40.000000 pytheus-0.0.7/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.7/tests/test_registry.py
```

### Comparing `pytheus-0.0.6/LICENSE` & `pytheus-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/PKG-INFO` & `pytheus-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.6
+Version: 0.0.7
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.6/README.md` & `pytheus-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pyproject.toml` & `pytheus-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytheus"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,14 +18,15 @@
 [project.optional-dependencies]
 test = [
   "pytest >= 7.0.0",
   "mypy == 1.1.1",
   "ruff == 0.0.260",
   "black == 23.3.0",
   "isort == 5.12.0",
+  "tox == 4.4.11",
 
   # mypy types
   "types-redis == 4.5.4.0",
 ]
 
 redis = [
   "redis >= 4.0.0",
```

### Comparing `pytheus-0.0.6/pytheus/backends/base.py` & `pytheus-0.0.7/pytheus/backends/base.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pytheus/backends/redis.py` & `pytheus-0.0.7/pytheus/backends/redis.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pytheus/exposition.py` & `pytheus-0.0.7/pytheus/exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pytheus/metrics.py` & `pytheus-0.0.7/pytheus/metrics.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pytheus/registry.py` & `pytheus-0.0.7/pytheus/registry.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/pytheus.egg-info/PKG-INFO` & `pytheus-0.0.7/pytheus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.6
+Version: 0.0.7
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.6/tests/test_exposition.py` & `pytheus-0.0.7/tests/test_exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/tests/test_metrics.py` & `pytheus-0.0.7/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.6/tests/test_registry.py` & `pytheus-0.0.7/tests/test_registry.py`

 * *Files identical despite different names*

