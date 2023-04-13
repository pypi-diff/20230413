# Comparing `tmp/sirms-1.2.2.tar.gz` & `tmp/sirms-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sirms-1.2.2.tar", last modified: Wed Apr 12 07:34:35 2023, max compression
+gzip compressed data, was "dist/sirms-1.2.3.tar", last modified: Thu Apr 13 08:41:46 2023, max compression
```

## Comparing `sirms-1.2.2.tar` & `sirms-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-12 07:34:35.000000 sirms-1.2.2/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-04-12 07:34:35.000000 sirms-1.2.2/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/canon.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/mols.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/labels.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.2/sirms/ppgfunctions.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/sirms.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/sdf.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.2/sirms/sirms_name.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/files.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       21 2023-04-12 07:32:40.000000 sirms-1.2.2/sirms/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3301 2023-04-12 07:32:39.000000 sirms-1.2.2/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      352 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1160 2021-02-06 19:29:33.000000 sirms-1.2.2/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-13 08:41:46.000000 sirms-1.2.3/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-04-13 08:41:46.000000 sirms-1.2.3/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/canon.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/mols.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/labels.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.3/sirms/ppgfunctions.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/sirms.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/sdf.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.3/sirms/sirms_name.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/files.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-04-13 08:40:13.000000 sirms-1.2.3/sirms/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3301 2023-04-13 08:32:29.000000 sirms-1.2.3/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      352 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1160 2021-02-06 19:29:33.000000 sirms-1.2.3/setup.py
```

### Comparing `sirms-1.2.2/PKG-INFO` & `sirms-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.2
+Version: 1.2.3
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
```

### Comparing `sirms-1.2.2/sirms/canon.py` & `sirms-1.2.3/sirms/canon.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/mols.py` & `sirms-1.2.3/sirms/mols.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/labels.py` & `sirms-1.2.3/sirms/labels.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/ppgfunctions.py` & `sirms-1.2.3/sirms/ppgfunctions.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/sirms.py` & `sirms-1.2.3/sirms/sirms.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/sdf.py` & `sirms-1.2.3/sirms/sdf.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/sirms_name.py` & `sirms-1.2.3/sirms/sirms_name.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms/files.py` & `sirms-1.2.3/sirms/files.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/README.md` & `sirms-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sirms-1.2.2/sirms.egg-info/PKG-INFO` & `sirms-1.2.3/sirms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.2
+Version: 1.2.3
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
```

### Comparing `sirms-1.2.2/setup.py` & `sirms-1.2.3/setup.py`

 * *Files identical despite different names*

