# Comparing `tmp/grai_source_dbt-0.2.6.tar.gz` & `tmp/grai_source_dbt-0.2.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.2.6.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.2.6a0.tar", max compression
```

## Comparing `grai_source_dbt-0.2.6.tar` & `grai_source_dbt-0.2.6a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      735 2023-04-13 21:16:18.180891 grai_source_dbt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.6/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.6/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     5964 2023-04-10 15:35:17.408407 grai_source_dbt-0.2.6/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      531 2023-04-10 15:35:17.409417 grai_source_dbt-0.2.6/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.6/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.6/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.6/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.6/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     5493 2023-04-12 17:40:08.414555 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.6/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.6/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.6/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.6/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.6/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.6/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.6/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6/setup.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      741 2023-04-12 16:58:27.208366 grai_source_dbt-0.2.6a0/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.6a0/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     5964 2023-04-10 15:35:17.408407 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      531 2023-04-10 15:35:17.409417 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     5499 2023-04-12 16:56:50.880225 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.6a0/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.6a0/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/setup.py
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/PKG-INFO
```

### Comparing `grai_source_dbt-0.2.6/pyproject.toml` & `grai_source_dbt-0.2.6a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.2.6"
+version = "0.2.6-alpha"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
```

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/base.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ParsedSourceDefinition,
 )
 from grai_schemas.v1.metadata.edges import EdgeTypeLabels
 
 from grai_source_dbt.loaders.base import BaseManifestLoader
 from grai_source_dbt.models.grai import Column, Edge, EdgeTerminus
 from grai_source_dbt.models.shared import Constraint
-from grai_source_dbt.utils import full_name
+from grai_source_dbt.utils import full_name, set_extra_fields
 
 NodeTypes = Union[
     CompiledAnalysisNode,
     CompiledDataTestNode,
     CompiledModelNode,
     CompiledHookNode,
     CompiledRPCNode,
@@ -68,15 +68,15 @@
                     unique_id = (node_id, test.column_name)
                     col_to_tests.setdefault(unique_id, [])
                     col_to_tests[unique_id].append(test)
         return col_to_tests
 
     @cached_property
     def node_map(self) -> Dict[str, DBTNodeType]:
-        node_resource_types = {"model", "seed", "snapshot"}
+        node_resource_types = {"model", "seed"}
         node_map = {
             node_id: node for node_id, node in self.manifest.nodes.items() if node.resource_type in node_resource_types
         }
         return node_map
 
     @cached_property
     def columns(self) -> Dict[Tuple[str, str], ColumnType]:
```

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6/setup.py` & `grai_source_dbt-0.2.6a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['dbt-artifacts-parser>=0.2.4,<0.3.0',
  'grai-client>=0.2.0,<0.3.0',
  'grai-schemas>=0.1.10,<0.2.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-dbt',
-    'version': '0.2.6',
+    'version': '0.2.6a0',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_dbt-0.2.6/PKG-INFO` & `grai_source_dbt-0.2.6a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.2.6
+Version: 0.2.6a0
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

