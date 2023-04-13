# Comparing `tmp/pyilcd-5.0.0.tar.gz` & `tmp/pyilcd-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyilcd-5.0.0.tar", last modified: Thu Apr 13 14:31:15 2023, max compression
+gzip compressed data, was "pyilcd-6.0.0.tar", last modified: Thu Apr 13 16:20:52 2023, max compression
```

## Comparing `pyilcd-5.0.0.tar` & `pyilcd-6.0.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.434860 pyilcd-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-13 14:31:05.000000 pyilcd-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 14:31:05.000000 pyilcd-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:31:15.434860 pyilcd-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 14:31:05.000000 pyilcd-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.422860 pyilcd-5.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 14:31:05.000000 pyilcd-5.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.426860 pyilcd-5.0.0/pyilcd/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/contact_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/flow_property_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/process_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.430860 pyilcd-5.0.0/pyilcd/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Categories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Documentation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ILCD.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Locations.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/unit_group_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.426860 pyilcd-5.0.0/pyilcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 14:31:15.434860 pyilcd-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.430860 pyilcd-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_contact_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_flow_propert_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_unit_group_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.558362 pyilcd-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-13 16:20:43.000000 pyilcd-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 16:20:43.000000 pyilcd-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 16:20:52.558362 pyilcd-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 16:20:43.000000 pyilcd-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.550361 pyilcd-6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 16:20:43.000000 pyilcd-6.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.550361 pyilcd-6.0.0/pyilcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/contact_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/flow_property_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.554361 pyilcd-6.0.0/pyilcd/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Categories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Documentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_ILCD.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_Locations.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/source_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/unit_group_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyilcd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.550361 pyilcd-6.0.0/pyilcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 16:20:52.000000 pyilcd-6.0.0/pyilcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 16:20:43.000000 pyilcd-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 16:20:52.558362 pyilcd-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:20:52.554361 pyilcd-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_contact_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_flow_property_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_source_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 16:20:43.000000 pyilcd-6.0.0/tests/test_unit_group_dataset.py
```

### Comparing `pyilcd-5.0.0/LICENSE` & `pyilcd-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/PKG-INFO` & `pyilcd-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 5.0.0
+Version: 6.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-5.0.0/README.md` & `pyilcd-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/docs/conf.py` & `pyilcd-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/__init__.py` & `pyilcd-6.0.0/pyilcd/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """pyilcd."""
 from .core import (
     parse_directory_contact_dataset,
     parse_directory_flow_dataset,
     parse_directory_flow_property_dataset,
     parse_directory_process_dataset,
+    parse_directory_source_dataset,
     parse_directory_unit_group_dataset,
     parse_file_contact_dataset,
     parse_file_flow_dataset,
     parse_file_flow_property_dataset,
     parse_file_process_dataset,
+    parse_file_source_dataset,
     parse_file_unit_group_dataset,
     save_ilcd_file,
     validate_file_contact_dataset,
     validate_file_flow_dataset,
     validate_file_flow_property_dataset,
     validate_file_process_dataset,
+    validate_file_source_dataset,
     validate_file_unit_group_dataset,
 )
 from .utils import get_version_tuple
 
 __all__ = (
     "__version__",
     "parse_directory_contact_dataset",
     "parse_directory_flow_dataset",
     "parse_directory_flow_property_dataset",
     "parse_directory_process_dataset",
+    "parse_directory_source_dataset",
     "parse_directory_unit_group_dataset",
     "parse_file_contact_dataset",
     "parse_file_flow_dataset",
     "parse_file_flow_property_dataset",
     "parse_file_process_dataset",
+    "parse_file_source_dataset",
     "parse_file_unit_group_dataset",
     "save_ilcd_file",
     "validate_file_contact_dataset",
     "validate_file_flow_dataset",
     "validate_file_flow_property_dataset",
     "validate_file_process_dataset",
+    "validate_file_source_dataset",
     "validate_file_unit_group_dataset",
 )
 
 __version__ = get_version_tuple()
```

### Comparing `pyilcd-5.0.0/pyilcd/common.py` & `pyilcd-6.0.0/pyilcd/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,7 +401,23 @@
     is hierachical, otherwise emtpy or not used."""
 
     catId = create_attribute_process_dataset("catId", str)
     """Unique identifier of the category. [Note: May be used by LCA
     software for it's category system. If used the identifer should
     be identical to the on defined in the referenced category file.
     Identifiers can be UUIDs, but also other forms are possible.]"""
+
+
+class ComplianceDeclarations(etree.ElementBase):
+    """Statements on compliance of several data set aspects with compliance
+    requirements as defined by the referenced compliance system (e.g. an
+    EPD scheme, handbook of a national or international data network such
+    as the ILCD, etc.)."""
+
+    @property
+    def compliances(self) -> List["Compliance"]:
+        """One compliance declaration"""
+        return get_element_list(self, "compliance")
+
+
+class Compliance(ComplianceGroup):
+    """One compliance declaration"""
```

### Comparing `pyilcd-5.0.0/pyilcd/config.py` & `pyilcd-6.0.0/pyilcd/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     )
     SCHEMA_UNIT_GROUP_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_UnitGroupDataSet.xsd"
     )
     SCHEMA_CONTACT_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_ContactDataSet.xsd"
     )
+    SCHEMA_SOURCE_DATASET: ClassVar[str] = os.path.join(
+        SCHEMA_DIR, "ILCD_SourceDataSet.xsd"
+    )
 
     DYNAMIC_DEFAULTS: ClassVar[
         Dict[str, Dict[str, Callable[[etree.ElementBase], str]]]
     ] = {}
     STATIC_DEFAULTS: ClassVar[Dict[str, Dict[str, str]]] = {
         "Classification": {
             "name": "ILCD",
```

### Comparing `pyilcd-5.0.0/pyilcd/contact_dataset.py` & `pyilcd-6.0.0/pyilcd/contact_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/core.py` & `pyilcd-6.0.0/pyilcd/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from .common import (
     Category,
     Class,
     Classification,
     ClassificationInformation,
     CommissionerAndGoal,
+    Compliance,
+    ComplianceDeclarations,
     DataQualityIndicator,
     DataQualityIndicators,
     FlowCategorization,
     FlowCategoryInformation,
     GlobalReference,
     Method,
     Scope,
@@ -25,33 +27,27 @@
     AdministrativeInformation as ContactAdministrativeInformation,
 )
 from .contact_dataset import ContactDataSet, ContactInformation
 from .contact_dataset import DataEntryBy as ContactDataEntryBy
 from .contact_dataset import DataSetInformation as ContactDataSetInformation
 from .contact_dataset import PublicationAndOwnership as ContactPublicationAndOwnership
 from .flow_dataset import AdministrativeInformation as FlowAdministrativeInformation
-from .flow_dataset import Compliance as FlowCompliance
-from .flow_dataset import ComplianceDeclarations as FlowComplianceDeclarations
 from .flow_dataset import DataEntryBy as FlowDataEntryBy
 from .flow_dataset import DataSetInformation as FlowDataSetInformation
 from .flow_dataset import FlowDataSet, FlowInformation, FlowProperties, FlowProperty
 from .flow_dataset import Geography as FlowGeography
 from .flow_dataset import LCIMethod
 from .flow_dataset import ModellingAndValidation as FlowModellingAndValidation
 from .flow_dataset import Name as FlowName
 from .flow_dataset import PublicationAndOwnership as FlowPublicationAndOwnership
 from .flow_dataset import QuantitativeReference as FlowQuantitativeReference
 from .flow_dataset import Technology as FlowTechnology
 from .flow_property_dataset import (
     AdministrativeInformation as FlowPropertyAdministrativeInformation,
 )
-from .flow_property_dataset import Compliance as FlowPropertyCompliance
-from .flow_property_dataset import (
-    ComplianceDeclarations as FlowPropertyComplianceDeclarations,
-)
 from .flow_property_dataset import DataEntryBy as FlowPropertyDataEntryBy
 from .flow_property_dataset import DataSetInformation as FlowPropertyDataSetInformation
 from .flow_property_dataset import DataSourcesTreatmentAndRepresentativeness as FPDSTAR
 from .flow_property_dataset import FlowPropertiesInformation, FlowPropertyDataSet
 from .flow_property_dataset import (
     ModellingAndValidation as FlowPropertyModellingAndValidation,
 )
@@ -94,21 +90,22 @@
 from .process_dataset import (
     ReferencesToDataSource,
     Review,
     SubLocationOfOperationSupplyOrProduction,
 )
 from .process_dataset import Technology as ProcessTechnology
 from .process_dataset import Time, Validation, VariableParameter
+from .source_dataset import AdministrativeInformation as SourceAdministrativeInformation
+from .source_dataset import DataEntryBy as SourceDataEntryBy
+from .source_dataset import DataSetInformation as SourceDataSetInformation
+from .source_dataset import PublicationAndOwnership as SourcePublicationAndOwnership
+from .source_dataset import ReferenceToDigitalFile, SourceDataSet, SourceInformation
 from .unit_group_dataset import (
     AdministrativeInformation as UnitGroupAdministrativeInformation,
 )
-from .unit_group_dataset import Compliance as UnitGroupCompliance
-from .unit_group_dataset import (
-    ComplianceDeclarations as UnitGroupComplianceDeclarations,
-)
 from .unit_group_dataset import DataEntryBy as UnitGroupDataEntryBy
 from .unit_group_dataset import DataSetInformation as UnitGroupDataSetInformation
 from .unit_group_dataset import (
     ModellingAndValidation as UnitGroupModellingAndValidation,
 )
 from .unit_group_dataset import (
     PublicationAndOwnership as UnitGroupPublicationAndOwnership,
@@ -121,14 +118,16 @@
     "allocations": Allocations,
     "category": Category,
     "class": Class,
     "classification": Classification,
     "completeness": Completeness,
     "completenessElementaryFlows": CompletenessElementaryFlows,
     "complementingProcesses": ComplementingProcesses,
+    "compliance": Compliance,
+    "complianceDeclarations": ComplianceDeclarations,
     "commissionerAndGoal": CommissionerAndGoal,
     "contactDataSet": ContactDataSet,
     "contactInformation": ContactInformation,
     "dataGenerator": DataGenerator,
     "dataQualityIndicator": DataQualityIndicator,
     "dataQualityIndicators": DataQualityIndicators,
     "elementaryFlowCategorization": FlowCategorization,
@@ -156,14 +155,15 @@
     "referenceToCompleteReviewReport": GlobalReference,
     "referenceToComplianceSystem": GlobalReference,
     "referenceToConvertedOriginalDataSetFrom": GlobalReference,
     "referenceToDataHandlingPrinciples": GlobalReference,
     "referenceToDataSetFormat": GlobalReference,
     "referenceToDataSetUseApproval": GlobalReference,
     "referenceToDataSource": GlobalReference,
+    "referenceToDigitalFile": ReferenceToDigitalFile,
     "referenceToEntitiesWithExclusiveAccess": GlobalReference,
     "referenceToExternalDocumentation": GlobalReference,
     "referenceToFlowDataSet": GlobalReference,
     "referenceToFlowPropertyDataSet": GlobalReference,
     "referenceToIncludedProcesses": GlobalReference,
     "referenceToLCAMethodDetails": GlobalReference,
     "referenceToLCIAMethodDataSet": GlobalReference,
@@ -178,14 +178,16 @@
     "referenceToSupportedImpactAssessmentMethods": GlobalReference,
     "referenceToTechnicalSpecification": GlobalReference,
     "referenceToTechnologyFlowDiagrammOrPicture": GlobalReference,
     "referenceToTechnologyPictogramme": GlobalReference,
     "referenceToUnchangedRepublication": GlobalReference,
     "referencesToDataSource": ReferencesToDataSource,
     "review": Review,
+    "sourceDataSet": SourceDataSet,
+    "sourceInformation": SourceInformation,
     "subLocationOfOperationSupplyOrProduction": (
         SubLocationOfOperationSupplyOrProduction
     ),
     "time": Time,
     "unit": Unit,
     "units": Units,
     "unitGroupDataSet": UnitGroupDataSet,
@@ -230,20 +232,18 @@
 
 class FlowDatasetLookup(etree.CustomElementClassLookup):
     """Custom XML lookup class for ILCD FlowDataset files."""
 
     def lookup(
         self, unused_node_type, unused_document, unused_namespace, name: str
     ) -> type:
-        """Maps ILCD ProcessDataset XML elements to custom FlowDataset classes."""
+        """Maps ILCD FlowDataset XML elements to custom FlowDataset classes."""
         lookupMap: Dict[str, type] = {
             "administrativeInformation": FlowAdministrativeInformation,
             "classificationInformation": FlowCategoryInformation,
-            "compliance": FlowCompliance,
-            "complianceDeclarations": FlowComplianceDeclarations,
             "dataEntryBy": FlowDataEntryBy,
             "dataSetInformation": FlowDataSetInformation,
             "geography": FlowGeography,
             "modellingAndValidation": FlowModellingAndValidation,
             "name": FlowName,
             "publicationAndOwnership": FlowPublicationAndOwnership,
             "quantitativeReference": FlowQuantitativeReference,
@@ -257,21 +257,19 @@
 
 class FlowPropertyDatasetLookup(etree.CustomElementClassLookup):
     """Custom XML lookup class for ILCD FlowPropertyDataset files."""
 
     def lookup(
         self, unused_node_type, unused_document, unused_namespace, name: str
     ) -> type:
-        """Maps ILCD ProcessDataset XML elements to custom FlowPropertyDataset
+        """Maps ILCD FlowPropertyDataset XML elements to custom FlowPropertyDataset
         classes."""
         lookupMap: Dict[str, type] = {
             "administrativeInformation": FlowPropertyAdministrativeInformation,
             "classificationInformation": ClassificationInformation,
-            "compliance": FlowPropertyCompliance,
-            "complianceDeclarations": FlowPropertyComplianceDeclarations,
             "dataEntryBy": FlowPropertyDataEntryBy,
             "dataSetInformation": FlowPropertyDataSetInformation,
             "dataSourcesTreatmentAndRepresentativeness": FPDSTAR,
             "modellingAndValidation": FlowPropertyModellingAndValidation,
             "publicationAndOwnership": FlowPropertyPublicationAndOwnership,
             "quantitativeReference": FlowPropertyQuantitativeReference,
         }
@@ -283,20 +281,19 @@
 
 class UnitGroupDatasetLookup(etree.CustomElementClassLookup):
     """Custom XML lookup class for ILCD UnitGroupDataset files."""
 
     def lookup(
         self, unused_node_type, unused_document, unused_namespace, name: str
     ) -> type:
-        """Maps ILCD ProcessDataset XML elements to custom UnitGroupDataset classes."""
+        """Maps ILCD UnitGroupDataset XML elements to custom UnitGroupDataset
+        classes."""
         lookupMap: Dict[str, type] = {
             "administrativeInformation": UnitGroupAdministrativeInformation,
             "classificationInformation": ClassificationInformation,
-            "compliance": UnitGroupCompliance,
-            "complianceDeclarations": UnitGroupComplianceDeclarations,
             "dataEntryBy": UnitGroupDataEntryBy,
             "dataSetInformation": UnitGroupDataSetInformation,
             "modellingAndValidation": UnitGroupModellingAndValidation,
             "publicationAndOwnership": UnitGroupPublicationAndOwnership,
             "quantitativeReference": UnitGroupQuantitativeReference,
         }
         try:
@@ -307,28 +304,48 @@
 
 class ContactDatasetLookup(etree.CustomElementClassLookup):
     """Custom XML lookup class for ILCD ContactDataset files."""
 
     def lookup(
         self, unused_node_type, unused_document, unused_namespace, name: str
     ) -> type:
-        """Maps ILCD ProcessDataset XML elements to custom ContactDataset classes."""
+        """Maps ILCD ContactDataset XML elements to custom ContactDataset classes."""
         lookupMap: Dict[str, type] = {
             "administrativeInformation": ContactAdministrativeInformation,
             "dataEntryBy": ContactDataEntryBy,
             "dataSetInformation": ContactDataSetInformation,
             "classificationInformation": ClassificationInformation,
             "publicationAndOwnership": ContactPublicationAndOwnership,
         }
         try:
             return lookupMap[name]
         except KeyError:
             return _check_common_lookup(name)
 
 
+class SourceDatasetLookup(etree.CustomElementClassLookup):
+    """Custom XML lookup class for ILCD SourceDataset files."""
+
+    def lookup(
+        self, unused_node_type, unused_document, unused_namespace, name: str
+    ) -> type:
+        """Maps ILCD SourceDataset XML elements to custom SourceDataset classes."""
+        lookupMap: Dict[str, type] = {
+            "administrativeInformation": SourceAdministrativeInformation,
+            "dataEntryBy": SourceDataEntryBy,
+            "dataSetInformation": SourceDataSetInformation,
+            "classificationInformation": ClassificationInformation,
+            "publicationAndOwnership": SourcePublicationAndOwnership,
+        }
+        try:
+            return lookupMap[name]
+        except KeyError:
+            return _check_common_lookup(name)
+
+
 def validate_file_process_dataset(
     file: Union[str, Path, StringIO]
 ) -> Union[None, List[str]]:
     """Validates an ILCD Process Dataset XML file against schema.
     Parameters:
     file: the str|Path path to the ILCD Process Dataset XML file or its StringIO
     representation.
@@ -381,14 +398,26 @@
     file: the str|Path path to the ILCD Contact Dataset XML file or its StringIO
     representation.
     Returns ``None`` if valid or a list of error strings.
     """
     return validate_file(file, Defaults.SCHEMA_CONTACT_DATASET)
 
 
+def validate_file_source_dataset(
+    file: Union[str, Path, StringIO]
+) -> Union[None, List[str]]:
+    """Validates an ILCD Source Dataset XML file against schema.
+    Parameters:
+    file: the str|Path path to the ILCD Source Dataset XML file or its StringIO
+    representation.
+    Returns ``None`` if valid or a list of error strings.
+    """
+    return validate_file(file, Defaults.SCHEMA_SOURCE_DATASET)
+
+
 def parse_file_process_dataset(file: Union[str, Path, StringIO]) -> ProcessDataSet:
     """Parses an ILCD Process Dataset XML file to custom ILCD classes.
     Parameters:
     file: the str|Path path to the ProcessDataset XML file or its StringIO
     representation.
     Returns a ProcessDataset class representing the root of the XML file.
     """
@@ -437,14 +466,24 @@
     file: the str|Path path to the Contact DataSet XML file or its StringIO
     representation.
     Returns a ContactDataSet class representing the root of the XML file.
     """
     return parse_file(file, Defaults.SCHEMA_CONTACT_DATASET, ContactDatasetLookup())
 
 
+def parse_file_source_dataset(file: Union[str, Path, StringIO]) -> SourceDataSet:
+    """Parses an ILCD Source DataSet XML file to custom ILCD classes.
+    Parameters:
+    file: the str|Path path to the Source DataSet XML file or its StringIO
+    representation.
+    Returns a SourceDataSet class representing the root of the XML file.
+    """
+    return parse_file(file, Defaults.SCHEMA_SOURCE_DATASET, SourceDatasetLookup())
+
+
 def parse_directory_process_dataset(
     dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
 ) -> List[Tuple[Path, ProcessDataSet]]:
     """Parses a directory of ILCD Process Dataset XML files to a list of
     custom ILCD classes.
     Parameters:
     dir_path: the directory path, should contain ILCD Process Dataset files.
@@ -478,15 +517,15 @@
     """
     if valid_suffixes is None:
         valid_suffixes = [".xml", ".ilcd"]
 
     return parse_directory(
         dir_path=dir_path,
         schema_path=Defaults.SCHEMA_FLOW_DATASET,
-        lookup=FlowDataSet(),
+        lookup=FlowDatasetLookup(),
         valid_suffixes=valid_suffixes,
     )
 
 
 def parse_directory_flow_property_dataset(
     dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
 ) -> List[Tuple[Path, FlowPropertyDataSet]]:
@@ -501,15 +540,15 @@
     """
     if valid_suffixes is None:
         valid_suffixes = [".xml", ".ilcd"]
 
     return parse_directory(
         dir_path=dir_path,
         schema_path=Defaults.SCHEMA_FLOW_PROPERTY_DATASET,
-        lookup=FlowPropertyDataSet(),
+        lookup=FlowPropertyDatasetLookup(),
         valid_suffixes=valid_suffixes,
     )
 
 
 def parse_directory_unit_group_dataset(
     dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
 ) -> List[Tuple[Path, UnitGroupDataSet]]:
@@ -552,14 +591,37 @@
         dir_path=dir_path,
         schema_path=Defaults.SCHEMA_CONTACT_DATASET,
         lookup=ContactDatasetLookup(),
         valid_suffixes=valid_suffixes,
     )
 
 
+def parse_directory_source_dataset(
+    dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
+) -> List[Tuple[Path, SourceDataSet]]:
+    """Parses a directory of ILCD Source Dataset XML files to a list of
+    custom ILCD classes.
+    Parameters:
+    dir_path: the directory path, should contain ILCD Source Dataset files.
+    valid_suffixes: a list of valid file suffixes which will only be considered for
+    parsing. If None, defaults to [".xml", ".ilcd"].
+    Returns a list of tuples of file paths and corresponding ILCD classes
+    representing the root of the XML file.
+    """
+    if valid_suffixes is None:
+        valid_suffixes = [".xml", ".ilcd"]
+
+    return parse_directory(
+        dir_path=dir_path,
+        schema_path=Defaults.SCHEMA_SOURCE_DATASET,
+        lookup=SourceDatasetLookup(),
+        valid_suffixes=valid_suffixes,
+    )
+
+
 def save_ilcd_file(
     root: etree.ElementBase, path: str, fill_defaults: bool = False
 ) -> None:
     """Saves an ILCD class to an XML file.
     Parameters:
     root: the ILCD class representing the root of the XML file.
     path: the path to save the ILCD XML file.
```

### Comparing `pyilcd-5.0.0/pyilcd/flow_dataset.py` & `pyilcd-6.0.0/pyilcd/flow_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from lxml import etree
 from lxmlh import get_element, get_element_list
 from pycasreg.validation import validate_cas
 
 from .common import (
-    ComplianceGroup,
+    ComplianceDeclarations,
     DataEntryByGroup1,
     DataEntryByGroup2,
     FlowCategoryInformation,
     GlobalReference,
     PublicationAndOwnershipGroup1,
 )
 from .helpers import (
@@ -235,30 +235,14 @@
 class LCIMethod(etree.ElementBase):
     """LCI methodological modelling aspects."""
 
     typeOfDataSet = create_element_text_flow_dataset("typeOfDataSet", str)
     """Names the basic type of the flow."""
 
 
-class ComplianceDeclarations(etree.ElementBase):
-    """Statements on compliance of several data set aspects with compliance
-    requirements as defined by the referenced compliance system (e.g. an
-    EPD scheme, handbook of a national or international data network such
-    as the ILCD, etc.)."""
-
-    @property
-    def compliances(self) -> List["Compliance"]:
-        """One compliance declaration"""
-        return get_element_list(self, "compliance")
-
-
-class Compliance(ComplianceGroup):
-    """One compliance declaration"""
-
-
 class DataEntryBy(DataEntryByGroup1, DataEntryByGroup2):
     """Staff or entity, that documented the generated data set, entering
     the information into the database; plus administrative information
     linked to the data entry activity.."""
 
 
 class PublicationAndOwnership(PublicationAndOwnershipGroup1):
```

### Comparing `pyilcd-5.0.0/pyilcd/flow_property_dataset.py` & `pyilcd-6.0.0/pyilcd/flow_property_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from lxml import etree
 from lxmlh import get_element, get_element_list
 
 from .common import (
     ClassificationInformation,
-    ComplianceGroup,
+    ComplianceDeclarations,
     DataEntryByGroup1,
     GlobalReference,
     PublicationAndOwnershipGroup1,
 )
 from .helpers import (
     create_attribute_flow_property_dataset,
     create_attribute_list_flow_property_dataset,
@@ -151,26 +151,14 @@
         """ "Source data set" of data source(s) used for the data
         set e.g. a paper, a questionnaire, a monography etc. The
         main raw data sources should be named, too. [Note: relevant
         especially for market price data.]"""
         return get_element_list(self, "referenceToDataSource")
 
 
-class ComplianceDeclarations(etree.ElementBase):
-    """Statements on compliance of several data set aspects with
-    compliance requirements as defined by the referenced compliance
-    system (e.g. an EPD scheme, handbook of a national or
-    international data network such as the ILCD, etc.)."""
-
-    @property
-    def compliances(self) -> List["Compliance"]:
-        """One compliance declaration"""
-        return get_element_list(self, "compliance")
-
-
 class DataEntryBy(DataEntryByGroup1):
     """Staff or entity, that documented the generated data set,
     entering the information into the database; plus administrative
     information linked to the data entry activity."""
 
 
 class PublicationAndOwnership(PublicationAndOwnershipGroup1):
@@ -179,11 +167,7 @@
 
     @property
     def referenceToOwnershipOfDataSet(self) -> "GlobalReference":
         """ "Contact data set" of the person or entity who owns this
         ata set. (Note: this is not necessarily the publisher of the
         ata set.)"""
         return get_element(self, "common:referenceToOwnershipOfDataSet")
-
-
-class Compliance(ComplianceGroup):
-    """One compliance declaration"""
```

### Comparing `pyilcd-5.0.0/pyilcd/helpers.py` & `pyilcd-6.0.0/pyilcd/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,22 @@
     name: str, attr_type: type, validator: Optional[Callable] = None
 ) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Contact Dataset attribute"""
     return create_attribute(name, attr_type, Defaults.SCHEMA_CONTACT_DATASET, validator)
 
 
+def create_attribute_source_dataset(
+    name: str, attr_type: type, validator: Optional[Callable] = None
+) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Source Dataset attribute"""
+    return create_attribute(name, attr_type, Defaults.SCHEMA_SOURCE_DATASET, validator)
+
+
 def create_element_text_process_dataset(name: str, element_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset element text"""
     return create_element_text(name, element_type, Defaults.SCHEMA_PROCESS_DATASET)
 
 
 def create_element_text_flow_dataset(name: str, element_type: type) -> property:
@@ -92,7 +100,13 @@
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_UNIT_GROUP_DATASET)
 
 
 def create_attribute_list_contact_dataset(name: str, attr_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Contact Dataset element text list"""
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_CONTACT_DATASET)
+
+
+def create_attribute_list_source_dataset(name: str, attr_type: type) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Source Dataset element text list"""
+    return create_attribute_list(name, attr_type, Defaults.SCHEMA_SOURCE_DATASET)
```

### Comparing `pyilcd-5.0.0/pyilcd/process_dataset.py` & `pyilcd-6.0.0/pyilcd/process_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Categories.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Categories.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Documentation.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Documentation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_ILCD.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_ILCD.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_Locations.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_Locations.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd` & `pyilcd-6.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/pyilcd/unit_group_dataset.py` & `pyilcd-6.0.0/pyilcd/unit_group_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from lxml import etree
 from lxmlh import get_element, get_element_list
 
 from .common import (
     ClassificationInformation,
-    ComplianceGroup,
+    ComplianceDeclarations,
     DataEntryByGroup1,
     GlobalReference,
     PublicationAndOwnershipGroup1,
 )
 from .helpers import (
     create_attribute_list_unit_group_dataset,
     create_attribute_unit_group_dataset,
@@ -155,26 +155,14 @@
     referenceToReferenceUnit = create_attribute_unit_group_dataset(
         "referenceToReferenceUnit", int
     )
     """The Unit group's unit in which the data set is expressed
     (data set internal reference)."""
 
 
-class ComplianceDeclarations(etree.ElementBase):
-    """Statements on compliance of several data set aspects with compliance
-    requirements as defined by the referenced compliance system (e.g. an EPD
-    scheme, handbook of a national or international data network such as the
-    ILCD, etc.)."""
-
-    @property
-    def compliances(self) -> List["Compliance"]:
-        """One compliance declaration"""
-        return get_element_list(self, "compliance")
-
-
 class DataEntryBy(DataEntryByGroup1):
     """Staff or entity, that documented the generated data set,
     entering the information into the database; plus administrative
     information linked to the data entry activity."""
 
 
 class PublicationAndOwnership(PublicationAndOwnershipGroup1):
@@ -207,11 +195,7 @@
     only significant digits of the value.]"""
 
     generalComment = create_attribute_list_unit_group_dataset("name", str)
     """General comment on each single unit, typically giving the
     long name and unit system from which this unit stems, and
     (if necessary) referring to specifc data sources used, or for
     workflow purposes about status of "finalisation" of an entry etc."""
-
-
-class Compliance(ComplianceGroup):
-    """One compliance declaration"""
```

### Comparing `pyilcd-5.0.0/pyilcd.egg-info/PKG-INFO` & `pyilcd-6.0.0/pyilcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 5.0.0
+Version: 6.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-5.0.0/pyilcd.egg-info/SOURCES.txt` & `pyilcd-6.0.0/pyilcd.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ./pyilcd/config.py
 ./pyilcd/contact_dataset.py
 ./pyilcd/core.py
 ./pyilcd/flow_dataset.py
 ./pyilcd/flow_property_dataset.py
 ./pyilcd/helpers.py
 ./pyilcd/process_dataset.py
+./pyilcd/source_dataset.py
 ./pyilcd/unit_group_dataset.py
 ./pyilcd/utils.py
 pyilcd/VERSION
 pyilcd.egg-info/PKG-INFO
 pyilcd.egg-info/SOURCES.txt
 pyilcd.egg-info/dependency_links.txt
 pyilcd.egg-info/not-zip-safe
@@ -39,10 +40,11 @@
 pyilcd/schemas/ILCD_SourceDataSet.xsd
 pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
 tests/test_common.py
 tests/test_config.py
 tests/test_contact_dataset.py
 tests/test_core.py
 tests/test_flow_dataset.py
-tests/test_flow_propert_dataset.py
+tests/test_flow_property_dataset.py
 tests/test_process_dataset.py
+tests/test_source_dataset.py
 tests/test_unit_group_dataset.py
```

### Comparing `pyilcd-5.0.0/setup.cfg` & `pyilcd-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/tests/test_common.py` & `pyilcd-6.0.0/tests/test_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Classification,
     DataQualityIndicator,
     GlobalReference,
     Method,
 )
 from pyilcd.flow_dataset import FlowDataSet
 from pyilcd.process_dataset import ProcessDataSet
+from pyilcd.unit_group_dataset import UnitGroupDataSet
 
 
 def test_classification_information(process_dataset: ProcessDataSet) -> None:
     """It parses attributes correctly."""
     dataSetInformation = process_dataset.processInformation.dataSetInformation
     classificationInformation = dataSetInformation.classificationInformation
 
@@ -30,17 +31,17 @@
     assert isinstance(
         review.dataQualityIndicators.dataQualityIndicators[0], DataQualityIndicator
     )
     assert isinstance(review.referenceToCompleteReviewReport, GlobalReference)
     assert isinstance(review.referenceToNameOfReviewerAndInstitution, GlobalReference)
 
 
-def test_compliance(process_dataset: ProcessDataSet) -> None:
+def test_compliance(unit_group_dataset: UnitGroupDataSet) -> None:
     """It parses attributes correctly."""
-    modellingAndValidation = process_dataset.modellingAndValidation
+    modellingAndValidation = unit_group_dataset.modellingAndValidation
     compliance = modellingAndValidation.complianceDeclarations.compliances[0]
 
     assert isinstance(compliance.referenceToComplianceSystem, GlobalReference)
 
 
 def test_commissioner_and_goal(process_dataset: ProcessDataSet) -> None:
     """It parses attributes correctly."""
```

### Comparing `pyilcd-5.0.0/tests/test_config.py` & `pyilcd-6.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/tests/test_contact_dataset.py` & `pyilcd-6.0.0/tests/test_contact_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/tests/test_flow_dataset.py` & `pyilcd-6.0.0/tests/test_flow_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test cases for the __flow_dataset__ module."""
 from pyilcd.common import GlobalReference
 from pyilcd.flow_dataset import (
-    Compliance,
+    ComplianceDeclarations,
     DataEntryBy,
     FlowCategoryInformation,
     FlowDataSet,
     Geography,
     LCIMethod,
     Name,
     QuantitativeReference,
@@ -31,15 +31,15 @@
 
 def test_modelling_and_validation(flow_dataset: FlowDataSet) -> None:
     """It parses attributes correctly."""
     modellingAndValidation = flow_dataset.modellingAndValidation
 
     assert isinstance(modellingAndValidation.lciMethod, LCIMethod)
     assert isinstance(
-        modellingAndValidation.complianceDeclarations.compliances[0], Compliance
+        modellingAndValidation.complianceDeclarations, ComplianceDeclarations
     )
 
 
 def test_administrative_information(flow_dataset: FlowDataSet) -> None:
     """It parses attributes correctly."""
     administrativeInformation = flow_dataset.administrativeInformation
```

### Comparing `pyilcd-5.0.0/tests/test_flow_propert_dataset.py` & `pyilcd-6.0.0/tests/test_flow_property_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """Test cases for the __flow_property_dataset__ module."""
 from pyilcd.common import ClassificationInformation, GlobalReference
-from pyilcd.flow_property_dataset import Compliance, DataEntryBy, FlowPropertyDataSet
+from pyilcd.flow_property_dataset import (
+    ComplianceDeclarations,
+    DataEntryBy,
+    FlowPropertyDataSet,
+)
 
 
 def test_flow_properties_information(
     flow_property_dataset: FlowPropertyDataSet,
 ) -> None:
     """It parses attributes correctly."""
     flowPropertiesInformation = flow_property_dataset.flowPropertiesInformation
@@ -21,21 +25,22 @@
 
 def test_modelling_and_validation(flow_property_dataset: FlowPropertyDataSet) -> None:
     """It parses attributes correctly."""
     modellingAndValidation = flow_property_dataset.modellingAndValidation
     dataSourcesTreatmentAndRepresentativeness = (
         modellingAndValidation.dataSourcesTreatmentAndRepresentativeness
     )
-    complianceDeclarations = modellingAndValidation.complianceDeclarations
 
     assert isinstance(
+        modellingAndValidation.complianceDeclarations, ComplianceDeclarations
+    )
+    assert isinstance(
         dataSourcesTreatmentAndRepresentativeness.referenceToDataSources[0],
         GlobalReference,
     )
-    assert isinstance(complianceDeclarations.compliances[0], Compliance)
 
 
 def test_administrative_information(flow_property_dataset: FlowPropertyDataSet) -> None:
     """It parses attributes correctly."""
     administrativeInformation = flow_property_dataset.administrativeInformation
     dataEntryBy = administrativeInformation.dataEntryBy
     publicationAndOwnership = administrativeInformation.publicationAndOwnership
```

### Comparing `pyilcd-5.0.0/tests/test_process_dataset.py` & `pyilcd-6.0.0/tests/test_process_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-5.0.0/tests/test_unit_group_dataset.py` & `pyilcd-6.0.0/tests/test_unit_group_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Test cases for the __unit_group_dataset__ module."""
 from pyilcd.common import ClassificationInformation, GlobalReference
 from pyilcd.unit_group_dataset import (
-    Compliance,
     DataEntryBy,
     QuantitativeReference,
     Unit,
     UnitGroupDataSet,
 )
 
 
@@ -17,23 +16,14 @@
 
     assert isinstance(
         dataSetInformation.classificationInformation, ClassificationInformation
     )
     assert isinstance(quantitativeReference, QuantitativeReference)
 
 
-def test_modelling_and_validation(unit_group_dataset: UnitGroupDataSet) -> None:
-    """It parses attributes correctly."""
-    modellingAndValidation = unit_group_dataset.modellingAndValidation
-
-    assert isinstance(
-        modellingAndValidation.complianceDeclarations.compliances[0], Compliance
-    )
-
-
 def test_administrative_information(unit_group_dataset: UnitGroupDataSet) -> None:
     """It parses attributes correctly."""
     administrativeInformation = unit_group_dataset.administrativeInformation
 
     assert isinstance(administrativeInformation.dataEntryBy, DataEntryBy)
     assert isinstance(
         administrativeInformation.publicationAndOwnership.referenceToOwnershipOfDataSet,
```

