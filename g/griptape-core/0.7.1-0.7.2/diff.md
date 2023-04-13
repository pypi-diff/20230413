# Comparing `tmp/griptape_core-0.7.1.tar.gz` & `tmp/griptape_core-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.7.1.tar", max compression
+gzip compressed data, was "griptape_core-0.7.2.tar", max compression
```

## Comparing `griptape_core-0.7.1.tar` & `griptape_core-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.7.1/LICENSE
--rw-r--r--   0        0        0     2822 2023-04-13 18:09:31.695590 griptape_core-0.7.1/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.7.1/griptape/__init__.py
--rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.7.1/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.7.1/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2559 2023-04-13 20:46:18.463809 griptape_core-0.7.1/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0      999 2023-04-13 18:09:31.698425 griptape_core-0.7.1/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.7.1/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.7.1/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3735 2023-04-12 21:11:39.051228 griptape_core-0.7.1/griptape/core/base_tool.py
--rw-r--r--   0        0        0      535 2023-04-12 21:11:39.052977 griptape_core-0.7.1/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.7.1/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.7.1/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.7.1/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.7.1/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.7.1/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.7.1/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.7.1/griptape/core/utils/command_runner.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.7.1/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.7.1/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.7.1/griptape/core/utils/python_runner.py
--rw-r--r--   0        0        0      708 2023-04-13 20:46:57.281099 griptape_core-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 griptape_core-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2822 2023-04-13 18:09:31.695590 griptape_core-0.7.2/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.7.2/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.7.2/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.7.2/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-13 20:46:18.463809 griptape_core-0.7.2/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0      999 2023-04-13 18:09:31.698425 griptape_core-0.7.2/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.7.2/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.7.2/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3898 2023-04-13 21:51:40.434409 griptape_core-0.7.2/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      535 2023-04-12 21:11:39.052977 griptape_core-0.7.2/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.7.2/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.7.2/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.7.2/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.7.2/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.7.2/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.7.2/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.7.2/griptape/core/utils/command_runner.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.7.2/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.7.2/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.7.2/griptape/core/utils/python_runner.py
+-rw-r--r--   0        0        0      708 2023-04-13 21:54:09.141611 griptape_core-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 griptape_core-0.7.2/PKG-INFO
```

### Comparing `griptape_core-0.7.1/LICENSE` & `griptape_core-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/README.md` & `griptape_core-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.7.2/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.7.2/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/base_tool.py` & `griptape_core-0.7.2/griptape/core/base_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import inspect
 import json
+import logging
 import os
 from abc import ABC
 from typing import Optional
 import yaml
 from attr import define, fields, Attribute
 from jinja2 import Template
 
 
 @define
 class BaseTool(ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
     REQUIREMENTS_FILE = "requirements.txt"
 
+    # Disable logging, unless it's an error, so that executors don't capture it as subprocess output.
+    logging.basicConfig(level=logging.ERROR)
+
     @property
     def name(self) -> str:
         return self.__class__.__name__
 
     @property
     def env_fields(self) -> list[Attribute]:
         return [f for f in fields(self.__class__) if f.metadata.get("env")]
```

### Comparing `griptape_core-0.7.1/griptape/core/decorators.py` & `griptape_core-0.7.2/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/executors/docker_executor.py` & `griptape_core-0.7.2/griptape/core/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/executors/local_executor.py` & `griptape_core-0.7.2/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/utils/j2.py` & `griptape_core-0.7.2/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/griptape/core/utils/python_runner.py` & `griptape_core-0.7.2/griptape/core/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.7.1/pyproject.toml` & `griptape_core-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.7.1"
+version = "0.7.2"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.7.1/PKG-INFO` & `griptape_core-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

