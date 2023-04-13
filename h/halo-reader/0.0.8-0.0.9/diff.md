# Comparing `tmp/halo-reader-0.0.8.tar.gz` & `tmp/halo-reader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halo-reader-0.0.8.tar", last modified: Wed Apr 12 11:30:47 2023, max compression
+gzip compressed data, was "halo-reader-0.0.9.tar", last modified: Thu Apr 13 12:01:53 2023, max compression
```

## Comparing `halo-reader-0.0.8.tar` & `halo-reader-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 11:30:24.000000 halo-reader-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 11:30:24.000000 halo-reader-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 11:30:47.855285 halo-reader-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-12 11:30:24.000000 halo-reader-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-12 11:30:24.000000 halo-reader-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:47.855285 halo-reader-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 11:30:24.000000 halo-reader-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.843284 halo-reader-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/halo_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 11:30:47.000000 halo-reader-0.0.8/src/halo_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/haloboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloboard/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.847284 halo-reader-0.0.8/src/halodata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/halodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/halodata/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.851285 halo-reader-0.0.8/src/haloreader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/attenuated_backscatter_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/background_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/src/haloreader/background_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-12 11:30:45.000000 halo-reader-0.0.8/src/haloreader/background_reader/background_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/background_reader/background_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/src/haloreader/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-12 11:30:46.000000 halo-reader-0.0.8/src/haloreader/data_reader/data_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/data_reader/data_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/grammar_header.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/halo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 11:30:24.000000 halo-reader-0.0.8/src/haloreader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:47.855285 halo-reader-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 11:30:24.000000 halo-reader-0.0.8/tests/test_halo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 12:01:23.000000 halo-reader-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 12:01:23.000000 halo-reader-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-13 12:01:53.755583 halo-reader-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 12:01:23.000000 halo-reader-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-13 12:01:23.000000 halo-reader-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:01:53.755583 halo-reader-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 12:01:23.000000 halo-reader-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.743583 halo-reader-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/halo_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:01:52.000000 halo-reader-0.0.9/src/halo_reader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 12:01:53.000000 halo-reader-0.0.9/src/halo_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/haloboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloboard/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.747583 halo-reader-0.0.9/src/halodata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/halodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/halodata/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.751583 halo-reader-0.0.9/src/haloreader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/attenuated_backscatter_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/background_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.751583 halo-reader-0.0.9/src/haloreader/background_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-13 12:01:51.000000 halo-reader-0.0.9/src/haloreader/background_reader/background_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/background_reader/background_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/src/haloreader/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-13 12:01:52.000000 halo-reader-0.0.9/src/haloreader/data_reader/data_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/data_reader/data_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/grammar_header.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 12:01:23.000000 halo-reader-0.0.9/src/haloreader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:01:53.755583 halo-reader-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-13 12:01:23.000000 halo-reader-0.0.9/tests/test_halo_reader.py
```

### Comparing `halo-reader-0.0.8/LICENSE` & `halo-reader-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/PKG-INFO` & `halo-reader-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.8
+Version: 0.0.9
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.8/README.md` & `halo-reader-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/pyproject.toml` & `halo-reader-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/setup.py` & `halo-reader-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/halo_reader.egg-info/PKG-INFO` & `halo-reader-0.0.9/src/halo_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.0.8
+Version: 0.0.9
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.0.8/src/halo_reader.egg-info/SOURCES.txt` & `halo-reader-0.0.9/src/halo_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloboard/app.py` & `halo-reader-0.0.9/src/haloboard/app.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloboard/static/favicon.ico` & `halo-reader-0.0.9/src/haloboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloboard/static/style.css` & `halo-reader-0.0.9/src/haloboard/static/style.css`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloboard/templates/index.html` & `halo-reader-0.0.9/src/haloboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/halodata/datasets.py` & `halo-reader-0.0.9/src/halodata/datasets.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/attenuated_backscatter_coefficient.py` & `halo-reader-0.0.9/src/haloreader/attenuated_backscatter_coefficient.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 from haloreader.type_guards import is_ndarray
 from haloreader.variable import Variable
 
 log = logging.getLogger(__name__)
 
 
-def compute_beta(intensity: Variable, range_: Variable, focus: Variable) -> Variable:
+def compute_beta(
+    intensity: Variable, range_: Variable, focus: Variable, wavelength: Variable
+) -> Variable:
     # pylint: disable=invalid-name
     """
     Parameters
     ----------
     range_
         distance from the instrument
     focus
@@ -44,21 +46,27 @@
             Antti Juhani Manninen, and Pablo Ortiz-Amezcua
         doi: https://doi.org/10.5194/amt-13-2849-2020
     """
     if not is_ndarray(intensity.data):
         raise TypeError
     if not is_ndarray(range_.data):
         raise TypeError
+    if not isinstance(wavelength.data, float):
+        raise TypeError
+    if wavelength.units != "m":
+        raise NotImplementedError(
+            f'Expected wavelength units "m", got "{wavelength.units}".'
+        )
 
     r = range_.data
     h = constants.Planck
     eta = 1
     c = constants.speed_of_light
     E = 1e-5
-    lambda_ = 1.5e-6
+    lambda_ = wavelength.data
     nu = c / lambda_
     B = 5e7
     A_e = compute_effective_receiver_energy(range_, focus, lambda_)
     snr = intensity.data - 1
     # ref: https://doi.org/10.5194/amt-13-2849-2020
     beta = 2 * h * nu * B * r**2 * snr / (eta * c * E * A_e)
     return Variable(
@@ -79,15 +87,15 @@
     # pylint: disable=invalid-name
     """
     Parameters
     ----------
     range_
         distance from the instrument
     focus
-        focal length og the telescope for the transmitter and receiver
+        effective focal length of the telescope for the transmitter and receiver
     lambda_
         laser wavelength
     """
     if not is_ndarray(range_.data):
         raise TypeError
     log.warning(
         "Using placeholder values from https://doi.org/10.5194/amt-13-2849-2020"
```

### Comparing `halo-reader-0.0.8/src/haloreader/attribute.py` & `halo-reader-0.0.9/src/haloreader/attribute.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/background_correction.py` & `halo-reader-0.0.9/src/haloreader/background_correction.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/background_reader/background_reader.c` & `halo-reader-0.0.9/src/haloreader/background_reader/background_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/background_reader/background_reader.pyx` & `halo-reader-0.0.9/src/haloreader/background_reader/background_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/cli.py` & `halo-reader-0.0.9/src/haloreader/cli.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/data_reader/data_reader.c` & `halo-reader-0.0.9/src/haloreader/data_reader/data_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/data_reader/data_reader.pyx` & `halo-reader-0.0.9/src/haloreader/data_reader/data_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/grammar_header.lark` & `halo-reader-0.0.9/src/haloreader/grammar_header.lark`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/halo.py` & `halo-reader-0.0.9/src/haloreader/halo.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,18 @@
         )
 
     def compute_beta(self) -> None:
         if not isinstance(self.intensity, Variable):
             raise TypeError
         log.warning("beta is computed using placeholder values")
         self.beta = haloreader.attenuated_backscatter_coefficient.compute_beta(
-            self.intensity, self.range, self.metadata.focus_range
+            self.intensity,
+            self.range,
+            self.metadata.focus_range,
+            self.metadata.wavelength,
         )
 
     def compute_noise_screen(self) -> Variable:
         if not isinstance(self.intensity, Variable):
             raise TypeError
         return haloreader.screen.compute_noise_screen(
             self.intensity, self.doppler_velocity
```

### Comparing `halo-reader-0.0.8/src/haloreader/metadata.py` & `halo-reader-0.0.9/src/haloreader/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     scantype: Attribute
     focus_range: Variable
     start_time: Variable
     resolution: Variable
     nrays: Variable | None = None
     nwaypoints: Variable | None = None
     instrument_spectral_width: Variable | None = None
-    wavelength: Variable | None = field(
+    wavelength: Variable = field(
         default_factory=lambda: Variable(
             name="wavelength",
             standard_name="radiation_wavelength",
             units="m",
-            data=1.5e-6,
+            data=1.565e-6,
         )
     )
     haloreader_version: Attribute = field(
         default_factory=lambda: Attribute(name="haloreader_version", value=pkgversion)
     )
     conventions: Attribute = field(
         default_factory=lambda: Attribute(name="Conventions", value="CF-1.8")
```

### Comparing `halo-reader-0.0.8/src/haloreader/read.py` & `halo-reader-0.0.9/src/haloreader/read.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/scantype.py` & `halo-reader-0.0.9/src/haloreader/scantype.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/screen.py` & `halo-reader-0.0.9/src/haloreader/screen.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/transformer.py` & `halo-reader-0.0.9/src/haloreader/transformer.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/type_guards.py` & `halo-reader-0.0.9/src/haloreader/type_guards.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/utils.py` & `halo-reader-0.0.9/src/haloreader/utils.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/src/haloreader/variable.py` & `halo-reader-0.0.9/src/haloreader/variable.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.0.8/tests/test_halo_reader.py` & `halo-reader-0.0.9/tests/test_halo_reader.py`

 * *Files identical despite different names*

