# Comparing `tmp/dargus-1.0.1.tar.gz` & `tmp/dargus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-f4ae7f3i/dargus-1.0.1.tar", last modified: Tue Apr 11 13:56:45 2023, max compression
+gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-3c59htmw/dargus-1.0.2.tar", last modified: Thu Apr 13 08:44:33 2023, max compression
```

## Comparing `dargus-1.0.1.tar` & `dargus-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.0.1/LICENSE
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-11 13:56:45.000000 dargus-1.0.1/PKG-INFO
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       73 2023-02-17 13:43:50.000000 dargus-1.0.1/README.md
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)        0 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/__init__.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13118 2023-03-29 12:05:47.000000 dargus-1.0.1/dargus/argus.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-04-11 13:10:00.000000 dargus-1.0.1/dargus/argus_cli.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2224 2023-03-29 12:05:47.000000 dargus-1.0.1/dargus/argus_config.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       43 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/argus_exceptions.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-02-06 09:28:40.000000 dargus-1.0.1/dargus/commons.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1567 2023-02-06 09:22:09.000000 dargus-1.0.1/dargus/utils.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)      889 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/validation_result.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     7118 2023-02-21 14:33:18.000000 dargus-1.0.1/dargus/validator.py
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/PKG-INFO
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/SOURCES.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/dependency_links.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/entry_points.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/requires.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/top_level.txt
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-04-11 13:50:24.000000 dargus-1.0.1/pyproject.toml
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-04-11 13:56:45.000000 dargus-1.0.1/setup.cfg
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       92 2023-02-17 14:07:57.000000 dargus-1.0.1/setup.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.0.2/LICENSE
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-13 08:44:33.000000 dargus-1.0.2/PKG-INFO
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       73 2023-02-17 13:43:50.000000 dargus-1.0.2/README.md
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)        0 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/__init__.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13228 2023-04-13 08:40:53.000000 dargus-1.0.2/dargus/argus.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-04-11 13:10:00.000000 dargus-1.0.2/dargus/argus_cli.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2350 2023-04-13 08:40:53.000000 dargus-1.0.2/dargus/argus_config.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       43 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/argus_exceptions.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-02-06 09:28:40.000000 dargus-1.0.2/dargus/commons.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1567 2023-02-06 09:22:09.000000 dargus-1.0.2/dargus/utils.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)      889 2020-07-29 10:38:30.000000 dargus-1.0.2/dargus/validation_result.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)     7118 2023-02-21 14:33:18.000000 dargus-1.0.2/dargus/validator.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/SOURCES.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/dependency_links.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/entry_points.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/requires.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-04-13 08:44:33.000000 dargus-1.0.2/dargus.egg-info/top_level.txt
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-04-13 08:43:59.000000 dargus-1.0.2/pyproject.toml
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-04-13 08:44:33.000000 dargus-1.0.2/setup.cfg
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       92 2023-02-17 14:07:57.000000 dargus-1.0.2/setup.py
```

### Comparing `dargus-1.0.1/LICENSE` & `dargus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/PKG-INFO` & `dargus-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.1/dargus/argus.py` & `dargus-1.0.2/dargus/argus.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,23 @@
 
     def __str__(self):
         return str(self.__dict__)
 
 
 class Argus:
     def __init__(self, test_folder, argus_config, out_fpath=None):
-        self.test_folder = test_folder
+        self.test_folder = os.path.realpath(os.path.expanduser(test_folder))
 
         self.config = argus_config
 
         if out_fpath is None:
             t = datetime.now().strftime('%Y%m%d%H%M%S')
             self.out_fpath = os.path.join(test_folder, 'argus_out_' + t + '.json')
         else:
+            out_fpath = os.path.realpath(os.path.expanduser(out_fpath))
             os.makedirs(os.path.dirname(out_fpath), exist_ok=True)
             self.out_fpath = out_fpath
 
         self.suites = []
 
         self.suite_ids = []
         self.test_ids = []
```

### Comparing `dargus-1.0.1/dargus/argus_cli.py` & `dargus-1.0.2/dargus/argus_cli.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/dargus/argus_config.py` & `dargus-1.0.2/dargus/argus_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 import requests
 import yaml
 
 
 class ArgusConfiguration(object):
     def __init__(self, config_input, validator=None, username=None, password=None, suites=None):
@@ -24,23 +25,24 @@
                 self._config[key] = config_input[key]
         else:
             config_dict = self._get_dictionary_from_file(config_input)
             for key in config_dict:
                 self._config[key] = config_dict[key]
 
         if validator is not None:
-            self._config['validator'] = validator
+            self._config['validator'] = os.path.realpath(os.path.expanduser(validator))
 
         if suites is not None:
             self._config['suites'] = suites.split(',')
 
 
     @staticmethod
     def _get_dictionary_from_file(config_fpath):
         try:
+            config_fpath = os.path.realpath(os.path.expanduser(config_fpath))
             config_fhand = open(config_fpath, 'r')
         except IOError:
             msg = 'Unable to read file "' + config_fpath + '"'
             raise IOError(msg)
 
         config_dict = None
         if config_fpath.endswith('.yml') or config_fpath.endswith('.yaml'):
```

### Comparing `dargus-1.0.1/dargus/commons.py` & `dargus-1.0.2/dargus/commons.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/dargus/utils.py` & `dargus-1.0.2/dargus/utils.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/dargus/validation_result.py` & `dargus-1.0.2/dargus/validation_result.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/dargus/validator.py` & `dargus-1.0.2/dargus/validator.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.1/dargus.egg-info/PKG-INFO` & `dargus-1.0.2/dargus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.1/pyproject.toml` & `dargus-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dargus"]
 
 [project]
 name = "dargus"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Python engine for testing and benchmarking REST web services"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
   {name="Daniel Perez-Gil", email="daniel.perez@zettagenomics.com"}
 ]
```

