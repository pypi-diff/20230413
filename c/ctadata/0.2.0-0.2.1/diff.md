# Comparing `tmp/ctadata-0.2.0.tar.gz` & `tmp/ctadata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.0.tar", max compression
+gzip compressed data, was "ctadata-0.2.1.tar", max compression
```

## Comparing `ctadata-0.2.0.tar` & `ctadata-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1976 2023-04-12 15:32:43.928799 ctadata-0.2.0/README.md
--rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.0/ctadata/__init__.py
--rw-r--r--   0        0        0     3220 2023-04-13 11:56:04.865225 ctadata-0.2.0/ctadata/api.py
--rw-r--r--   0        0        0      850 2023-04-13 12:12:59.548331 ctadata-0.2.0/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.0/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-04-13 12:26:44.425929 ctadata-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 ctadata-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1976 2023-04-12 15:32:43.928799 ctadata-0.2.1/README.md
+-rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.1/ctadata/__init__.py
+-rw-r--r--   0        0        0     3220 2023-04-13 11:56:04.865225 ctadata-0.2.1/ctadata/api.py
+-rw-r--r--   0        0        0      850 2023-04-13 12:12:59.548331 ctadata-0.2.1/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.1/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-04-13 12:35:47.719374 ctadata-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 ctadata-0.2.1/PKG-INFO
```

### Comparing `ctadata-0.2.0/README.md` & `ctadata-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.0/ctadata/__init__.py` & `ctadata-0.2.1/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.0/ctadata/api.py` & `ctadata-0.2.1/ctadata/api.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.0/ctadata/cli.py` & `ctadata-0.2.1/ctadata/cli.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.0/PKG-INFO` & `ctadata-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctadata
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Volodymyr Savchenko
 Author-email: contact@volodymyrsavchenko.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

