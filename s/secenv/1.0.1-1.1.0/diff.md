# Comparing `tmp/secenv-1.0.1.tar.gz` & `tmp/secenv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secenv-1.0.1.tar", last modified: Wed Mar 29 09:15:46 2023, max compression
+gzip compressed data, was "secenv-1.1.0.tar", last modified: Thu Apr 13 12:24:31 2023, max compression
```

## Comparing `secenv-1.0.1.tar` & `secenv-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.693184 secenv-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-03-29 09:14:44.000000 secenv-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    50212 2023-03-29 09:15:46.693184 secenv-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8953 2023-03-29 09:14:44.000000 secenv-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1161 2023-03-29 09:15:17.000000 secenv-1.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.689184 secenv-1.0.1/secenv/
--rw-rw-rw-   0 root         (0) root         (0)     8424 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3750 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.689184 secenv-1.0.1/secenv/contexts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/contexts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/contexts/aws_assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.693184 secenv-1.0.1/secenv/stores/
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3169 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/aws.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/env.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/pass.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/scaleway.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/stores/vault.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-03-29 09:14:44.000000 secenv-1.0.1/secenv/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.689184 secenv-1.0.1/secenv.egg-info/
--rw-r--r--   0 root         (0) root         (0)    50212 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      699 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-29 09:15:46.000000 secenv-1.0.1/secenv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 09:15:46.693184 secenv-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-29 09:14:44.000000 secenv-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:15:46.693184 secenv-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_config_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_context_output.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_gen_context.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_list_contexts.py
--rw-rw-rw-   0 root         (0) root         (0)    10980 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-03-29 09:14:44.000000 secenv-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-13 12:23:58.000000 secenv-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-04-13 12:24:31.913085 secenv-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8953 2023-04-13 12:23:58.000000 secenv-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-13 12:23:59.000000 secenv-1.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/secenv/
+-rw-rw-rw-   0 root         (0) root         (0)     8556 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3750 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/secenv/contexts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/contexts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/contexts/aws_assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/secenv/stores/
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/pass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/scaleway.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/stores/vault.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-04-13 12:23:58.000000 secenv-1.1.0/secenv/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/secenv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 12:24:31.000000 secenv-1.1.0/secenv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:24:31.913085 secenv-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-13 12:23:58.000000 secenv-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:24:31.913085 secenv-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_config_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_context_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_fill_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_gen_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_list_contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)    10980 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-13 12:23:58.000000 secenv-1.1.0/tests/test_utils.py
```

### Comparing `secenv-1.0.1/LICENSE` & `secenv-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/PKG-INFO` & `secenv-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.0.1
+Version: 1.1.0
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.0.1/README.md` & `secenv-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/pyproject.toml` & `secenv-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "secenv"
-version = "1.0.1"
+version = "1.1.0"
 description = "An utility tool to list, read and fill secrets from multiple stores."
 readme = "README.md"
 authors = [{ name = "Keltio Labs", email = "labs@keltio.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `secenv-1.0.1/secenv/__init__.py` & `secenv-1.1.0/secenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,20 @@
             print(f"Config error: store '{secret_config['store']}' not found")
             sys.exit(1)
 
         store = stores[secret_config["store"]]
         secret = {k: v for k, v in secret_config.items() if k not in ["store"]}
         fill_secret(store, secret)
 
+    import os
+
+    for env in os.environ:
+        if env.startswith("MY_ENV"):
+            print(env + ": " + os.environ.get(env))
+
 
 def gen_context(name: str, stores: Dict[str, StoreInterface]) -> Dict[str, str]:
     """
     Generate the context specified in the configuration object.
 
     Args:
         name (str): Name of the context to generate
```

### Comparing `secenv-1.0.1/secenv/context.py` & `secenv-1.1.0/secenv/context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/secenv/contexts/aws_assume_role.py` & `secenv-1.1.0/secenv/contexts/aws_assume_role.py`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/secenv/stores/aws.py` & `secenv-1.1.0/secenv/stores/aws.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import boto3
 import json
 import os
-from . import EnvPrefix, StoreInterface, cached, ask_secret, SecretNotFoundError
+from . import (
+    EnvPrefix,
+    StoreInterface,
+    cached,
+    ask_secret,
+    SecretNotFoundError,
+    generate_secret,
+)
 
 
 # This dictionary is used to store the ARN of a secret given its name.
 _secrets_arns = {}
 
 
 class Store(StoreInterface):
@@ -72,20 +79,25 @@
 
         _secrets_arns[secret] = value["ARN"]
         return value["SecretString"]
 
     def filter(self, secret, key):
         return json.loads(secret)[key]
 
-    def fill_secret(self, secret, keys=[]):
+    def fill_secret(self, secret, keys=[], generate=None):
         if keys:
             values = {}
             for key in keys:
-                values[key] = ask_secret(self.name, secret, key)
+                if generate:
+                    values[key] = generate_secret(generate)
+                else:
+                    values[key] = ask_secret(self.name, secret, key)
             secret_value = json.dumps(values)
+        elif generate:
+            secret_value = generate_secret(generate)
         else:
             secret_value = ask_secret(self.name, secret)
 
         if secret in _secrets_arns:
             # Update secret
             arn = _secrets_arns[secret]
```

### Comparing `secenv-1.0.1/secenv/stores/azure.py` & `secenv-1.1.0/secenv/stores/azure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from azure.keyvault.secrets import SecretClient
 from azure.identity import DefaultAzureCredential
 from azure.core.exceptions import ResourceNotFoundError
-from . import StoreInterface, cached, ask_secret, SecretNotFoundError
+
+from . import StoreInterface, cached, ask_secret, SecretNotFoundError, generate_secret
 
 
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
         key_vault = super().get_from_config(name, "key_vault", infos)
 
@@ -22,10 +23,13 @@
     def read_secret(self, secret):
         try:
             res = self.client.get_secret(secret).value
         except ResourceNotFoundError:
             raise SecretNotFoundError(self.name, secret)
         return res
 
-    def fill_secret(self, secret):
-        secret_value = ask_secret(self.name, secret)
+    def fill_secret(self, secret, generate=None):
+        if generate:
+            secret_value = generate_secret(generate)
+        else:
+            secret_value = ask_secret(self.name, secret)
         self.client.set_secret(secret, secret_value)
```

### Comparing `secenv-1.0.1/secenv/stores/bitwarden.py` & `secenv-1.1.0/secenv/stores/bitwarden.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,9 @@
             if "no entry found" in stderr:
                 raise SecretNotFoundError(self.name, secret)
             raise Exception(
                 f"bitwarden store '{self.name}': rbw error during execution: {stderr}"
             )
         return result.stdout.strip().decode("utf-8")
 
-    def fill_secret(self, secret):
+    def fill_secret(self, secret, generate=None):
         raise Exception("Can't write secrets to Bitwarden for now.")
```

### Comparing `secenv-1.0.1/secenv/stores/gcp.py` & `secenv-1.1.0/secenv/stores/gcp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import google.api_core.exceptions
 from google.cloud import secretmanager
-from . import StoreInterface, cached, ask_secret, SecretNotFoundError
+from . import StoreInterface, cached, ask_secret, SecretNotFoundError, generate_secret
 
 
 def _setup_creds(fn):
     def inner(*args, **kwargs):
         # args[0] == self
         creds = args[0]._creds
         if creds:
@@ -48,16 +48,19 @@
             secret_obj = self.client.access_secret_version(request={"name": name})
         except google.api_core.exceptions.NotFound:
             raise SecretNotFoundError(self.name, secret)
 
         self._existing_secrets[secret] = True
         return secret_obj.payload.data.decode()
 
-    def fill_secret(self, secret):
-        secret_value = ask_secret(self.name, secret)
+    def fill_secret(self, secret, generate=None):
+        if generate:
+            secret_value = generate_secret(generate)
+        else:
+            secret_value = ask_secret(self.name, secret)
 
         if secret not in self._existing_secrets:
             self.client.create_secret(
                 request={
                     "parent": f"projects/{self.project_id}",
                     "secret_id": secret,
                     "secret": {"replication": {"automatic": {}}},
```

### Comparing `secenv-1.0.1/secenv/stores/pass.py` & `secenv-1.1.0/secenv/stores/pass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import passpy
-from . import StoreInterface, cached, ask_secret, SecretNotFoundError
+from . import StoreInterface, cached, ask_secret, SecretNotFoundError, generate_secret
 
 
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
         directory = super().get_from_config(
             name, "directory", infos, default="~/.password-store"
@@ -17,10 +17,13 @@
     def read_secret(self, secret):
         res = self.store.get_key(secret)
         if res:
             return res
         else:
             raise SecretNotFoundError(self.name, secret)
 
-    def fill_secret(self, secret):
-        value = ask_secret(self.name, secret)
-        self.store.set_key(secret, value, force=True)
+    def fill_secret(self, secret, generate=None):
+        if generate:
+            secret_value = generate_secret(generate)
+        else:
+            secret_value = ask_secret(self.name, secret)
+        self.store.set_key(secret, secret_value, force=True)
```

### Comparing `secenv-1.0.1/secenv/stores/scaleway.py` & `secenv-1.1.0/secenv/stores/scaleway.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import json
 import requests
 
-from . import StoreInterface, ask_secret, cached, SecretNotFoundError
+from . import StoreInterface, ask_secret, cached, SecretNotFoundError, generate_secret
 
 
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
         region = super().get_from_config(name, "region", infos)
         self.project_id = super().get_from_config(name, "project_id", infos)
@@ -49,20 +49,25 @@
         if "type" in ret and ret["type"] == "not_found":
             raise SecretNotFoundError(self.name, secret)
         return base64.b64decode(ret["data"]).decode()
 
     def filter(self, secret, key):
         return json.loads(secret)[key]
 
-    def fill_secret(self, secret, keys=[]):
+    def fill_secret(self, secret, keys=[], generate=None):
         if keys:
             values = {}
             for key in keys:
-                values[key] = ask_secret(self.name, secret, key)
+                if generate:
+                    values[key] = generate_secret(generate)
+                else:
+                    values[key] = ask_secret(self.name, secret, key)
             secret_value = json.dumps(values)
+        elif generate:
+            secret_value = generate_secret(generate)
         else:
             secret_value = ask_secret(self.name, secret)
 
         try:
             uid = self._name_to_uid(secret)
         except Exception:
             # except SecretNotFoundError:
```

### Comparing `secenv-1.0.1/secenv/stores/vault.py` & `secenv-1.1.0/secenv/stores/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hvac
 import hvac.exceptions
-from . import StoreInterface, ask_secret, cached, SecretNotFoundError
+from . import StoreInterface, ask_secret, cached, SecretNotFoundError, generate_secret
 
 
 class Store(StoreInterface):
     def __init__(self, name, infos):
         self.name = name
         self.url = super().get_from_config(name, "url", infos)
         self.token = super().get_from_config(name, "token", infos)
@@ -27,19 +27,24 @@
             raise Exception(f"vault store '{self.name}': error during execution: {e}")
 
         return read_response
 
     def filter(self, secret, key):
         return secret["data"]["data"][key]
 
-    def fill_secret(self, secret, engine="", keys=[]):
+    def fill_secret(self, secret, engine="", keys=[], generate=None):
         if keys:
             values = {}
             for key in keys:
-                values[key] = ask_secret(self.name, secret, key)
+                if generate:
+                    values[key] = generate_secret(generate)
+                else:
+                    values[key] = ask_secret(self.name, secret, key)
             secret_value = values
+        elif generate:
+            secret_value = {secret: generate_secret(generate)}
         else:
             secret_value = {secret: ask_secret(self.name, secret)}
 
         self.client.secrets.kv.create_or_update_secret(
             path=secret, mount_point=engine, secret=secret_value
         )
```

### Comparing `secenv-1.0.1/secenv/utils.py` & `secenv-1.1.0/secenv/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from enum import Enum
+
+
 def escape(s) -> str:
     s = repr(str(s))
     if "$" in s and s[0] == '"':
         # "$" -> "\$"
         s = s.replace("$", "\\$")
     if "\\'" in s and s[0] == "'":
         # '\'' -> ''"'"''
@@ -30,10 +33,33 @@
 
 def yes_no(ask):
     return input(ask + " [yN] ").lower() in ["y", "yes"]
 
 
 class SecretNotFoundError(Exception):
     def __init__(self, store, secret):
-        self.store = store
-        self.secret = secret
         super().__init__(f"Secret '{secret}' not found in store '{store}'")
+
+
+class SecretTypeNotValidError(Exception):
+    def __init__(self, type):
+        super().__init__(f"Secret type '{type}' is not valid")
+
+
+class SecretGenerationError(Exception):
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
+class SecretType(Enum):
+    PASSWORD = "password"
+    DUMMY = "dummy"
+
+    @classmethod
+    def from_config(cls, config):
+        if "type" not in config:
+            raise Exception("Secret generation config is missing 'type' field")
+
+        for t in cls:
+            if config["type"] == t.value:
+                return (t, config)
+        raise SecretTypeNotValidError(config["type"])
```

### Comparing `secenv-1.0.1/secenv.egg-info/PKG-INFO` & `secenv-1.1.0/secenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.0.1
+Version: 1.1.0
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.0.1/secenv.egg-info/SOURCES.txt` & `secenv-1.1.0/secenv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 secenv/stores/env.py
 secenv/stores/gcp.py
 secenv/stores/pass.py
 secenv/stores/scaleway.py
 secenv/stores/vault.py
 tests/test_config_file.py
 tests/test_context_output.py
+tests/test_fill_secrets.py
 tests/test_gen_context.py
 tests/test_list_contexts.py
 tests/test_stores.py
 tests/test_utils.py
```

### Comparing `secenv-1.0.1/tests/test_context_output.py` & `secenv-1.1.0/tests/test_context_output.py`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/tests/test_gen_context.py` & `secenv-1.1.0/tests/test_gen_context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/tests/test_stores.py` & `secenv-1.1.0/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `secenv-1.0.1/tests/test_utils.py` & `secenv-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

