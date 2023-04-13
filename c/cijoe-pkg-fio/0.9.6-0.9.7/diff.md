# Comparing `tmp/cijoe-pkg-fio-0.9.6.tar.gz` & `tmp/cijoe-pkg-fio-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cijoe-pkg-fio-0.9.6.tar", last modified: Mon Oct 10 14:10:15 2022, max compression
+gzip compressed data, was "cijoe-pkg-fio-0.9.7.tar", last modified: Thu Apr 13 00:00:01 2023, max compression
```

## Comparing `cijoe-pkg-fio-0.9.6.tar` & `cijoe-pkg-fio-0.9.7.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.362112 cijoe-pkg-fio-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.362112 cijoe-pkg-fio-0.9.6/src/cijoe/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.362112 cijoe-pkg-fio-0.9.6/src/cijoe/fio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.362112 cijoe-pkg-fio-0.9.6/src/cijoe/fio/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/src/cijoe/fio/selftest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/selftest/test_fio_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/src/cijoe/fio/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/check.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     8127 2022-10-10 14:10:04.000000 cijoe-pkg-fio-0.9.6/src/cijoe/fio/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 14:10:15.366112 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-10 14:10:15.000000 cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.149081 cijoe-pkg-fio-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.149081 cijoe-pkg-fio-0.9.7/src/cijoe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe/fio/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe/fio/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/configs/default-config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe/fio/selftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/selftest/test_fio_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe/fio/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/workflows/example.workflow
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-12 23:59:49.000000 cijoe-pkg-fio-0.9.7/src/cijoe/fio/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:00:01.153081 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 00:00:01.000000 cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/top_level.txt
```

### Comparing `cijoe-pkg-fio-0.9.6/LICENSE` & `cijoe-pkg-fio-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-fio-0.9.6/PKG-INFO` & `cijoe-pkg-fio-0.9.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-fio
-Version: 0.9.6
-Summary: UNKNOWN
-Home-page: https://github.com/refenv/cijoe-pkg-fio/
+Version: 0.9.7
+Summary: A loosely coupled approach to systems development and testing
+Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: BSD
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `cijoe-pkg-fio-0.9.6/README.rst` & `cijoe-pkg-fio-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-fio-0.9.6/src/cijoe/fio/selftest/test_fio_wrapper.py` & `cijoe-pkg-fio-0.9.7/src/cijoe/fio/selftest/test_fio_wrapper.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-fio-0.9.6/src/cijoe/fio/worklets/build.py` & `cijoe-pkg-fio-0.9.7/src/cijoe/fio/scripts/build.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Retargetable: True
 ------------------
 """
 from pathlib import Path
 
 
-def worklet_entry(args, cijoe, step):
+def main(args, cijoe, step):
     """Install qemu"""
 
     commands = [
         "make clean",
         f"./configure --prefix={ cijoe.config.options['fio']['build']['prefix'] }",
         "make -j $(nproc)",
     ]
```

### Comparing `cijoe-pkg-fio-0.9.6/src/cijoe/fio/wrapper.py` & `cijoe-pkg-fio-0.9.7/src/cijoe/fio/wrapper.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/PKG-INFO` & `cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-fio
-Version: 0.9.6
-Summary: UNKNOWN
-Home-page: https://github.com/refenv/cijoe-pkg-fio/
+Version: 0.9.7
+Summary: A loosely coupled approach to systems development and testing
+Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: BSD
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `cijoe-pkg-fio-0.9.6/src/cijoe_pkg_fio.egg-info/SOURCES.txt` & `cijoe-pkg-fio-0.9.7/src/cijoe_pkg_fio.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 README.rst
 pyproject.toml
+setup.cfg
 setup.py
 src/cijoe/fio/__init__.py
 src/cijoe/fio/wrapper.py
 src/cijoe/fio/configs/__init__.py
+src/cijoe/fio/configs/default-config.toml
+src/cijoe/fio/scripts/__init__.py
+src/cijoe/fio/scripts/build.py
+src/cijoe/fio/scripts/check.py
+src/cijoe/fio/scripts/install.py
 src/cijoe/fio/selftest/__init__.py
 src/cijoe/fio/selftest/test_fio_wrapper.py
 src/cijoe/fio/workflows/__init__.py
-src/cijoe/fio/worklets/__init__.py
-src/cijoe/fio/worklets/build.py
-src/cijoe/fio/worklets/check.py
-src/cijoe/fio/worklets/install.py
+src/cijoe/fio/workflows/example.workflow
 src/cijoe_pkg_fio.egg-info/PKG-INFO
 src/cijoe_pkg_fio.egg-info/SOURCES.txt
 src/cijoe_pkg_fio.egg-info/dependency_links.txt
 src/cijoe_pkg_fio.egg-info/not-zip-safe
 src/cijoe_pkg_fio.egg-info/requires.txt
 src/cijoe_pkg_fio.egg-info/top_level.txt
```

