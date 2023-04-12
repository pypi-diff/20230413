# Comparing `tmp/fling_core-0.1.1.tar.gz` & `tmp/fling_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_core-0.1.1.tar", max compression
+gzip compressed data, was "fling_core-0.1.2.tar", max compression
```

## Comparing `fling_core-0.1.1.tar` & `fling_core-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      197 2023-04-12 20:35:42.928996 fling_core-0.1.1/README.md
--rw-r--r--   0        0        0      467 2023-04-12 20:34:01.559188 fling_core-0.1.1/fling_core/__init__.py
--rw-r--r--   0        0        0      226 2023-04-12 19:36:22.012522 fling_core-0.1.1/fling_core/fling.yaml
--rw-r--r--   0        0        0     1242 2023-04-12 19:37:34.124123 fling_core-0.1.1/fling_core/github.py
--rw-r--r--   0        0        0      441 2023-04-07 22:11:58.517112 fling_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 fling_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      197 2023-04-12 20:35:42.928996 fling_core-0.1.2/README.md
+-rw-r--r--   0        0        0      467 2023-04-12 23:14:08.566947 fling_core-0.1.2/fling_core/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-12 23:11:40.096255 fling_core-0.1.2/fling_core/fling.yaml
+-rw-r--r--   0        0        0     1242 2023-04-12 19:37:34.124123 fling_core-0.1.2/fling_core/github.py
+-rw-r--r--   0        0        0      441 2023-04-12 23:14:01.441139 fling_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 fling_core-0.1.2/PKG-INFO
```

### Comparing `fling_core-0.1.1/fling_core/github.py` & `fling_core-0.1.2/fling_core/github.py`

 * *Files identical despite different names*

### Comparing `fling_core-0.1.1/PKG-INFO` & `fling_core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fling core components for Side Project Management
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

