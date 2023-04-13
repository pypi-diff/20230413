# Comparing `tmp/griptape_core-0.6.0.tar.gz` & `tmp/griptape_core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.6.0.tar", max compression
+gzip compressed data, was "griptape_core-0.7.0.tar", max compression
```

## Comparing `griptape_core-0.6.0.tar` & `griptape_core-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.6.0/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.6.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.6.0/griptape/__init__.py
--rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.6.0/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.6.0/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-12 20:48:35.984034 griptape_core-0.6.0/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1006 2023-04-12 20:48:35.986046 griptape_core-0.6.0/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.6.0/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.6.0/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3735 2023-04-12 21:11:39.051228 griptape_core-0.6.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      535 2023-04-12 21:11:39.052977 griptape_core-0.6.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.6.0/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.6.0/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.6.0/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.6.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.6.0/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.6.0/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.6.0/griptape/core/utils/command_runner.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.6.0/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.6.0/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.6.0/griptape/core/utils/python_runner.py
--rw-r--r--   0        0        0      708 2023-04-13 16:40:01.308697 griptape_core-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2822 2023-04-13 18:09:31.695590 griptape_core-0.7.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.7.0/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.7.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.7.0/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-12 20:48:35.984034 griptape_core-0.7.0/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0      999 2023-04-13 18:09:31.698425 griptape_core-0.7.0/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.7.0/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.7.0/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3735 2023-04-12 21:11:39.051228 griptape_core-0.7.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      535 2023-04-12 21:11:39.052977 griptape_core-0.7.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.7.0/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.7.0/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.7.0/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.7.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.7.0/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.7.0/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.7.0/griptape/core/utils/command_runner.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.7.0/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.7.0/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.7.0/griptape/core/utils/python_runner.py
+-rw-r--r--   0        0        0      708 2023-04-13 18:10:10.882783 griptape_core-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 griptape_core-0.7.0/PKG-INFO
```

### Comparing `griptape_core-0.6.0/LICENSE` & `griptape_core-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/README.md` & `griptape_core-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 ```
 
 Convert tool actions into LangChain tools:
 
 ```python
 agent = initialize_agent(
     [
-        LangchainToolAdapter(executor=tool_executor).generate(google_search.search),
-        LangchainToolAdapter(executor=tool_executor).generate(calculator.calculate)
+        LangchainToolAdapter(executor=tool_executor).generate_tool(google_search.search),
+        LangchainToolAdapter(executor=tool_executor).generate_tool(calculator.calculate)
     ],
     OpenAI(temperature=0.5, model_name="text-davinci-003"),
     agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION,
     verbose=True
 )
 
 agent.run("What is 42^42?")
```

### Comparing `griptape_core-0.6.0/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.7.0/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.7.0/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import json
 import langchain.tools
 from attr import define
 from griptape.core import BaseAdapter
 
 
 @define
 class LangchainToolAdapter(BaseAdapter):
-    def generate(self, tool_action: callable) -> langchain.tools.BaseTool:
+    def generate_tool(self, tool_action: callable) -> langchain.tools.BaseTool:
         tool = tool_action.__self__
 
         # Double up curly brackets for correct f-string parsing in LangChain prompt templates.
         description = tool.action_description(tool_action).replace("{", "{{").replace("}", "}}")
 
         def _run(_self, value: str) -> str:
             return self.executor.execute(tool_action, value.encode()).decode()
```

### Comparing `griptape_core-0.6.0/griptape/core/base_tool.py` & `griptape_core-0.7.0/griptape/core/base_tool.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/decorators.py` & `griptape_core-0.7.0/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/executors/docker_executor.py` & `griptape_core-0.7.0/griptape/core/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/executors/local_executor.py` & `griptape_core-0.7.0/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/utils/j2.py` & `griptape_core-0.7.0/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/griptape/core/utils/python_runner.py` & `griptape_core-0.7.0/griptape/core/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.6.0/pyproject.toml` & `griptape_core-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.6.0/PKG-INFO` & `griptape_core-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -76,16 +76,16 @@
 ```
 
 Convert tool actions into LangChain tools:
 
 ```python
 agent = initialize_agent(
     [
-        LangchainToolAdapter(executor=tool_executor).generate(google_search.search),
-        LangchainToolAdapter(executor=tool_executor).generate(calculator.calculate)
+        LangchainToolAdapter(executor=tool_executor).generate_tool(google_search.search),
+        LangchainToolAdapter(executor=tool_executor).generate_tool(calculator.calculate)
     ],
     OpenAI(temperature=0.5, model_name="text-davinci-003"),
     agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION,
     verbose=True
 )
 
 agent.run("What is 42^42?")
```

