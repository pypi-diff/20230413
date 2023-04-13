# Comparing `tmp/twinlab-0.0.0.tar.gz` & `tmp/twinlab-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-0.0.0.tar", max compression
+gzip compressed data, was "twinlab-0.0.1.tar", max compression
```

## Comparing `twinlab-0.0.0.tar` & `twinlab-0.0.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1048 2023-04-11 13:00:56.988184 twinlab-0.0.0/README.md
--rw-r--r--   0        0        0      599 2023-04-11 13:02:25.939143 twinlab-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      512 2023-04-11 13:00:57.064400 twinlab-0.0.0/twinlab/__init__.py
--rw-r--r--   0        0        0     5388 2023-04-11 13:02:54.913146 twinlab-0.0.0/twinlab/client.py
--rw-r--r--   0        0        0      532 2023-04-05 20:53:11.331012 twinlab-0.0.0/twinlab/settings.py
--rw-r--r--   0        0        0     2981 2023-04-11 13:00:57.066914 twinlab-0.0.0/twinlab/utils.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-04-11 13:00:56.988184 twinlab-0.0.1/README.md
+-rw-r--r--   0        0        0      599 2023-04-13 18:59:14.918264 twinlab-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      567 2023-04-13 18:03:34.457859 twinlab-0.0.1/twinlab/__init__.py
+-rw-r--r--   0        0        0     5314 2023-04-13 18:03:34.464734 twinlab-0.0.1/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-04-13 18:03:34.464988 twinlab-0.0.1/twinlab/plotting.py
+-rw-r--r--   0        0        0      532 2023-04-05 20:53:11.331012 twinlab-0.0.1/twinlab/settings.py
+-rw-r--r--   0        0        0     3846 2023-04-13 18:03:34.469148 twinlab-0.0.1/twinlab/utils.py
+-rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-0.0.1/PKG-INFO
```

### Comparing `twinlab-0.0.0/README.md` & `twinlab-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-0.0.0/pyproject.toml` & `twinlab-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "0.0.0"
+version = "0.0.1"
 description = "Client interface for twinLab"
 authors = ["Alexander Mead <alexander@digilab.co.uk>", "Freddy Wordingham <freddy@digilab.co.uk>"]
 repository = "https://github.com/digiLab-ai/twinLab-client"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
```

### Comparing `twinlab-0.0.0/twinlab/__init__.py` & `twinlab-0.0.1/twinlab/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Utility functions
 from .utils import get_command_line_args
 
 # API dataset functions
+from .client import upload_big_dataset
 from .client import upload_dataset
 from .client import query_dataset
 from .client import list_datasets
 from .client import delete_dataset
 
 # API campaign functions
 from .client import train_campaign
 from .client import query_campaign
 from .client import sample_campaign
 from .client import list_campaigns
 from .client import delete_campaign
 
 # Plotting functions
-from .utils import get_boundaries
-from .utils import get_alpha
+from .plotting import get_blur_boundaries
+from .plotting import get_blur_alpha
```

### Comparing `twinlab-0.0.0/twinlab/client.py` & `twinlab-0.0.1/twinlab/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,53 @@
 # Third-party imports
 import requests
 import pandas as pd
 
 # Project imports
 from . import utils
 
+### Dataset functions ###
 
-def upload_dataset(training_file: str, server="cloud", verbose=False) -> None:
+
+def upload_dataset(filepath: str, server="cloud", verbose=False) -> None:
     """
     Upload dataset
+    TODO: Retire in favour of upload_big_dataset?
     """
     url = utils.get_server_url(server) + "/upload_dataset"
-    files = {"file": (training_file, open(training_file, "rb"), "text/csv")}
+    files = {"file": (filepath, open(filepath, "rb"), "text/csv")}
     headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
     r = requests.post(url, files=files, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
 
 
+def upload_big_dataset(filepath: str, server="cloud", verbose=False) -> None:
+    """
+    Upload big dataset
+    TODO: Replace upload_dataset with this?
+    """
+    lambda_url = utils.get_server_url(server) + "/generate_upload_url"
+    headers = utils.STANDARD_HEADERS.copy()  #  TODO: Is .copy() necessary?
+    headers["X-Dataset"] = filepath
+    r = requests.get(lambda_url, headers=headers)
+    utils.check_response(r)
+    if verbose:
+        utils.print_response_message(r)
+    upload_url = r.json()["url"]
+    print(f"Uploading {filepath} to {upload_url}. \n")
+    utils.upload_file_to_presigned_url(
+        filepath, upload_url, verbose=verbose)
+    process_url = utils.get_server_url(server) + "/process_uploaded_dataset"
+    r = requests.post(process_url, headers=headers)
+    if verbose:
+        utils.print_response_message(r)
+
+
 def query_dataset(dataset: str, server="cloud", verbose=False) -> pd.DataFrame:
     """
     Query dataset
     """
     url = utils.get_server_url(server) + "/query_dataset"
     headers = utils.STANDARD_HEADERS.copy()
     headers["X-Dataset"] = dataset
@@ -44,28 +69,34 @@
     """
     url = utils.get_server_url(server) + "/list_datasets"
     headers = utils.STANDARD_HEADERS.copy()
     r = requests.get(url, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
+    response = r.json()
+    return response["datasets"]
 
 
 def delete_dataset(dataset: str, server="cloud", verbose=False) -> None:
     """
     Delete campaign directory from S3
     """
     url = utils.get_server_url(server) + "/delete_dataset"
     headers = utils.STANDARD_HEADERS.copy()
     headers["X-Dataset"] = dataset
     r = requests.post(url, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
 
+###  ###
+
+### Campaign functions ###
+
 
 def train_campaign(params: dict, campaign: str, server="cloud", verbose=False) -> None:
     """
     Train campaign
     TODO: Set default train_test_split?
     """
     url = utils.get_server_url(server) + "/train_campaign"
@@ -86,28 +117,30 @@
     headers["X-Campaign"] = campaign
     r = requests.get(url, headers=headers)
     utils.check_response(r)
     metadata = utils.extract_item_from_response(r, "metadata")
     if verbose:
         utils.print_response_message(r)
         print("Metadata:")
-        pprint(metadata)
+        pprint(metadata, compact=True, sort_dicts=False)
     return metadata
 
 
 def list_campaigns(server="cloud", verbose=False) -> list:
     """
     List campaigns in S3
     """
     url = utils.get_server_url(server) + "/list_campaigns"
     headers = utils.STANDARD_HEADERS.copy()
     r = requests.get(url, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
+    response = r.json()
+    return response["campaigns"]
 
 
 def sample_campaign(
     test_file: str, campaign: str, server="cloud", verbose=False
 ) -> tuple:
     """
     Sample campaign
@@ -133,50 +166,8 @@
     """
     url = utils.get_server_url(server) + "/delete_campaign"
     headers = utils.STANDARD_HEADERS.copy()
     headers["X-Campaign"] = campaign
     r = requests.post(url, headers=headers)
     utils.check_response(r)
     if verbose:
-        utils.print_response_text(r)
-
-
-def delete_dataset(dataset: str, server="cloud", verbose=False) -> None:
-    """
-    Delete campaign directory from S3
-    """
-    url = utils.get_server_url(server) + "/delete_dataset"
-    headers = utils.STANDARD_HEADERS.copy()
-    headers["X-Dataset"] = dataset
-    r = requests.post(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_text(r)
-
-
-def list_campaigns(server="cloud", verbose=False) -> list:
-    """
-    List campaigns in S3
-    """
-    url = utils.get_server_url(server) + "/list_campaigns"
-    headers = utils.STANDARD_HEADERS.copy()
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_text(r)
-
-    response = r.json()
-    return response["campaign_ids"]
-
-
-def list_datasets(server="cloud", verbose=False) -> list:
-    """
-    List datasets in S3
-    """
-    url = utils.get_server_url(server) + "/list_datasets"
-    headers = utils.STANDARD_HEADERS.copy()
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_text(r)
-    response = r.json()
-    return response["datasets"]
+        utils.print_response_message(r)
```

### Comparing `twinlab-0.0.0/twinlab/settings.py` & `twinlab-0.0.1/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-0.0.0/twinlab/utils.py` & `twinlab-0.0.1/twinlab/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 # Standard imports
 import argparse
 import json
 from pprint import pprint
 
 # Third-party imports
 import requests
-import numpy as np
 import pandas as pd
 
 # Project imports
 from .settings import ENV
 
 STANDARD_HEADERS = {
     "X-Group": ENV.GROUP_NAME,
     "X-User": ENV.USER_NAME,
 }
 
-### Plotting ###
-
-
-def get_boundaries(n: int) -> np.ndarray:
-    """
-    Get boundaries for making a nice probability distribution of a Gaussian
-    """
-    frac = 1./(2.*(n+1.))
-    fmin, fmax = frac, 1.-frac
-    f = np.linspace(fmin, fmax, n)
-    dy = -np.sqrt(2.)*np.log(f)
-    return dy
-
-
-def get_alpha(n: int, alpha_mid=0.99) -> float:
-    """
-    Get a sensible alpha value for a given number of samples
-    """
-    alpha = 1.-(1.-alpha_mid)**(1/n)
-    return alpha
+### Utility functions ###
 
-###  ###
 
-### Utility functions ###
+# def unwrap_payload(event: dict) -> dict:
+#     """
+#     Return payload and decode if it is base64 encoded
+#     TODO: Not used yet...
+#     """
+#     if "body" not in event:  # Get body
+#         raise Exception("No body in request")
+#     body = event["body"]
+#     if "isBase64Encoded" in event:  # Decode
+#         if event["isBase64Encoded"]:
+#             body = base64.b64decode(body)
+#     try:  # Parse
+#         payload = json.loads(body)
+#     except:
+#         raise Exception("Could not parse body as JSON")
+#     return payload
 
 
 def get_command_line_args() -> argparse.Namespace:
     """
     Parse command-line arguments
     """
     parser = argparse.ArgumentParser()
@@ -70,14 +64,36 @@
     return baseURL
 
 ### ###
 
 ### HTTP requests ###
 
 
+def upload_file_to_presigned_url(file_path, presigned_url, verbose=False):
+    """
+    Upload a file to the specified pre-signed URL.
+
+    :param file_path: The path to the file you want to upload.
+    :param presigned_url: The pre-signed URL generated for uploading the file.
+    :return: True if the upload is successful, False otherwise.
+    """
+
+    with open(file_path, "rb") as file:
+        headers = {"Content-Type": "application/octet-stream"}
+        response = requests.put(presigned_url, data=file, headers=headers)
+    if verbose:
+        if response.status_code == 200:
+            print(f"File {file_path} uploaded successfully.")
+        else:
+            print(f"File upload failed")
+            print(f"Status code: {response.status_code}")
+            print(f"Reason: {response.text}")
+        print()
+
+
 def extract_csv_from_response(response: requests.Response, name: str) -> pd.DataFrame:
     """
     Extract CSV from response
     """
     body = response.json()  # Get the body of the response as a dictionary
     data = body[name]  # Get the entry corresponding to the field name
     df = pd.read_json(data, orient="split")
@@ -118,10 +134,10 @@
     print()
 
 
 def check_response(r: requests.Response) -> None:
     if r.status_code != 200:
         print("Status code:", r.status_code)
         print_response_message(r)
-        raise RuntimeError("Response error")\
+        raise RuntimeError("Response error")
 
 ### ###
```

### Comparing `twinlab-0.0.0/PKG-INFO` & `twinlab-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 0.0.0
+Version: 0.0.1
 Summary: Client interface for twinLab
 Home-page: https://github.com/digiLab-ai/twinLab-client
 Author: Alexander Mead
 Author-email: alexander@digilab.co.uk
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

