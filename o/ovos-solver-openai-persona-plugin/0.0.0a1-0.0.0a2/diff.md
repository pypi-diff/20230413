# Comparing `tmp/ovos-solver-openai-persona-plugin-0.0.0a1.tar.gz` & `tmp/ovos-solver-openai-persona-plugin-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-solver-openai-persona-plugin-0.0.0a1.tar", last modified: Mon Mar 20 02:48:01 2023, max compression
+gzip compressed data, was "ovos-solver-openai-persona-plugin-0.0.0a2.tar", last modified: Thu Apr 13 20:17:30 2023, max compression
```

## Comparing `ovos-solver-openai-persona-plugin-0.0.0a1.tar` & `ovos-solver-openai-persona-plugin-0.0.0a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:48:01.196030 ovos-solver-openai-persona-plugin-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-20 02:48:01.196030 ovos-solver-openai-persona-plugin-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:48:01.192030 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/engines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-20 02:47:55.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:48:01.192030 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-20 02:48:01.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 02:48:00.000000 ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 02:48:01.196030 ovos-solver-openai-persona-plugin-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2333 2023-03-20 02:47:52.000000 ovos-solver-openai-persona-plugin-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 20:17:25.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:17:30.000000 ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:17:30.289983 ovos-solver-openai-persona-plugin-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2333 2023-04-13 20:17:23.000000 ovos-solver-openai-persona-plugin-0.0.0a2/setup.py
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/LICENSE` & `ovos-solver-openai-persona-plugin-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/PKG-INFO` & `ovos-solver-openai-persona-plugin-0.0.0a2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ovos-solver-openai-persona-plugin
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A question solver plugin for ovos
 Home-page: https://github.com/OpenVoiceOS/ovos-solver-plugin-openai-persona
 Author: jarbasai
 Author-email: jarbasai@mailfence.com
 License: MIT
-Description: # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> Persona
+Description: # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> OpenAI Persona
          
         Give OpenVoiceOS some sass with OpenAI!
         
         Leverages [OpenAI Completions API](https://platform.openai.com/docs/api-reference/completions/create) to create some fun interactions.  Phrases not explicitly handled by other skills will be run by a LLM, so nearly every interaction will have _some_ response.  But be warned, Mycroft might become a bit obnoxious...
         
         
         ## Usage
@@ -25,15 +25,10 @@
         print(bot.get_spoken_answer("describe quantum mechanics in simple terms"))
         # Quantum mechanics is a branch of physics that deals with the behavior of particles on a very small scale, such as atoms and subatomic particles. It explores the idea that particles can exist in multiple states at once and that their behavior is not predictable in the traditional sense.
         print(bot.spoken_answer("Quem encontrou o caminho maritimo para o Brazil", {"lang": "pt-pt"}))
         # Explorador português Pedro Álvares Cabral é creditado com a descoberta do Brasil em 1500
         
         ```
         
-        ## Inspiration
-        
-        MycroftAI wanted to start an initiative called ‘Persona’ - a tool to help build distinct personalities for Mycroft. Think Sassy Mycroft, Polite Mycroft and so on.
-        
-        the technology just wasn't there yet and the [backend implementation](https://mycroft.ai/blog/mycrofts-goals-for-19-08/#back-end-persona) was never finished or made public but the beta skill is still available (non-functional) https://github.com/MycroftAI/skill-fallback-persona
 Keywords: ovos plugin utterance fallback query
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/README.md` & `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-# <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> Persona
- 
-Give OpenVoiceOS some sass with OpenAI!
-
-Leverages [OpenAI Completions API](https://platform.openai.com/docs/api-reference/completions/create) to create some fun interactions.  Phrases not explicitly handled by other skills will be run by a LLM, so nearly every interaction will have _some_ response.  But be warned, Mycroft might become a bit obnoxious...
-
-
-## Usage
-
-Spoken answers api with OpenAI completions backend, prompt engineering is used to behave like a voice assistant
-
-```python
-from ovos_solver_openai_persona import OpenAIPersonaSolver
-
-bot = OpenAIPersonaSolver({"key": "sk-XXX",
-                           "persona": "helpful, creative, clever, and very friendly"})
-print(bot.get_spoken_answer("describe quantum mechanics in simple terms"))
-# Quantum mechanics is a branch of physics that deals with the behavior of particles on a very small scale, such as atoms and subatomic particles. It explores the idea that particles can exist in multiple states at once and that their behavior is not predictable in the traditional sense.
-print(bot.spoken_answer("Quem encontrou o caminho maritimo para o Brazil", {"lang": "pt-pt"}))
-# Explorador português Pedro Álvares Cabral é creditado com a descoberta do Brasil em 1500
-
-```
-
-## Inspiration
-
-MycroftAI wanted to start an initiative called ‘Persona’ - a tool to help build distinct personalities for Mycroft. Think Sassy Mycroft, Polite Mycroft and so on.
-
-the technology just wasn't there yet and the [backend implementation](https://mycroft.ai/blog/mycrofts-goals-for-19-08/#back-end-persona) was never finished or made public but the beta skill is still available (non-functional) https://github.com/MycroftAI/skill-fallback-persona
+Metadata-Version: 2.1
+Name: ovos-solver-openai-persona-plugin
+Version: 0.0.0a2
+Summary: A question solver plugin for ovos
+Home-page: https://github.com/OpenVoiceOS/ovos-solver-plugin-openai-persona
+Author: jarbasai
+Author-email: jarbasai@mailfence.com
+License: MIT
+Description: # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> OpenAI Persona
+         
+        Give OpenVoiceOS some sass with OpenAI!
+        
+        Leverages [OpenAI Completions API](https://platform.openai.com/docs/api-reference/completions/create) to create some fun interactions.  Phrases not explicitly handled by other skills will be run by a LLM, so nearly every interaction will have _some_ response.  But be warned, Mycroft might become a bit obnoxious...
+        
+        
+        ## Usage
+        
+        Spoken answers api with OpenAI completions backend, prompt engineering is used to behave like a voice assistant
+        
+        ```python
+        from ovos_solver_openai_persona import OpenAIPersonaSolver
+        
+        bot = OpenAIPersonaSolver({"key": "sk-XXX",
+                                   "persona": "helpful, creative, clever, and very friendly"})
+        print(bot.get_spoken_answer("describe quantum mechanics in simple terms"))
+        # Quantum mechanics is a branch of physics that deals with the behavior of particles on a very small scale, such as atoms and subatomic particles. It explores the idea that particles can exist in multiple states at once and that their behavior is not predictable in the traditional sense.
+        print(bot.spoken_answer("Quem encontrou o caminho maritimo para o Brazil", {"lang": "pt-pt"}))
+        # Explorador português Pedro Álvares Cabral é creditado com a descoberta do Brasil em 1500
+        
+        ```
+        
+Keywords: ovos plugin utterance fallback query
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/__init__.py` & `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/engines.py` & `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/engines.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from neon_solvers import AbstractSolver
 
 
 class OpenAICompletionsSolver(AbstractSolver):
     api_url = "https://api.openai.com/v1/completions"
 
     def __init__(self, config=None, name="OpenAI"):
-        super().__init__(name=name, priority=25, config=config,
-                         enable_cache=False, enable_tx=False)
+        super().__init__(name=name, priority=25, config=config)
         self.engine = self.config.get("model", "text-davinci-002")  # "ada" cheaper and faster, "davinci" better
         self.stop_token = "<|im_end|>"
         self.key = self.config.get("key")  # TODO - raise error if missing
 
     # OpenAI API integration
     def _do_api_request(self, prompt):
         headers = {
@@ -50,16 +49,15 @@
         return answer
 
 
 class OpenAIChatCompletionsSolver(AbstractSolver):
     api_url = "https://api.openai.com/v1/chat/completions"
 
     def __init__(self, config=None, name="OpenAI Chat"):
-        super().__init__(name=name, priority=25, config=config,
-                         enable_cache=False, enable_tx=False)
+        super().__init__(name=name, priority=25, config=config)
         self.engine = self.config.get("model", "gpt-3.5-turbo")  # "ada" cheaper and faster, "davinci" better
         self.stop_token = "<|im_end|>"
         self.key = self.config.get("key")  # TODO - raise error if missing
         self.memory = config.get("enable_memory", True)
         self.max_utts = config.get("memory_size", 15)
         self.qa_pairs = []  # tuple of q+a
         self.current_q = None
```

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona/prompts.py` & `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona/prompts.py`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt` & `ovos-solver-openai-persona-plugin-0.0.0a2/ovos_solver_openai_persona_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-solver-openai-persona-plugin-0.0.0a1/setup.py` & `ovos-solver-openai-persona-plugin-0.0.0a2/setup.py`

 * *Files identical despite different names*

