# Comparing `tmp/quickstart-vdk-0.2.834544423.dev9115.tar.gz` & `tmp/quickstart-vdk-0.2.835757538.dev9183.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.834544423.dev9115.tar", last modified: Wed Apr 12 04:25:43 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.835757538.dev9183.tar", last modified: Thu Apr 13 04:24:38 2023, max compression
```

## Comparing `quickstart-vdk-0.2.834544423.dev9115.tar` & `quickstart-vdk-0.2.835757538.dev9183.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:25:43.760694 quickstart-vdk-0.2.834544423.dev9115/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-12 04:25:43.760694 quickstart-vdk-0.2.834544423.dev9115/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-12 04:22:52.000000 quickstart-vdk-0.2.834544423.dev9115/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:25:43.760694 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-12 04:25:43.000000 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 04:25:43.000000 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 04:25:43.000000 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-12 04:25:43.000000 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-12 04:25:43.000000 quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 04:25:43.760694 quickstart-vdk-0.2.834544423.dev9115/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-12 04:25:33.000000 quickstart-vdk-0.2.834544423.dev9115/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:25:43.760694 quickstart-vdk-0.2.834544423.dev9115/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-12 04:22:52.000000 quickstart-vdk-0.2.834544423.dev9115/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:24:38.880313 quickstart-vdk-0.2.835757538.dev9183/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-13 04:24:38.876313 quickstart-vdk-0.2.835757538.dev9183/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-13 04:21:57.000000 quickstart-vdk-0.2.835757538.dev9183/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:24:38.876313 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-13 04:24:38.000000 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-13 04:24:38.000000 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 04:24:38.000000 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-13 04:24:38.000000 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-13 04:24:38.000000 quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 04:24:38.880313 quickstart-vdk-0.2.835757538.dev9183/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-13 04:24:30.000000 quickstart-vdk-0.2.835757538.dev9183/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 04:24:38.876313 quickstart-vdk-0.2.835757538.dev9183/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-13 04:21:57.000000 quickstart-vdk-0.2.835757538.dev9183/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.834544423.dev9115/PKG-INFO` & `quickstart-vdk-0.2.835757538.dev9183/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.834544423.dev9115
+Version: 0.2.835757538.dev9183
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.834544423.dev9115/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.835757538.dev9183/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.834544423.dev9115
+Version: 0.2.835757538.dev9183
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.834544423.dev9115/setup.py` & `quickstart-vdk-0.2.835757538.dev9183/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.834544423.dev9115"
+__version__ = "0.2.835757538.dev9183"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

