# Comparing `tmp/openplayground-0.1.3.tar.gz` & `tmp/openplayground-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplayground-0.1.3.tar", max compression
+gzip compressed data, was "openplayground-0.1.4.tar", max compression
```

## Comparing `openplayground-0.1.3.tar` & `openplayground-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,23 @@
--rw-r--r--   0        0        0     1074 2023-03-24 23:54:37.772845 openplayground-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     3919 2023-04-03 22:54:58.500611 openplayground-0.1.3/README.md
--rw-r--r--   0        0        0      816 2023-04-04 03:44:59.765262 openplayground-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 00:18:19.571576 openplayground-0.1.3/server/__init__.py
--rwxr-xr-x   0        0        0    11170 2023-04-04 03:28:44.526761 openplayground-0.1.3/server/app.py
--rw-r--r--   0        0        0        0 2023-03-27 02:28:06.083858 openplayground-0.1.3/server/lib/__init__.py
--rw-r--r--   0        0        0     4473 2023-04-04 00:19:47.703583 openplayground-0.1.3/server/lib/api/__init__.py
--rw-r--r--   0        0        0     6573 2023-04-04 00:12:46.670793 openplayground-0.1.3/server/lib/api/inference.py
--rw-r--r--   0        0        0     4677 2023-04-04 00:12:59.317725 openplayground-0.1.3/server/lib/api/provider.py
--rw-r--r--   0        0        0      273 2023-03-27 03:16:51.467759 openplayground-0.1.3/server/lib/api/response_utils.py
--rw-r--r--   0        0        0     4613 2023-04-03 23:59:42.397511 openplayground-0.1.3/server/lib/entities.py
--rw-r--r--   0        0        0     1692 2023-04-03 22:41:03.375487 openplayground-0.1.3/server/lib/event_emitter.py
--rw-r--r--   0        0        0    30421 2023-04-03 20:54:17.133808 openplayground-0.1.3/server/lib/inference/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 23:54:37.778250 openplayground-0.1.3/server/lib/inference/huggingface/__init__.py
--rw-r--r--   0        0        0     7943 2023-03-25 02:42:59.727198 openplayground-0.1.3/server/lib/inference/huggingface/generator.py
--rw-r--r--   0        0        0      363 2023-03-25 02:42:47.499028 openplayground-0.1.3/server/lib/inference/huggingface/helpers.py
--rwxr-xr-x   0        0        0     5319 2023-03-25 02:45:12.811318 openplayground-0.1.3/server/lib/inference/huggingface/hf.py
--rwxr-xr-x   0        0        0     6871 2023-04-04 00:12:02.228659 openplayground-0.1.3/server/lib/sse.py
--rw-r--r--   0        0        0     1862 2023-04-03 21:01:39.678086 openplayground-0.1.3/server/lib/sseserver.py
--rw-r--r--   0        0        0     6764 2023-04-04 01:58:44.306783 openplayground-0.1.3/server/lib/storage.py
--rw-r--r--   0        0        0    18563 2023-04-03 21:00:46.964993 openplayground-0.1.3/server/models.json
--rwxr-xr-x   0        0        0      284 2023-03-24 23:54:37.778730 openplayground-0.1.3/server/requirements.txt
--rw-r--r--   0        0        0  6271018 2023-04-04 01:04:31.355655 openplayground-0.1.3/server/static/index.2d3ace14.js
--rw-r--r--   0        0        0  7139143 2023-04-04 01:04:31.369400 openplayground-0.1.3/server/static/index.2d3ace14.js.map
--rw-r--r--   0        0        0   882312 2023-04-04 01:57:07.472536 openplayground-0.1.3/server/static/index.5530e416.js
--rw-r--r--   0        0        0   224100 2023-04-04 01:57:08.602507 openplayground-0.1.3/server/static/index.5530e416.js.br
--rw-r--r--   0        0        0   273500 2023-04-04 01:57:07.497322 openplayground-0.1.3/server/static/index.5530e416.js.gz
--rw-r--r--   0        0        0    51614 2023-04-04 01:04:31.141944 openplayground-0.1.3/server/static/index.61d3354a.css
--rw-r--r--   0        0        0    15095 2023-04-04 01:04:31.147201 openplayground-0.1.3/server/static/index.61d3354a.css.map
--rw-r--r--   0        0        0    43532 2023-04-04 01:57:04.090794 openplayground-0.1.3/server/static/index.c0b28010.css
--rw-r--r--   0        0        0     7130 2023-04-04 01:57:04.129496 openplayground-0.1.3/server/static/index.c0b28010.css.br
--rw-r--r--   0        0        0     8277 2023-04-04 01:57:04.091056 openplayground-0.1.3/server/static/index.c0b28010.css.gz
--rw-r--r--   0        0        0      814 2023-04-04 01:57:07.472445 openplayground-0.1.3/server/static/index.html
--rw-r--r--   0        0        0      275 2023-04-04 01:57:07.473773 openplayground-0.1.3/server/static/index.html.br
--rw-r--r--   0        0        0      423 2023-04-04 01:57:07.472650 openplayground-0.1.3/server/static/index.html.gz
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 openplayground-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-07 16:23:09.045621 openplayground-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     4527 2023-04-11 18:22:21.034872 openplayground-0.1.4/README.md
+-rw-r--r--   0        0        0      948 2023-04-13 16:55:18.502927 openplayground-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 16:23:09.051828 openplayground-0.1.4/server/__init__.py
+-rwxr-xr-x   0        0        0    15398 2023-04-13 16:52:49.106643 openplayground-0.1.4/server/app.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:23:09.052030 openplayground-0.1.4/server/lib/__init__.py
+-rw-r--r--   0        0        0     4473 2023-04-07 16:23:09.052190 openplayground-0.1.4/server/lib/api/__init__.py
+-rw-r--r--   0        0        0     4632 2023-04-13 16:52:49.107315 openplayground-0.1.4/server/lib/api/inference.py
+-rw-r--r--   0        0        0     4538 2023-04-07 16:23:09.052376 openplayground-0.1.4/server/lib/api/provider.py
+-rw-r--r--   0        0        0      273 2023-04-07 16:23:09.052444 openplayground-0.1.4/server/lib/api/response_utils.py
+-rw-r--r--   0        0        0     5034 2023-04-07 16:23:09.052543 openplayground-0.1.4/server/lib/entities.py
+-rw-r--r--   0        0        0     1636 2023-04-07 16:23:09.052628 openplayground-0.1.4/server/lib/event_emitter.py
+-rw-r--r--   0        0        0    30494 2023-04-13 16:52:49.108251 openplayground-0.1.4/server/lib/inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:23:09.052945 openplayground-0.1.4/server/lib/inference/huggingface/__init__.py
+-rw-r--r--   0        0        0     7943 2023-04-07 16:23:09.053086 openplayground-0.1.4/server/lib/inference/huggingface/generator.py
+-rw-r--r--   0        0        0      363 2023-04-07 16:23:09.053160 openplayground-0.1.4/server/lib/inference/huggingface/helpers.py
+-rwxr-xr-x   0        0        0     5505 2023-04-11 18:35:56.373509 openplayground-0.1.4/server/lib/inference/huggingface/hf.py
+-rwxr-xr-x   0        0        0     6856 2023-04-11 19:08:01.155341 openplayground-0.1.4/server/lib/sse.py
+-rw-r--r--   0        0        0     1864 2023-04-11 19:09:52.213288 openplayground-0.1.4/server/lib/sseserver.py
+-rw-r--r--   0        0        0    10480 2023-04-07 16:23:09.053510 openplayground-0.1.4/server/lib/storage.py
+-rw-r--r--   0        0        0    18738 2023-04-13 16:53:10.326323 openplayground-0.1.4/server/models.json
+-rwxr-xr-x   0        0        0      284 2023-04-07 16:23:09.053689 openplayground-0.1.4/server/requirements.txt
+-rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 openplayground-0.1.4/PKG-INFO
```

### Comparing `openplayground-0.1.3/LICENSE` & `openplayground-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.3/README.md` & `openplayground-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 https://user-images.githubusercontent.com/111631/227399583-39b23f48-9823-4571-a906-985dbe282b20.mp4
 
 #### Features
 
 - Use any model from [OpenAI](), [Anthropic](), [Cohere](), [Forefront](), [HuggingFace](), [Aleph Alpha](), and [llama.cpp]().
 - Full playground UI, including history, parameter tuning, keyboard shortcuts, and logprops.
-- Compare models side-by-side with the same prompt, individually tune model parameters, and retry with different paramaters.
+- Compare models side-by-side with the same prompt, individually tune model parameters, and retry with different parameters.
 - Automatically detects local models in your HuggingFace cache, and lets you install new ones.
 - Works OK on your phone.
 - Probably won't kill everyone.
 
 ## Try on nat.dev
 
 Try the hosted version: [nat.dev](https://nat.dev).
@@ -20,24 +20,38 @@
 ## How to install and run
 
 ```sh
 $ pip install openplayground
 $ openplayground run
 ```
 
-This runs a Flask process, so you can add the typical flags such as setting a different port `openplayground run -p 1235` and others. 
+Alternatively, run it as a docker container:
+```sh
+$ docker run --name openplayground -p 5432:5432 -d --volume openplayground:/web/config natorg/openplayground
+```
+
+This runs a Flask process, so you can add the typical flags such as setting a different port `openplayground run -p 1235` and others.
 
 ## How to run for development
 
 ```sh
 $ git clone https://github.com/nat/openplayground
 $ cd app && npm install && npx parcel watch src/index.html --no-cache
-$ cd server && pip3 install -r requirements.txt && python app.py
+$ cd server && pip3 install -r requirements.txt && cd .. && python3 -m server.app
+```
+
+## Docker
+
+```sh
+$ docker build . --tag "openplayground"
+$ docker run --name openplayground -p 5432:5432 -d --volume openplayground:/web/config openplayground
 ```
 
+First volume is optional. It's used to store API keys, models settings.
+
 ## Ideas for contributions
 
 - Add a token counter to the playground
 - Add a cost counter to the playground and the compare page
 - Measure and display time to first token
 - Setup automatic builds with GitHub Actions
 - The default parameters for each model are configured in the `server/models.json` file. If you find better default parameters for a model, please submit a pull request!
@@ -45,27 +59,28 @@
 - Easier way to install open source models directly from openplayground, with `openplayground install <model>` or in the UI.
 - Find and fix bugs
 - ChatGPT UI, with turn-by-turn, markdown rendering, chatgpt plugin support, etc.
 - We will probably need multimodal inputs and outputs at some point in 2023
 
 ### llama.cpp
 
-
-## Adding models to openplayground 
+## Adding models to openplayground
 
 Models and providers have three types in openplayground:
-+ Searchable
-+ Local inference
-+ API
+
+- Searchable
+- Local inference
+- API
 
 You can add models in `server/models.json` with the following schema:
 
 #### Local inference
 
 For models running locally on your device you can add them to openplayground like the following (a minimal example):
+
 ```json
 "llama": {
     "api_key" : false,
     "models" : {
         "llama-70b": {
             "parameters": {
                 "temperature": {
@@ -82,14 +97,15 @@
 ```
 
 Keep in mind you will need to add a generation method for your model in `server/app.py`. Take a look at `local_text_generation()` as an example.
 
 #### API Provider Inference
 
 This is for model providers like OpenAI, cohere, forefront, and more. You can connect them easily into openplayground (a minimal example):
+
 ```json
 "cohere": {
     "api_key" : true,
     "models" : {
         "xlarge": {
             "parameters": {
                 "temperature": {
@@ -124,7 +140,11 @@
                 0.1,
                 1.0
             ]
         },
     }
 }
 ```
+
+#### Credits
+
+Instigated by Nat Friedman. Initial implementation by [Zain Huda](https://github.com/zainhuda) as a repl.it bounty. Many features and extensive refactoring by Alex Lourenco.
```

### Comparing `openplayground-0.1.3/pyproject.toml` & `openplayground-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "openplayground"
-version = "0.1.3"
+version = "0.1.4"
 description = "An LLM playground you can run on your laptop."
 authors = ["Nat Friedman <nat@nat.org>"]
 readme = "README.md"
+homepage = "https://nat.dev/"
+repository = "https://github.com/nat/openplayground"
+keywords = ["llm", "playground", "openplayground"]
 packages = [
-    { include = "server", from = "" },
+  { include = "server", from = "" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aleph_alpha_client="^2.16.1"
 anthropic = "^0.2.3"
 cachetools="^5.3.0"
```

### Comparing `openplayground-0.1.3/server/lib/api/__init__.py` & `openplayground-0.1.4/server/lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.3/server/lib/api/provider.py` & `openplayground-0.1.4/server/lib/api/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import json
 import requests
 
 from .response_utils import create_response_message
-from ..entities import Model, ModelEncoder, Provider
+from ..entities import Model, ModelEncoder
 
-from flask import g, request, jsonify, jsonify, Blueprint, current_app
+from flask import g, request, jsonify, Blueprint, current_app
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 provider_bp = Blueprint('provider', __name__, url_prefix='/provider')
 
 @provider_bp.before_app_request
@@ -23,15 +23,14 @@
     model_name = request.view_args.get('model_name')
 
     provider = g.provider = storage.get_provider(provider_name)
 
     if provider is None:
         return create_response_message(f"Invalid provider: {provider_name}", 400)
     
-    print(f"provider: {provider}")
     if not provider.search_url and (model_name and not provider.has_model(model_name)):
         return create_response_message(f"Invalid model: {model_name}", 400)
     
     g.model = provider.get_model(model_name)
        
 @provider_bp.route('/<string:provider_name>/models')
 def provider_models(provider_name):
@@ -67,16 +66,17 @@
     provider = g.provider
     model = g.model
 
     #if it made it this far then it has to a dynamic model (HF/OpenPlayground Hub)
     if model is None:
         model = Model(
             name=model_name,
+            capabilities=provider.default_capabilities,
             provider=provider_name,
-            status='pending',
+            status="ready" if provider.remote_inference else "pending",
             enabled=True,
             parameters=provider.default_parameters
         )
         provider.add_model(model)
     else:
         model.enabled = not model.enabled
         provider.update_model(model.name, model)
@@ -127,18 +127,14 @@
     logger.info(f"Storing API key for {provider_name}")
 
     data = request.get_json(force=True)
     storage = g.get('storage')
 
     api_key = data['apiKey']
     if api_key is None:
-        return create_response_message(f"Invalid API key", 400)
-    
+        return create_response_message("Invalid API key", 400)
+
     storage.update_provider_api_key(provider_name, api_key)
- 
+
     response = jsonify({'status': 'success'})
     response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
-
-@provider_bp.route('/<string:provider_name>/search-models/<string:model_name_pattern>', methods=['GET'])
-def provider_search_model(provider_name, model_name_pattern):
-    pass
+    return response
```

### Comparing `openplayground-0.1.3/server/lib/entities.py` & `openplayground-0.1.4/server/lib/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 import json
 from typing import List
 from .event_emitter import EventEmitter, EVENTS
 
 class Model:
     def __init__(
-        self, name: str, enabled: bool, provider: str, status: str, parameters: dict = None
+        self, name: str, enabled: bool, capabilities: List[str],  provider: str, status: str, parameters: dict = None
     ):
         self.name = name
+        self.capabilities = capabilities
         self.enabled = enabled
         self.provider = provider
         self.status = status
         self.parameters = parameters
 
     def copy(self):
         return Model(
             name=self.name,
+            capabilities=self.capabilities,
             enabled=self.enabled,
             provider=self.provider,
             status=self.status,
             parameters=self.parameters.copy()
         )
 
     def __repr__(self):
-        return f'Model({self.name}, {self.enabled}, {self.provider}, {self.status}, {self.parameters})'
+        return f'Model({self.name}, {self.capabilities}, {self.enabled}, {self.provider}, {self.status}, {self.parameters})'
 
 class ModelEncoder(json.JSONEncoder):
     def __init__(self, *args, serialize_as_list=True, **kwargs):
         self.serialize_as_list = serialize_as_list
         super().__init__(*args, **kwargs)
 
     def default(self, obj):
         if isinstance(obj, Model):
-            properties = {"enabled": obj.enabled, "status": obj.status, "parameters": obj.parameters}
+            properties = {
+                "capabilities": obj.capabilities,
+                "enabled": obj.enabled, "status": obj.status, "parameters": obj.parameters
+            }
             if self.serialize_as_list:
                 return {**{"name": obj.name, "provider": obj.provider}, **properties}
             else:
                 return {f"{obj.provider}:{obj.name}": properties}
         return super().default(obj)
 
 class Provider:
     def __init__(
         self, name: str, models: List[Model], remote_inference: bool = False,
-        default_parameters: dict = None, api_key: str = None, requires_api_key: bool = False,
+        default_capabilities: List[str] = None, default_parameters: dict = None,
+        api_key: str = None, requires_api_key: bool = False,
         search_url: str = None
     ):
         self.event_emitter = EventEmitter()
         self.name = name
         self.models = models
         self.remote_inference = remote_inference
+        self.default_capabilities = default_capabilities
         self.default_parameters = default_parameters
         self.api_key = api_key
         self.requires_api_key = requires_api_key
         self.search_url = search_url
     
     def has_model(self, model_name: str) -> bool:
-        for model in self.models:
-            if model.name == model_name:
-                return True
-        return False
+        return any(model.name == model_name for model in self.models)
     
     def get_model(self, model_name: str) -> Model:
         for model in self.models:
             if model.name == model_name:
                 return model
             
     def update_model(self, model_name: str, model: Model) -> None:
@@ -84,14 +88,15 @@
                 return
             
     def copy(self):
         return Provider(
             name=self.name,
             models=[model.copy() for model in self.models],
             remote_inference=self.remote_inference,
+            default_capabilities=self.default_capabilities.copy() if self.default_capabilities else None,
             default_parameters=self.default_parameters.copy() if self.default_parameters else None,
             api_key=self.api_key,
             requires_api_key=self.requires_api_key,
             search_url=self.search_url
         )
     
     def __repr__(self):
@@ -101,15 +106,16 @@
     def __init__(self, *args, serialize_models_as_list=True, **kwargs):
         self.serialize_models_as_list = serialize_models_as_list
         super().__init__(*args, **kwargs)
 
     def default(self, obj):
         if isinstance(obj, Provider):
             models = [{
-                "name": model.name, "enabled": model.enabled, "provider": model.provider,
+                "name": model.name, "capabilities": model.capabilities,
+                "enabled": model.enabled, "provider": model.provider,
                 "status": model.status, "parameters": model.parameters
             } for model in obj.models]
             
             if not self.serialize_models_as_list:
                 models = dict(zip([model["name"] for model in models], models))
         
             return {self.to_camel_case(k): v for k, v in obj.__dict__.items() if k not in {'models', 'event_emitter'}} | {'models': models}
```

### Comparing `openplayground-0.1.3/server/lib/event_emitter.py` & `openplayground-0.1.4/server/lib/event_emitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,23 +30,21 @@
         with self._lock:
             if event not in self.listeners:
                 self.listeners[event] = []
             self.listeners[event].append(listener)
 
     def off(self, event, listener):
         with self._lock:
-            if event in self.listeners:
-                if listener in self.listeners[event]:
-                    self.listeners[event].remove(listener)
+            if event in self.listeners and listener in self.listeners[event]:
+                self.listeners[event].remove(listener)
 
     def emit(self, event: EVENTS, *args, **kwargs):
-        if event in EVENTS.__members__.values():
-            if event.value not in self.listeners:
-                return
+        if event not in EVENTS.__members__.values():
+            raise ValueError(f"Invalid event type: {event}")
+        if event.value not in self.listeners:
+            return
 
-            with self._lock:
-                listeners_to_notify = self.listeners[event.value].copy()
+        with self._lock:
+            listeners_to_notify = self.listeners[event.value].copy()
 
-            for listener in listeners_to_notify:
-                listener(event, *args, **kwargs)
-        else:
-            raise ValueError("Invalid event type: %s" % event)
+        for listener in listeners_to_notify:
+            listener(event, *args, **kwargs)
```

### Comparing `openplayground-0.1.3/server/lib/inference/__init__.py` & `openplayground-0.1.4/server/lib/inference/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 class InferenceAnnouncer:
     def __init__(self, sse_topic):
         self.sse_topic = sse_topic
         self.cancel_cache = cachetools.TTLCache(maxsize=1000, ttl=60)
 
     def __format_message__(self, event: str, infer_result: InferenceResult) -> str:
-        logger.info("formatting message")
+        logger.debug("formatting message")
         encoded = {
             "message": infer_result.token,
             "modelName": infer_result.model_name,
             "modelTag": infer_result.model_tag,
             "modelProvider": infer_result.model_provider,
         }
 
@@ -113,15 +113,15 @@
 
         message = None
         if event == "done":
             message = json.dumps({"data": {}, "type": "done"})
         else:
             message = self.__format_message__(event=event, infer_result=infer_result)
 
-        logger.info(f"Announcing {event} for uuid: {infer_result.uuid}, message: {message}")
+        logger.debug(f"Announcing {event} for uuid: {infer_result.uuid}, message: {message}")
         self.sse_topic.publish(message)
 
         return True
 
     def cancel_callback(self, message):
         if message['type'] == 'pmessage':
             data = json.loads(message['data'])
@@ -140,15 +140,15 @@
             model_name=inference_request.model_name,
             model_tag=inference_request.model_tag,
             model_provider=inference_request.model_provider,
             token=None,
             probability=None,
             top_n_distribution=None
         )
-    
+
         if not self.announcer.announce(InferenceResult(
             uuid=inference_request.uuid,
             model_name=inference_request.model_name,
             model_tag=inference_request.model_tag,
             model_provider=inference_request.model_provider,
             token="[INITIALIZING]",
             probability=None,
@@ -176,15 +176,15 @@
         except openai.error.PermissionError as e:
             infer_result.token = f"[ERROR] OpenAI API request was not permitted: {e}"
             logger.error(f"OpenAI API request was not permitted: {e}")
         except openai.error.RateLimitError as e:
             infer_result.token = f"[ERROR] OpenAI API request exceeded rate limit: {e}"
             logger.error(f"OpenAI API request exceeded rate limit: {e}")
         except requests.exceptions.RequestException as e:
-            logging.error("RequestException: {}".format(e))
+            logging.error(f"RequestException: {e}")
             infer_result.token = f"[ERROR] No response from {infer_result.model_provider } after sixty seconds"
         except ValueError as e:
             if infer_result.model_provider == "huggingface-local":
                 infer_result.token = f"[ERROR] Error parsing response from local inference: {traceback.format_exc()}"
                 logger.error(f"Error parsing response from local inference: {traceback.format_exc()}")
             else:
                 infer_result.token = f"[ERROR] Error parsing response from API: {e}"
@@ -200,15 +200,15 @@
     
     def __openai_chat_generation__(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         openai.api_key = provider_details.api_key
 
         current_date = datetime.now().strftime("%Y-%m-%d")
 
         if inference_request.model_name == "gpt-4":
-            system_content = f"You are GPT-4, a large language model trained by OpenAI. Answer as concisely as possible"
+            system_content = "You are GPT-4, a large language model trained by OpenAI. Answer as concisely as possible"
         else:
             system_content = f"You are ChatGPT, a large language model trained by OpenAI. Answer as concisely as possible. Knowledge cutoff: 2021-09-01 Current date: {current_date}"
 
         response = openai.ChatCompletion.create(
              model=inference_request.model_name,
              messages = [
                 {"role": "system", "content": system_content},
@@ -229,15 +229,15 @@
         for event in response:
             response = event['choices'][0]
             if response['finish_reason'] == "stop":
                 break
 
             delta = response['delta']
 
-            if not "content" in delta:
+            if "content" not in delta:
                 continue
 
             generated_token = delta["content"]
             tokens += generated_token
 
             infer_response = InferenceResult(
                 uuid=inference_request.uuid,
@@ -322,15 +322,15 @@
 
             if not self.announcer.announce(infer_response, event="infer"):
                 cancelled = True
                 logger.info(f"Cancelled inference for {inference_request.uuid} - {inference_request.model_name}")
 
     def openai_text_generation(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         # TODO: Add a meta field to the inference so we know when a model is chat vs text
-        if inference_request.model_name == "gpt-3.5-turbo" or inference_request.model_name == "gpt-4":
+        if inference_request.model_name in ["gpt-3.5-turbo", "gpt-4"]:
             self.__error_handler__(self.__openai_chat_generation__, provider_details, inference_request)
         else:
             self.__error_handler__(self.__openai_text_generation__, provider_details, inference_request)
 
     def __cohere_text_generation__(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         with requests.post("https://api.cohere.ai/generate",
             headers={
@@ -398,15 +398,14 @@
                 }
             },
             timeout=60
         )
 
         content_type = response.headers["content-type"]
 
-        total_tokens = 0
         cancelled = False
 
         if response.status_code != 200:
             raise Exception(f"Request failed: {response.status_code} {response.reason}")
 
         if content_type == "application/json":
             return_data = json.loads(response.content.decode("utf-8"))
@@ -419,68 +418,72 @@
                 model_tag=inference_request.model_tag,
                 model_provider=inference_request.model_provider,
                 token=outputs,
                 probability=None,
                 top_n_distribution=None
             ), event="infer")
         else:
+            total_tokens = 0
             for response in response.iter_lines():
                 response = response.decode('utf-8')
                 if response == "":
                     continue
 
                 response_json = json.loads(response[5:])
                 if "error" in response:
                     error = response_json["error"]
                     raise Exception(f"{error}")
 
                 token = response_json['token']
-                
+
                 total_tokens += 1
-                
+
                 if token["special"]:
                     continue
-                
+
                 if cancelled: continue
 
-                if not self.announcer.announce(InferenceResult(
-                    uuid=inference_request.uuid,
-                    model_name=inference_request.model_name,
-                    model_tag=inference_request.model_tag,
-                    model_provider=inference_request.model_provider,
-                    token= " " if token['id'] == 3 else response_json['token']['text'],
-                    probability=response_json['token']['logprob'],
-                    top_n_distribution=None
-                ), event="infer"):
+                if not self.announcer.announce(
+                    InferenceResult(
+                        uuid=inference_request.uuid,
+                        model_name=inference_request.model_name,
+                        model_tag=inference_request.model_tag,
+                        model_provider=inference_request.model_provider,
+                        token=" " if token['id'] == 3 else token['text'],
+                        probability=token['logprob'],
+                        top_n_distribution=None,
+                    ),
+                    event="infer",
+                ):
                     cancelled = True
                     logger.info(f"Cancelled inference for {inference_request.uuid} - {inference_request.model_name}")
            
     def huggingface_text_generation(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         self.__error_handler__(self.__huggingface_text_generation__, provider_details, inference_request)
 
     def __forefront_text_generation__(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         with requests.post(
-            f"https://shared-api.forefront.link/organization/gPn2ZLSO3mTh/{inference_request.model_name}/completions/{provider_details.version_key}",
-            headers={
-                "Authorization": f"Bearer {provider_details.api_key}",
-                "Content-Type": "application/json",
-            },
-            data=json.dumps({
-                "text": inference_request.prompt,
-                "top_p": float(inference_request.model_parameters['topP']),
-                "top_k": int(inference_request.model_parameters['topK']),
-                "temperature":  float(inference_request.model_parameters['temperature']),
-                "repetition_penalty":  float(inference_request.model_parameters['repetitionPenalty']),
-                "length": int(inference_request.model_parameters['maximumLength']),
-                "stop": inference_request.model_parameters['stopSequences'],
-                "logprobs": 5,
-                "stream": True,
-            }),
-            stream=True
-        ) as response:
+                f"https://shared-api.forefront.link/organization/gPn2ZLSO3mTh/{inference_request.model_name}/completions/{provider_details.version_key}",
+                headers={
+                    "Authorization": f"Bearer {provider_details.api_key}",
+                    "Content-Type": "application/json",
+                },
+                data=json.dumps({
+                    "text": inference_request.prompt,
+                    "top_p": float(inference_request.model_parameters['topP']),
+                    "top_k": int(inference_request.model_parameters['topK']),
+                    "temperature":  float(inference_request.model_parameters['temperature']),
+                    "repetition_penalty":  float(inference_request.model_parameters['repetitionPenalty']),
+                    "length": int(inference_request.model_parameters['maximumLength']),
+                    "stop": inference_request.model_parameters['stopSequences'],
+                    "logprobs": 5,
+                    "stream": True,
+                }),
+                stream=True
+            ) as response:
             if response.status_code != 200:
                 raise Exception(f"Request failed: {response.status_code} {response.reason}")
             cancelled = False
             total_tokens = 0
             aggregate_string_length = 0
 
             for packet in sseclient.SSEClient(response).events():
@@ -511,33 +514,33 @@
                     tokens = logprobs["tokens"]
                     token_logprobs = logprobs["token_logprobs"]
 
                     new_tokens = tokens[total_tokens:]
 
                     for index, new_token in enumerate(new_tokens):
                         generated_token = new_token
-            
+
                         probability = token_logprobs[total_tokens + index]
                         top_logprobs = logprobs["top_logprobs"][total_tokens + index]
-                            
+
                         chosen_log_prob = 0
                         prob_dist = ProablityDistribution(
                             log_prob_sum=0, simple_prob_sum=0, tokens={},
                         )
 
                         for token, log_prob in top_logprobs.items():
                             if log_prob == -3000.0: continue
                             simple_prob = round(math.exp(log_prob) * 100, 2)
                             prob_dist.tokens[token] = [log_prob, simple_prob]
 
-                            if token == new_token:
+                            if token == generated_token:
                                 chosen_log_prob = round(log_prob, 2)
-            
+
                             prob_dist.simple_prob_sum += simple_prob
-                            
+
                         prob_dist.tokens = dict(
                             sorted(prob_dist.tokens.items(), key=lambda item: item[1][0], reverse=True)
                         )
                         prob_dist.log_prob_sum = chosen_log_prob
                         prob_dist.simple_prob_sum = round(prob_dist.simple_prob_sum, 2)
 
                         if not self.announcer.announce(InferenceResult(
@@ -561,14 +564,15 @@
                 if cancelled: continue
 
     def forefront_text_generation(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         self.__error_handler__(self.__forefront_text_generation__, provider_details, inference_request)
 
     def __local_text_generation__(self, provider_details: ProviderDetails, inference_request: InferenceRequest):
         cancelled = False
+        logger.info(f"Starting inference for {inference_request.uuid} - {inference_request.model_name}")
 
         hf = HFInference(inference_request.model_name)
         output = hf.generate(
             prompt=inference_request.prompt,
             max_length=int(inference_request.model_parameters['maximumLength']),
             top_p=float(inference_request.model_parameters['topP']),
             top_k=int(inference_request.model_parameters['topK']),
```

### Comparing `openplayground-0.1.3/server/lib/inference/huggingface/generator.py` & `openplayground-0.1.4/server/lib/inference/huggingface/generator.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.3/server/lib/inference/huggingface/hf.py` & `openplayground-0.1.4/server/lib/inference/huggingface/hf.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,67 +2,70 @@
 import transformers
 import psutil
 import torch
 import importlib
 import logging
 import warnings
 
-from transformers import AutoTokenizer, AutoConfig, PreTrainedModel, PreTrainedTokenizer
+from transformers import AutoTokenizer, AutoConfig, PreTrainedModel, PreTrainedTokenizer, AutoModelForCausalLM
 from .generator import greedy_search_generator
 from .helpers import StoppingCriteriaSub
 
 # monkey patch for transformers
 transformers.generation.utils.GenerationMixin.greedy_search = greedy_search_generator
 os.environ['TOKENIZERS_PARALLELISM'] = 'true'
 
 # Set constants
 MODULE = importlib.import_module("transformers") # dynamic import of module class, AutoModel not good enough for text generation
-DEVICE = "cuda" if torch.cuda.is_available() else "cpu" # suport gpu inference if possible
+DEVICE = "cuda" if torch.cuda.is_available() else "cpu" # support gpu inference if possible
 
 logger = logging.getLogger(__name__)
 
 class HFInference:
     '''
     Class for huggingface local inference
     '''
     def __init__(self, model_name: str):
         self.model_name = model_name
         self.model, self.tokenizer = self.load_model(model_name)
 
     # Helper function to load model from transformers library
-    def load_model(self, model_name: str)-> tuple([PreTrainedModel, PreTrainedTokenizer]):
+    def load_model(self, model_name: str) -> (PreTrainedModel, PreTrainedTokenizer):
         '''
         Load model from transformers library
         dynamically instantiates the right model class for text generation from model config architecture
         '''
         tokenizer = AutoTokenizer.from_pretrained(model_name)
         config = AutoConfig.from_pretrained(model_name) # load config for model
-        model_class = getattr(MODULE, config.architectures[0]) # get model class from config
-        model = model_class.from_pretrained(model_name, config=config) # dynamically load right model class for text generation
-
-        param_size = 0
-        for param in model.parameters():
-            param_size += param.nelement() * param.element_size()
-        buffer_size = 0
-        for buffer in model.buffers():
-            buffer_size += buffer.nelement() * buffer.element_size()
+        if config.architectures:
+            model_classname = config.architectures[0]
+            model_class = getattr(MODULE, model_classname) # get model class from config
+            model = model_class.from_pretrained(model_name, config=config) # dynamically load right model class for text generation
+        else:
+            model = AutoModelForCausalLM.from_pretrained(model_name, device_map='auto' if DEVICE == 'cuda' else None)
 
+        param_size = sum(
+            param.nelement() * param.element_size() for param in model.parameters()
+        )
+        buffer_size = sum(
+            buffer.nelement() * buffer.element_size() for buffer in model.buffers()
+        )
         size_all_mb = (param_size + buffer_size) / 1024**2
         logger.info('model size: {:.3f}MB'.format(size_all_mb))
 
         if DEVICE == 'cuda':
             device_memory = torch.cuda.get_device_properties(0).total_memory / 1024**2
         else:
             device_memory = psutil.virtual_memory().total / 1024**2
 
         logger.info('device memory: {:.3f}MB'.format(device_memory))
 
         if size_all_mb > device_memory * 0.95: #some padding
             raise Exception('Model size is too large for host to run inference on')
-        
+
         model.to(DEVICE) # gpu inference if possible
         return model, tokenizer
 
     def generate(self, 
             prompt: str, 
             max_length: int, 
             temperature: float, 
@@ -89,24 +92,24 @@
                 top_p=top_p,
                 repetition_penalty=repetition_penalty,
                 early_stopping=False,
                 # stopping_criteria=stopping_criteria if stopping_criteria else None,
             )
         except Exception as e:
             raise Exception(f"Error generating text: {e}")
-        
+
         curr_token = ""
         sentence = "<|endoftext|>"
         first_token = True
         for output in outputs:
             next_token = output
             if len(next_token.size()) > 1: continue # skip the last generated full array
-            curr = self.tokenizer.convert_ids_to_tokens(next_token, skip_special_tokens=True)
-        
-            if (curr):
+            if curr := self.tokenizer.convert_ids_to_tokens(
+                next_token, skip_special_tokens=True
+            ):
                 curr = curr[0] # string with special character potentially
                 if (curr[0] == "Ġ"): # BPE tokenizer
                     curr_token = curr_token.replace("Ċ", "\n")
                     curr_token = curr.replace("Ġ", " ")
                     sentence += curr_token # we can yield here/print here
                     yield curr_token
                     # BPE
@@ -119,15 +122,15 @@
                     sentence += curr_token # we can yield here/print here
                     yield curr_token
                 else:
                     curr_token = curr
                     curr_token = curr_token.replace("Ċ", "\n")
                     yield curr_token
                     sentence += curr_token
-                
+
                 curr_token = ""
 
         # dispatch last token, if we can
         if curr_token != "": 
             yield curr_token # send only if non empty
 
-        logger.info(f'[COMPLETION]: {sentence}')           
+        logger.info(f'[COMPLETION]: {sentence}')
```

### Comparing `openplayground-0.1.3/server/lib/sse.py` & `openplayground-0.1.4/server/lib/sse.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,35 +123,34 @@
         :param channel: If you want to direct different events to different
             clients, you may specify a channel for this event to go to.
             Only clients listening to the same channel will receive this event.
             Defaults to "sse".
         """
         message = Message(data, type=type, id=id, retry=retry)
         msg_json = json.dumps(message.to_dict())
-        logger.info(f"PUBLISHING: {msg_json} to channel: {channel}")
+        logger.debug(f"PUBLISHING: {msg_json} to channel: {channel}")
         return self.sse_server.sse_publish(channel=channel, message=msg_json)
 
     def messages(self, channel='sse'):
         """
         A generator of :class:`~flask_sse.Message` objects from the given channel.
         """
         self.sse_server.sse_subscribe(channel)
         try:
             for pubsub_message in self.sse_server.sse_listen(channel)._getvalue():
-                logger.info(f"pubsub_message: {pubsub_message}")            
+                logger.debug(f"pubsub_message: {pubsub_message}")            
                 if pubsub_message['type'] == 'message':
                     msg_dict = json.loads(pubsub_message['data'])
                     if msg_dict["type"] == "done":
                         logger.info("Done streaming SSE")
                         break
 
                     yield Message(**msg_dict)
         except GeneratorExit:
             logger.error("GeneratorExit")
-            pass
         finally:
             logger.info(f"Unsubscribing from channel: {channel}")
             try:
                 self.sse_server.sse_unsubscribe(channel)
             except ConnectionError:
                 pass
         return None
```

### Comparing `openplayground-0.1.3/server/lib/sseserver.py` & `openplayground-0.1.4/server/lib/sseserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def listen(self):
         logger.info("LISTENING")
         q = queue.Queue(maxsize=50) # what about multiprocessing.Queue?
         self.listeners.append(q)
         return q
 
     def publish(self, message: str):
-        logger.info(f"PUBLISHING {message}")
+        logger.debug(f"PUBLISHING {message}")
         for i in reversed(range(len(self.listeners))):
             try:
                 self.listeners[i].put_nowait(message)
             except queue.Full:
                 del self.listeners[i]
 
 class SSEQueueWithTopic:
@@ -28,15 +28,15 @@
     def listen(self, topic: str):
         logger.info(f"LISTENING TO: {topic}")
         if topic not in self.pubsub:
             raise ValueError(f"Channel {topic} not found")
         return self.pubsub[topic].listen()
 
     def publish(self, topic: str, message: str):
-        logger.info(f"PUBLISHING TO: {topic} MESSAGE: {message}")
+        logger.debug(f"PUBLISHING TO: {topic} MESSAGE: {message}")
         if topic not in self.pubsub:
             raise ValueError(f"Topic {topic} not found")
         self.pubsub[topic].announce(message=message)
     
     def add_topic(self, topic: str):
         logger.info(f"SUBSCRIBING TO: {topic}")
         if topic not in self.pubsub:
```

### Comparing `openplayground-0.1.3/server/models.json` & `openplayground-0.1.4/server/models.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9190535241874528%*

 * *Differences: {"'aleph-alpha'": "{'models': {'luminous-supreme-control': {'parameters': {'repetitionPenalty': "*

 * *                  "{'range': {insert: [(0, 0.1)], delete: [0]}}}, 'capabilities': ['logprobs'], "*

 * *                  "delete: ['meta']}, 'luminous-base': {'parameters': {'repetitionPenalty': "*

 * *                  "{'range': {insert: [(0, 0.1)], delete: [0]}}}, 'capabilities': ['logprobs'], "*

 * *                  "delete: ['meta']}, 'luminous-supreme': {'parameters': {'repetitionPenalty': "*

 * *                  "{'range' […]*

```diff
@@ -1,26 +1,26 @@
 {
     "aleph-alpha": {
         "models": {
             "luminous-base": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "maximumLength": {
                         "range": [
                             50,
                             1024
                         ],
                         "value": 200
                     },
                     "repetitionPenalty": {
                         "range": [
-                            0,
+                            0.1,
                             1
                         ],
                         "value": 1
                     },
                     "stopSequences": {
                         "range": [],
                         "value": []
@@ -46,29 +46,29 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "luminous-extended": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "maximumLength": {
                         "range": [
                             50,
                             1024
                         ],
                         "value": 200
                     },
                     "repetitionPenalty": {
                         "range": [
-                            0,
+                            0.1,
                             1
                         ],
                         "value": 1
                     },
                     "stopSequences": {
                         "range": [],
                         "value": []
@@ -94,29 +94,29 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "luminous-supreme": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "maximumLength": {
                         "range": [
                             50,
                             1024
                         ],
                         "value": 200
                     },
                     "repetitionPenalty": {
                         "range": [
-                            0,
+                            0.1,
                             1
                         ],
                         "value": 1
                     },
                     "stopSequences": {
                         "range": [],
                         "value": []
@@ -142,29 +142,29 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "luminous-supreme-control": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "maximumLength": {
                         "range": [
                             50,
                             1024
                         ],
                         "value": 200
                     },
                     "repetitionPenalty": {
                         "range": [
-                            0,
+                            0.1,
                             1
                         ],
                         "value": 1
                     },
                     "stopSequences": {
                         "range": [],
                         "value": []
@@ -195,19 +195,19 @@
             }
         },
         "remoteInference": true,
         "requiresAPIKey": true
     },
     "anthropic": {
         "models": {
-            "claude-instant-v1.0": {
-                "enabled": false,
-                "meta": [
+            "claude-instant-v1": {
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -250,19 +250,19 @@
                             1
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
-            "claude-v1.2": {
-                "enabled": false,
-                "meta": [
+            "claude-v1": {
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -312,16 +312,16 @@
         },
         "remoteInference": true,
         "requiresAPIKey": true
     },
     "cohere": {
         "models": {
             "command-medium-nightly": {
+                "capabilities": [],
                 "enabled": false,
-                "meta": [],
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -365,16 +365,16 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "command-xlarge-nightly": {
+                "capabilities": [],
                 "enabled": false,
-                "meta": [],
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -418,16 +418,16 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "medium": {
+                "capabilities": [],
                 "enabled": false,
-                "meta": [],
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -471,16 +471,16 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "xlarge": {
+                "capabilities": [],
                 "enabled": false,
-                "meta": [],
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 1
@@ -528,26 +528,26 @@
                 "status": "ready"
             }
         },
         "remoteInference": true,
         "requiresAPIKey": true
     },
     "huggingface": {
-        "defaultMeta": [],
+        "defaultCapabilities": [],
         "defaultParameters": {
             "maximumLength": {
                 "range": [
                     50,
                     1024
                 ],
                 "value": 200
             },
             "repetitionPenalty": {
                 "range": [
-                    0,
+                    0.1,
                     2
                 ],
                 "value": 1
             },
             "stopSequences": {
                 "range": [],
                 "value": []
@@ -564,38 +564,38 @@
                     1,
                     500
                 ],
                 "value": 1
             },
             "topP": {
                 "range": [
-                    0.1,
-                    1
+                    0.01,
+                    0.99
                 ],
-                "value": 1
+                "value": 0.99
             }
         },
         "models": {},
         "remoteInference": true,
         "requiresAPIKey": true,
         "searchURL": "https://huggingface.co/api/quicksearch?q={searchQuery}&type=model"
     },
     "huggingface-local": {
-        "defaultMeta": [],
+        "defaultCapabilities": [],
         "defaultParameters": {
             "maximumLength": {
                 "range": [
                     50,
                     1024
                 ],
                 "value": 200
             },
             "repetitionPenalty": {
                 "range": [
-                    0,
+                    0.1,
                     2
                 ],
                 "value": 1
             },
             "temperature": {
                 "range": [
                     0.1,
@@ -609,31 +609,31 @@
                     500
                 ],
                 "value": 1
             },
             "topP": {
                 "range": [
                     0.1,
-                    1
+                    0.99
                 ],
-                "value": 1
+                "value": 0.99
             }
         },
         "models": {},
         "remoteInference": false,
         "requiresAPIKey": false,
         "searchURL": "https://huggingface.co/api/quicksearch?q={searchQuery}&type=model"
     },
     "openai": {
         "models": {
             "gpt-3.5-turbo": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -670,18 +670,18 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "gpt-4": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -718,18 +718,18 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "text-ada-001": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -766,18 +766,18 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "text-babbage-001": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -814,18 +814,18 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "text-curie-001": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -862,18 +862,18 @@
                         ],
                         "value": 1
                     }
                 },
                 "status": "ready"
             },
             "text-davinci-003": {
-                "enabled": false,
-                "meta": [
+                "capabilities": [
                     "logprobs"
                 ],
+                "enabled": false,
                 "parameters": {
                     "frequencyPenalty": {
                         "range": [
                             0,
                             1
                         ],
                         "value": 0
@@ -914,26 +914,26 @@
                 "status": "ready"
             }
         },
         "remoteInference": true,
         "requiresAPIKey": true
     },
     "openplayground": {
-        "defaultMeta": [],
+        "defaultCapabilities": [],
         "defaultParameters": {
             "maximumLength": {
                 "range": [
                     50,
                     1024
                 ],
                 "value": 200
             },
             "repetitionPenalty": {
                 "range": [
-                    0,
+                    0.1,
                     2
                 ],
                 "value": 1
             },
             "temperature": {
                 "range": [
                     0.1,
```

### Comparing `openplayground-0.1.3/PKG-INFO` & `openplayground-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: openplayground
-Version: 0.1.3
+Version: 0.1.4
 Summary: An LLM playground you can run on your laptop.
+Home-page: https://nat.dev/
+Keywords: llm,playground,openplayground
 Author: Nat Friedman
 Author-email: nat@nat.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,27 +22,28 @@
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: sseclient (>=0.0.27,<0.0.28)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.27.1,<5.0.0)
+Project-URL: Repository, https://github.com/nat/openplayground
 Description-Content-Type: text/markdown
 
 # openplayground
 
 An LLM playground you can run on your laptop.
 
 https://user-images.githubusercontent.com/111631/227399583-39b23f48-9823-4571-a906-985dbe282b20.mp4
 
 #### Features
 
 - Use any model from [OpenAI](), [Anthropic](), [Cohere](), [Forefront](), [HuggingFace](), [Aleph Alpha](), and [llama.cpp]().
 - Full playground UI, including history, parameter tuning, keyboard shortcuts, and logprops.
-- Compare models side-by-side with the same prompt, individually tune model parameters, and retry with different paramaters.
+- Compare models side-by-side with the same prompt, individually tune model parameters, and retry with different parameters.
 - Automatically detects local models in your HuggingFace cache, and lets you install new ones.
 - Works OK on your phone.
 - Probably won't kill everyone.
 
 ## Try on nat.dev
 
 Try the hosted version: [nat.dev](https://nat.dev).
@@ -48,24 +51,38 @@
 ## How to install and run
 
 ```sh
 $ pip install openplayground
 $ openplayground run
 ```
 
-This runs a Flask process, so you can add the typical flags such as setting a different port `openplayground run -p 1235` and others. 
+Alternatively, run it as a docker container:
+```sh
+$ docker run --name openplayground -p 5432:5432 -d --volume openplayground:/web/config natorg/openplayground
+```
+
+This runs a Flask process, so you can add the typical flags such as setting a different port `openplayground run -p 1235` and others.
 
 ## How to run for development
 
 ```sh
 $ git clone https://github.com/nat/openplayground
 $ cd app && npm install && npx parcel watch src/index.html --no-cache
-$ cd server && pip3 install -r requirements.txt && python app.py
+$ cd server && pip3 install -r requirements.txt && cd .. && python3 -m server.app
+```
+
+## Docker
+
+```sh
+$ docker build . --tag "openplayground"
+$ docker run --name openplayground -p 5432:5432 -d --volume openplayground:/web/config openplayground
 ```
 
+First volume is optional. It's used to store API keys, models settings.
+
 ## Ideas for contributions
 
 - Add a token counter to the playground
 - Add a cost counter to the playground and the compare page
 - Measure and display time to first token
 - Setup automatic builds with GitHub Actions
 - The default parameters for each model are configured in the `server/models.json` file. If you find better default parameters for a model, please submit a pull request!
@@ -73,27 +90,28 @@
 - Easier way to install open source models directly from openplayground, with `openplayground install <model>` or in the UI.
 - Find and fix bugs
 - ChatGPT UI, with turn-by-turn, markdown rendering, chatgpt plugin support, etc.
 - We will probably need multimodal inputs and outputs at some point in 2023
 
 ### llama.cpp
 
-
-## Adding models to openplayground 
+## Adding models to openplayground
 
 Models and providers have three types in openplayground:
-+ Searchable
-+ Local inference
-+ API
+
+- Searchable
+- Local inference
+- API
 
 You can add models in `server/models.json` with the following schema:
 
 #### Local inference
 
 For models running locally on your device you can add them to openplayground like the following (a minimal example):
+
 ```json
 "llama": {
     "api_key" : false,
     "models" : {
         "llama-70b": {
             "parameters": {
                 "temperature": {
@@ -110,14 +128,15 @@
 ```
 
 Keep in mind you will need to add a generation method for your model in `server/app.py`. Take a look at `local_text_generation()` as an example.
 
 #### API Provider Inference
 
 This is for model providers like OpenAI, cohere, forefront, and more. You can connect them easily into openplayground (a minimal example):
+
 ```json
 "cohere": {
     "api_key" : true,
     "models" : {
         "xlarge": {
             "parameters": {
                 "temperature": {
@@ -153,7 +172,11 @@
                 1.0
             ]
         },
     }
 }
 ```
 
+#### Credits
+
+Instigated by Nat Friedman. Initial implementation by [Zain Huda](https://github.com/zainhuda) as a repl.it bounty. Many features and extensive refactoring by Alex Lourenco.
+
```

