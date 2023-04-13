# Comparing `tmp/pyinflux3-0.7.4.tar.gz` & `tmp/pyinflux3-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.4.tar", last modified: Thu Apr 13 14:43:36 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.5.tar", last modified: Thu Apr 13 14:47:44 2023, max compression
```

## Comparing `pyinflux3-0.7.4.tar` & `pyinflux3-0.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:36.929100 pyinflux3-0.7.4/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2435 2023-04-13 14:43:36.928755 pyinflux3-0.7.4/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.4/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:36.925517 pyinflux3-0.7.4/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.4/influxdb_client_3/__init__.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:43:36.928083 pyinflux3-0.7.4/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2435 2023-04-13 14:43:36.000000 pyinflux3-0.7.4/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      219 2023-04-13 14:43:36.000000 pyinflux3-0.7.4/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 14:43:36.000000 pyinflux3-0.7.4/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       80 2023-04-13 14:43:36.000000 pyinflux3-0.7.4/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 14:43:36.000000 pyinflux3-0.7.4/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)     1664 2023-04-13 14:42:28.000000 pyinflux3-0.7.4/setup-client.py
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 14:43:36.929229 pyinflux3-0.7.4/setup.cfg
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.691131 pyinflux3-0.7.5/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 14:47:44.690784 pyinflux3-0.7.5/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.5/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.686756 pyinflux3-0.7.5/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.5/influxdb_client_3/__init__.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 14:47:44.690122 pyinflux3-0.7.5/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      219 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)      101 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 14:47:44.000000 pyinflux3-0.7.5/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1794 2023-04-13 14:47:39.000000 pyinflux3-0.7.5/setup-client.py
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 14:47:44.691234 pyinflux3-0.7.5/setup.cfg
```

### Comparing `pyinflux3-0.7.4/PKG-INFO` & `pyinflux3-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.4
+Version: 0.7.5
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 
 # About
 This is a community repository of Python code for InfluxDB with IOx. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
```

### Comparing `pyinflux3-0.7.4/README.md` & `pyinflux3-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.4/influxdb_client_3/__init__.py` & `pyinflux3-0.7.5/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.4/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.5/pyinflux3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.4
+Version: 0.7.5
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 
 # About
 This is a community repository of Python code for InfluxDB with IOx. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
```

### Comparing `pyinflux3-0.7.4/setup-client.py` & `pyinflux3-0.7.5/setup-client.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.7.4"
+    return "v0.7.5"
 
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -45,10 +45,13 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-    ]
-
+    ],
+   # Use extras_require to make data_files and entry_points optional
+    extras_require={
+        'cli': ['pyinflux3-cli']
+    },
 )
```

