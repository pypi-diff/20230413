# Comparing `tmp/openart-0.0.1.tar.gz` & `tmp/openart-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openart-0.0.1.tar", last modified: Wed Apr 12 22:23:16 2023, max compression
+gzip compressed data, was "openart-0.0.2.tar", last modified: Wed Apr 12 22:43:36 2023, max compression
```

## Comparing `openart-0.0.1.tar` & `openart-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:23:16.333576 openart-0.0.1/
--rw-r--r--   0 zero      (1000) zero      (1001)     1064 2023-04-12 22:21:15.000000 openart-0.0.1/LICENSE
--rw-r--r--   0 zero      (1000) zero      (1001)     1362 2023-04-12 22:23:16.333576 openart-0.0.1/PKG-INFO
-drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:23:16.333576 openart-0.0.1/openart/
--rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 21:44:23.000000 openart-0.0.1/openart/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1001)      354 2023-04-12 22:11:18.000000 openart-0.0.1/openart/openart.py
-drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:23:16.333576 openart-0.0.1/openart.egg-info/
--rw-r--r--   0 zero      (1000) zero      (1001)     1362 2023-04-12 22:23:16.000000 openart-0.0.1/openart.egg-info/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1001)      217 2023-04-12 22:23:16.000000 openart-0.0.1/openart.egg-info/SOURCES.txt
--rw-r--r--   0 zero      (1000) zero      (1001)        1 2023-04-12 22:23:16.000000 openart-0.0.1/openart.egg-info/dependency_links.txt
--rw-r--r--   0 zero      (1000) zero      (1001)       13 2023-04-12 22:23:16.000000 openart-0.0.1/openart.egg-info/top_level.txt
--rw-r--r--   0 zero      (1000) zero      (1001)       38 2023-04-12 22:23:16.333576 openart-0.0.1/setup.cfg
--rw-r--r--   0 zero      (1000) zero      (1001)      354 2023-04-12 22:14:26.000000 openart-0.0.1/setup.py
-drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:23:16.333576 openart-0.0.1/test/
--rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 21:44:59.000000 openart-0.0.1/test/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 22:11:02.000000 openart-0.0.1/test/test_openart.py
+drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:43:36.103659 openart-0.0.2/
+-rw-r--r--   0 zero      (1000) zero      (1001)     1064 2023-04-12 22:21:15.000000 openart-0.0.2/LICENSE
+-rw-r--r--   0 zero      (1000) zero      (1001)     1446 2023-04-12 22:43:36.100326 openart-0.0.2/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 22:33:07.000000 openart-0.0.2/README.md
+drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:43:36.090326 openart-0.0.2/openart/
+-rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 21:44:23.000000 openart-0.0.2/openart/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1001)      354 2023-04-12 22:11:18.000000 openart-0.0.2/openart/openart.py
+drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:43:36.100326 openart-0.0.2/openart.egg-info/
+-rw-r--r--   0 zero      (1000) zero      (1001)     1446 2023-04-12 22:43:35.000000 openart-0.0.2/openart.egg-info/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1001)      227 2023-04-12 22:43:35.000000 openart-0.0.2/openart.egg-info/SOURCES.txt
+-rw-r--r--   0 zero      (1000) zero      (1001)        1 2023-04-12 22:43:35.000000 openart-0.0.2/openart.egg-info/dependency_links.txt
+-rw-r--r--   0 zero      (1000) zero      (1001)       13 2023-04-12 22:43:35.000000 openart-0.0.2/openart.egg-info/top_level.txt
+-rw-r--r--   0 zero      (1000) zero      (1001)       38 2023-04-12 22:43:36.103659 openart-0.0.2/setup.cfg
+-rw-r--r--   0 zero      (1000) zero      (1001)      609 2023-04-12 22:37:04.000000 openart-0.0.2/setup.py
+drwxr-xr-x   0 zero      (1000) zero      (1001)        0 2023-04-12 22:43:36.100326 openart-0.0.2/test/
+-rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 21:44:59.000000 openart-0.0.2/test/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1001)        0 2023-04-12 22:11:02.000000 openart-0.0.2/test/test_openart.py
```

### Comparing `openart-0.0.1/LICENSE` & `openart-0.0.2/LICENSE`

 * *Files identical despite different names*

