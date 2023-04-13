# Comparing `tmp/spatialcsv-0.0.3.tar.gz` & `tmp/spatialcsv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialcsv-0.0.3.tar", last modified: Fri Apr  7 18:11:48 2023, max compression
+gzip compressed data, was "spatialcsv-0.0.5.tar", last modified: Thu Apr 13 01:33:55 2023, max compression
```

## Comparing `spatialcsv-0.0.3.tar` & `spatialcsv-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.3/LICENSE
--rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.3/MANIFEST.in
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1416 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      604 2023-04-06 01:34:42.000000 spatialcsv-0.0.3/README.md
--rw-r--r--   0 thomer    (1000) thomer    (1000)       20 2023-04-02 13:04:24.000000 spatialcsv-0.0.3/requirements.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/setup.cfg
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-07 18:08:15.000000 spatialcsv-0.0.3/setup.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/spatialcsv/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-07 18:08:15.000000 spatialcsv-0.0.3/spatialcsv/__init__.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.3/spatialcsv/cli.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1694 2023-04-07 17:27:44.000000 spatialcsv-0.0.3/spatialcsv/spatialcsv.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/spatialcsv.egg-info/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1416 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      395 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/SOURCES.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       21 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/dependency_links.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/entry_points.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.3/spatialcsv.egg-info/not-zip-safe
--rw-r--r--   0 thomer    (1000) thomer    (1000)       19 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/requires.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-07 18:11:47.000000 spatialcsv-0.0.3/spatialcsv.egg-info/top_level.txt
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-07 18:11:48.009990 spatialcsv-0.0.3/tests/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.3/tests/test_spatialcsv.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.5/LICENSE
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.5/MANIFEST.in
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      672 2023-04-12 23:58:14.000000 spatialcsv-0.0.5/README.md
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 01:16:34.000000 spatialcsv-0.0.5/requirements.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/setup.cfg
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-13 01:31:05.000000 spatialcsv-0.0.5/setup.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/spatialcsv/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-13 01:31:05.000000 spatialcsv-0.0.5/spatialcsv/__init__.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.5/spatialcsv/cli.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     4257 2023-04-13 01:12:49.000000 spatialcsv-0.0.5/spatialcsv/spatialcsv.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/spatialcsv.egg-info/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      395 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/SOURCES.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       39 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/dependency_links.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/entry_points.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.5/spatialcsv.egg-info/not-zip-safe
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/requires.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-13 01:33:55.000000 spatialcsv-0.0.5/spatialcsv.egg-info/top_level.txt
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 01:33:55.444374 spatialcsv-0.0.5/tests/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.5/tests/test_spatialcsv.py
```

### Comparing `spatialcsv-0.0.3/LICENSE` & `spatialcsv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.3/PKG-INFO` & `spatialcsv-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.3
+Version: 0.0.5
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -32,12 +32,12 @@
 
 -   Free software: GNU General Public License v3
 -   Documentation: https://tjhomer.github.io/spatialcsv/
     
 
 ## Features
 
--   TODO
+-   Will take a csv with Latitude and Longitude columns and add to a web map
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `spatialcsv-0.0.3/README.md` & `spatialcsv-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 -   Free software: GNU General Public License v3
 -   Documentation: https://tjhomer.github.io/spatialcsv/
     
 
 ## Features
 
--   TODO
+-   Will take a csv with Latitude and Longitude columns and add to a web map
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `spatialcsv-0.0.3/setup.py` & `spatialcsv-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     keywords='spatialcsv',
     name='spatialcsv',
     packages=find_packages(include=['spatialcsv', 'spatialcsv.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/TJHomer/spatialcsv',
-    version='0.0.3',
+    version='0.0.5',
     zip_safe=False,
 )
```

### Comparing `spatialcsv-0.0.3/spatialcsv.egg-info/PKG-INFO` & `spatialcsv-0.0.5/spatialcsv.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.3
+Version: 0.0.5
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -32,12 +32,12 @@
 
 -   Free software: GNU General Public License v3
 -   Documentation: https://tjhomer.github.io/spatialcsv/
     
 
 ## Features
 
--   TODO
+-   Will take a csv with Latitude and Longitude columns and add to a web map
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

