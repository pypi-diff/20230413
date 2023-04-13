# Comparing `tmp/utbot_executor-1.5.5.tar.gz` & `tmp/utbot_executor-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utbot_executor-1.5.5.tar", max compression
+gzip compressed data, was "utbot_executor-1.5.6.tar", max compression
```

## Comparing `utbot_executor-1.5.5.tar` & `utbot_executor-1.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.5/LICENSE
--rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.5/README.md
--rw-r--r--   0        0        0      419 2023-04-13 10:36:34.468611 utbot_executor-1.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.5/utbot_executor/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.5/utbot_executor/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.5/utbot_executor/deep_serialization/__init__.py
--rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.5/utbot_executor/deep_serialization/deep_serialization.py
--rw-r--r--   0        0        0     1528 2023-04-10 14:27:35.374234 utbot_executor-1.5.5/utbot_executor/deep_serialization/example.py
--rw-r--r--   0        0        0     8848 2023-04-10 15:10:05.485066 utbot_executor-1.5.5/utbot_executor/deep_serialization/json_converter.py
--rw-r--r--   0        0        0    10449 2023-04-13 10:36:34.448609 utbot_executor-1.5.5/utbot_executor/deep_serialization/memory_objects.py
--rw-r--r--   0        0        0      510 2023-04-13 10:36:34.461944 utbot_executor-1.5.5/utbot_executor/deep_serialization/numpy_serialization.py
--rw-r--r--   0        0        0     5445 2023-04-10 14:28:17.024941 utbot_executor-1.5.5/utbot_executor/deep_serialization/test_json.json
--rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.5/utbot_executor/deep_serialization/utils.py
--rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.5/utbot_executor/executor.py
--rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.5/utbot_executor/listener.py
--rw-r--r--   0        0        0      873 2023-04-10 14:43:37.877093 utbot_executor-1.5.5/utbot_executor/memory_compressor.py
--rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.5/utbot_executor/parser.py
--rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.5/utbot_executor/utils.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 utbot_executor-1.5.5/setup.py
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 utbot_executor-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-10-03 19:39:38.276000 utbot_executor-1.5.6/LICENSE
+-rw-r--r--   0        0        0     1058 2023-02-27 11:20:59.630921 utbot_executor-1.5.6/README.md
+-rw-r--r--   0        0        0      419 2023-04-13 10:48:54.758209 utbot_executor-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 06:22:44.305237 utbot_executor-1.5.6/utbot_executor/__init__.py
+-rw-r--r--   0        0        0     1039 2023-03-27 09:02:56.888080 utbot_executor-1.5.6/utbot_executor/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-21 06:50:17.028607 utbot_executor-1.5.6/utbot_executor/deep_serialization/__init__.py
+-rw-r--r--   0        0        0     2090 2023-03-30 13:06:09.660414 utbot_executor-1.5.6/utbot_executor/deep_serialization/deep_serialization.py
+-rw-r--r--   0        0        0     1528 2023-04-10 14:27:35.374234 utbot_executor-1.5.6/utbot_executor/deep_serialization/example.py
+-rw-r--r--   0        0        0     8848 2023-04-10 15:10:05.485066 utbot_executor-1.5.6/utbot_executor/deep_serialization/json_converter.py
+-rw-r--r--   0        0        0    10449 2023-04-13 10:36:34.448609 utbot_executor-1.5.6/utbot_executor/deep_serialization/memory_objects.py
+-rw-r--r--   0        0        0      367 2023-04-13 10:48:54.744876 utbot_executor-1.5.6/utbot_executor/deep_serialization/numpy_serialization.py
+-rw-r--r--   0        0        0     5445 2023-04-10 14:28:17.024941 utbot_executor-1.5.6/utbot_executor/deep_serialization/test_json.json
+-rw-r--r--   0        0        0     3871 2023-04-10 11:32:19.241414 utbot_executor-1.5.6/utbot_executor/deep_serialization/utils.py
+-rw-r--r--   0        0        0     7975 2023-03-30 13:06:09.677079 utbot_executor-1.5.6/utbot_executor/executor.py
+-rw-r--r--   0        0        0     3192 2023-03-02 10:22:46.865281 utbot_executor-1.5.6/utbot_executor/listener.py
+-rw-r--r--   0        0        0      873 2023-04-10 14:43:37.877093 utbot_executor-1.5.6/utbot_executor/memory_compressor.py
+-rw-r--r--   0        0        0     2578 2023-03-30 11:31:56.739251 utbot_executor-1.5.6/utbot_executor/parser.py
+-rw-r--r--   0        0        0      288 2023-03-23 15:10:03.405564 utbot_executor-1.5.6/utbot_executor/utils.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 utbot_executor-1.5.6/setup.py
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 utbot_executor-1.5.6/PKG-INFO
```

### Comparing `utbot_executor-1.5.5/LICENSE` & `utbot_executor-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/README.md` & `utbot_executor-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/__main__.py` & `utbot_executor-1.5.6/utbot_executor/__main__.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/deep_serialization.py` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/deep_serialization.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/example.py` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/example.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/json_converter.py` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/json_converter.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/memory_objects.py` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/memory_objects.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/test_json.json` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/test_json.json`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/deep_serialization/utils.py` & `utbot_executor-1.5.6/utbot_executor/deep_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/executor.py` & `utbot_executor-1.5.6/utbot_executor/executor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/listener.py` & `utbot_executor-1.5.6/utbot_executor/listener.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/memory_compressor.py` & `utbot_executor-1.5.6/utbot_executor/memory_compressor.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/utbot_executor/parser.py` & `utbot_executor-1.5.6/utbot_executor/parser.py`

 * *Files identical despite different names*

### Comparing `utbot_executor-1.5.5/setup.py` & `utbot_executor-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utbot-executor = utbot_executor:utbot_executor']}
 
 setup_kwargs = {
     'name': 'utbot-executor',
-    'version': '1.5.5',
+    'version': '1.5.6',
     'description': '',
     'long_description': '# UtBot Executor\n\nUtil for python code execution and state serialization.\n\n## Installation\n\nYou can install module from [PyPI](https://pypi.org/project/utbot-executor/):\n\n```bash\npython -m pip install utbot-executor\n```\n\n## Usage\n\n### From console with socket listener\n\nRun with your `<hostname>` and `<port>` for socket connection\n```bash\n$ python -m utbot_executor <hostname> <port> <logfile> [<loglevel DEBUG | INFO | ERROR>]\n```\n\n### Result format:\n\n```json\n{\n        "status": "success",\n        "isException": bool,\n        "statements": list[int],\n        "missedStatements": list[int],\n        "stateBefore": memory json dump,\n        "stateAfter": memory json dump,\n        "argsIds": list[str],\n        "kwargs": list[str],\n        "resultId": str,\n}\n```\n\nor error format:\n\n```json\n{\n        "status": "fail",\n        "exception": str (traceback),\n}\n```\n\n#### States format\n\nTODO\n\n### Submodule `deep_serialization`\n\nJSON serializer and deserializer for python objects\n\n## Source\n\nGitHub [repository](https://github.com/tamarinvs19/utbot_executor)\n',
     'author': 'Vyacheslav Tamarin',
     'author_email': 'vyacheslav.tamarin@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `utbot_executor-1.5.5/PKG-INFO` & `utbot_executor-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utbot-executor
-Version: 1.5.5
+Version: 1.5.6
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: vyacheslav.tamarin@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

