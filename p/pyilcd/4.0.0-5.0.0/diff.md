# Comparing `tmp/pyilcd-4.0.0.tar.gz` & `tmp/pyilcd-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyilcd-4.0.0.tar", last modified: Thu Apr 13 01:43:42 2023, max compression
+gzip compressed data, was "pyilcd-5.0.0.tar", last modified: Thu Apr 13 14:31:15 2023, max compression
```

## Comparing `pyilcd-4.0.0.tar` & `pyilcd-5.0.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.858326 pyilcd-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-13 01:43:33.000000 pyilcd-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 01:43:33.000000 pyilcd-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 01:43:42.858326 pyilcd-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 01:43:33.000000 pyilcd-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.854326 pyilcd-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 01:43:33.000000 pyilcd-4.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.854326 pyilcd-4.0.0/pyilcd/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/flow_property_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/process_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.858326 pyilcd-4.0.0/pyilcd/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Categories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Documentation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_ILCD.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_Locations.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/unit_group_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyilcd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.854326 pyilcd-4.0.0/pyilcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 01:43:42.000000 pyilcd-4.0.0/pyilcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 01:43:33.000000 pyilcd-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 01:43:42.858326 pyilcd-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:43:42.858326 pyilcd-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_flow_propert_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-13 01:43:33.000000 pyilcd-4.0.0/tests/test_unit_group_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.434860 pyilcd-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-13 14:31:05.000000 pyilcd-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 14:31:05.000000 pyilcd-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:31:15.434860 pyilcd-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 14:31:05.000000 pyilcd-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.422860 pyilcd-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 14:31:05.000000 pyilcd-5.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.426860 pyilcd-5.0.0/pyilcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/contact_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/flow_property_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.430860 pyilcd-5.0.0/pyilcd/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Categories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Documentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ILCD.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_Locations.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/unit_group_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyilcd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.426860 pyilcd-5.0.0/pyilcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 14:31:15.000000 pyilcd-5.0.0/pyilcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 14:31:05.000000 pyilcd-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 14:31:15.434860 pyilcd-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:31:15.430860 pyilcd-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_contact_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_flow_propert_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-13 14:31:05.000000 pyilcd-5.0.0/tests/test_unit_group_dataset.py
```

### Comparing `pyilcd-4.0.0/LICENSE` & `pyilcd-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/PKG-INFO` & `pyilcd-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 4.0.0
+Version: 5.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-4.0.0/README.md` & `pyilcd-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/docs/conf.py` & `pyilcd-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/__init__.py` & `pyilcd-5.0.0/pyilcd/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """pyilcd."""
 from .core import (
+    parse_directory_contact_dataset,
     parse_directory_flow_dataset,
     parse_directory_flow_property_dataset,
     parse_directory_process_dataset,
     parse_directory_unit_group_dataset,
+    parse_file_contact_dataset,
     parse_file_flow_dataset,
     parse_file_flow_property_dataset,
     parse_file_process_dataset,
     parse_file_unit_group_dataset,
     save_ilcd_file,
+    validate_file_contact_dataset,
     validate_file_flow_dataset,
     validate_file_flow_property_dataset,
     validate_file_process_dataset,
     validate_file_unit_group_dataset,
 )
 from .utils import get_version_tuple
 
 __all__ = (
     "__version__",
+    "parse_directory_contact_dataset",
     "parse_directory_flow_dataset",
     "parse_directory_flow_property_dataset",
     "parse_directory_process_dataset",
     "parse_directory_unit_group_dataset",
+    "parse_file_contact_dataset",
     "parse_file_flow_dataset",
     "parse_file_flow_property_dataset",
     "parse_file_process_dataset",
     "parse_file_unit_group_dataset",
     "save_ilcd_file",
+    "validate_file_contact_dataset",
     "validate_file_flow_dataset",
     "validate_file_flow_property_dataset",
     "validate_file_process_dataset",
     "validate_file_unit_group_dataset",
 )
 
 __version__ = get_version_tuple()
```

### Comparing `pyilcd-4.0.0/pyilcd/common.py` & `pyilcd-5.0.0/pyilcd/common.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/config.py` & `pyilcd-5.0.0/pyilcd/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     )
     SCHEMA_FLOW_PROPERTY_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_FlowPropertyDataSet.xsd"
     )
     SCHEMA_UNIT_GROUP_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_UnitGroupDataSet.xsd"
     )
+    SCHEMA_CONTACT_DATASET: ClassVar[str] = os.path.join(
+        SCHEMA_DIR, "ILCD_ContactDataSet.xsd"
+    )
 
     DYNAMIC_DEFAULTS: ClassVar[
         Dict[str, Dict[str, Callable[[etree.ElementBase], str]]]
     ] = {}
     STATIC_DEFAULTS: ClassVar[Dict[str, Dict[str, str]]] = {
         "Classification": {
             "name": "ILCD",
```

### Comparing `pyilcd-4.0.0/pyilcd/core.py` & `pyilcd-5.0.0/pyilcd/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     FlowCategorization,
     FlowCategoryInformation,
     GlobalReference,
     Method,
     Scope,
 )
 from .config import Defaults
+from .contact_dataset import (
+    AdministrativeInformation as ContactAdministrativeInformation,
+)
+from .contact_dataset import ContactDataSet, ContactInformation
+from .contact_dataset import DataEntryBy as ContactDataEntryBy
+from .contact_dataset import DataSetInformation as ContactDataSetInformation
+from .contact_dataset import PublicationAndOwnership as ContactPublicationAndOwnership
 from .flow_dataset import AdministrativeInformation as FlowAdministrativeInformation
 from .flow_dataset import Compliance as FlowCompliance
 from .flow_dataset import ComplianceDeclarations as FlowComplianceDeclarations
 from .flow_dataset import DataEntryBy as FlowDataEntryBy
 from .flow_dataset import DataSetInformation as FlowDataSetInformation
 from .flow_dataset import FlowDataSet, FlowInformation, FlowProperties, FlowProperty
 from .flow_dataset import Geography as FlowGeography
@@ -115,14 +122,16 @@
     "category": Category,
     "class": Class,
     "classification": Classification,
     "completeness": Completeness,
     "completenessElementaryFlows": CompletenessElementaryFlows,
     "complementingProcesses": ComplementingProcesses,
     "commissionerAndGoal": CommissionerAndGoal,
+    "contactDataSet": ContactDataSet,
+    "contactInformation": ContactInformation,
     "dataGenerator": DataGenerator,
     "dataQualityIndicator": DataQualityIndicator,
     "dataQualityIndicators": DataQualityIndicators,
     "elementaryFlowCategorization": FlowCategorization,
     "flowDataSet": FlowDataSet,
     "flowInformation": FlowInformation,
     "flowProperties": FlowProperties,
@@ -137,14 +146,15 @@
     "LCIAResults": LCIAResults,
     "LCIMethod": LCIMethod,
     "LCIMethodAndAllocation": LCIMethodAndAllocation,
     "locationOfOperationSupplyOrProduction": (LocationOfOperationSupplyOrProduction),
     "mathematicalRelations": MathematicalRelations,
     "processDataSet": ProcessDataSet,
     "processInformation": ProcessInformation,
+    "referenceToContact": GlobalReference,
     "referenceToCommissioner": GlobalReference,
     "referenceToComplementingProcess": GlobalReference,
     "referenceToCompleteReviewReport": GlobalReference,
     "referenceToComplianceSystem": GlobalReference,
     "referenceToConvertedOriginalDataSetFrom": GlobalReference,
     "referenceToDataHandlingPrinciples": GlobalReference,
     "referenceToDataSetFormat": GlobalReference,
@@ -153,14 +163,15 @@
     "referenceToEntitiesWithExclusiveAccess": GlobalReference,
     "referenceToExternalDocumentation": GlobalReference,
     "referenceToFlowDataSet": GlobalReference,
     "referenceToFlowPropertyDataSet": GlobalReference,
     "referenceToIncludedProcesses": GlobalReference,
     "referenceToLCAMethodDetails": GlobalReference,
     "referenceToLCIAMethodDataSet": GlobalReference,
+    "referenceToLogo": GlobalReference,
     "referenceToNameOfReviewerAndInstitution": GlobalReference,
     "referenceToOwnershipOfDataSet": GlobalReference,
     "referenceToPersonOrEntityEnteringTheData": GlobalReference,
     "referenceToPersonOrEntityGeneratingTheDataSet": GlobalReference,
     "referenceToPrecedingDataSetVersion": GlobalReference,
     "referenceToReferenceUnitGroup": GlobalReference,
     "referenceToRegistrationAuthority": GlobalReference,
@@ -290,14 +301,34 @@
         }
         try:
             return lookupMap[name]
         except KeyError:
             return _check_common_lookup(name)
 
 
+class ContactDatasetLookup(etree.CustomElementClassLookup):
+    """Custom XML lookup class for ILCD ContactDataset files."""
+
+    def lookup(
+        self, unused_node_type, unused_document, unused_namespace, name: str
+    ) -> type:
+        """Maps ILCD ProcessDataset XML elements to custom ContactDataset classes."""
+        lookupMap: Dict[str, type] = {
+            "administrativeInformation": ContactAdministrativeInformation,
+            "dataEntryBy": ContactDataEntryBy,
+            "dataSetInformation": ContactDataSetInformation,
+            "classificationInformation": ClassificationInformation,
+            "publicationAndOwnership": ContactPublicationAndOwnership,
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
@@ -338,14 +369,26 @@
     file: the str|Path path to the ILCD Unit Group Dataset XML file or its StringIO
     representation.
     Returns ``None`` if valid or a list of error strings.
     """
     return validate_file(file, Defaults.SCHEMA_UNIT_GROUP_DATASET)
 
 
+def validate_file_contact_dataset(
+    file: Union[str, Path, StringIO]
+) -> Union[None, List[str]]:
+    """Validates an ILCD Contact Dataset XML file against schema.
+    Parameters:
+    file: the str|Path path to the ILCD Contact Dataset XML file or its StringIO
+    representation.
+    Returns ``None`` if valid or a list of error strings.
+    """
+    return validate_file(file, Defaults.SCHEMA_CONTACT_DATASET)
+
+
 def parse_file_process_dataset(file: Union[str, Path, StringIO]) -> ProcessDataSet:
     """Parses an ILCD Process Dataset XML file to custom ILCD classes.
     Parameters:
     file: the str|Path path to the ProcessDataset XML file or its StringIO
     representation.
     Returns a ProcessDataset class representing the root of the XML file.
     """
@@ -377,21 +420,31 @@
 
 
 def parse_file_unit_group_dataset(file: Union[str, Path, StringIO]) -> UnitGroupDataSet:
     """Parses an ILCD Unit Group DataSet XML file to custom ILCD classes.
     Parameters:
     file: the str|Path path to the Unit Group DataSet XML file or its StringIO
     representation.
-    Returns a FlowPropertyDataSet class representing the root of the XML file.
+    Returns a UnitGroupDataSet class representing the root of the XML file.
     """
     return parse_file(
         file, Defaults.SCHEMA_UNIT_GROUP_DATASET, UnitGroupDatasetLookup()
     )
 
 
+def parse_file_contact_dataset(file: Union[str, Path, StringIO]) -> ContactDataSet:
+    """Parses an ILCD Contact DataSet XML file to custom ILCD classes.
+    Parameters:
+    file: the str|Path path to the Contact DataSet XML file or its StringIO
+    representation.
+    Returns a ContactDataSet class representing the root of the XML file.
+    """
+    return parse_file(file, Defaults.SCHEMA_CONTACT_DATASET, ContactDatasetLookup())
+
+
 def parse_directory_process_dataset(
     dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
 ) -> List[Tuple[Path, ProcessDataSet]]:
     """Parses a directory of ILCD Process Dataset XML files to a list of
     custom ILCD classes.
     Parameters:
     dir_path: the directory path, should contain ILCD Process Dataset files.
@@ -476,14 +529,37 @@
         dir_path=dir_path,
         schema_path=Defaults.SCHEMA_UNIT_GROUP_DATASET,
         lookup=UnitGroupDatasetLookup(),
         valid_suffixes=valid_suffixes,
     )
 
 
+def parse_directory_contact_dataset(
+    dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
+) -> List[Tuple[Path, ContactDataSet]]:
+    """Parses a directory of ILCD Contact Dataset XML files to a list of
+    custom ILCD classes.
+    Parameters:
+    dir_path: the directory path, should contain ILCD Contact Dataset files.
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
+        schema_path=Defaults.SCHEMA_CONTACT_DATASET,
+        lookup=ContactDatasetLookup(),
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

### Comparing `pyilcd-4.0.0/pyilcd/flow_dataset.py` & `pyilcd-5.0.0/pyilcd/flow_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/flow_property_dataset.py` & `pyilcd-5.0.0/pyilcd/flow_property_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/helpers.py` & `pyilcd-5.0.0/pyilcd/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,22 @@
     """Helper wrapper method for creating setters and getters for an ilcd
     Unit Group Dataset attribute"""
     return create_attribute(
         name, attr_type, Defaults.SCHEMA_UNIT_GROUP_DATASET, validator
     )
 
 
+def create_attribute_contact_dataset(
+    name: str, attr_type: type, validator: Optional[Callable] = None
+) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Contact Dataset attribute"""
+    return create_attribute(name, attr_type, Defaults.SCHEMA_CONTACT_DATASET, validator)
+
+
 def create_element_text_process_dataset(name: str, element_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset element text"""
     return create_element_text(name, element_type, Defaults.SCHEMA_PROCESS_DATASET)
 
 
 def create_element_text_flow_dataset(name: str, element_type: type) -> property:
@@ -78,7 +86,13 @@
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_FLOW_PROPERTY_DATASET)
 
 
 def create_attribute_list_unit_group_dataset(name: str, attr_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Unit Group Dataset element text list"""
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_UNIT_GROUP_DATASET)
+
+
+def create_attribute_list_contact_dataset(name: str, attr_type: type) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Contact Dataset element text list"""
+    return create_attribute_list(name, attr_type, Defaults.SCHEMA_CONTACT_DATASET)
```

### Comparing `pyilcd-4.0.0/pyilcd/process_dataset.py` & `pyilcd-5.0.0/pyilcd/process_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Categories.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Categories.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Documentation.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Documentation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_ILCD.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_ILCD.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_Locations.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_Locations.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd` & `pyilcd-5.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/pyilcd/unit_group_dataset.py` & `pyilcd-5.0.0/pyilcd/unit_group_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,15 +116,17 @@
 
     commonUUID = create_attribute_unit_group_dataset("common:UUID", str)
     """Automatically generated Universally Unique Identifier of this data
     set. Together with the "Data set version", the UUID uniquely identifies each data
     set."""
 
     names = create_attribute_list_unit_group_dataset("common:name", str)
-    """Name of flow property."""
+    """Name of the unit group, typically indicating for which flow property or group
+    of flow properties it is used. The individual units are named in the "Units"
+    section of the "Unit group data set"."""
 
     synonyms = create_attribute_list_unit_group_dataset("common:synonyms", str)
     """Synonyms / alternative names / brands of the good, service, or
     process. Separated by semicolon."""
 
     generalComments = create_attribute_list_unit_group_dataset(
         "common:generalComment", str
```

### Comparing `pyilcd-4.0.0/pyilcd.egg-info/PKG-INFO` & `pyilcd-5.0.0/pyilcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 4.0.0
+Version: 5.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-4.0.0/pyilcd.egg-info/SOURCES.txt` & `pyilcd-5.0.0/pyilcd.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 ./docs/conf.py
 ./pyilcd/__init__.py
 ./pyilcd/common.py
 ./pyilcd/config.py
+./pyilcd/contact_dataset.py
 ./pyilcd/core.py
 ./pyilcd/flow_dataset.py
 ./pyilcd/flow_property_dataset.py
 ./pyilcd/helpers.py
 ./pyilcd/process_dataset.py
 ./pyilcd/unit_group_dataset.py
 ./pyilcd/utils.py
@@ -35,12 +36,13 @@
 pyilcd/schemas/ILCD_LCIAMethodologies.xsd
 pyilcd/schemas/ILCD_Locations.xsd
 pyilcd/schemas/ILCD_ProcessDataSet.xsd
 pyilcd/schemas/ILCD_SourceDataSet.xsd
 pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
 tests/test_common.py
 tests/test_config.py
+tests/test_contact_dataset.py
 tests/test_core.py
 tests/test_flow_dataset.py
 tests/test_flow_propert_dataset.py
 tests/test_process_dataset.py
 tests/test_unit_group_dataset.py
```

### Comparing `pyilcd-4.0.0/setup.cfg` & `pyilcd-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_common.py` & `pyilcd-5.0.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_config.py` & `pyilcd-5.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_core.py` & `pyilcd-5.0.0/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pytest
 
 from pyilcd.core import (
     _check_common_lookup,
     parse_file_process_dataset,
     save_ilcd_file,
+    validate_file_contact_dataset,
     validate_file_flow_dataset,
     validate_file_flow_property_dataset,
     validate_file_process_dataset,
     validate_file_unit_group_dataset,
 )
 
 
@@ -40,14 +41,19 @@
 
 
 def test_validate_file_unit_group_dataset_success() -> None:
     """It validates file successfully."""
     assert validate_file_unit_group_dataset("data/sample_unitgroup.xml") is None
 
 
+def test_validate_file_contact_dataset_success() -> None:
+    """It validates file successfully."""
+    assert validate_file_contact_dataset("data/sample_contact.xml") is None
+
+
 def _validate_file_fail(
     validator: Callable[[Union[str, Path, StringIO]], Union[None, List[str]]]
 ) -> None:
     xml = StringIO("<ilcd></ilcd>")
     errorExpected = (
         "<string>:1:0:ERROR:SCHEMASV:SCHEMAV_CVC_ELT_1: Element 'ilcd': "
         "No matching global declaration available for the validation root."
@@ -73,14 +79,19 @@
 
 
 def test_validate_file_unit_group_dataset_fail() -> None:
     """It validates file successfully."""
     _validate_file_fail(validate_file_unit_group_dataset)
 
 
+def test_validate_file_contact_dataset_fail() -> None:
+    """It validates file successfully."""
+    _validate_file_fail(validate_file_contact_dataset)
+
+
 def test_save_ilcd_file() -> None:
     """It saves read file correctly."""
     inputPath = "data/sample_process.xml"
     processDataset = parse_file_process_dataset(inputPath)
     outputPath = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
     save_ilcd_file(processDataset, outputPath, fill_defaults=False)
```

### Comparing `pyilcd-4.0.0/tests/test_flow_dataset.py` & `pyilcd-5.0.0/tests/test_flow_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_flow_propert_dataset.py` & `pyilcd-5.0.0/tests/test_flow_propert_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_process_dataset.py` & `pyilcd-5.0.0/tests/test_process_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-4.0.0/tests/test_unit_group_dataset.py` & `pyilcd-5.0.0/tests/test_unit_group_dataset.py`

 * *Files identical despite different names*

