# Comparing `tmp/pylife-odbserver-2.0.2rc1.tar.gz` & `tmp/pylife-odbserver-2.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylife-odbserver-2.0.2rc1.tar", last modified: Tue Dec 13 10:55:16 2022, max compression
+gzip compressed data, was "pylife-odbserver-2.0.3rc1.tar", last modified: Thu Apr 13 08:57:29 2023, max compression
```

## Comparing `pylife-odbserver-2.0.2rc1.tar` & `pylife-odbserver-2.0.3rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      408 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/odbserver/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/odbserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/odbserver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/odbserver/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-13 10:55:16.000000 pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-13 10:55:16.000000 pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:55:16.000000 pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-13 10:55:16.000000 pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:16.436666 pylife-odbserver-2.0.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 10:55:08.000000 pylife-odbserver-2.0.2rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/odbserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/odbserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/odbserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/odbserver/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 08:57:29.000000 pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 08:57:29.000000 pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:57:29.000000 pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:57:29.000000 pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:29.518379 pylife-odbserver-2.0.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 08:57:22.000000 pylife-odbserver-2.0.3rc1/tests/conftest.py
```

### Comparing `pylife-odbserver-2.0.2rc1/.coveragerc` & `pylife-odbserver-2.0.3rc1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/LICENSE` & `pylife-odbserver-2.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/PKG-INFO` & `pylife-odbserver-2.0.3rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbserver
-Version: 2.0.2rc1
+Version: 2.0.3rc1
 Summary: A server for odbAccess to be acessed by pylife-odbclient
 Home-page: http://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Classifier: Programming Language :: Python
 Requires-Python: <3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.2rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc1 Summary: A
 server for odbAccess to be acessed by pylife-odbclient Home-page: http://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Classifier: Programming
 Language :: Python Requires-Python: <3 Description-Content-Type: text/markdown;
 charset=UTF-8 License-File: LICENSE License-File: AUTHORS.rst # pylife-
 odbserver A server for odbAccess to be accessed by pylife-odbclient ## Purpose
 Unfortunately Abaqus still comes with a python-2.x engine. So you can't access
```

### Comparing `pylife-odbserver-2.0.2rc1/README.md` & `pylife-odbserver-2.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/odbserver/__main__.py` & `pylife-odbserver-2.0.3rc1/odbserver/__main__.py`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/odbserver/interface.py` & `pylife-odbserver-2.0.3rc1/odbserver/interface.py`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/pylife_odbserver.egg-info/PKG-INFO` & `pylife-odbserver-2.0.3rc1/pylife_odbserver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbserver
-Version: 2.0.2rc1
+Version: 2.0.3rc1
 Summary: A server for odbAccess to be acessed by pylife-odbclient
 Home-page: http://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Classifier: Programming Language :: Python
 Requires-Python: <3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.2rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbserver Version: 2.0.3rc1 Summary: A
 server for odbAccess to be acessed by pylife-odbclient Home-page: http://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Classifier: Programming
 Language :: Python Requires-Python: <3 Description-Content-Type: text/markdown;
 charset=UTF-8 License-File: LICENSE License-File: AUTHORS.rst # pylife-
 odbserver A server for odbAccess to be accessed by pylife-odbclient ## Purpose
 Unfortunately Abaqus still comes with a python-2.x engine. So you can't access
```

### Comparing `pylife-odbserver-2.0.2rc1/setup.cfg` & `pylife-odbserver-2.0.3rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylife-odbserver-2.0.2rc1/setup.py` & `pylife-odbserver-2.0.3rc1/setup.py`

 * *Files identical despite different names*

