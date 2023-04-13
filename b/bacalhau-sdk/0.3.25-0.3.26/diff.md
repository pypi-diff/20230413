# Comparing `tmp/bacalhau_sdk-0.3.25.tar.gz` & `tmp/bacalhau_sdk-0.3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_sdk-0.3.25.tar", max compression
+gzip compressed data, was "bacalhau_sdk-0.3.26.tar", max compression
```

## Comparing `bacalhau_sdk-0.3.25.tar` & `bacalhau_sdk-0.3.26.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10247 2023-03-21 22:35:25.900689 bacalhau_sdk-0.3.25/LICENSE
--rw-r--r--   0        0        0     7400 2023-03-21 22:35:25.900689 bacalhau_sdk-0.3.25/README.md
--rw-r--r--   0        0        0      133 2023-03-21 22:35:25.900689 bacalhau_sdk-0.3.25/bacalhau_sdk/__init__.py
--rw-r--r--   0        0        0     3031 2023-03-21 22:36:05.617029 bacalhau_sdk-0.3.25/bacalhau_sdk/api.py
--rw-r--r--   0        0        0     5375 2023-03-21 22:36:06.369047 bacalhau_sdk-0.3.25/bacalhau_sdk/config.py
--rw-r--r--   0        0        0     2745 2023-03-21 22:36:31.989351 bacalhau_sdk-0.3.25/pyproject.toml
--rw-r--r--   0        0        0       42 2023-03-21 22:35:25.900689 bacalhau_sdk-0.3.25/tests/__init__.py
--rw-r--r--   0        0        0     6721 2023-03-21 22:35:25.900689 bacalhau_sdk-0.3.25/tests/test_config.py
--rw-r--r--   0        0        0     9256 1970-01-01 00:00:00.000000 bacalhau_sdk-0.3.25/PKG-INFO
+-rw-r--r--   0        0        0    10247 2023-04-13 11:42:00.866649 bacalhau_sdk-0.3.26/LICENSE
+-rw-r--r--   0        0        0     7459 2023-04-13 11:42:00.866649 bacalhau_sdk-0.3.26/README.md
+-rw-r--r--   0        0        0      133 2023-04-13 11:42:00.866649 bacalhau_sdk-0.3.26/bacalhau_sdk/__init__.py
+-rw-r--r--   0        0        0     3020 2023-04-13 11:42:00.866649 bacalhau_sdk-0.3.26/bacalhau_sdk/api.py
+-rw-r--r--   0        0        0     5375 2023-04-13 11:42:00.866649 bacalhau_sdk-0.3.26/bacalhau_sdk/config.py
+-rw-r--r--   0        0        0     2745 2023-04-13 11:58:23.183951 bacalhau_sdk-0.3.26/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-04-13 11:42:00.870649 bacalhau_sdk-0.3.26/tests/__init__.py
+-rw-r--r--   0        0        0     6721 2023-04-13 11:42:00.870649 bacalhau_sdk-0.3.26/tests/test_config.py
+-rw-r--r--   0        0        0     9315 1970-01-01 00:00:00.000000 bacalhau_sdk-0.3.26/PKG-INFO
```

### Comparing `bacalhau_sdk-0.3.25/LICENSE` & `bacalhau_sdk-0.3.26/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.25/README.md` & `bacalhau_sdk-0.3.26/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 * List, create and inspect Bacalhau jobs using Python objects :balloon:
 * Use the production network, or set the following environment variables to target any Bacalhau network out there:
     * `BACALHAU_API_HOST`
     * `BACALHAU_API_PORT`
 * Generate a key pair used to sign requests stored in the path specified by the `BACALHAU_DIR` env var (default: `~/.bacalhau`)
 ## Install
 
+### From PyPi:
+
+```console
+$ pip install bacalhau-sdk
+```
+
 ### From source:
 
 Clone the public repository:
 
 ``` console
 $ git clone https://github.com/bacalhau-project/bacalhau/
 ```
```

### Comparing `bacalhau_sdk-0.3.25/bacalhau_sdk/api.py` & `bacalhau_sdk-0.3.26/bacalhau_sdk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     sanitized_data = client.sanitize_for_serialization(data)
     json_data = json.dumps(sanitized_data, indent=None, separators=(", ", ": "))
     json_bytes = json_data.encode("utf-8")
     signature = sign_for_client(json_bytes)
     client_public_key = get_client_public_key()
     submit_req = SubmitRequest(
         client_public_key=client_public_key,
-        job_create_payload=sanitized_data,
+        payload=sanitized_data,
         signature=signature,
     )
     return api_instance.submit(submit_req)
 
 
 def list():
     """List all jobs."""
```

### Comparing `bacalhau_sdk-0.3.25/bacalhau_sdk/config.py` & `bacalhau_sdk-0.3.26/bacalhau_sdk/config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.25/pyproject.toml` & `bacalhau_sdk-0.3.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "bacalhau-sdk"
-version = "0.3.25"
+version = "0.3.26"
 homepage = "https://github.com/bacalhau-project/bacalhau/"
 repository = "https://github.com/bacalhau-project/bacalhau/"
 documentation = "https://docs.bacalhau.org/"
 keywords = ["bacalhau", "Filecoin", "IPFS", "cod", "compute over data", "verifiable computation"]
 description = "Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin."
 authors = ["Enrico Rotundo <team@bacalhau.org>"]
 readme = "README.md"
```

### Comparing `bacalhau_sdk-0.3.25/tests/test_config.py` & `bacalhau_sdk-0.3.26/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.25/PKG-INFO` & `bacalhau_sdk-0.3.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-sdk
-Version: 0.3.25
+Version: 0.3.26
 Summary: Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin.
 Home-page: https://github.com/bacalhau-project/bacalhau/
 License: Apache-2.0
 Keywords: bacalhau,Filecoin,IPFS,cod,compute over data,verifiable computation
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 Requires-Python: >=3.8.1,<3.12
@@ -55,14 +55,20 @@
 * List, create and inspect Bacalhau jobs using Python objects :balloon:
 * Use the production network, or set the following environment variables to target any Bacalhau network out there:
     * `BACALHAU_API_HOST`
     * `BACALHAU_API_PORT`
 * Generate a key pair used to sign requests stored in the path specified by the `BACALHAU_DIR` env var (default: `~/.bacalhau`)
 ## Install
 
+### From PyPi:
+
+```console
+$ pip install bacalhau-sdk
+```
+
 ### From source:
 
 Clone the public repository:
 
 ``` console
 $ git clone https://github.com/bacalhau-project/bacalhau/
 ```
```

