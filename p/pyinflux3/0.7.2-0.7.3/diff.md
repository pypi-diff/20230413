# Comparing `tmp/pyinflux3-0.7.2.tar.gz` & `tmp/pyinflux3-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.7.2.tar", last modified: Thu Apr 13 13:19:16 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.3.tar", last modified: Thu Apr 13 13:30:16 2023, max compression
```

## Comparing `pyinflux3-0.7.2.tar` & `pyinflux3-0.7.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.104330 pyinflux3-0.7.2/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:19:16.103871 pyinflux3-0.7.2/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.2/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.100456 pyinflux3-0.7.2/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.2/influxdb_client_3/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.7.2/influxdb_client_3/influx3.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:19:16.103162 pyinflux3-0.7.2/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      241 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       95 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 13:19:16.000000 pyinflux3-0.7.2/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 13:19:16.104499 pyinflux3-0.7.2/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     2121 2023-04-13 13:19:12.000000 pyinflux3-0.7.2/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:30:16.529216 pyinflux3-0.7.3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:30:16.528733 pyinflux3-0.7.3/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1742 2023-04-12 13:42:15.000000 pyinflux3-0.7.3/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:30:16.524647 pyinflux3-0.7.3/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.7.3/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.7.3/influxdb_client_3/influx3.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-13 13:30:16.527988 pyinflux3-0.7.3/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2455 2023-04-13 13:30:16.000000 pyinflux3-0.7.3/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      241 2023-04-13 13:30:16.000000 pyinflux3-0.7.3/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-13 13:30:16.000000 pyinflux3-0.7.3/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       95 2023-04-13 13:30:16.000000 pyinflux3-0.7.3/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-13 13:30:16.000000 pyinflux3-0.7.3/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-13 13:30:16.529331 pyinflux3-0.7.3/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2123 2023-04-13 13:30:07.000000 pyinflux3-0.7.3/setup.py
```

### Comparing `pyinflux3-0.7.2/PKG-INFO` & `pyinflux3-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.2
+Version: 0.7.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.2/README.md` & `pyinflux3-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.2/influxdb_client_3/__init__.py` & `pyinflux3-0.7.3/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.2/influxdb_client_3/influx3.py` & `pyinflux3-0.7.3/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.7.2/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.3/pyinflux3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.7.2
+Version: 0.7.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.7.2/setup.py` & `pyinflux3-0.7.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import setup
 import os
 import re
 import sys
 
 binary_name = "influx3"
 binary_destination = os.path.join("bin", binary_name)
-data_files = {'influx3': ['influxdb_client_3/influx3.py']} if 'cli' in sys.argv else {}
-entry_points = {'console_scripts': [f"{binary_name} = influxdb_client_3.influx3:main"]} if 'cli' in sys.argv else {}
+
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def get_version_from_github_ref():
     github_ref = os.environ.get("GITHUB_REF")
     if not github_ref:
@@ -25,40 +24,43 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.7.2"
+    return "v0.7.3"
 
+
+data_files = {'influx3': ['influxdb_client_3/influx3.py']} if 'cli' in sys.argv else {}
+entry_points = {'console_scripts': [f"{binary_name} = influxdb_client_3.influx3:main"]} if 'cli' in sys.argv else {}
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/pyinflux3',
     packages=['influxdb_client_3'],
-    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit', 'pandas', "tabulate"],
+    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     # Use extras_require to make data_files and entry_points optional
     extras_require={
-        'cli': ['pathlib']
+        'cli': ['pathlib', 'pygments', 'prompt_toolkit', 'pandas', "tabulate"]
     },
     # Conditionally include data_files and entry_points
     data_files=data_files,
     entry_points=entry_points,
 )
```

