# Comparing `tmp/sirms-1.2.3.tar.gz` & `tmp/sirms-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sirms-1.2.3.tar", last modified: Thu Apr 13 08:41:46 2023, max compression
+gzip compressed data, was "dist/sirms-1.2.4.tar", last modified: Thu Apr 13 09:19:50 2023, max compression
```

## Comparing `sirms-1.2.3.tar` & `sirms-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-13 08:41:46.000000 sirms-1.2.3/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-04-13 08:41:46.000000 sirms-1.2.3/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/canon.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/mols.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/labels.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.3/sirms/ppgfunctions.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/sirms.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/sdf.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.3/sirms/sirms_name.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.3/sirms/files.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-04-13 08:40:13.000000 sirms-1.2.3/sirms/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3301 2023-04-13 08:32:29.000000 sirms-1.2.3/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      352 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-13 08:41:46.000000 sirms-1.2.3/sirms.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1160 2021-02-06 19:29:33.000000 sirms-1.2.3/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 09:19:50.000000 sirms-1.2.4/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4584 2023-04-13 09:19:50.000000 sirms-1.2.4/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-04-13 09:19:50.000000 sirms-1.2.4/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/canon.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/mols.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/labels.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.4/sirms/ppgfunctions.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/sirms.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/sdf.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.4/sirms/sirms_name.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.4/sirms/files.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-04-13 09:17:59.000000 sirms-1.2.4/sirms/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms/utilities/
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5644 2021-02-06 19:35:37.000000 sirms-1.2.4/sirms/utilities/calc_atomic_properties_chemaxon.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-04-13 09:16:04.000000 sirms-1.2.4/sirms/utilities/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3374 2023-04-13 09:18:59.000000 sirms-1.2.4/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4584 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      431 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-13 09:19:50.000000 sirms-1.2.4/sirms.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1177 2023-04-13 09:16:29.000000 sirms-1.2.4/setup.py
```

### Comparing `sirms-1.2.3/PKG-INFO` & `sirms-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.3
+Version: 1.2.4
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
         
@@ -74,14 +74,17 @@
         
         version 1.2.1 (08.02.2021)
         - fix README formatting
         
         version 1.2.2 (12.04.2023)
         - fix examples in README
         
+        version 1.2.4 (13.04.2023)
+        - fix import calc_atomic_properties_chemaxon
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
```

### Comparing `sirms-1.2.3/sirms/canon.py` & `sirms-1.2.4/sirms/canon.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/mols.py` & `sirms-1.2.4/sirms/mols.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/labels.py` & `sirms-1.2.4/sirms/labels.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/ppgfunctions.py` & `sirms-1.2.4/sirms/ppgfunctions.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/sirms.py` & `sirms-1.2.4/sirms/sirms.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/sdf.py` & `sirms-1.2.4/sirms/sdf.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/sirms_name.py` & `sirms-1.2.4/sirms/sirms_name.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/sirms/files.py` & `sirms-1.2.4/sirms/files.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.3/README.md` & `sirms-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,7 +65,10 @@
 - reorganized as a Python package
 
 version 1.2.1 (08.02.2021)
 - fix README formatting
 
 version 1.2.2 (12.04.2023)
 - fix examples in README
+
+version 1.2.4 (13.04.2023)
+- fix import calc_atomic_properties_chemaxon
```

### Comparing `sirms-1.2.3/sirms.egg-info/PKG-INFO` & `sirms-1.2.4/sirms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.3
+Version: 1.2.4
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
         
@@ -74,14 +74,17 @@
         
         version 1.2.1 (08.02.2021)
         - fix README formatting
         
         version 1.2.2 (12.04.2023)
         - fix examples in README
         
+        version 1.2.4 (13.04.2023)
+        - fix import calc_atomic_properties_chemaxon
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
```

### Comparing `sirms-1.2.3/setup.py` & `sirms-1.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     version=sirms.__version__,
     author="Pavel Polishchuk",
     author_email="pavel_polishchuk@ukr.net",
     description="SiRMS: simplex representation of molecular structure",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DrrDom/sirms",
-    packages=['sirms'],
+    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering :: Chemistry"
     ],
```

