# Comparing `tmp/pycachera-3.0.2.tar.gz` & `tmp/pycachera-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycachera-3.0.2.tar", last modified: Wed Apr 12 03:37:45 2023, max compression
+gzip compressed data, was "pycachera-4.0.0.tar", last modified: Thu Apr 13 03:34:56 2023, max compression
```

## Comparing `pycachera-3.0.2.tar` & `pycachera-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-12 03:37:36.000000 pycachera-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-12 03:37:45.947222 pycachera-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-04-12 03:37:36.000000 pycachera-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/pycachera/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 03:37:36.000000 pycachera-3.0.2/pycachera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 03:37:36.000000 pycachera-3.0.2/pycachera/cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/pycachera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 03:37:45.947222 pycachera-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-12 03:37:36.000000 pycachera-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-13 03:34:47.000000 pycachera-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 03:34:56.195941 pycachera-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-04-13 03:34:47.000000 pycachera-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/pycachera/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5265 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/pycachera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 03:34:56.195941 pycachera-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-13 03:34:47.000000 pycachera-4.0.0/setup.py
```

### Comparing `pycachera-3.0.2/LICENSE` & `pycachera-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycachera-3.0.2/PKG-INFO` & `pycachera-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycachera
-Version: 3.0.2
+Version: 4.0.0
 Summary: A powerfull python caching tool
 Home-page: https://github.com/antolonappan/pycachera
 Author: Anto Idicherian Lonappan
 Author-email: mail@antolonappan.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycachera-3.0.2/README.md` & `pycachera-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pycachera-3.0.2/pycachera/cacher.py` & `pycachera-4.0.0/pycachera/cacher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import numpy as np
 from hashlib import md5
 import pickle as pl
 from numpy import ndarray
 import pandas as pd
-
+from pycachera import mpi
         
 class Cache(object):
     """
     This is a decorator class, used for caching functions and class attributes.
     
     Args(optional):
         :cachefolder (*str*): Folder for caching; if not found, the cache folder is set to '.cache' in the current working directory
@@ -124,14 +124,17 @@
                 else:
                     a += str(0)
             
             if type(tag) == pd.DataFrame:
                 a += ''.join(map(str,list(tag.columns)))
                 a += f'{len(tag)}'
 
+        
+        a += str(mpi.rank)
+
         return md5(a.encode()).hexdigest()
     
     def file_writer(self,name,data):
         """
         Writes data to a file
         save the data in a pickle file
         """
```

### Comparing `pycachera-3.0.2/pycachera.egg-info/PKG-INFO` & `pycachera-4.0.0/pycachera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycachera
-Version: 3.0.2
+Version: 4.0.0
 Summary: A powerfull python caching tool
 Home-page: https://github.com/antolonappan/pycachera
 Author: Anto Idicherian Lonappan
 Author-email: mail@antolonappan.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycachera-3.0.2/setup.py` & `pycachera-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 files = ["pycachera/*"]
 setup(
         name = 'pycachera',
         packages = ['pycachera'],
         package_data = {'pycachera' : files },
-        version = '3.0.2',
+        version = '4.0.0',
         install_requires = ['numpy','pandas'],
         description = 'A powerfull python caching tool',
         author = 'Anto Idicherian Lonappan',
         author_email = 'mail@antolonappan.me',
         url = 'https://github.com/antolonappan/pycachera',
         long_description=long_description,
         long_description_content_type="text/markdown",
```

