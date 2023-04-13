# Comparing `tmp/pyinflux3-0.7.1.tar.gz` & `tmp/pyinflux3-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.1.tar", last modified: Thu Apr 13 13:09:23 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.2.tar", last modified: Thu Apr 13 13:19:16 2023, max compression
```

## Comparing `pyinflux3-0.7.1.tar` & `pyinflux3-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.064792 pyinflux3-0.7.1/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:09:23.064461 pyinflux3-0.7.1/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.1/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.060600 pyinflux3-0.7.1/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.1/influxdb_client_3/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.7.1/influxdb_client_3/influx3.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.063811 pyinflux3-0.7.1/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       95 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 13:09:23.064902 pyinflux3-0.7.1/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1946 2023-04-13 13:09:20.000000 pyinflux3-0.7.1/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.104330 pyinflux3-0.7.2/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:19:16.103871 pyinflux3-0.7.2/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.2/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.100456 pyinflux3-0.7.2/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.2/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.7.2/influxdb_client_3/influx3.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.103162 pyinflux3-0.7.2/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      241 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       95 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 13:19:16.104499 pyinflux3-0.7.2/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2121 2023-04-13 13:19:12.000000 pyinflux3-0.7.2/setup.py
```

### Comparing `pyinflux3-0.7.1/PKG-INFO` & `pyinflux3-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.1
+Version: 0.7.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.1/README.md` & `pyinflux3-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.1/influxdb_client_3/__init__.py` & `pyinflux3-0.7.2/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.1/influxdb_client_3/influx3.py` & `pyinflux3-0.7.2/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.1/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.2/pyinflux3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.1
+Version: 0.7.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.1/setup.py` & `pyinflux3-0.7.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from setuptools import setup
 import os
 import re
+import sys
 
 binary_name = "influx3"
 binary_destination = os.path.join("bin", binary_name)
+data_files = {'influx3': ['influxdb_client_3/influx3.py']} if 'cli' in sys.argv else {}
+entry_points = {'console_scripts': [f"{binary_name} = influxdb_client_3.influx3:main"]} if 'cli' in sys.argv else {}
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def get_version_from_github_ref():
     github_ref = os.environ.get("GITHUB_REF")
     if not github_ref:
@@ -22,15 +25,15 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.7.1"
+    return "v0.7.2"
 
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -50,11 +53,12 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     # Use extras_require to make data_files and entry_points optional
     extras_require={
         'cli': ['pathlib']
     },
-    data_files=[('influx3', ['influxdb_client_3/influx3.py'])],
-    entry_points={"console_scripts": [f"{binary_name} = influxdb_client_3.influx3:main"]},
+    # Conditionally include data_files and entry_points
+    data_files=data_files,
+    entry_points=entry_points,
 )
```

