# Comparing `tmp/aiolifx-0.8.8.tar.gz` & `tmp/aiolifx-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolifx-0.8.8.tar", last modified: Wed Feb  8 15:00:46 2023, max compression
+gzip compressed data, was "aiolifx-0.8.9.tar", last modified: Thu Feb  9 13:37:03 2023, max compression
```

## Comparing `aiolifx-0.8.8.tar` & `aiolifx-0.8.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-08 15:00:46.179081 aiolifx-0.8.8/
--rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-0.8.8/LICENSE.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-0.8.8/MANIFEST.in
--rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-08 15:00:46.179081 aiolifx-0.8.8/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)     3316 2022-09-29 07:38:39.000000 aiolifx-0.8.8/README.md
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-08 15:00:46.179081 aiolifx-0.8.8/aiolifx/
--rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-0.8.8/aiolifx/__init__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    19095 2022-09-24 03:41:41.000000 aiolifx-0.8.8/aiolifx/__main__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    75045 2023-02-08 14:59:15.000000 aiolifx-0.8.8/aiolifx/aiolifx.py
--rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-0.8.8/aiolifx/connection.py
--rw-rw-r--   0 fw        (1000) fw        (1000)     6393 2021-05-03 10:41:06.000000 aiolifx-0.8.8/aiolifx/message.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    55837 2022-09-29 07:36:29.000000 aiolifx-0.8.8/aiolifx/msgtypes.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    30247 2023-02-08 14:41:06.000000 aiolifx-0.8.8/aiolifx/products.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    20159 2022-09-29 07:36:29.000000 aiolifx-0.8.8/aiolifx/unpack.py
--rwxrwxr-x   0 fw        (1000) fw        (1000)     1473 2022-04-26 14:59:59.000000 aiolifx-0.8.8/aiolifx/update-products.py
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-08 15:00:46.179081 aiolifx-0.8.8/aiolifx.egg-info/
--rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)      455 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/SOURCES.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/dependency_links.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       50 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/entry_points.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/not-zip-safe
--rw-rw-r--   0 fw        (1000) fw        (1000)       17 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/requires.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        8 2023-02-08 15:00:46.000000 aiolifx-0.8.8/aiolifx.egg-info/top_level.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       79 2023-02-08 15:00:46.179081 aiolifx-0.8.8/setup.cfg
--rw-rw-r--   0 fw        (1000) fw        (1000)     1205 2023-02-08 14:54:14.000000 aiolifx-0.8.8/setup.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-0.8.9/LICENSE.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-0.8.9/MANIFEST.in
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-09 13:37:03.513687 aiolifx-0.8.9/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3316 2022-09-29 07:38:39.000000 aiolifx-0.8.9/README.md
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/aiolifx/
+-rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-0.8.9/aiolifx/__init__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    19095 2022-09-24 03:41:41.000000 aiolifx-0.8.9/aiolifx/__main__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    75045 2023-02-08 14:59:15.000000 aiolifx-0.8.9/aiolifx/aiolifx.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-0.8.9/aiolifx/connection.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)     6393 2021-05-03 10:41:06.000000 aiolifx-0.8.9/aiolifx/message.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    55837 2022-09-29 07:36:29.000000 aiolifx-0.8.9/aiolifx/msgtypes.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    30251 2023-02-09 13:33:52.000000 aiolifx-0.8.9/aiolifx/products.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    20159 2022-09-29 07:36:29.000000 aiolifx-0.8.9/aiolifx/unpack.py
+-rwxrwxr-x   0 fw        (1000) fw        (1000)     1473 2022-04-26 14:59:59.000000 aiolifx-0.8.9/aiolifx/update-products.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2023-02-09 13:37:03.513687 aiolifx-0.8.9/aiolifx.egg-info/
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3785 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)      455 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       50 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/entry_points.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/not-zip-safe
+-rw-rw-r--   0 fw        (1000) fw        (1000)       17 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/requires.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        8 2023-02-09 13:37:03.000000 aiolifx-0.8.9/aiolifx.egg-info/top_level.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       79 2023-02-09 13:37:03.513687 aiolifx-0.8.9/setup.cfg
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1205 2023-02-09 13:35:35.000000 aiolifx-0.8.9/setup.py
```

### Comparing `aiolifx-0.8.8/LICENSE.txt` & `aiolifx-0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/PKG-INFO` & `aiolifx-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 0.8.8
+Version: 0.8.9
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiolifx-0.8.8/README.md` & `aiolifx-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/__main__.py` & `aiolifx-0.8.9/aiolifx/__main__.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/aiolifx.py` & `aiolifx-0.8.9/aiolifx/aiolifx.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/connection.py` & `aiolifx-0.8.9/aiolifx/connection.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/message.py` & `aiolifx-0.8.9/aiolifx/message.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/msgtypes.py` & `aiolifx-0.8.9/aiolifx/msgtypes.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/products.py` & `aiolifx-0.8.9/aiolifx/products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1013,34 +1013,34 @@
         "multizone": True,
         "relays": False,
     },
     121: {
         "buttons": False,
         "chain": False,
         "color": True,
-        "extended_multizone": True,
+        "extended_multizone": False,
         "hev": False,
         "infrared": False,
         "matrix": False,
         "max_kelvin": 9000,
         "min_kelvin": 1500,
-        "multizone": True,
+        "multizone": False,
         "relays": False,
     },
     122: {
         "buttons": False,
         "chain": False,
         "color": True,
-        "extended_multizone": True,
+        "extended_multizone": False,
         "hev": False,
         "infrared": False,
         "matrix": False,
         "max_kelvin": 9000,
         "min_kelvin": 1500,
-        "multizone": True,
+        "multizone": False,
         "relays": False,
     },
     123: {
         "buttons": False,
         "chain": False,
         "color": True,
         "extended_multizone": False,
```

### Comparing `aiolifx-0.8.8/aiolifx/unpack.py` & `aiolifx-0.8.9/aiolifx/unpack.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx/update-products.py` & `aiolifx-0.8.9/aiolifx/update-products.py`

 * *Files identical despite different names*

### Comparing `aiolifx-0.8.8/aiolifx.egg-info/PKG-INFO` & `aiolifx-0.8.9/aiolifx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 0.8.8
+Version: 0.8.9
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiolifx-0.8.8/setup.py` & `aiolifx-0.8.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 import setuptools
 
-version = "0.8.8"
+version = "0.8.9"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiolifx",
     packages=["aiolifx"],
```

