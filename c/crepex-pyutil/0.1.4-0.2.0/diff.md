# Comparing `tmp/crepex_pyutil-0.1.4.tar.gz` & `tmp/crepex_pyutil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepex_pyutil-0.1.4.tar", max compression
+gzip compressed data, was "crepex_pyutil-0.2.0.tar", max compression
```

## Comparing `crepex_pyutil-0.1.4.tar` & `crepex_pyutil-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.1.4/README.md
--rw-r--r--   0        0        0      395 2023-04-12 06:59:28.882157 crepex_pyutil-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.1.4/src/crepex_pyutil/__init__.py
--rw-r--r--   0        0        0      664 2023-04-12 05:49:04.763845 crepex_pyutil-0.1.4/src/crepex_pyutil/exceptions.py
--rw-r--r--   0        0        0       42 2023-04-12 05:38:24.028393 crepex_pyutil-0.1.4/src/crepex_pyutil/requests/__init__.py
--rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.1.4/src/crepex_pyutil/requests/helper.py
--rwxr-xr-x   0        0        0     1327 2023-04-12 07:16:42.946864 crepex_pyutil-0.1.4/src/crepex_pyutil/string.py
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.2.0/README.md
+-rw-r--r--   0        0        0      395 2023-04-13 11:48:30.777549 crepex_pyutil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.2.0/src/crepex_pyutil/__init__.py
+-rwxr-xr-x   0        0        0     2826 2023-04-13 11:48:15.785079 crepex_pyutil-0.2.0/src/crepex_pyutil/dates.py
+-rw-r--r--   0        0        0      664 2023-04-12 05:49:04.763845 crepex_pyutil-0.2.0/src/crepex_pyutil/exceptions.py
+-rw-r--r--   0        0        0       42 2023-04-12 05:38:24.028393 crepex_pyutil-0.2.0/src/crepex_pyutil/requests/__init__.py
+-rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.2.0/src/crepex_pyutil/requests/helper.py
+-rwxr-xr-x   0        0        0     1327 2023-04-12 07:16:42.946864 crepex_pyutil-0.2.0/src/crepex_pyutil/string.py
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.2.0/PKG-INFO
```

### Comparing `crepex_pyutil-0.1.4/README.md` & `crepex_pyutil-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.1.4/src/crepex_pyutil/exceptions.py` & `crepex_pyutil-0.2.0/src/crepex_pyutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.1.4/src/crepex_pyutil/requests/helper.py` & `crepex_pyutil-0.2.0/src/crepex_pyutil/requests/helper.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.1.4/src/crepex_pyutil/string.py` & `crepex_pyutil-0.2.0/src/crepex_pyutil/string.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.1.4/PKG-INFO` & `crepex_pyutil-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepex-pyutil
-Version: 0.1.4
+Version: 0.2.0
 Summary: CrepeX python utilities
 Author: Hyunwoo Shim
 Author-email: hyunwoo.shim@crepe-x.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

