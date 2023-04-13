# Comparing `tmp/netrohomeapi-0.1.1.tar.gz` & `tmp/netrohomeapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netrohomeapi-0.1.1.tar", last modified: Thu Apr 13 14:01:51 2023, max compression
+gzip compressed data, was "netrohomeapi-0.1.2.tar", last modified: Thu Apr 13 14:14:14 2023, max compression
```

## Comparing `netrohomeapi-0.1.1.tar` & `netrohomeapi-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.167073 netrohomeapi-0.1.1/netrohomeapi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/netrohomeapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/netrohomeapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:14:14.443585 netrohomeapi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:14:14.443585 netrohomeapi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:14:14.443585 netrohomeapi-0.1.2/netrohomeapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/netrohomeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/netrohomeapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/netrohomeapi/netrohomeapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:14:14.443585 netrohomeapi-0.1.2/netrohomeapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:14:14.000000 netrohomeapi-0.1.2/netrohomeapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 14:14:14.000000 netrohomeapi-0.1.2/netrohomeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:14:14.000000 netrohomeapi-0.1.2/netrohomeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 14:14:14.000000 netrohomeapi-0.1.2/netrohomeapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 14:14:14.000000 netrohomeapi-0.1.2/netrohomeapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 14:14:14.443585 netrohomeapi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 14:13:57.000000 netrohomeapi-0.1.2/setup.py
```

### Comparing `netrohomeapi-0.1.1/LICENSE` & `netrohomeapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netrohomeapi-0.1.1/PKG-INFO` & `netrohomeapi-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: netrohomeapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for NetroHome API
 Home-page: https://github.com/GeorgeBark/netrohomeapi
-Download-URL: https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.2.tar.gz
 Author: George Bark
 Author-email: georgebark2000@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netrohomeapi-0.1.1/netrohomeapi/models.py` & `netrohomeapi-0.1.2/netrohomeapi/models.py`

 * *Files identical despite different names*

### Comparing `netrohomeapi-0.1.1/netrohomeapi/netrohomeapi.py` & `netrohomeapi-0.1.2/netrohomeapi/netrohomeapi.py`

 * *Files identical despite different names*

### Comparing `netrohomeapi-0.1.1/netrohomeapi.egg-info/PKG-INFO` & `netrohomeapi-0.1.2/netrohomeapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: netrohomeapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for NetroHome API
 Home-page: https://github.com/GeorgeBark/netrohomeapi
-Download-URL: https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.2.tar.gz
 Author: George Bark
 Author-email: georgebark2000@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netrohomeapi-0.1.1/setup.py` & `netrohomeapi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='netrohomeapi',
     packages=['netrohomeapi'],
-    version='0.1.1',
+    version='0.1.2',
     license='MIT',
     description='Python wrapper for NetroHome API',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     author='George Bark',
     author_email='georgebark2000@gmail.com',
     url='https://github.com/GeorgeBark/netrohomeapi',
-    download_url='https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.1.tar.gz',
+    download_url='https://github.com/GeorgeBark/netrohomeapi/archive/refs/tags/v0.1.2.tar.gz',
     install_requires=[
         'aiohttp',
         'pydantic'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

