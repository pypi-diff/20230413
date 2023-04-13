# Comparing `tmp/sienna-0.2.0.tar.gz` & `tmp/sienna-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sienna-0.2.0.tar", max compression
+gzip compressed data, was "sienna-0.2.1.tar", max compression
```

## Comparing `sienna-0.2.0.tar` & `sienna-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      380 2023-04-13 10:11:35.652110 sienna-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-04-13 10:11:35.652403 sienna-0.2.0/sienna/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-13 10:11:35.652653 sienna-0.2.0/sienna/core.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 sienna-0.2.0/setup.py
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 sienna-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-04-13 10:50:11.093087 sienna-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1378 2023-04-13 10:49:17.864625 sienna-0.2.1/sienna/.null-ls_875572_core.py
+-rw-r--r--   0        0        0       62 2023-04-13 10:11:35.652403 sienna-0.2.1/sienna/__init__.py
+-rw-r--r--   0        0        0     1347 2023-04-13 10:50:11.093305 sienna-0.2.1/sienna/core.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 sienna-0.2.1/setup.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 sienna-0.2.1/PKG-INFO
```

### Comparing `sienna-0.2.0/sienna/core.py` & `sienna-0.2.1/sienna/.null-ls_875572_core.py`

 * *Files identical despite different names*

