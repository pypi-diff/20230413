# Comparing `tmp/pyinflux3-0.7.0.tar.gz` & `tmp/pyinflux3-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.0.tar", last modified: Tue Apr 11 17:56:19 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.1.tar", last modified: Thu Apr 13 13:09:23 2023, max compression
```

## Comparing `pyinflux3-0.7.0.tar` & `pyinflux3-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.830894 pyinflux3-0.7.0/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/influxdb_client_3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/influxdb_client_3/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.064792 pyinflux3-0.7.1/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:09:23.064461 pyinflux3-0.7.1/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.1/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.060600 pyinflux3-0.7.1/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.1/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.7.1/influxdb_client_3/influx3.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:09:23.063811 pyinflux3-0.7.1/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/entry_points.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       95 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 13:09:23.000000 pyinflux3-0.7.1/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 13:09:23.064902 pyinflux3-0.7.1/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1946 2023-04-13 13:09:20.000000 pyinflux3-0.7.1/setup.py
```

### Comparing `pyinflux3-0.7.0/PKG-INFO` & `pyinflux3-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.0
+Version: 0.7.1
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
 
 # Add a Config
-You can drop a config files call config.json next to the python code: 
+You can drop a config file called config.json in the directory where you are running the influx3 command:
 
 ```json
 {
 {
     "my-config": {
         "namespace": "your-namespace",
         "host": "your-host",
@@ -38,30 +39,30 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
 % influx3 sql "select * from anomalies"
 ```
 
 ```
 % influx3 write testmes f=7 
 ```
 
-# Run and Query Interactively
-So far only the query command is supported.
+# Query and Write Interactively
+
 
 ```
 % influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
```

### Comparing `pyinflux3-0.7.0/README.md` & `pyinflux3-0.7.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This is a community repository of Python code for InfluxDB with IOx. While this code is built on officially supported APIs, the library and CLI here are not officially support by Influx Data. 
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
 # Add a Config
-You can drop a config files call config.json next to the python code: 
+You can drop a config file called config.json in the directory where you are running the influx3 command:
 
 ```json
 {
 {
     "my-config": {
         "namespace": "your-namespace",
         "host": "your-host",
@@ -20,30 +20,30 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
 % influx3 sql "select * from anomalies"
 ```
 
 ```
 % influx3 write testmes f=7 
 ```
 
-# Run and Query Interactively
-So far only the query command is supported.
+# Query and Write Interactively
+
 
 ```
 % influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
```

### Comparing `pyinflux3-0.7.0/influxdb_client_3/__init__.py` & `pyinflux3-0.7.1/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.0/influxdb_client_3/influx3.py` & `pyinflux3-0.7.1/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.0/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.1/pyinflux3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.0
+Version: 0.7.1
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
 
 # Add a Config
-You can drop a config files call config.json next to the python code: 
+You can drop a config file called config.json in the directory where you are running the influx3 command:
 
 ```json
 {
 {
     "my-config": {
         "namespace": "your-namespace",
         "host": "your-host",
@@ -38,30 +39,30 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
 % influx3 sql "select * from anomalies"
 ```
 
 ```
 % influx3 write testmes f=7 
 ```
 
-# Run and Query Interactively
-So far only the query command is supported.
+# Query and Write Interactively
+
 
 ```
 % influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
```

### Comparing `pyinflux3-0.7.0/setup.py` & `pyinflux3-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.6.3"
+    return "v0.7.1"
 
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -46,11 +46,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
+    # Use extras_require to make data_files and entry_points optional
+    extras_require={
+        'cli': ['pathlib']
+    },
     data_files=[('influx3', ['influxdb_client_3/influx3.py'])],
     entry_points={"console_scripts": [f"{binary_name} = influxdb_client_3.influx3:main"]},
+)
 
-)
```

