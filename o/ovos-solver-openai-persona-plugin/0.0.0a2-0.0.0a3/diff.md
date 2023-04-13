# Comparing `tmp/ovos-solver-openai-persona-plugin-0.0.0a2.tar.gz` & `tmp/ovos-solver-openai-persona-plugin-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-solver-openai-persona-plugin-0.0.0a2.tar", last modified: Thu Apr 13 20:17:30 2023, max compression
+gzip compressed data, was "ovos-solver-openai-persona-plugin-0.0.0a3.tar", last modified: Thu Apr 13 21:59:59 2023, max compression
```

## Comparing `ovos-solver-openai-persona-plugin-0.0.0a2.tar` & `ovos-solver-openai-persona-plugin-0.0.0a3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/engines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 20:17:25.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2333 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:59.512327 ovos-solver-openai-persona-plugin-0.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 21:59:59.512327 ovos-solver-openai-persona-plugin-0.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:59.512327 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 21:59:54.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:59.512327 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:59:59.000000 ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:59:59.512327 ovos-solver-openai-persona-plugin-0.0.0a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2333 2023-04-13 21:59:50.000000 ovos-solver-openai-persona-plugin-0.0.0a3/setup.py
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/LICENSE` & `ovos-solver-openai-persona-plugin-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/PKG-INFO` & `ovos-solver-openai-persona-plugin-0.0.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-openai-persona-plugin
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A question solver plugin for ovos
 Home-page: https://github.com/OpenVoiceOS/ovos-solver-plugin-openai-persona
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Description: # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> OpenAI Persona
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/README.md` & `ovos-solver-openai-persona-plugin-0.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/__init__.py` & `ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/engines.py` & `ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/engines.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 
 import requests
-from neon_solvers import AbstractSolver
+from ovos_plugin_manager.templates.solvers import AbstractSolver
 
 
 class OpenAICompletionsSolver(AbstractSolver):
     api_url = "https://api.openai.com/v1/completions"
 
     def __init__(self, config=None, name="OpenAI"):
-        super().__init__(name=name, priority=25, config=config)
+        super().__init__(name=name, priority=25, config=config,
+                         enable_cache=False, enable_tx=False)
         self.engine = self.config.get("model", "text-davinci-002")  # "ada" cheaper and faster, "davinci" better
         self.stop_token = "<|im_end|>"
         self.key = self.config.get("key")  # TODO - raise error if missing
 
     # OpenAI API integration
     def _do_api_request(self, prompt):
         headers = {
@@ -49,15 +50,16 @@
         return answer
 
 
 class OpenAIChatCompletionsSolver(AbstractSolver):
     api_url = "https://api.openai.com/v1/chat/completions"
 
     def __init__(self, config=None, name="OpenAI Chat"):
-        super().__init__(name=name, priority=25, config=config)
+        super().__init__(name=name, priority=25, config=config,
+                         enable_cache=False, enable_tx=False)
         self.engine = self.config.get("model", "gpt-3.5-turbo")  # "ada" cheaper and faster, "davinci" better
         self.stop_token = "<|im_end|>"
         self.key = self.config.get("key")  # TODO - raise error if missing
         self.memory = config.get("enable_memory", True)
         self.max_utts = config.get("memory_size", 15)
         self.qa_pairs = []  # tuple of q+a
         self.current_q = None
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/prompts.py` & `ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona/prompts.py`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO` & `ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-solver-openai-persona-plugin
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A question solver plugin for ovos
 Home-page: https://github.com/OpenVoiceOS/ovos-solver-plugin-openai-persona
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
 Description: # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> OpenAI Persona
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt` & `ovos-solver-openai-persona-plugin-0.0.0a3/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a2/setup.py` & `ovos-solver-openai-persona-plugin-0.0.0a3/setup.py`

 * *Files identical despite different names*

