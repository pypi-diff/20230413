# Comparing `tmp/baseten-0.5.3.tar.gz` & `tmp/baseten-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.5.3.tar", max compression
+gzip compressed data, was "baseten-0.6.0.tar", max compression
```

## Comparing `baseten-0.5.3.tar` & `baseten-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
--rw-r--r--   0        0        0     5041 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-02-17 17:30:53.073565 baseten-0.5.3/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-02-17 17:30:53.073565 baseten-0.5.3/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2022-12-01 02:40:15.840611 baseten-0.5.3/baseten/common/__init__.py
--rw-r--r--   0        0        0    28723 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-02-13 15:42:56.461909 baseten-0.5.3/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18046 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2847 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/settings.py
--rw-r--r--   0        0        0     1677 2023-02-17 19:05:37.058149 baseten-0.5.3/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     4778 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-02-09 17:17:41.388477 baseten-0.5.3/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-03-29 18:18:46.511694 baseten-0.5.3/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-03-29 18:18:46.519694 baseten-0.5.3/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-03-29 18:18:46.527694 baseten-0.5.3/baseten/training/datasets.py
--rw-r--r--   0        0        0    33979 2023-03-29 18:18:46.527694 baseten-0.5.3/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-02-17 22:53:32.164930 baseten-0.5.3/baseten/training/logs.py
--rw-r--r--   0        0        0      435 2023-02-15 15:35:27.530522 baseten-0.5.3/baseten/training/snippet.py
--rw-r--r--   0        0        0      479 2023-02-09 17:17:41.392477 baseten-0.5.3/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-02-23 20:44:26.962676 baseten-0.5.3/pypi_readme.md
--rw-r--r--   0        0        0     1989 2023-03-29 18:37:45.662591 baseten-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 baseten-0.5.3/setup.py
--rw-r--r--   0        0        0     2267 1970-01-01 00:00:00.000000 baseten-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29147 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    18044 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2847 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-04-13 00:37:53.970549 baseten-0.6.0/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-04-13 00:37:53.974550 baseten-0.6.0/pypi_readme.md
+-rw-r--r--   0        0        0     2008 2023-04-13 00:40:03.950711 baseten-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 baseten-0.6.0/PKG-INFO
```

### Comparing `baseten-0.5.3/baseten/__init__.py` & `baseten-0.6.0/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/baseten_deployed_model.py` & `baseten-0.6.0/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/cli.py` & `baseten-0.6.0/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/client_commands/baseten_cli.py` & `baseten-0.6.0/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/client_commands/dataset_cli.py` & `baseten-0.6.0/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.0/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/client_commands/models_cli.py` & `baseten-0.6.0/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.0/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/api.py` & `baseten-0.6.0/baseten/common/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
 import json
 import logging
-import tarfile
-import tempfile
+import os
 from typing import IO, Dict, List, Optional, Tuple, Union
 
+import boto3
 import requests
+from boto3.s3.transfer import TransferConfig
 from colorama import Fore
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 from tqdm import tqdm
 
 from baseten.common import settings
 from baseten.common.core import ApiError, AuthorizationError
 from baseten.common.util import base64_encoded_json_str
@@ -415,14 +416,31 @@
     }}
     """
     resp = _post_graphql_query(api_key, query_string)
     return resp["data"]["signed_s3_upload_url"]
 
 
 @with_api_key
+def model_s3_upload_credentials(api_key):
+    query_string = """
+    {
+        model_s3_upload_credentials {
+            s3_bucket
+            s3_key
+            aws_access_key_id
+            aws_secret_access_key
+            aws_session_token
+        }
+    }
+    """
+    resp = _post_graphql_query(api_key, query_string)
+    return resp["data"]["model_s3_upload_credentials"]
+
+
+@with_api_key
 def signed_s3_upload_and_download_post(api_key, file_name):
     query_string = f"""
     {{
       signed_s3_upload_url(model_file_name: "{file_name}"){{
         url,
         get_url,
         form_fields {{
@@ -695,26 +713,20 @@
     Returns:
         str: The key for the uploaded model
 
     Raises:
         RequestException: If there was an error communicating with the server.
     """
 
-    model_file_name = f"{file_name}.{file_ext}"
-    this_signed_s3_upload_post = signed_s3_upload_post(model_file_name)
-    logger.debug(f"Signed s3 upload post:\n{json.dumps(this_signed_s3_upload_post, indent=4)}")
-
-    form_fields = this_signed_s3_upload_post["form_fields"]
-    form_fields["AWSAccessKeyId"] = form_fields.pop(
-        "aws_access_key_id"
-    )  # S3 expects key name AWSAccessKeyId
-    form_fields["file"] = (file_name, serialize_file)
+    temp_credentials_s3_upload = model_s3_upload_credentials()
+    s3_key = temp_credentials_s3_upload.pop("s3_key")
+    s3_bucket = temp_credentials_s3_upload.pop("s3_bucket")
     logger.info("🚀 Uploading model to Baseten 🚀")
-
-    return _upload_file(this_signed_s3_upload_post, form_fields)
+    _multipart_upload_boto3(serialize_file.name, s3_bucket, s3_key, temp_credentials_s3_upload)
+    return s3_key
 
 
 def upload_user_file(io_stream: IO, file_name: str) -> str:
     signed_s3_upload_post = user_files_signed_s3_upload_post(file_name)
     logger.debug(f"Signed s3 upload post:\n{json.dumps(signed_s3_upload_post, indent=4)}")
 
     form_fields = signed_s3_upload_post["form_fields"]
@@ -739,14 +751,34 @@
     form_fields["file"] = (file_name, open(file_path, "rb"))
 
     _upload_file(signed_s3_upload_post, form_fields)
 
     return signed_s3_upload_post
 
 
+def _multipart_upload_boto3(file_path, bucket_name, key, credentials):
+    s3_resource = boto3.resource("s3", **credentials)
+    filesize = os.stat(file_path).st_size
+
+    with tqdm(
+        total=filesize,
+        desc="Upload",
+        unit="B",
+        unit_scale=True,
+    ) as pbar:
+        s3_resource.Object(bucket_name, key).upload_file(
+            file_path,
+            Config=TransferConfig(
+                max_concurrency=10,
+                use_threads=True,
+            ),
+            Callback=pbar.update,
+        )
+
+
 def _upload_file(this_signed_s3_upload_post: dict, form_fields: dict) -> str:
     encoder = MultipartEncoder(fields=form_fields)
     encoder_len = encoder.len
     pbar = tqdm(
         total=encoder_len,
         unit_scale=True,
         bar_format="Upload Progress: {percentage:3.0f}%% |%s{bar:100}%s| {n_fmt}/{total_fmt}"
@@ -768,23 +800,14 @@
     logger.info("🔮 Upload successful!🔮")
 
     logger.debug(f"File upload HTTP status code: {resp.status_code} and content:\n{resp.content}")  # type: ignore
 
     return this_signed_s3_upload_post["form_fields"]["key"]
 
 
-def _tar_a_list_of_files(list_of_files: List[str]) -> tempfile._TemporaryFileWrapper:
-    temp_file = tempfile.NamedTemporaryFile(suffix=".tgz")
-    with tarfile.open(temp_file.name, "w:gz") as tar:
-        for file in list_of_files:
-            tar.add(file)
-    temp_file.file.seek(0)
-    return temp_file
-
-
 @with_api_key
 def deactivate_model_version(api_key, model_version_id):
     query_string = f"""
     mutation {{
         deactivate_model_version(model_version_id: "{model_version_id}") {{
           ok
         }}
```

### Comparing `baseten-0.5.3/baseten/common/core.py` & `baseten-0.6.0/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/error_handler.py` & `baseten-0.6.0/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/files.py` & `baseten-0.6.0/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/lib_support.py` & `baseten-0.6.0/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/model_deployer.py` & `baseten-0.6.0/baseten/common/model_deployer.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
     logger.info(f"Serializing {Fore.BLUE}{model_name}{Style.RESET_ALL} truss.")
 
     # If the truss is not scattered then gather is a no-op and returns path to
     # original truss. So, there's no additional cost to gather for trusses
     # without external packages.
     gathered_truss = TrussHandle(b10_truss.gather())
-    temp_file = _compress_truss(b10_truss=gathered_truss)
+    temp_file = _archive_truss(b10_truss=gathered_truss)
     logger.info("Making contact with Baseten 👋 👽")
     s3_key = api.upload_model(temp_file, "tgz", MODEL_FILENAME)
     # String that can be passed through graphql api
     config = base64_encoded_json_str(gathered_truss._spec._config.to_dict())
     if not publish:
         model_id, model_version_id = deploy_draft_truss(
             model_name=model_name,
@@ -421,15 +421,15 @@
         f"💳 Add a payment method to reactivate your models and deploy new versions: {billing_url}"
         if no_credit_remaining
         else f"💳 Add a payment method to keep your models running once credit runs out: {billing_url}"
     )
     logger.info(add_payment_method_str)
 
 
-def _compress_truss(b10_truss: TrussHandle):
+def _archive_truss(b10_truss: TrussHandle):
     try:
         truss_dir = b10_truss._spec.truss_dir
         temp_file = create_tar_with_progress_bar(truss_dir)
     except PermissionError:
         # Windows bug with Tempfile causes PermissionErrors
         temp_file = create_tar_with_progress_bar(truss_dir, delete=False)
     temp_file.file.seek(0)
```

### Comparing `baseten-0.5.3/baseten/common/settings.py` & `baseten-0.6.0/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/tar.py` & `baseten-0.6.0/baseten/common/tar.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 from tqdm import tqdm
 
 
 def create_tar_with_progress_bar(source_dir: Path, delete=True):
     total_size = sum(f.stat().st_size for f in source_dir.glob("**/*") if f.is_file())
 
+    # Keeping the .tgz suffix for backwards compatibility even though
+    # this tar is uncompressed for upload
     temp_file = tempfile.NamedTemporaryFile(suffix=".tgz", delete=delete)
-    with tarfile.open(temp_file.name, "w:gz") as tar:
+    with tarfile.open(temp_file.name, "w:") as tar:
         with tqdm(total=total_size, unit="B", unit_scale=True, unit_divisor=1024) as pbar:
 
             def file_read_progress_callback(bytes_read: int):
                 pbar.update(bytes_read)
 
             for file_path in source_dir.glob("**/*"):
                 if file_path.is_file():
```

### Comparing `baseten-0.5.3/baseten/common/types.py` & `baseten-0.6.0/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/common/util.py` & `baseten-0.6.0/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/models/flan_t5.py` & `baseten-0.6.0/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/models/llama.py` & `baseten-0.6.0/baseten/models/llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 from baseten.baseten_deployed_model import BasetenDeployedModel
 from baseten.models.foundational_model import FoundationalModel
 from baseten.models.util import requests_error_handling
 
 
 class Llama(FoundationalModel):
     """
-    Llama is a text-to-text generation model from Meta.
+    LLaMA is a text-to-text generation model from Meta.
+
+    !!! note
+        This `Llama` model object is only available as the interface for a fine-tuned model.
 
     **Examples:**
+
+    ```python
+    model = Llama(model_id="llama-1234")
+    completion = model("What is the meaning of life?", max_length=256)
+    ```
     """
 
     def __init__(self, model_id: Optional[str] = None):
-        """ """
+        """
+        Args:
+            model_id: The ID for a deployed model created from a LLaMA fine-tuning run.
+        """
 
         self._id = model_id
         self._is_user_model = self._id is not None
         self._model = self._set_user_model()
 
     def status(self) -> str:
         return self._model.status
 
     def id(self) -> str:
         return self._model.id
 
     def _set_user_model(self) -> BasetenDeployedModel:
         """Creates internal BasetenDeployedModel object that points to users
-        deployed Llama model. If the user does not have a deployed model,
+        deployed LLaMA model. If the user does not have a deployed model,
         we will create one for them.
         """
         if self._is_user_model:
             return BasetenDeployedModel(model_id=self._id)
         else:
             raise ValueError("No model id provided")
```

### Comparing `baseten-0.5.3/baseten/models/stable_diffusion.py` & `baseten-0.6.0/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/models/util.py` & `baseten-0.6.0/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/models/whisper.py` & `baseten-0.6.0/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/training/datasets.py` & `baseten-0.6.0/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/baseten/training/finetuning.py` & `baseten-0.6.0/baseten/training/finetuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         for this type of FineTuning configuration.
         """
 
 
 @dataclass
 class LlamaConfig(FinetuningConfig):
     """
-    Training config for Llama-7B.
+    Training config for LLaMA-7B.
 
     **Examples:**
 
     ```python
-    from baseten.training import Dataset, FlanT5BaseConfig
+    from baseten.training import Dataset, LlamaConfig
 
     config = LlamaConfig(
         input_dataset=Dataset("DATASET_ID"),
         epochs=3,
         learning_rate=5e-5,
         max_steps=1000,
         train_batch_size=8,
@@ -77,16 +77,18 @@
         report_to="wandb"
     )
     ```
 
     Args:
         model_id:
             Pretrained model to fine-tune
-        output_dir:
-            Path to output directory
+        source_col_name:
+            Name of the source column in the input CSV
+        target_col_name:
+            Name of the target column in the input CSV
         evaluation_strategy:
             Interval for evaluation (default: "epoch")
         train_batch_size:
             Batch size for training (default: 8)
         train_micro_batch_size:
             Micro batch size for training (default: 4)
         sample_batch_size:
@@ -127,16 +129,14 @@
             Whether to disable tqdm progress bars (default: True)
         label_smoothing_factor:
             The label smoothing factor to use (default: 0.0)
         adafactor:
             Whether to use the Adafactor optimizer (default: False)
         report_to:
             Destination for metrics reporting (default: None)
-        dataset_source_key:
-            Column name for the source text in the input dataset (default: "source")
         max_length:
             Maximum input length (default: 256)
         lora_r:
             Number of attention heads for LORA (default: 8)
         lora_target_modules:
             List of target modules for LORA (default: ["q_proj", "v_proj"])
         lora_alpha:
```

### Comparing `baseten-0.5.3/baseten/training/logs.py` & `baseten-0.6.0/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/pypi_readme.md` & `baseten-0.6.0/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.5.3/pyproject.toml` & `baseten-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.5.3"
+version = "0.6.0"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
@@ -35,14 +35,15 @@
 types-requests = "^2.28.11.7"
 types-setuptools = "^65.6.0.2"
 types-pillow = "^9.3.0.4"
 types-pyyaml = "^6.0.12.2"
 halo = "^0.0.31"
 types-pytz = "^2022.7.1.0"
 pytz = "^2022.7.1"
+boto3 = ">=1.26.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 wheel = "^0.37.1"
 flake8 = "^3.7"
 tox = "^3.14"
 coverage = "^4.5"
```

### Comparing `baseten-0.5.3/PKG-INFO` & `baseten-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.5.3
+Version: 0.6.0
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
+Requires-Dist: boto3 (>=1.26.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: colorama (>=0.4.3)
 Requires-Dist: coolname (>=1.1.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: joblib (>=0.12.5)
 Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
```

