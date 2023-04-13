# Comparing `tmp/gradio_client-0.1.1.tar.gz` & `tmp/gradio_client-0.1.2b1.tar.gz`

## Comparing `gradio_client-0.1.1.tar` & `gradio_client-0.1.2b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.1/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.1/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/__init__.py
--rw-r--r--   0        0        0    45076 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/media_data.py
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/serializing.py
--rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.1/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.1/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/__init__.py
+-rw-r--r--   0        0        0    45304 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/serializing.py
+-rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/utils.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/PKG-INFO
```

### Comparing `gradio_client-0.1.1/README.md` & `gradio_client-0.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.1/gradio_client/client.py` & `gradio_client-0.1.2b1/gradio_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,21 @@
 
         """
         if self.serialize:
             api_info_url = urllib.parse.urljoin(self.src, utils.API_INFO_URL)
         else:
             api_info_url = urllib.parse.urljoin(self.src, utils.RAW_API_INFO_URL)
         r = requests.get(api_info_url, headers=self.headers)
-        if r.ok:
+
+        # Versions of Gradio older than 3.26 returned format of the API info
+        # from the /info endpoint
+        if (
+            version.parse(self.config.get("version", "2.0")) >= version.Version("3.26")
+            and r.ok
+        ):
             info = r.json()
         else:
             fetch = requests.post(
                 utils.SPACE_FETCHER_URL,
                 json={"serialize": self.serialize, "config": json.dumps(self.config)},
             )
             if fetch.ok:
```

### Comparing `gradio_client-0.1.1/gradio_client/documentation.py` & `gradio_client-0.1.2b1/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.1/gradio_client/media_data.py` & `gradio_client-0.1.2b1/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.1/gradio_client/serializing.py` & `gradio_client-0.1.2b1/gradio_client/serializing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from __future__ import annotations
 
 import json
 import os
 import uuid
-from abc import ABC, abstractmethod
+from abc import ABC
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 from gradio_client import media_data, utils
 from gradio_client.data_classes import FileData
 
 
 class Serializable(ABC):
-    @abstractmethod
     def api_info(self) -> Dict[str, List[str]]:
         """
         The typing information for this component as a dictionary whose values are a list of 2 strings: [Python type, language-agnostic description].
         Keys of the dictionary are: raw_input, raw_output, serialized_input, serialized_output
         """
-        pass
+        raise NotImplementedError()
 
-    @abstractmethod
     def example_inputs(self) -> Dict[str, Any]:
         """
         The example inputs for this component as a dictionary whose values are example inputs compatible with this component.
         Keys of the dictionary are: raw, serialized
         """
+        raise NotImplementedError()
+
+    # For backwards compatibility
+    def input_api_info(self) -> Tuple[str, str]:
+        api_info = self.api_info()
+        return (api_info["serialized_input"][0], api_info["serialized_input"][1])
+
+    # For backwards compatibility
+    def output_api_info(self) -> Tuple[str, str]:
+        api_info = self.api_info()
+        return (api_info["serialized_output"][0], api_info["serialized_output"][1])
 
     def serialize(self, x: Any, load_dir: str | Path = ""):
         """
         Convert data from human-readable format to serialized format for a browser.
         """
         return x
```

### Comparing `gradio_client-0.1.1/gradio_client/utils.py` & `gradio_client-0.1.2b1/gradio_client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,14 @@
         library_version=__version__,
     )
     r = requests.post(
         f"https://huggingface.co/api/spaces/{space_id}/sleeptime",
         json={"seconds": timeout_in_seconds},
         headers=headers,
     )
-    print("r", r, r.status_code)
     try:
         huggingface_hub.utils.hf_raise_for_status(r)
     except huggingface_hub.utils.HfHubHTTPError:
         raise SpaceDuplicationError(
             f"Could not set sleep timeout on duplicated Space. Please visit {SPACE_URL.format(space_id)} "
             "to set a timeout manually to reduce billing charges."
         )
```

### Comparing `gradio_client-0.1.1/.gitignore` & `gradio_client-0.1.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.1/pyproject.toml` & `gradio_client-0.1.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.1/PKG-INFO` & `gradio_client-0.1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.1.1
+Version: 0.1.2b1
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

