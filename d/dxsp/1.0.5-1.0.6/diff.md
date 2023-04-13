# Comparing `tmp/dxsp-1.0.5.tar.gz` & `tmp/dxsp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.5.tar", max compression
+gzip compressed data, was "dxsp-1.0.6.tar", max compression
```

## Comparing `dxsp-1.0.5.tar` & `dxsp-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 08:47:58.222262 dxsp-1.0.5/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-13 08:47:58.222262 dxsp-1.0.5/README.md
--rw-r--r--   0        0        0       47 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8589 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    15819 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 08:47:58.870270 dxsp-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 12:57:29.227748 dxsp-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-13 12:57:29.227748 dxsp-1.0.6/README.md
+-rw-r--r--   0        0        0      137 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8589 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15819 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 12:57:30.143748 dxsp-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.6/PKG-INFO
```

### Comparing `dxsp-1.0.5/LICENSE` & `dxsp-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.5/README.md` & `dxsp-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.5/dxsp/assets/blockchains.py` & `dxsp-1.0.6/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.5/dxsp/main.py` & `dxsp-1.0.6/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.5/pyproject.toml` & `dxsp-1.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.5"
+version = "1.0.6"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.5/PKG-INFO` & `dxsp-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.5
+Version: 1.0.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

