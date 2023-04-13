# Comparing `tmp/maplab-0.2.1.tar.gz` & `tmp/maplab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maplab-0.2.1.tar", last modified: Wed Apr  5 18:47:51 2023, max compression
+gzip compressed data, was "maplab-0.2.2.tar", last modified: Thu Apr 13 19:16:16 2023, max compression
```

## Comparing `maplab-0.2.1.tar` & `maplab-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:47:51.397320 maplab-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 18:47:41.000000 maplab-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 18:47:41.000000 maplab-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-05 18:47:51.397320 maplab-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 18:47:41.000000 maplab-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:47:51.397320 maplab-0.2.1/maplab/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-05 18:47:41.000000 maplab-0.2.1/maplab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-05 18:47:41.000000 maplab-0.2.1/maplab/maplab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:47:51.397320 maplab-0.2.1/maplab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 18:47:51.000000 maplab-0.2.1/maplab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 18:47:41.000000 maplab-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-05 18:47:51.397320 maplab-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-05 18:47:41.000000 maplab-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:16:16.407204 maplab-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 19:16:07.000000 maplab-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 19:16:07.000000 maplab-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 19:16:16.407204 maplab-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 19:16:07.000000 maplab-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:16:16.407204 maplab-0.2.2/maplab/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 19:16:07.000000 maplab-0.2.2/maplab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-13 19:16:07.000000 maplab-0.2.2/maplab/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-04-13 19:16:07.000000 maplab-0.2.2/maplab/maplab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:16:16.407204 maplab-0.2.2/maplab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 19:16:16.000000 maplab-0.2.2/maplab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 19:16:07.000000 maplab-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-13 19:16:16.407204 maplab-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-13 19:16:07.000000 maplab-0.2.2/setup.py
```

### Comparing `maplab-0.2.1/LICENSE` & `maplab-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maplab-0.2.1/PKG-INFO` & `maplab-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maplab
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/hwilli72/maplab
 Author: Hannah Williams
 Author-email: hwilli72@vols.utk.edu
 License: MIT license
 Keywords: maplab
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `maplab-0.2.1/README.md` & `maplab-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `maplab-0.2.1/maplab.egg-info/PKG-INFO` & `maplab-0.2.2/maplab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maplab
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/hwilli72/maplab
 Author: Hannah Williams
 Author-email: hwilli72@vols.utk.edu
 License: MIT license
 Keywords: maplab
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `maplab-0.2.1/setup.py` & `maplab-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='maplab',
     name='maplab',
     packages=find_packages(include=['maplab', 'maplab.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hwilli72/maplab',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

