# Comparing `tmp/utbot_executor-1.5.6.tar.gz` & `tmp/utbot_executor-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.5.6.tar", max compression
+gzip compressed data, was "utbot_executor-1.6.0.tar", max compression
```

## Comparing `utbot_executor-1.5.6.tar` & `utbot_executor-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.6/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.6/README.md
--rw-r--r--   0        0        0      419 2023-04-13 10:48:54.758209 utbot_executor-1.5.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.6/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.6/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.6/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.6/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1528 2023-04-10 14:27:35.374234 utbot_executor-1.5.6/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8848 2023-04-10 15:10:05.485066 utbot_executor-1.5.6/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0    10449 2023-04-13 10:36:34.448609 utbot_executor-1.5.6/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0      367 2023-04-13 10:48:54.744876 utbot_executor-1.5.6/utbot_executor/deep_serialization/numpy_serialization.py
--rw-r--r--   0        0        0     5445 2023-04-10 14:28:17.024941 utbot_executor-1.5.6/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.6/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.6/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.6/utbot_executor/listener.py
--rw-r--r--   0        0        0      873 2023-04-10 14:43:37.877093 utbot_executor-1.5.6/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.6/utbot_executor/parser.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.6/utbot_executor/utils.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 utbot_executor-1.5.6/setup.py
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 utbot_executor-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.6.0/README.md
+-rw-r--r--   0        0        0      401 2023-04-13 11:07:17.985828 utbot_executor-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.6.0/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.6.0/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.6.0/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.6.0/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1469 2023-04-13 11:03:00.871191 utbot_executor-1.6.0/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8848 2023-04-13 11:04:25.397297 utbot_executor-1.6.0/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0    10449 2023-04-13 11:04:25.397297 utbot_executor-1.6.0/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0      413 2023-04-13 11:10:20.054988 utbot_executor-1.6.0/utbot_executor/deep_serialization/numpy_serialization.py
+-rw-r--r--   0        0        0     5445 2023-04-13 11:04:25.397297 utbot_executor-1.6.0/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-04-13 11:04:25.397297 utbot_executor-1.6.0/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.6.0/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.6.0/utbot_executor/listener.py
+-rw-r--r--   0        0        0      873 2023-04-13 11:04:25.397297 utbot_executor-1.6.0/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.6.0/utbot_executor/parser.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.6.0/utbot_executor/utils.py
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 utbot_executor-1.6.0/setup.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 utbot_executor-1.6.0/PKG-INFO
```

### Comparing `utbot_executor-1.5.6/LICENSE` & `utbot_executor-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/README.md` & `utbot_executor-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/__main__.py` & `utbot_executor-1.6.0/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import datetime
 import json
 from pprint import pprint
 
-import numpy as numpy
-
 from utbot_executor.deep_serialization.memory_objects import PythonSerializer
 from utbot_executor.deep_serialization.json_converter import MemoryDumpEncoder
 from utbot_executor.deep_serialization.deep_serialization import deserialize_objects
 
 
 class B:
     def __init__(self, b1, b2, b3):
@@ -29,19 +27,18 @@
 def run():
     from pprint import pprint
 
     # c = ["Alex"]
     # b = B(1, 2, 3)
     # b.b1 = B(4, 5, b)
     # a = [1, 2, float('inf'), "abc", {1: 1}, None, b, c]
-    # x = Node("x")
-    # y = Node("y")
-    # x.children.append(y)
-    # y.children.append(x)
-    x = numpy.array([101])
+    x = Node("x")
+    y = Node("y")
+    x.children.append(y)
+    y.children.append(x)
     serializer_ = PythonSerializer()
     pprint(serializer_.write_object_to_memory(x))
     pprint(serializer_.memory.objects)
     with open('test_json.json', 'w') as fout:
         print(json.dumps({'objects': serializer_.memory}, cls=MemoryDumpEncoder, indent=True), file=fout)
 
 
@@ -49,13 +46,13 @@
     # run()
     with open('test_json.json', 'r') as fin:
         data = fin.read()
     print(data)
     pprint(deserialize_objects(["140340324106560"], data, [
         'copyreg',
         'utbot_executor.deep_serialization.example',
-        'datetime',
+        'datetime'
     ]))
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/memory_objects.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/test_json.json` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/test_json.json`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.6.0/utbot_executor/deep_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/executor.py` & `utbot_executor-1.6.0/utbot_executor/executor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/listener.py` & `utbot_executor-1.6.0/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/memory_compressor.py` & `utbot_executor-1.6.0/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/utbot_executor/parser.py` & `utbot_executor-1.6.0/utbot_executor/parser.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.6/setup.py` & `utbot_executor-1.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,32 +3,28 @@
 
 packages = \
 ['utbot_executor', 'utbot_executor.deep_serialization']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['numpy>=1.24.2,<2.0.0']
-
 entry_points = \
 {'console_scripts': ['utbot-executor = utbot_executor:utbot_executor']}
 
 setup_kwargs = {
     'name': 'utbot-executor',
-    'version': '1.5.6',
+    'version': '1.6.0',
     'description': '',
     'long_description': '# UtBot Executor\n\nUtil for python code execution and state serialization.\n\n## Installation\n\nYou can install module from [PyPI](https://pypi.org/project/utbot-executor/):\n\n```bash\npython -m pip install utbot-executor\n```\n\n## Usage\n\n### From console with socket listener\n\nRun with your `<hostname>` and `<port>` for socket connection\n```bash\n$ python -m utbot_executor <hostname> <port> <logfile> [<loglevel DEBUG | INFO | ERROR>]\n```\n\n### Result format:\n\n```json\n{\n        "status": "success",\n        "isException": bool,\n        "statements": list[int],\n        "missedStatements": list[int],\n        "stateBefore": memory json dump,\n        "stateAfter": memory json dump,\n        "argsIds": list[str],\n        "kwargs": list[str],\n        "resultId": str,\n}\n```\n\nor error format:\n\n```json\n{\n        "status": "fail",\n        "exception": str (traceback),\n}\n```\n\n#### States format\n\nTODO\n\n### Submodule `deep_serialization`\n\nJSON serializer and deserializer for python objects\n\n## Source\n\nGitHub [repository](https://github.com/tamarinvs19/utbot_executor)\n',
     'author': 'Vyacheslav Tamarin',
     'author_email': 'vyacheslav.tamarin@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `utbot_executor-1.5.6/PKG-INFO` & `utbot_executor-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.5.6
+Version: 1.6.0
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # UtBot Executor
 
 Util for python code execution and state serialization.
 
 ## Installation
```

