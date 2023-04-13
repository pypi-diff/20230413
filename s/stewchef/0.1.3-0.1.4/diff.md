# Comparing `tmp/stewchef-0.1.3.tar.gz` & `tmp/stewchef-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.3.tar", max compression
+gzip compressed data, was "stewchef-0.1.4.tar", max compression
```

## Comparing `stewchef-0.1.3.tar` & `stewchef-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.3/README.md
--rw-r--r--   0        0        0      489 2023-04-12 10:21:10.875274 stewchef-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.3/stewchef/__init__.py
--rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.3/stewchef/main.py
--rw-r--r--   0        0        0     6544 1970-01-01 00:00:00.000000 stewchef-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.4/README.md
+-rw-r--r--   0        0        0      490 2023-04-13 13:38:43.970900 stewchef-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.4/stewchef/__init__.py
+-rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.4/stewchef/main.py
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stewchef-0.1.4/PKG-INFO
```

### Comparing `stewchef-0.1.3/README.md` & `stewchef-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.3/stewchef/main.py` & `stewchef-0.1.4/stewchef/main.py`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.3/PKG-INFO` & `stewchef-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: stewchef
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MediaWiki API wrapper for RegiSoup
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
-Requires-Dist: regisoup (>=0.1.7,<0.2.0)
+Requires-Dist: regisoup (>=0.1.10,<0.2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # **StewChef: Cook up some RegiSoup**
```

