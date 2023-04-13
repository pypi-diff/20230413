# Comparing `tmp/gradio_client-0.1.0.tar.gz` & `tmp/gradio_client-0.1.1.tar.gz`

## Comparing `gradio_client-0.1.0.tar` & `gradio_client-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.0/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.0/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/__init__.py
--rw-r--r--   0        0        0    44631 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/documentation.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/serializing.py
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.0/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/__init__.py
+-rw-r--r--   0        0        0    45076 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/serializing.py
+-rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.1/PKG-INFO
```

### Comparing `gradio_client-0.1.0/README.md` & `gradio_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.0/gradio_client/client.py` & `gradio_client-0.1.1/gradio_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import concurrent.futures
 import json
 import re
 import threading
 import time
 import urllib.parse
 import uuid
+import warnings
 from concurrent.futures import Future, TimeoutError
 from datetime import datetime
 from pathlib import Path
 from threading import Lock
 from typing import Any, Callable, Dict, List, Tuple
 
 import huggingface_hub
 import requests
 import websockets
+from huggingface_hub import SpaceStage
 from huggingface_hub.utils import (
     RepositoryNotFoundError,
     build_hf_headers,
     send_telemetry,
 )
 from packaging import version
 from typing_extensions import Literal
@@ -53,25 +55,28 @@
     """
 
     def __init__(
         self,
         src: str,
         hf_token: str | None = None,
         max_workers: int = 40,
+        serialize: bool = True,
         verbose: bool = True,
     ):
         """
         Parameters:
             src: Either the name of the Hugging Face Space to load, (e.g. "abidlabs/whisper-large-v2") or the full URL (including "http" or "https") of the hosted Gradio app to load (e.g. "http://mydomain.com/app" or "https://bec81a83-5b5c-471e.gradio.live/").
             hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
             max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
+            serialize: Whether the client should serialize the inputs and deserialize the outputs of the remote API. If set to False, the client will pass the inputs and outputs as-is, without serializing/deserializing them. E.g. you if you set this to False, you'd submit an image in base64 format instead of a filepath, and you'd get back an image in base64 format from the remote API instead of a filepath.
             verbose: Whether the client should print statements to the console.
         """
         self.verbose = verbose
         self.hf_token = hf_token
+        self.serialize = serialize
         self.headers = build_hf_headers(
             token=hf_token,
             library_name="gradio_client",
             library_version=utils.__version__,
         )
         self.space_id = None
 
@@ -82,18 +87,18 @@
             if _src is None:
                 raise ValueError(
                     f"Could not find Space: {src}. If it is a private Space, please provide an hf_token."
                 )
             self.space_id = src
         self.src = _src
         state = self._get_space_state()
-        if state == utils.BUILDING_RUNTIME:
+        if state == SpaceStage.BUILDING:
             if self.verbose:
                 print("Space is still building. Please wait...")
-            while self._get_space_state() == utils.BUILDING_RUNTIME:
+            while self._get_space_state() == SpaceStage.BUILDING:
                 time.sleep(2)  # so we don't get rate limited by the API
                 pass
         if state in utils.INVALID_RUNTIME:
             raise ValueError(
                 f"The current space is in the invalid state: {state}. "
                 "Please contact the owner to fix this."
             )
@@ -147,21 +152,21 @@
 
         Parameters:
             from_id: The name of the Hugging Face Space to duplicate in the format "{username}/{space_id}", e.g. "gradio/whisper".
             to_id: The name of the new Hugging Face Space to create, e.g. "abidlabs/whisper-duplicate". If not provided, the new Space will be named "{your_HF_username}/{space_id}".
             hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
             private: Whether the new Space should be private (True) or public (False). Defaults to True.
             hardware: The hardware tier to use for the new Space. Defaults to the same hardware tier as the original Space. Options include "cpu-basic", "cpu-upgrade", "t4-small", "t4-medium", "a10g-small", "a10g-large", "a100-large", subject to availability.
-            secrets: A dictionary of (secret key, secret value) to pass to the new Space. Defaults to None.
+            secrets: A dictionary of (secret key, secret value) to pass to the new Space. Defaults to None. Secrets are only used when the Space is duplicated for the first time, and are not updated if the duplicated Space already exists.
             sleep_timeout: The number of minutes after which the duplicate Space will be puased if no requests are made to it (to minimize billing charges). Defaults to 5 minutes.
             max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
             verbose: Whether the client should print statements to the console.
         """
         try:
-            info = huggingface_hub.get_space_runtime(from_id, token=hf_token)
+            original_info = huggingface_hub.get_space_runtime(from_id, token=hf_token)
         except RepositoryNotFoundError:
             raise ValueError(
                 f"Could not find Space: {from_id}. If it is a private Space, please provide an `hf_token`."
             )
         if to_id:
             if "/" in to_id:
                 to_id = to_id.split("/")[1]
@@ -172,41 +177,48 @@
             )
         try:
             huggingface_hub.get_space_runtime(space_id, token=hf_token)
             if verbose:
                 print(
                     f"Using your existing Space: {utils.SPACE_URL.format(space_id)} 🤗"
                 )
+            if secrets is not None:
+                warnings.warn(
+                    "Secrets are only used when the Space is duplicated for the first time, and are not updated if the duplicated Space already exists."
+                )
         except RepositoryNotFoundError:
             if verbose:
                 print(f"Creating a duplicate of {from_id} for your own use... 🤗")
             huggingface_hub.duplicate_space(
                 from_id=from_id,
                 to_id=space_id,
                 token=hf_token,
                 exist_ok=True,
                 private=private,
             )
+            if secrets is not None:
+                for key, value in secrets.items():
+                    huggingface_hub.add_space_secret(
+                        space_id, key, value, token=hf_token
+                    )
             utils.set_space_timeout(
                 space_id, hf_token=hf_token, timeout_in_seconds=sleep_timeout * 60
             )
             if verbose:
                 print(f"Created new Space: {utils.SPACE_URL.format(space_id)}")
         current_info = huggingface_hub.get_space_runtime(space_id, token=hf_token)
-        current_hardware = current_info.hardware or "cpu-basic"
-        if hardware is None:
-            hardware = info.hardware
+        current_hardware = (
+            current_info.hardware or huggingface_hub.SpaceHardware.CPU_BASIC
+        )
+        hardware = hardware or original_info.hardware
         if not current_hardware == hardware:
             huggingface_hub.request_space_hardware(space_id, hardware)  # type: ignore
             print(
                 f"-------\nNOTE: this Space uses upgraded hardware: {hardware}... see billing info at https://huggingface.co/settings/billing\n-------"
             )
-        if secrets is not None:
-            for key, value in secrets.items():
-                huggingface_hub.add_space_secret(space_id, key, value, token=hf_token)
         if verbose:
             print("")
         client = cls(
             space_id, hf_token=hf_token, max_workers=max_workers, verbose=verbose
         )
         return client
 
@@ -316,52 +328,85 @@
         Example:
             from gradio_client import Client
             client = Client(src="gradio/calculator")
             client.view_api(return_format="dict")
             >> {
                 'named_endpoints': {
                     '/predict': {
-                        'parameters': {
-                            'num1': ['int | float', 'value', 'Number'],
-                            'operation': ['str', 'value', 'Radio'],
-                            'num2': ['int | float', 'value', 'Number']
+                        'parameters': [
+                            {
+                                'label': 'num1',
+                                'type_python': 'int | float',
+                                'type_description': 'numeric value',
+                                'component': 'Number',
+                                'example_input': '5'
                             },
-                        'returns': {
-                            'output': ['int | float', 'value', 'Number']
-                            }
-                        }
+                            {
+                                'label': 'operation',
+                                'type_python': 'str',
+                                'type_description': 'string value',
+                                'component': 'Radio',
+                                'example_input': 'add'
+                            },
+                            {
+                                'label': 'num2',
+                                'type_python': 'int | float',
+                                'type_description': 'numeric value',
+                                'component': 'Number',
+                                'example_input': '5'
+                            },
+                        ],
+                        'returns': [
+                            {
+                                'label': 'output',
+                                'type_python': 'int | float',
+                                'type_description': 'numeric value',
+                                'component': 'Number',
+                            },
+                        ]
                     },
+                    '/flag': {
+                        'parameters': [
+                            ...
+                            ],
+                        'returns': [
+                            ...
+                            ]
+                        }
+                    }
                 'unnamed_endpoints': {
                     2: {
-                        'parameters': {
-                            'parameter_0': ['str', 'value', 'Dataset']
-                            },
-                        'returns': {
-                            'num1': ['int | float', 'value', 'Number'],
-                            'operation': ['str', 'value', 'Radio'],
-                            'num2': ['int | float', 'value', 'Number'],
-                            'output': ['int | float', 'value', 'Number']
-                            }
+                        'parameters': [
+                            ...
+                            ],
+                        'returns': [
+                            ...
+                            ]
                         }
                     }
                 }
             }
 
         """
-        info: Dict[str, Dict[str | int, Dict[str, Dict[str, List[str]]]]] = {
-            "named_endpoints": {},
-            "unnamed_endpoints": {},
-        }
-
-        for endpoint in self.endpoints:
-            if endpoint.is_valid:
-                if endpoint.api_name:
-                    info["named_endpoints"][endpoint.api_name] = endpoint.get_info()
-                else:
-                    info["unnamed_endpoints"][endpoint.fn_index] = endpoint.get_info()
+        if self.serialize:
+            api_info_url = urllib.parse.urljoin(self.src, utils.API_INFO_URL)
+        else:
+            api_info_url = urllib.parse.urljoin(self.src, utils.RAW_API_INFO_URL)
+        r = requests.get(api_info_url, headers=self.headers)
+        if r.ok:
+            info = r.json()
+        else:
+            fetch = requests.post(
+                utils.SPACE_FETCHER_URL,
+                json={"serialize": self.serialize, "config": json.dumps(self.config)},
+            )
+            if fetch.ok:
+                info = fetch.json()["api"]
+            else:
+                raise ValueError(f"Could not fetch api info for {self.src}")
 
         num_named_endpoints = len(info["named_endpoints"])
         num_unnamed_endpoints = len(info["unnamed_endpoints"])
         if num_named_endpoints == 0 and all_endpoints is None:
             all_endpoints = True
 
         human_info = "Client.predict() Usage Info\n---------------------------\n"
@@ -387,43 +432,45 @@
 
     def reset_session(self) -> None:
         self.session_hash = str(uuid.uuid4())
 
     def _render_endpoints_info(
         self,
         name_or_index: str | int,
-        endpoints_info: Dict[str, Dict[str, List[str]]],
+        endpoints_info: Dict[str, List[Dict[str, str]]],
     ) -> str:
-        parameter_names = list(endpoints_info["parameters"].keys())
+        parameter_names = list(p["label"] for p in endpoints_info["parameters"])
+        parameter_names = [utils.sanitize_parameter_names(p) for p in parameter_names]
         rendered_parameters = ", ".join(parameter_names)
         if rendered_parameters:
             rendered_parameters = rendered_parameters + ", "
-        return_value_names = list(endpoints_info["returns"].keys())
-        rendered_return_values = ", ".join(return_value_names)
-        if len(return_value_names) > 1:
+        return_values = list(p["label"] for p in endpoints_info["returns"])
+        return_values = [utils.sanitize_parameter_names(r) for r in return_values]
+        rendered_return_values = ", ".join(return_values)
+        if len(return_values) > 1:
             rendered_return_values = f"({rendered_return_values})"
 
         if isinstance(name_or_index, str):
             final_param = f'api_name="{name_or_index}"'
         elif isinstance(name_or_index, int):
             final_param = f"fn_index={name_or_index}"
         else:
             raise ValueError("name_or_index must be a string or integer")
 
         human_info = f"\n - predict({rendered_parameters}{final_param}) -> {rendered_return_values}\n"
         human_info += "    Parameters:\n"
         if endpoints_info["parameters"]:
-            for label, info in endpoints_info["parameters"].items():
-                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
+            for info in endpoints_info["parameters"]:
+                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {info['type_python']} ({info['type_description']})\n"
         else:
             human_info += "     - None\n"
         human_info += "    Returns:\n"
         if endpoints_info["returns"]:
-            for label, info in endpoints_info["returns"].items():
-                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
+            for info in endpoints_info["returns"]:
+                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {info['type_python']} ({info['type_description']})\n"
         else:
             human_info += "     - None\n"
 
         return human_info
 
     def __repr__(self):
         return self.view_api(print_info=False, return_format="str")
@@ -479,130 +526,80 @@
         if hasattr(self, "executor"):
             self.executor.shutdown(wait=True)
 
     def _space_name_to_src(self, space) -> str | None:
         return huggingface_hub.space_info(space, token=self.hf_token).host  # type: ignore
 
     def _get_config(self) -> Dict:
-        assert self.src is not None
-        r = requests.get(self.src, headers=self.headers)
-        # some basic regex to extract the config
-        result = re.search(r"window.gradio_config = (.*?);[\s]*</script>", r.text)
-        try:
-            config = json.loads(result.group(1))  # type: ignore
-        except AttributeError:
-            raise ValueError(f"Could not get Gradio config from: {self.src}")
-        if "allow_flagging" in config:
-            raise ValueError(
-                "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
-            )
-        return config
+        r = requests.get(
+            urllib.parse.urljoin(self.src, utils.CONFIG_URL), headers=self.headers
+        )
+        if r.ok:
+            return r.json()
+        else:  # to support older versions of Gradio
+            r = requests.get(self.src, headers=self.headers)
+            # some basic regex to extract the config
+            result = re.search(r"window.gradio_config = (.*?);[\s]*</script>", r.text)
+            try:
+                config = json.loads(result.group(1))  # type: ignore
+            except AttributeError:
+                raise ValueError(f"Could not get Gradio config from: {self.src}")
+            if "allow_flagging" in config:
+                raise ValueError(
+                    "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
+                )
+            return config
 
 
 class Endpoint:
     """Helper class for storing all the information about a single API endpoint."""
 
     def __init__(self, client: Client, fn_index: int, dependency: Dict):
         self.client: Client = client
         self.fn_index = fn_index
         self.dependency = dependency
-        self.api_name: str | None = dependency.get("api_name")
-        if self.api_name:
-            self.api_name = "/" + self.api_name
+        api_name = dependency.get("api_name")
+        self.api_name: str | None = None if api_name is None else "/" + api_name
         self.use_ws = self._use_websocket(self.dependency)
         self.input_component_types = []
         self.output_component_types = []
         self.root_url = client.src + "/" if not client.src.endswith("/") else client.src
         try:
             self.serializers, self.deserializers = self._setup_serializers()
             self.is_valid = self.dependency[
                 "backend_fn"
             ]  # Only a real API endpoint if backend_fn is True and serializers are valid
         except AssertionError:
             self.is_valid = False
 
-    def get_info(self) -> Dict[str, Dict[str, List[str]]]:
-        """
-        Dictionary format:
-            {
-                "parameters": {
-                    "parameter_1_name": ["type", "description", "component_type"],
-                    "parameter_2_name": ["type", "description", "component_type"],
-                    ...
-                },
-                "returns": {
-                    "value_1_name": ["type", "description", "component_type"],
-                    ...
-                }
-            }
-        """
-        parameters = {}
-        for i, input in enumerate(self.dependency["inputs"]):
-            for component in self.client.config["components"]:
-                if component["id"] == input:
-                    label = (
-                        component["props"]
-                        .get("label", f"parameter_{i}")
-                        .lower()
-                        .replace(" ", "_")
-                    )
-                    if "info" in component:
-                        info = component["info"]["input"]
-                    else:
-                        info = self.serializers[i].input_api_info()
-                    info = list(info)
-                    component_type = component.get("type", "component").capitalize()
-                    info.append(component_type)
-                    if not component_type.lower() == utils.STATE_COMPONENT:
-                        parameters[label] = info
-        returns = {}
-        for o, output in enumerate(self.dependency["outputs"]):
-            for component in self.client.config["components"]:
-                if component["id"] == output:
-                    label = (
-                        component["props"]
-                        .get("label", f"value_{o}")
-                        .lower()
-                        .replace(" ", "_")
-                    )
-                    if "info" in component:
-                        info = component["info"]["output"]
-                    else:
-                        info = self.deserializers[o].output_api_info()
-                    info = list(info)
-                    component_type = component.get("type", "component").capitalize()
-                    info.append(component_type)
-                    if not component_type.lower() == utils.STATE_COMPONENT:
-                        returns[label] = info
-
-        return {"parameters": parameters, "returns": returns}
-
     def __repr__(self):
-        return json.dumps(self.get_info(), indent=4)
+        return f"Endpoint src: {self.client.src}, api_name: {self.api_name}, fn_index: {self.fn_index}"
 
     def __str__(self):
-        return json.dumps(self.get_info(), indent=4)
+        return self.__repr__()
 
     def make_end_to_end_fn(self, helper: Communicator | None = None):
 
         _predict = self.make_predict(helper)
 
         def _inner(*data):
             if not self.is_valid:
                 raise utils.InvalidAPIEndpointError()
-            inputs = self.serialize(*data)
-            predictions = _predict(*inputs)
-            output = self.deserialize(*predictions)
+            if self.client.serialize:
+                data = self.serialize(*data)
+            predictions = _predict(*data)
+            if self.client.serialize:
+                predictions = self.deserialize(*predictions)
             # Append final output only if not already present
             # for consistency between generators and not generators
             if helper:
                 with helper.lock:
                     if not helper.job.outputs:
-                        helper.job.outputs.append(output)
-            return output
+                        helper.job.outputs.append(predictions)
+            return predictions
 
         return _inner
 
     def make_predict(self, helper: Communicator | None = None):
         def _predict(*data) -> Tuple:
             data = json.dumps(
                 {
```

### Comparing `gradio_client-0.1.0/gradio_client/documentation.py` & `gradio_client-0.1.1/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.0/gradio_client/utils.py` & `gradio_client-0.1.1/gradio_client/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 from threading import Lock
 from typing import Any, Callable, Dict, List, Tuple
 
 import fsspec.asyn
 import httpx
 import huggingface_hub
 import requests
+from huggingface_hub import SpaceStage
 from websockets.legacy.protocol import WebSocketCommonProtocol
 
 API_URL = "/api/predict/"
 WS_URL = "/queue/join"
 UPLOAD_URL = "/upload"
+CONFIG_URL = "/config"
+API_INFO_URL = "/info"
+RAW_API_INFO_URL = "/info?serialize=False"
+SPACE_FETCHER_URL = "https://gradio-space-api-fetcher.hf.space/api"
 RESET_URL = "/reset"
 SPACE_URL = "https://hf.space/{}"
+
 STATE_COMPONENT = "state"
 INVALID_RUNTIME = [
-    "NO_APP_FILE",
-    "CONFIG_ERROR",
-    "BUILD_ERROR",
-    "RUNTIME_ERROR",
-    "PAUSED",
+    SpaceStage.NO_APP_FILE,
+    SpaceStage.CONFIG_ERROR,
+    SpaceStage.BUILD_ERROR,
+    SpaceStage.RUNTIME_ERROR,
+    SpaceStage.PAUSED,
 ]
-BUILDING_RUNTIME = "BUILDING"
 
 __version__ = (pkgutil.get_data(__name__, "version.txt") or b"").decode("ascii").strip()
 
 
 class TooManyRequestsError(Exception):
     """Raised when the API returns a 429 status code."""
 
@@ -54,14 +59,20 @@
 
 class InvalidAPIEndpointError(Exception):
     """Raised when the API endpoint is invalid."""
 
     pass
 
 
+class SpaceDuplicationError(Exception):
+    """Raised when something goes wrong with a Space Duplication."""
+
+    pass
+
+
 class Status(Enum):
     """Status codes presented to client users."""
 
     STARTING = "STARTING"
     JOINING_QUEUE = "JOINING_QUEUE"
     QUEUE_FULL = "QUEUE_FULL"
     IN_QUEUE = "IN_QUEUE"
@@ -314,15 +325,15 @@
     path = str(path)
     if is_valid_url(path):
         return encode_url_to_base64(path)
     else:
         return encode_file_to_base64(path)
 
 
-def decode_base64_to_binary(encoding) -> Tuple[bytes, str | None]:
+def decode_base64_to_binary(encoding: str) -> Tuple[bytes, str | None]:
     extension = get_extension(encoding)
     try:
         data = encoding.split(",")[1]
     except IndexError:
         data = ""
     return base64.b64decode(data), extension
 
@@ -336,15 +347,29 @@
             if len(filename) == 0:
                 break
             filename = filename[:-1]
             filename_len = len(filename.encode())
     return filename
 
 
-def decode_base64_to_file(encoding, file_path=None, dir=None, prefix=None):
+def sanitize_parameter_names(original_param_name: str) -> str:
+    """Strips invalid characters from a parameter name and replaces spaces with underscores."""
+    return (
+        "".join([char for char in original_param_name if char.isalnum() or char in " "])
+        .replace(" ", "_")
+        .lower()
+    )
+
+
+def decode_base64_to_file(
+    encoding: str,
+    file_path: str | None = None,
+    dir: str | Path | None = None,
+    prefix: str | None = None,
+):
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
     data, extension = decode_base64_to_binary(encoding)
     if file_path is not None and prefix is None:
         filename = Path(file_path).name
         prefix = filename
         if "." in filename:
@@ -364,29 +389,29 @@
             dir=dir,
         )
     file_obj.write(data)
     file_obj.flush()
     return file_obj
 
 
-def dict_or_str_to_json_file(jsn, dir=None):
+def dict_or_str_to_json_file(jsn: str | Dict | List, dir: str | Path | None = None):
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
 
     file_obj = tempfile.NamedTemporaryFile(
         delete=False, suffix=".json", dir=dir, mode="w+"
     )
     if isinstance(jsn, str):
         jsn = json.loads(jsn)
     json.dump(jsn, file_obj)
     file_obj.flush()
     return file_obj
 
 
-def file_to_json(file_path: str | Path) -> Dict:
+def file_to_json(file_path: str | Path) -> Dict | List:
     with open(file_path) as f:
         return json.load(f)
 
 
 ###########################
 # HuggingFace Hub API Utils
 ###########################
@@ -396,19 +421,27 @@
     timeout_in_seconds: int = 300,
 ):
     headers = huggingface_hub.utils.build_hf_headers(
         token=hf_token,
         library_name="gradio_client",
         library_version=__version__,
     )
-    requests.post(
+    r = requests.post(
         f"https://huggingface.co/api/spaces/{space_id}/sleeptime",
         json={"seconds": timeout_in_seconds},
         headers=headers,
     )
+    print("r", r, r.status_code)
+    try:
+        huggingface_hub.utils.hf_raise_for_status(r)
+    except huggingface_hub.utils.HfHubHTTPError:
+        raise SpaceDuplicationError(
+            f"Could not set sleep timeout on duplicated Space. Please visit {SPACE_URL.format(space_id)} "
+            "to set a timeout manually to reduce billing charges."
+        )
 
 
 ########################
 # Misc utils
 ########################
```

### Comparing `gradio_client-0.1.0/.gitignore` & `gradio_client-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.0/pyproject.toml` & `gradio_client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.0/PKG-INFO` & `gradio_client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

