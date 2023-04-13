# Comparing `tmp/pyilcd-2.0.0.tar.gz` & `tmp/pyilcd-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyilcd-2.0.0.tar", last modified: Wed Apr 12 13:59:58 2023, max compression
+gzip compressed data, was "pyilcd-3.0.0.tar", last modified: Wed Apr 12 16:14:54 2023, max compression
```

## Comparing `pyilcd-2.0.0.tar` & `pyilcd-3.0.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.679233 pyilcd-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-12 13:59:49.000000 pyilcd-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 13:59:49.000000 pyilcd-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 13:59:58.679233 pyilcd-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-12 13:59:49.000000 pyilcd-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.671233 pyilcd-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 13:59:49.000000 pyilcd-2.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/process_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Categories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Documentation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ILCD.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_Locations.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyilcd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/pyilcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 13:59:58.000000 pyilcd-2.0.0/pyilcd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 13:59:49.000000 pyilcd-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 13:59:58.679233 pyilcd-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:59:58.675233 pyilcd-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_flow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-12 13:59:49.000000 pyilcd-2.0.0/tests/test_process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.404123 pyilcd-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-04-12 16:14:43.000000 pyilcd-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 16:14:43.000000 pyilcd-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 16:14:54.404123 pyilcd-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-12 16:14:43.000000 pyilcd-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.396123 pyilcd-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 16:14:43.000000 pyilcd-3.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.400123 pyilcd-3.0.0/pyilcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/flow_property_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58769 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/process_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.404123 pyilcd-3.0.0/pyilcd/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Categories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   103898 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    62500 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Documentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_ILCD.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    89067 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_Locations.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   157604 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyilcd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.400123 pyilcd-3.0.0/pyilcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 16:14:54.000000 pyilcd-3.0.0/pyilcd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 16:14:43.000000 pyilcd-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 16:14:54.404123 pyilcd-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:14:54.404123 pyilcd-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_flow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_flow_propert_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-12 16:14:43.000000 pyilcd-3.0.0/tests/test_process_dataset.py
```

### Comparing `pyilcd-2.0.0/LICENSE` & `pyilcd-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/PKG-INFO` & `pyilcd-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 2.0.0
+Version: 3.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-2.0.0/README.md` & `pyilcd-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/docs/conf.py` & `pyilcd-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/common.py` & `pyilcd-3.0.0/pyilcd/common.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/config.py` & `pyilcd-3.0.0/pyilcd/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     SCHEMA_DIR: ClassVar[str] = os.path.join(Path(__file__).parent.resolve(), "schemas")
     SCHEMA_PROCESS_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_ProcessDataSet.xsd"
     )
     SCHEMA_FLOW_DATASET: ClassVar[str] = os.path.join(
         SCHEMA_DIR, "ILCD_FlowDataSet.xsd"
     )
+    SCHEMA_FLOW_PROPERTY_DATASET: ClassVar[str] = os.path.join(
+        SCHEMA_DIR, "ILCD_FlowPropertyDataSet.xsd"
+    )
 
     DYNAMIC_DEFAULTS: ClassVar[
         Dict[str, Dict[str, Callable[[etree.ElementBase], str]]]
     ] = {}
     STATIC_DEFAULTS: ClassVar[Dict[str, Dict[str, str]]] = {
         "Classification": {
             "name": "ILCD",
```

### Comparing `pyilcd-2.0.0/pyilcd/core.py` & `pyilcd-3.0.0/pyilcd/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,34 @@
 from .flow_dataset import Geography as FlowGeography
 from .flow_dataset import LCIMethod
 from .flow_dataset import ModellingAndValidation as FlowModellingAndValidation
 from .flow_dataset import Name as FlowName
 from .flow_dataset import PublicationAndOwnership as FlowPublicationAndOwnership
 from .flow_dataset import QuantitativeReference as FlowQuantitativeReference
 from .flow_dataset import Technology as FlowTechnology
+from .flow_property_dataset import (
+    AdministrativeInformation as FlowPropertyAdministrativeInformation,
+)
+from .flow_property_dataset import Compliance as FlowPropertyCompliance
+from .flow_property_dataset import (
+    ComplianceDeclarations as FlowPropertyComplianceDeclarations,
+)
+from .flow_property_dataset import DataEntryBy as FlowPropertyDataEntryBy
+from .flow_property_dataset import DataSetInformation as FlowPropertyDataSetInformation
+from .flow_property_dataset import DataSourcesTreatmentAndRepresentativeness as FPDSTAR
+from .flow_property_dataset import FlowPropertiesInformation, FlowPropertyDataSet
+from .flow_property_dataset import (
+    ModellingAndValidation as FlowPropertyModellingAndValidation,
+)
+from .flow_property_dataset import (
+    PublicationAndOwnership as FlowPropertyPublicationAndOwnership,
+)
+from .flow_property_dataset import (
+    QuantitativeReference as FlowPropertyQuantitativeReference,
+)
 from .process_dataset import (
     AdministrativeInformation as ProcessAdministrativeInformation,
 )
 from .process_dataset import (
     Allocation,
     Allocations,
     ComplementingProcesses,
@@ -45,19 +65,16 @@
     CompletenessElementaryFlows,
 )
 from .process_dataset import Compliance as ProcessCompliance
 from .process_dataset import ComplianceDeclarations as ProcessComplianceDeclarations
 from .process_dataset import DataEntryBy as ProcessDataEntryBy
 from .process_dataset import DataGenerator
 from .process_dataset import DataSetInformation as ProcessDataSetInformation
-from .process_dataset import (
-    DataSourcesTreatmentAndRepresentativeness,
-    Exchange,
-    Exchanges,
-)
+from .process_dataset import DataSourcesTreatmentAndRepresentativeness as PDSTAR
+from .process_dataset import Exchange, Exchanges
 from .process_dataset import Geography as ProcessGeography
 from .process_dataset import (
     LCIAResult,
     LCIAResults,
     LCIMethodAndAllocation,
     LocationOfOperationSupplyOrProduction,
     MathematicalRelations,
@@ -74,32 +91,31 @@
 )
 from .process_dataset import Technology as ProcessTechnology
 from .process_dataset import Time, Validation, VariableParameter
 
 COMMON_LOOK_UP: Dict[str, type] = {
     "allocation": Allocation,
     "allocations": Allocations,
-    "dataSourcesTreatmentAndRepresentativeness": (
-        DataSourcesTreatmentAndRepresentativeness
-    ),
     "category": Category,
     "class": Class,
     "classification": Classification,
     "completeness": Completeness,
     "completenessElementaryFlows": CompletenessElementaryFlows,
     "complementingProcesses": ComplementingProcesses,
     "commissionerAndGoal": CommissionerAndGoal,
     "dataGenerator": DataGenerator,
     "dataQualityIndicator": DataQualityIndicator,
     "dataQualityIndicators": DataQualityIndicators,
     "elementaryFlowCategorization": FlowCategorization,
     "flowDataSet": FlowDataSet,
     "flowInformation": FlowInformation,
     "flowProperties": FlowProperties,
+    "flowPropertiesInformation": FlowPropertiesInformation,
     "flowProperty": FlowProperty,
+    "flowPropertyDataSet": FlowPropertyDataSet,
     "method": Method,
     "scope": Scope,
     "exchange": Exchange,
     "exchanges": Exchanges,
     "LCIAResult": LCIAResult,
     "LCIAResults": LCIAResults,
     "LCIMethod": LCIMethod,
@@ -125,14 +141,15 @@
     "referenceToLCAMethodDetails": GlobalReference,
     "referenceToLCIAMethodDataSet": GlobalReference,
     "referenceToNameOfReviewerAndInstitution": GlobalReference,
     "referenceToOwnershipOfDataSet": GlobalReference,
     "referenceToPersonOrEntityEnteringTheData": GlobalReference,
     "referenceToPersonOrEntityGeneratingTheDataSet": GlobalReference,
     "referenceToPrecedingDataSetVersion": GlobalReference,
+    "referenceToReferenceUnitGroup": GlobalReference,
     "referenceToRegistrationAuthority": GlobalReference,
     "referenceToSupportedImpactAssessmentMethods": GlobalReference,
     "referenceToTechnicalSpecification": GlobalReference,
     "referenceToTechnologyFlowDiagrammOrPicture": GlobalReference,
     "referenceToTechnologyPictogramme": GlobalReference,
     "referenceToUnchangedRepublication": GlobalReference,
     "referencesToDataSource": ReferencesToDataSource,
@@ -158,14 +175,15 @@
 
     def lookup(self, unused_node_type, unused_document, unused_namespace, name) -> type:
         """Maps ILCD ProcessDataset XML elements to custom ProcessDataset classes."""
         lookupMap: Dict[str, type] = {
             "administrativeInformation": ProcessAdministrativeInformation,
             "dataEntryBy": ProcessDataEntryBy,
             "dataSetInformation": ProcessDataSetInformation,
+            "dataSourcesTreatmentAndRepresentativeness": PDSTAR,
             "classificationInformation": ClassificationInformation,
             "compliance": ProcessCompliance,
             "complianceDeclarations": ProcessComplianceDeclarations,
             "geography": ProcessGeography,
             "modellingAndValidation": ProcessModellingAndValidation,
             "name": ProcessName,
             "publicationAndOwnership": ProcessPublicationAndOwnership,
@@ -201,14 +219,39 @@
         }
         try:
             return lookupMap[name]
         except KeyError:
             return _check_common_lookup(name)
 
 
+class FlowPropertyDatasetLookup(etree.CustomElementClassLookup):
+    """Custom XML lookup class for ILCD FlowPropertyDataset files."""
+
+    def lookup(
+        self, unused_node_type, unused_document, unused_namespace, name: str
+    ) -> type:
+        """Maps ILCD ProcessDataset XML elements to custom FlowDataset classes."""
+        lookupMap: Dict[str, type] = {
+            "administrativeInformation": FlowPropertyAdministrativeInformation,
+            "classificationInformation": ClassificationInformation,
+            "compliance": FlowPropertyCompliance,
+            "complianceDeclarations": FlowPropertyComplianceDeclarations,
+            "dataEntryBy": FlowPropertyDataEntryBy,
+            "dataSetInformation": FlowPropertyDataSetInformation,
+            "dataSourcesTreatmentAndRepresentativeness": FPDSTAR,
+            "modellingAndValidation": FlowPropertyModellingAndValidation,
+            "publicationAndOwnership": FlowPropertyPublicationAndOwnership,
+            "quantitativeReference": FlowPropertyQuantitativeReference,
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
@@ -225,14 +268,26 @@
     file: the str|Path path to the ILCD Flow Dataset XML file or its StringIO
     representation.
     Returns ``None`` if valid or a list of error strings.
     """
     return validate_file(file, Defaults.SCHEMA_FLOW_DATASET)
 
 
+def validate_file_flow_property_dataset(
+    file: Union[str, Path, StringIO]
+) -> Union[None, List[str]]:
+    """Validates an ILCD Flow Property Dataset XML file against schema.
+    Parameters:
+    file: the str|Path path to the ILCD Flow Property Dataset XML file or its StringIO
+    representation.
+    Returns ``None`` if valid or a list of error strings.
+    """
+    return validate_file(file, Defaults.SCHEMA_FLOW_PROPERTY_DATASET)
+
+
 def parse_file_process_dataset(file: Union[str, Path, StringIO]) -> ProcessDataSet:
     """Parses an ILCD Process Dataset XML file to custom ILCD classes.
     Parameters:
     file: the str|Path path to the ProcessDataset XML file or its StringIO
     representation.
     Returns a ProcessDataset class representing the root of the XML file.
     """
@@ -245,14 +300,28 @@
     file: the str|Path path to the Flow DataSet XML file or its StringIO
     representation.
     Returns a FlowDataSet class representing the root of the XML file.
     """
     return parse_file(file, Defaults.SCHEMA_FLOW_DATASET, FlowDatasetLookup())
 
 
+def parse_file_flow_property_dataset(
+    file: Union[str, Path, StringIO]
+) -> FlowPropertyDataSet:
+    """Parses an ILCD Flow Property DataSet XML file to custom ILCD classes.
+    Parameters:
+    file: the str|Path path to the Flow Property DataSet XML file or its StringIO
+    representation.
+    Returns a FlowPropertyDataSet class representing the root of the XML file.
+    """
+    return parse_file(
+        file, Defaults.SCHEMA_FLOW_PROPERTY_DATASET, FlowPropertyDatasetLookup()
+    )
+
+
 def parse_directory_process_dataset(
     dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
 ) -> List[Tuple[Path, ProcessDataSet]]:
     """Parses a directory of ILCD Process Dataset XML files to a list of
     custom ILCD classes.
     Parameters:
     dir_path: the directory path, should contain ILCD Process Dataset files.
@@ -291,14 +360,37 @@
         dir_path=dir_path,
         schema_path=Defaults.SCHEMA_FLOW_DATASET,
         lookup=FlowDataSet(),
         valid_suffixes=valid_suffixes,
     )
 
 
+def parse_directory_flow_property_dataset(
+    dir_path: Union[str, Path], valid_suffixes: Union[List[str], None] = None
+) -> List[Tuple[Path, FlowPropertyDataSet]]:
+    """Parses a directory of ILCD Flow Property Dataset XML files to a list of
+    custom ILCD classes.
+    Parameters:
+    dir_path: the directory path, should contain ILCD Flow Property Dataset files.
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
+        schema_path=Defaults.SCHEMA_FLOW_PROPERTY_DATASET,
+        lookup=FlowPropertyDataSet(),
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

### Comparing `pyilcd-2.0.0/pyilcd/flow_dataset.py` & `pyilcd-3.0.0/pyilcd/flow_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/helpers.py` & `pyilcd-3.0.0/pyilcd/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,24 @@
     name: str, attr_type: type, validator: Optional[Callable] = None
 ) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Flow Dataset attribute"""
     return create_attribute(name, attr_type, Defaults.SCHEMA_FLOW_DATASET, validator)
 
 
+def create_attribute_flow_property_dataset(
+    name: str, attr_type: type, validator: Optional[Callable] = None
+) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Flow Property Dataset attribute"""
+    return create_attribute(
+        name, attr_type, Defaults.SCHEMA_FLOW_PROPERTY_DATASET, validator
+    )
+
+
 def create_element_text_process_dataset(name: str, element_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Process Dataset element text"""
     return create_element_text(name, element_type, Defaults.SCHEMA_PROCESS_DATASET)
 
 
 def create_element_text_flow_dataset(name: str, element_type: type) -> property:
@@ -40,7 +50,13 @@
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_PROCESS_DATASET)
 
 
 def create_attribute_list_flow_dataset(name: str, attr_type: type) -> property:
     """Helper wrapper method for creating setters and getters for an ilcd
     Flow Dataset element text list"""
     return create_attribute_list(name, attr_type, Defaults.SCHEMA_FLOW_DATASET)
+
+
+def create_attribute_list_flow_property_dataset(name: str, attr_type: type) -> property:
+    """Helper wrapper method for creating setters and getters for an ilcd
+    Flow Property Dataset element text list"""
+    return create_attribute_list(name, attr_type, Defaults.SCHEMA_FLOW_PROPERTY_DATASET)
```

### Comparing `pyilcd-2.0.0/pyilcd/process_dataset.py` & `pyilcd-3.0.0/pyilcd/process_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Categories.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Categories.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_EnumerationValues.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_Groups.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Common_Validation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_ContactDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Documentation.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Documentation.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_FlowDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_FlowPropertyDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_ILCD.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_ILCD.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_LCIAMethodDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_LCIAMethodologies.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_Locations.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_Locations.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_ProcessDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_SourceDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd` & `pyilcd-3.0.0/pyilcd/schemas/ILCD_UnitGroupDataSet.xsd`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/pyilcd.egg-info/PKG-INFO` & `pyilcd-3.0.0/pyilcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilcd
-Version: 2.0.0
+Version: 3.0.0
 Summary: A Python package that converts ILCD XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyilcd
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: GPL-3.0
```

### Comparing `pyilcd-2.0.0/pyilcd.egg-info/SOURCES.txt` & `pyilcd-3.0.0/pyilcd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 ./docs/conf.py
 ./pyilcd/__init__.py
 ./pyilcd/common.py
 ./pyilcd/config.py
 ./pyilcd/core.py
 ./pyilcd/flow_dataset.py
+./pyilcd/flow_property_dataset.py
 ./pyilcd/helpers.py
 ./pyilcd/process_dataset.py
 ./pyilcd/utils.py
 pyilcd/VERSION
 pyilcd.egg-info/PKG-INFO
 pyilcd.egg-info/SOURCES.txt
 pyilcd.egg-info/dependency_links.txt
@@ -35,8 +36,9 @@
 pyilcd/schemas/ILCD_ProcessDataSet.xsd
 pyilcd/schemas/ILCD_SourceDataSet.xsd
 pyilcd/schemas/ILCD_UnitGroupDataSet.xsd
 tests/test_common.py
 tests/test_config.py
 tests/test_core.py
 tests/test_flow_dataset.py
+tests/test_flow_propert_dataset.py
 tests/test_process_dataset.py
```

### Comparing `pyilcd-2.0.0/setup.cfg` & `pyilcd-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/tests/test_common.py` & `pyilcd-3.0.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/tests/test_config.py` & `pyilcd-3.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/tests/test_core.py` & `pyilcd-3.0.0/tests/test_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Test cases for the __core__ module."""
 import os
 import tempfile
 from io import StringIO
+from pathlib import Path
+from typing import Callable, List, Union
 
 import pytest
 
 from pyilcd.core import (
     _check_common_lookup,
     parse_file_process_dataset,
     save_ilcd_file,
     validate_file_flow_dataset,
+    validate_file_flow_property_dataset,
     validate_file_process_dataset,
 )
 
 
 def test_check_common_lookup() -> None:
     """It validates file successfully."""
     with pytest.raises(KeyError):
@@ -26,36 +29,45 @@
 
 
 def test_validate_file_flow_dataset_success() -> None:
     """It validates file successfully."""
     assert validate_file_flow_dataset("data/sample_flow.xml") is None
 
 
-def test_validate_file_process_dataset_fail() -> None:
+def test_validate_file_flow_property_dataset_success() -> None:
     """It validates file successfully."""
+    assert validate_file_flow_property_dataset("data/sample_flowproperty.xml") is None
+
+
+def _validate_file_fail(
+    validator: Callable[[Union[str, Path, StringIO]], Union[None, List[str]]]
+) -> None:
     xml = StringIO("<ilcd></ilcd>")
     errorExpected = (
         "<string>:1:0:ERROR:SCHEMASV:SCHEMAV_CVC_ELT_1: Element 'ilcd': "
         "No matching global declaration available for the validation root."
     )
-    errorActual = validate_file_process_dataset(xml)
+    errorActual = validator(xml)
     assert errorActual is not None
     assert str(errorActual[0]) == errorExpected
 
 
+def test_validate_file_process_dataset_fail() -> None:
+    """It validates file successfully."""
+    _validate_file_fail(validate_file_process_dataset)
+
+
 def test_validate_file_flow_dataset_fail() -> None:
     """It validates file successfully."""
-    xml = StringIO("<ilcd></ilcd>")
-    errorExpected = (
-        "<string>:1:0:ERROR:SCHEMASV:SCHEMAV_CVC_ELT_1: Element 'ilcd': "
-        "No matching global declaration available for the validation root."
-    )
-    errorActual = validate_file_flow_dataset(xml)
-    assert errorActual is not None
-    assert str(errorActual[0]) == errorExpected
+    _validate_file_fail(validate_file_flow_dataset)
+
+
+def test_validate_file_flow_property_dataset_fail() -> None:
+    """It validates file successfully."""
+    _validate_file_fail(validate_file_flow_property_dataset)
 
 
 def test_save_ilcd_file() -> None:
     """It saves read file correctly."""
     inputPath = "data/sample_process.xml"
     processDataset = parse_file_process_dataset(inputPath)
     outputPath = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
```

### Comparing `pyilcd-2.0.0/tests/test_flow_dataset.py` & `pyilcd-3.0.0/tests/test_flow_dataset.py`

 * *Files identical despite different names*

### Comparing `pyilcd-2.0.0/tests/test_process_dataset.py` & `pyilcd-3.0.0/tests/test_process_dataset.py`

 * *Files identical despite different names*

