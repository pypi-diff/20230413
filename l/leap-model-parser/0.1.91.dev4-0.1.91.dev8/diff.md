# Comparing `tmp/leap_model_parser-0.1.91.dev4.tar.gz` & `tmp/leap_model_parser-0.1.91.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.91.dev4.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.91.dev8.tar", max compression
```

## Comparing `leap_model_parser-0.1.91.dev4.tar` & `leap_model_parser-0.1.91.dev8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43326 2023-04-10 08:45:01.664324 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   415723 2023-04-10 08:45:01.664324 leap_model_parser-0.1.91.dev4/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-04-10 08:45:01.660324 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1062 2023-04-10 08:45:01.656324 leap_model_parser-0.1.91.dev4/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-04-13 14:41:50.222916 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   416303 2023-04-13 14:41:50.222916 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-04-13 14:41:50.214917 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     6768 2023-04-13 14:41:50.226917 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1062 2023-04-13 14:41:50.210917 leap_model_parser-0.1.91.dev8/pyproject.toml
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev8/PKG-INFO
```

### Comparing `leap_model_parser-0.1.91.dev4/LICENSE` & `leap_model_parser-0.1.91.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/nodedata.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import Union
+from enum import Enum
 from typing import List
 from dataclasses import dataclass
-from enum import Enum
-from typing import Union
 
 
 class ActivationsEnum(Enum):
     relu = "relu"
     softmax = "softmax"
     selu = "selu"
     softplus = "softplus"
```

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999455337690633%*

 * *Differences: {'135': "{'inputs_data': {'inputs': {insert: [(1, OrderedDict([('name', 'initial_h_state'), "*

 * *        "('approval_connection', ['Input', 'Dataset', 'Layer', 'CustomLayer'])])), (2, "*

 * *        "OrderedDict([('name', 'initial_c_state'), ('approval_connection', ['Input', 'Dataset', "*

 * *        "'Layer', 'CustomLayer'])]))]}}}"}*

```diff
@@ -14570,14 +14570,32 @@
                     "approval_connection": [
                         "Input",
                         "Dataset",
                         "Layer",
                         "CustomLayer"
                     ],
                     "name": "input"
+                },
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "initial_h_state"
+                },
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "initial_c_state"
                 }
             ]
         },
         "menu_sections": [
             "Layer",
             "Onnx"
         ],
```

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
-from typing import List, Optional
+from typing import List, Optional, Callable, Any
 
 import yaml
 from leap_model_parser.utils.layerpedia.layerpedia import Layerpedia
 from leap_model_parser.utils.tlinspection.leapinspection import LeapInspect
+from copy import deepcopy
 
 
 class TensorFlowInspection(LeapInspect):
 
     def __init__(self):
         file_path = os.path.dirname(os.path.abspath(__file__))
         with open(f'{file_path}/ui_components_config.yaml') as f:
@@ -51,14 +52,32 @@
                     arg['default_val'] = override_def
             _args.append(arg)
         return _args
 
     def filter_node(self, node):
         return node['name'] in self.ignores['clsignore']
 
+    def get_filled_group_values(self, node_type: str, class_pointer: Callable[..., Any]) -> dict:
+        if node_type == 'customonnxlayer':
+            var_names = class_pointer.__dict__['call'].__code__.co_varnames
+            arg_names = var_names[1:class_pointer.__dict__['call'].__code__.co_argcount]  # remove self
+            if len(arg_names) == 1:
+                return self.group_type[node_type]
+            else:
+                config_dict = deepcopy(self.group_type[node_type])
+                inputs_list = config_dict['inputs_data']['inputs']
+                for arg in arg_names[1:]:
+                    inputs_list.append(
+                        {'name': f'{arg}',
+                         'approval_connection': ['Input', 'Dataset', 'Layer', 'CustomLayer']}
+                    )
+                return config_dict
+        else:
+            return self.group_type[node_type]
+
     def inspect_lib(self, lib):
         # TODO: extract only classes and not aliases
         classes = LeapInspect.get_classes(lib, self.ignores['lib_ignore'])
         nodes = []
         for node_cls in classes:
             if self.filter_node(node_cls):
                 continue
@@ -74,15 +93,15 @@
             enable_bigger_input_rank = self.query_layerpedia_enable_bigger_input_rank(
                 node_cls['name'])
             if enable_bigger_input_rank:
                 node['enable_bigger_input_rank'] = enable_bigger_input_rank
             template_node = {}
             for d in [*node_cls['parents'], node['name']]:
                 if d in self.group_type:
-                    template_node = {**template_node, **self.group_type[d]}
+                    template_node = {**template_node, **self.get_filled_group_values(d, node_cls['class'])}
             node = {**template_node, **node}
             if 'hash' in node and not self.query_layerpedia_is_trainable(node_cls['name']):
                 node.pop('hash')
             nodes.append(node)
         return nodes
 
     def inspect(self, dist: str) -> List[dict]:
```

### Comparing `leap_model_parser-0.1.91.dev4/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev4/pyproject.toml` & `leap_model_parser-0.1.91.dev8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.91.dev4"
+version = "0.1.91.dev8"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.82.dev7"
+onnx2kerastl = "0.0.82.dev8"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.91.dev4/PKG-INFO` & `leap_model_parser-0.1.91.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.91.dev4
+Version: 0.1.91.dev8
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.82.dev7)
+Requires-Dist: onnx2kerastl (==0.0.82.dev8)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

