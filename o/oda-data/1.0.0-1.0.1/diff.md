# Comparing `tmp/oda_data-1.0.0.tar.gz` & `tmp/oda_data-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_data-1.0.0.tar", max compression
+gzip compressed data, was "oda_data-1.0.1.tar", max compression
```

## Comparing `oda_data-1.0.0.tar` & `oda_data-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0     1069 2023-02-20 09:53:00.243074 oda_data-1.0.0/LICENSE
--rw-r--r--   0        0        0     5055 2023-02-20 09:53:00.243074 oda_data-1.0.0/README.md
--rw-r--r--   0        0        0      157 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/.raw_data/README.md
--rw-r--r--   0        0        0      184 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/README.md
--rw-r--r--   0        0        0     1190 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/__init__.py
--rw-r--r--   0        0        0      782 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/classes/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/classes/__init__.py
--rw-r--r--   0        0        0    22978 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/classes/oda_data.py
--rw-r--r--   0        0        0      360 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/classes/representations.py
--rw-r--r--   0        0        0      476 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/clean_data/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/clean_data/__init__.py
--rw-r--r--   0        0        0     5283 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/clean_data/common.py
--rw-r--r--   0        0        0      844 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/config.py
--rw-r--r--   0        0        0     3189 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/__init__.py
--rw-r--r--   0        0        0     5761 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/common.py
--rw-r--r--   0        0        0     2030 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/crs.py
--rw-r--r--   0        0        0      840 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/dac1.py
--rw-r--r--   0        0        0      847 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/dac2a.py
--rw-r--r--   0        0        0      889 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/get_data/multisystem.py
--rw-r--r--   0        0        0      119 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/indicators/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/indicators/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/indicators/linked_indicators.py
--rw-r--r--   0        0        0     6434 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/indicators/research_indicators.py
--rw-r--r--   0        0        0     6836 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/indicators/sector_components.py
--rw-r--r--   0        0        0      698 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/logger.py
--rw-r--r--   0        0        0      603 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/read_data/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/read_data/__init__.py
--rw-r--r--   0        0        0     2682 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/read_data/read.py
--rw-r--r--   0        0        0    10207 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/Available indicators.md
--rw-r--r--   0        0        0     5540 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/README.md
--rw-r--r--   0        0        0     2570 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/channel_codes.json
--rw-r--r--   0        0        0     6617 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/crs_config.json
--rw-r--r--   0        0        0      862 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/dac1_config.json
--rw-r--r--   0        0        0      859 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/dac2a_config.json
--rw-r--r--   0        0        0     7759 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/donor_groupings.json
--rw-r--r--   0        0        0    27497 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/indicators.json
--rw-r--r--   0        0        0     1506 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/key_columns.json
--rw-r--r--   0        0        0     2762 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/multisystem_config.json
--rw-r--r--   0        0        0    17756 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/settings/recipient_groupings.json
--rw-r--r--   0        0        0       78 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/tools/README.md
--rw-r--r--   0        0        0        0 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/tools/__init__.py
--rw-r--r--   0        0        0      799 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/tools/groupings.py
--rw-r--r--   0        0        0     5658 2023-02-20 09:53:00.243074 oda_data-1.0.0/oda_data/tools/names.py
--rw-r--r--   0        0        0     1039 2023-02-20 09:53:00.243074 oda_data-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 oda_data-1.0.0/setup.py
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 oda_data-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 16:13:58.602182 oda_data-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5055 2023-04-13 16:13:58.602182 oda_data-1.0.1/README.md
+-rw-r--r--   0        0        0      157 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/.raw_data/README.md
+-rw-r--r--   0        0        0      184 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/README.md
+-rw-r--r--   0        0        0     1190 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/classes/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/classes/__init__.py
+-rw-r--r--   0        0        0    22978 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/classes/oda_data.py
+-rw-r--r--   0        0        0      360 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/classes/representations.py
+-rw-r--r--   0        0        0      476 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/__init__.py
+-rw-r--r--   0        0        0     5283 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/common.py
+-rw-r--r--   0        0        0      844 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/config.py
+-rw-r--r--   0        0        0     3189 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/__init__.py
+-rw-r--r--   0        0        0     5761 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/common.py
+-rw-r--r--   0        0        0     2030 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/crs.py
+-rw-r--r--   0        0        0      840 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/dac1.py
+-rw-r--r--   0        0        0      847 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/dac2a.py
+-rw-r--r--   0        0        0      889 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/multisystem.py
+-rw-r--r--   0        0        0      119 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/__init__.py
+-rw-r--r--   0        0        0     1512 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/linked_indicators.py
+-rw-r--r--   0        0        0     6434 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/research_indicators.py
+-rw-r--r--   0        0        0     6836 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/sector_components.py
+-rw-r--r--   0        0        0      698 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/logger.py
+-rw-r--r--   0        0        0      603 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/__init__.py
+-rw-r--r--   0        0        0     2682 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/read.py
+-rw-r--r--   0        0        0    10207 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/Available indicators.md
+-rw-r--r--   0        0        0     5540 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/README.md
+-rw-r--r--   0        0        0     2570 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/channel_codes.json
+-rw-r--r--   0        0        0     6617 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/crs_config.json
+-rw-r--r--   0        0        0      862 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/dac1_config.json
+-rw-r--r--   0        0        0      859 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/dac2a_config.json
+-rw-r--r--   0        0        0     7759 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/donor_groupings.json
+-rw-r--r--   0        0        0    27497 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/indicators.json
+-rw-r--r--   0        0        0     1506 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/key_columns.json
+-rw-r--r--   0        0        0     2762 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/multisystem_config.json
+-rw-r--r--   0        0        0    17756 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/recipient_groupings.json
+-rw-r--r--   0        0        0       78 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/groupings.py
+-rw-r--r--   0        0        0     5658 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/names.py
+-rw-r--r--   0        0        0     1039 2023-04-13 16:13:58.606182 oda_data-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 oda_data-1.0.1/PKG-INFO
```

### Comparing `oda_data-1.0.0/LICENSE` & `oda_data-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/README.md` & `oda_data-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/__init__.py` & `oda_data-1.0.1/oda_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from oda_data.classes.oda_data import ODAData
 from oda_data.get_data.crs import download_crs
 from oda_data.get_data.dac1 import download_dac1
 from oda_data.get_data.dac2a import download_dac2a
 from oda_data.get_data.multisystem import download_multisystem
 from oda_data.read_data.read import read_crs, read_dac1, read_dac2a, read_multisystem
```

### Comparing `oda_data-1.0.0/oda_data/classes/README.md` & `oda_data-1.0.1/oda_data/classes/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/classes/oda_data.py` & `oda_data-1.0.1/oda_data/classes/oda_data.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/clean_data/common.py` & `oda_data-1.0.1/oda_data/clean_data/common.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/config.py` & `oda_data-1.0.1/oda_data/config.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/README.md` & `oda_data-1.0.1/oda_data/get_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/common.py` & `oda_data-1.0.1/oda_data/get_data/common.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/crs.py` & `oda_data-1.0.1/oda_data/get_data/crs.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/dac1.py` & `oda_data-1.0.1/oda_data/get_data/dac1.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/dac2a.py` & `oda_data-1.0.1/oda_data/get_data/dac2a.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/get_data/multisystem.py` & `oda_data-1.0.1/oda_data/get_data/multisystem.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/indicators/linked_indicators.py` & `oda_data-1.0.1/oda_data/indicators/linked_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/indicators/research_indicators.py` & `oda_data-1.0.1/oda_data/indicators/research_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/indicators/sector_components.py` & `oda_data-1.0.1/oda_data/indicators/sector_components.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/logger.py` & `oda_data-1.0.1/oda_data/logger.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/read_data/README.md` & `oda_data-1.0.1/oda_data/read_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/read_data/read.py` & `oda_data-1.0.1/oda_data/read_data/read.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/Available indicators.md` & `oda_data-1.0.1/oda_data/settings/Available indicators.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/README.md` & `oda_data-1.0.1/oda_data/settings/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/channel_codes.json` & `oda_data-1.0.1/oda_data/settings/channel_codes.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/crs_config.json` & `oda_data-1.0.1/oda_data/settings/crs_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/dac1_config.json` & `oda_data-1.0.1/oda_data/settings/dac1_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/dac2a_config.json` & `oda_data-1.0.1/oda_data/settings/dac2a_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/donor_groupings.json` & `oda_data-1.0.1/oda_data/settings/donor_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/indicators.json` & `oda_data-1.0.1/oda_data/settings/indicators.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/key_columns.json` & `oda_data-1.0.1/oda_data/settings/key_columns.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/multisystem_config.json` & `oda_data-1.0.1/oda_data/settings/multisystem_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/settings/recipient_groupings.json` & `oda_data-1.0.1/oda_data/settings/recipient_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/tools/groupings.py` & `oda_data-1.0.1/oda_data/tools/groupings.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/oda_data/tools/names.py` & `oda_data-1.0.1/oda_data/tools/names.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.0/pyproject.toml` & `oda_data-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oda_data"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python package to work with Official Development Assistance data from the OECD DAC."
 readme = "README.md"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 packages = [{ include = "oda_data" }]
 classifiers = ["Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `oda_data-1.0.0/setup.py` & `oda_data-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: oda-data
+Version: 1.0.1
+Summary: A python package to work with Official Development Assistance data from the OECD DAC.
+Author: Jorge Rivera
+Author-email: jorge.rivera@one.org
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bblocks (>=1,<2)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pydeflate (>=1.3.1,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Description-Content-Type: text/markdown
+
+[![pypi](https://img.shields.io/pypi/v/oda_data.svg)](https://pypi.org/project/oda_data/)
+[![python](https://img.shields.io/pypi/pyversions/oda_data.svg)](https://pypi.org/project/oda_data/)
+[![codecov](https://codecov.io/gh/ONEcampaign/oda_data_package/branch/main/graph/badge.svg?token=G8N8BWWPL8)](https://codecov.io/gh/ONEcampaign/oda_data_package)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# The ODA Data Package
+This package contains key tools used by The ONE Campaign to analyse Official Development Assistance (ODA) data from
+the OECD [DAC](https://www.oecd.org/dac/stats/) databases.
+
+Interacting with the DAC databases can be a complex task. There are many databases, tables, and web interfaces which
+can be used to get the data you need. This means that getting the right ODA data can require expert knowledge not only
+of ODA, but also of how the DAC databases and tools are organised.
+
+This package aims to simplify this process and make it easier for users to get the data they need.
+
+Please submit questions, feedback or requests via 
+the [issues page](https://github.com/ONEcampaign/oda_data_package/issues).
+
+## Getting started
+
+### Installation
+The package can be installed using pip:
+
+```bash
+pip install oda-data --upgrade
+```
+
+The package is compatible with Python 3.10 and above.
+
+### Basic usage
+
+Most users can get the data they need by using the `ODAData` class.
+
+An object of this class can handle:
+- getting data for specific indicators (one or more)
+- filtering the data for specific donors, recipients(if relevant), years.
+- returning the data in a variety of currency/prices combinations.
+
+For example, to get Total ODA in net flows and grant equivalents, in constant 2021 Euros, for 2018-2021.
+
+```python
+from oda_data import ODAData, set_data_path
+
+# set the path to the folder where the data should be stored
+set_data_path("path/to/data/folder")
+
+# create object, specifying key details of the desired output
+data = ODAData(years=range(2018,2022), currency="EUR", prices="constant", base_year=2021)
+
+# load the desired indicators
+data.load_indicator(indicators = ["total_oda_flow_net", "total_oda_ge"])
+
+# get the data
+df = data.get_data()
+
+print(df.head(6))
+```
+This would result in the following dataframe:
+
+|   donor_code | donor_name   |   year |   value | indicator          | currency   | prices   |
+|-------------:|:-------------|-------:|--------:|:-------------------|:-----------|:---------|
+|            1 | Austria      |   2021 | 1261.76 | total_oda_flow_net | EUR        | constant |
+|            1 | Austria      |   2021 | 1240.31 | total_oda_ge       | EUR        | constant |
+|            2 | Belgium      |   2021 | 2176.38 | total_oda_flow_net | EUR        | constant |
+|            2 | Belgium      |   2021 | 2174.38 | total_oda_ge       | EUR        | constant |
+|            3 | Denmark      |   2021 | 2424.51 | total_oda_flow_net | EUR        | constant |
+|            3 | Denmark      |   2021 | 2430.65 | total_oda_ge       | EUR        | constant |
+
+
+To print the full list of available indicators, you can call `.get_available_indicators()`.
+
+For full details on the available indicators and how we calculate them,
+see the indicators [documentation](oda_data/settings/Available indicators.md)
+
+## Tutorials
+For more detailed examples of how to use the package, see the [tutorials](tutorials).
+- A [tutorial notebook](tutorials/1.%20total_donor_oda.ipynb) on loading the package and getting total oda data
+- A [tutorial notebook](tutorials/2.%20total_recipient_oda_by_donor.ipynb) on getting ODA by donor and recipient
+  (including both bilateral and imputed multilateral data)
+- A [tutorial notebook](tutorials/3.%20sector_analysis_by_donor_and_recipient.ipynb) on getting ODA by sectors
+  (including both bilateral and imputed multilateral data)
+
+Please reach out if you have questions or need help with using the package for your analysis.
+
+## Key features
+
+- **Speed up analysis** - The package handles downloading, cleaning and loading all the data, so you can focus on the 
+analysis. The data is downloaded from the bulk download service of the OECD, and once it is stored locally, producing
+the output is extremely fast.
+- **Access all of our analysis** - Besides the classic OECD DAC indicators, the package also provides access to the
+data and analysis produced by ONE. This includes gender or climate data in gross disbursement terms (instead of
+commitments) and our multilateral sectors imputations.
+- **Get data in the currency and prices you need** - ODA data is only available in US dollars (current or constant 
+prices) and local currency units (current prices). The package allows you to view the data in US dollars, Euros,
+British Pounds and Canadian dollars, in both current and constant prices. We can add any other DAC currency if you
+request it via the [issues page](https://github.com/ONEcampaign/oda_data_package/issues)
 
-packages = \
-['oda_data',
- 'oda_data.classes',
- 'oda_data.clean_data',
- 'oda_data.get_data',
- 'oda_data.indicators',
- 'oda_data.read_data',
- 'oda_data.tools']
-
-package_data = \
-{'': ['*'], 'oda_data': ['.raw_data/*', 'settings/*']}
-
-install_requires = \
-['bblocks>=1,<2',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'lxml>=4.9.2,<5.0.0',
- 'pandas>=1.5.2,<2.0.0',
- 'pydeflate>=1.3.1,<2.0.0',
- 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'oda-data',
-    'version': '1.0.0',
-    'description': 'A python package to work with Official Development Assistance data from the OECD DAC.',
-    'long_description': '[![pypi](https://img.shields.io/pypi/v/oda_data.svg)](https://pypi.org/project/oda_data/)\n[![python](https://img.shields.io/pypi/pyversions/oda_data.svg)](https://pypi.org/project/oda_data/)\n[![codecov](https://codecov.io/gh/ONEcampaign/oda_data_package/branch/main/graph/badge.svg?token=G8N8BWWPL8)](https://codecov.io/gh/ONEcampaign/oda_data_package)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# The ODA Data Package\nThis package contains key tools used by The ONE Campaign to analyse Official Development Assistance (ODA) data from\nthe OECD [DAC](https://www.oecd.org/dac/stats/) databases.\n\nInteracting with the DAC databases can be a complex task. There are many databases, tables, and web interfaces which\ncan be used to get the data you need. This means that getting the right ODA data can require expert knowledge not only\nof ODA, but also of how the DAC databases and tools are organised.\n\nThis package aims to simplify this process and make it easier for users to get the data they need.\n\nPlease submit questions, feedback or requests via \nthe [issues page](https://github.com/ONEcampaign/oda_data_package/issues).\n\n## Getting started\n\n### Installation\nThe package can be installed using pip:\n\n```bash\npip install oda-data --upgrade\n```\n\nThe package is compatible with Python 3.10 and above.\n\n### Basic usage\n\nMost users can get the data they need by using the `ODAData` class.\n\nAn object of this class can handle:\n- getting data for specific indicators (one or more)\n- filtering the data for specific donors, recipients(if relevant), years.\n- returning the data in a variety of currency/prices combinations.\n\nFor example, to get Total ODA in net flows and grant equivalents, in constant 2021 Euros, for 2018-2021.\n\n```python\nfrom oda_data import ODAData, set_data_path\n\n# set the path to the folder where the data should be stored\nset_data_path("path/to/data/folder")\n\n# create object, specifying key details of the desired output\ndata = ODAData(years=range(2018,2022), currency="EUR", prices="constant", base_year=2021)\n\n# load the desired indicators\ndata.load_indicator(indicators = ["total_oda_flow_net", "total_oda_ge"])\n\n# get the data\ndf = data.get_data()\n\nprint(df.head(6))\n```\nThis would result in the following dataframe:\n\n|   donor_code | donor_name   |   year |   value | indicator          | currency   | prices   |\n|-------------:|:-------------|-------:|--------:|:-------------------|:-----------|:---------|\n|            1 | Austria      |   2021 | 1261.76 | total_oda_flow_net | EUR        | constant |\n|            1 | Austria      |   2021 | 1240.31 | total_oda_ge       | EUR        | constant |\n|            2 | Belgium      |   2021 | 2176.38 | total_oda_flow_net | EUR        | constant |\n|            2 | Belgium      |   2021 | 2174.38 | total_oda_ge       | EUR        | constant |\n|            3 | Denmark      |   2021 | 2424.51 | total_oda_flow_net | EUR        | constant |\n|            3 | Denmark      |   2021 | 2430.65 | total_oda_ge       | EUR        | constant |\n\n\nTo print the full list of available indicators, you can call `.get_available_indicators()`.\n\nFor full details on the available indicators and how we calculate them,\nsee the indicators [documentation](oda_data/settings/Available indicators.md)\n\n## Tutorials\nFor more detailed examples of how to use the package, see the [tutorials](tutorials).\n- A [tutorial notebook](tutorials/1.%20total_donor_oda.ipynb) on loading the package and getting total oda data\n- A [tutorial notebook](tutorials/2.%20total_recipient_oda_by_donor.ipynb) on getting ODA by donor and recipient\n  (including both bilateral and imputed multilateral data)\n- A [tutorial notebook](tutorials/3.%20sector_analysis_by_donor_and_recipient.ipynb) on getting ODA by sectors\n  (including both bilateral and imputed multilateral data)\n\nPlease reach out if you have questions or need help with using the package for your analysis.\n\n## Key features\n\n- **Speed up analysis** - The package handles downloading, cleaning and loading all the data, so you can focus on the \nanalysis. The data is downloaded from the bulk download service of the OECD, and once it is stored locally, producing\nthe output is extremely fast.\n- **Access all of our analysis** - Besides the classic OECD DAC indicators, the package also provides access to the\ndata and analysis produced by ONE. This includes gender or climate data in gross disbursement terms (instead of\ncommitments) and our multilateral sectors imputations.\n- **Get data in the currency and prices you need** - ODA data is only available in US dollars (current or constant \nprices) and local currency units (current prices). The package allows you to view the data in US dollars, Euros,\nBritish Pounds and Canadian dollars, in both current and constant prices. We can add any other DAC currency if you\nrequest it via the [issues page](https://github.com/ONEcampaign/oda_data_package/issues)\n\n## Contributing\nInterested in contributing to the package? Please reach out.\n',
-    'author': 'Jorge Rivera',
-    'author_email': 'jorge.rivera@one.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+## Contributing
+Interested in contributing to the package? Please reach out.
 
-
-setup(**setup_kwargs)
```

