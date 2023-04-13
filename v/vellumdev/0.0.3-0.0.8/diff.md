# Comparing `tmp/vellumdev-0.0.3.tar.gz` & `tmp/vellumdev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellumdev-0.0.3.tar", max compression
+gzip compressed data, was "vellumdev-0.0.8.tar", max compression
```

## Comparing `vellumdev-0.0.3.tar` & `vellumdev-0.0.8.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      350 2023-04-06 21:56:32.332208 vellumdev-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1863 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/__init__.py
--rw-r--r--   0        0        0     1791 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/__init__.py
--rw-r--r--   0        0        0     8722 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/client.py
--rw-r--r--   0        0        0      348 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/core/remove_none_from_headers.py
--rw-r--r--   0        0        0     2740 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/types/__init__.py
--rw-r--r--   0        0        0     1117 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/types/document.py
--rw-r--r--   0        0        0     1501 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      639 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/types/finish_reason_enum.py
--rw-r--r--   0        0        0      826 2023-04-06 21:56:32.332208 vellumdev-0.0.3/src/vellum/api/types/generate_options_request.py
--rw-r--r--   0        0        0     1482 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_request_body_request.py
--rw-r--r--   0        0        0     1193 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_request_request.py
--rw-r--r--   0        0        0      897 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_response.py
--rw-r--r--   0        0        0      936 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_result.py
--rw-r--r--   0        0        0      992 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_result_data.py
--rw-r--r--   0        0        0      840 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/generate_result_error.py
--rw-r--r--   0        0        0      435 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/logprobs_enum.py
--rw-r--r--   0        0        0      483 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_type_enum.py
--rw-r--r--   0        0        0     1071 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_version_build_config.py
--rw-r--r--   0        0        0      947 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     1169 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_version_exec_config_read.py
--rw-r--r--   0        0        0     1560 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_version_read.py
--rw-r--r--   0        0        0      934 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0      873 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/normalized_log_probs.py
--rw-r--r--   0        0        0      874 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      643 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/provider_enum.py
--rw-r--r--   0        0        0     1280 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_request_body_request.py
--rw-r--r--   0        0        0     1098 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_request_options_request.py
--rw-r--r--   0        0        0      952 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_response.py
--rw-r--r--   0        0        0     1039 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_result.py
--rw-r--r--   0        0        0      834 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_result_merging_request.py
--rw-r--r--   0        0        0      961 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/search_weights_request.py
--rw-r--r--   0        0        0     1778 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0     1330 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/submit_completion_actuals_request_request.py
--rw-r--r--   0        0        0     1684 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/upload_document_request_body_request.py
--rw-r--r--   0        0        0      837 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/api/types/upload_document_response.py
--rw-r--r--   0        0        0      370 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/environment.py
--rw-r--r--   0        0        0        0 2023-04-06 21:56:32.336208 vellumdev-0.0.3/src/vellum/py.typed
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 vellumdev-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      412 2023-04-13 01:40:12.670539 vellumdev-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1392 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/__init__.py
+-rw-r--r--   0        0        0     8569 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/client.py
+-rw-r--r--   0        0        0      348 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      428 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/environment.py
+-rw-r--r--   0        0        0        0 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/py.typed
+-rw-r--r--   0        0        0      543 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      258 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      291 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/errors/internal_server_error.py
+-rw-r--r--   0        0        0      285 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      136 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/commons/types/error_response.py
+-rw-r--r--   0        0        0      159 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/completion_actuals/__init__.py
+-rw-r--r--   0        0        0     4028 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/completion_actuals/client.py
+-rw-r--r--   0        0        0      186 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/completion_actuals/types/__init__.py
+-rw-r--r--   0        0        0      921 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/completion_actuals/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      145 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/document/__init__.py
+-rw-r--r--   0        0        0     4619 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/document/client.py
+-rw-r--r--   0        0        0      164 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/document/types/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/resources/document/types/upload_document_response.py
+-rw-r--r--   0        0        0     1298 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0     1145 2023-04-13 01:40:12.670539 vellumdev-0.0.8/src/vellum/types/document.py
+-rw-r--r--   0        0        0     1044 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      639 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      826 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0      834 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0      821 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0      936 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0      870 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      756 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      435 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      873 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0      874 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      880 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/search_request_options.py
+-rw-r--r--   0        0        0      813 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0      848 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0      791 2023-04-13 01:40:12.674540 vellumdev-0.0.8/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellumdev-0.0.8/PKG-INFO
```

### Comparing `vellumdev-0.0.3/src/vellum/api/core/datetime_utils.py` & `vellumdev-0.0.8/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/core/jsonable_encoder.py` & `vellumdev-0.0.8/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/types/document.py` & `vellumdev-0.0.8/src/vellum/types/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
+import uuid
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class Document(pydantic.BaseModel):
-    id: str = pydantic.Field(description=("The ID of the document.\n"))
-    label: str = pydantic.Field(description=("The human-readable name for the document.\n"))
+    id: uuid.UUID
+    label: str = pydantic.Field(
+        description=("A human-readable label for the document. Defaults to the originally uploaded file's file name.\n")
+    )
     external_id: typing.Optional[str] = pydantic.Field(
         description=(
-            "The unique ID of the document as represented in an external system and specified when it was originally uploaded.\n"
+            "The unique id of this document as it exists in the user's system. If not provided, will be set to the document's id.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/enriched_normalized_completion.py` & `vellumdev-0.0.8/src/vellum/types/enriched_normalized_completion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
+import uuid
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .finish_reason_enum import FinishReasonEnum
 from .normalized_log_probs import NormalizedLogProbs
 
 
 class EnrichedNormalizedCompletion(pydantic.BaseModel):
-    id: str = pydantic.Field(description=("The Vellum-generated ID of the completion.\n"))
-    external_id: typing.Optional[str] = pydantic.Field(
-        description=(
-            "The external ID that was originally provided along with the generation request, which uniquely identifies this generation in an external system.\n"
-        )
-    )
-    text: str = pydantic.Field(description=("The text generated by the LLM.\n"))
+    id: uuid.UUID
+    external_id: typing.Optional[str]
+    text: str
     finish_reason: FinishReasonEnum
     logprobs: typing.Optional[NormalizedLogProbs]
-    model_version_id: str = pydantic.Field(
-        description=("The ID of the model version used to generate this completion.\n")
-    )
+    model_version_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/finish_reason_enum.py` & `vellumdev-0.0.8/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_options_request.py` & `vellumdev-0.0.8/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_request_body_request.py` & `vellumdev-0.0.8/src/vellum/types/generate_result_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,31 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .generate_options_request import GenerateOptionsRequest
-from .generate_request_request import GenerateRequestRequest
+from .enriched_normalized_completion import EnrichedNormalizedCompletion
 
 
-class GenerateRequestBodyRequest(pydantic.BaseModel):
-    deployment_id: typing.Optional[str] = pydantic.Field(
-        description=("The ID of the deployment. Must provide either this or deployment_name.\n")
-    )
-    deployment_name: typing.Optional[str] = pydantic.Field(
-        description=("The name of the deployment. Must provide either this or deployment_id.\n")
-    )
-    requests: typing.List[GenerateRequestRequest] = pydantic.Field(
-        description=(
-            "The generation requests to make. Supplying multiple will perform a bulk request to the LLM provided when possible.\n"
-        )
-    )
-    options: typing.Optional[GenerateOptionsRequest]
+class GenerateResultData(pydantic.BaseModel):
+    completions: typing.List[EnrichedNormalizedCompletion]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_request_request.py` & `vellumdev-0.0.8/src/vellum/types/normalized_token_log_probs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,19 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GenerateRequestRequest(pydantic.BaseModel):
-    input_values: typing.Dict[str, typing.Any] = pydantic.Field(
-        description=("Key/value pairs for each template variable defined in the deployment's prompt.\n")
-    )
-    external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
-        description=(
-            "Optionally include a unique identifier for each generation, as represented outside of Vellum. Note that this should generally be a list of length one.\n"
-        )
-    )
+class NormalizedTokenLogProbs(pydantic.BaseModel):
+    token: str
+    logprob: typing.Optional[float]
+    top_logprobs: typing.Optional[typing.Dict[str, float]]
+    text_offset: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_response.py` & `vellumdev-0.0.8/src/vellum/types/generate_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .generate_result import GenerateResult
 
 
 class GenerateResponse(pydantic.BaseModel):
-    results: typing.List[GenerateResult] = pydantic.Field(description=("The results of each generation request.\n"))
+    results: typing.List[GenerateResult]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_result.py` & `vellumdev-0.0.8/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_result_data.py` & `vellumdev-0.0.8/src/vellum/resources/commons/types/error_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
-from .enriched_normalized_completion import EnrichedNormalizedCompletion
+from ....core.datetime_utils import serialize_datetime
 
 
-class GenerateResultData(pydantic.BaseModel):
-    completions: typing.List[EnrichedNormalizedCompletion] = pydantic.Field(
-        description=("The generated completions. This will generally be a list of length one.\n")
-    )
+class ErrorResponse(pydantic.BaseModel):
+    detail: str = pydantic.Field(description=("Details about why the request failed.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/generate_result_error.py` & `vellumdev-0.0.8/src/vellum/types/search_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .document import Document
 
 
-class GenerateResultError(pydantic.BaseModel):
-    message: str = pydantic.Field(description=("The error message returned by the LLM provider.\n"))
+class SearchResult(pydantic.BaseModel):
+    document: Document
+    text: str
+    keywords: typing.List[str]
+    score: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/model_version_build_config.py` & `vellumdev-0.0.8/src/vellum/types/generate_result_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .model_version_sandbox_snapshot import ModelVersionSandboxSnapshot
 
 
-class ModelVersionBuildConfig(pydantic.BaseModel):
-    base_model: str = pydantic.Field(
-        description=(
-            "The name of the base model used to create this model version, as identified by the LLM provider.\n"
-        )
-    )
-    sandbox_snapshot: typing.Optional[ModelVersionSandboxSnapshot]
+class GenerateResultError(pydantic.BaseModel):
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/model_version_exec_config_parameters.py` & `vellumdev-0.0.8/src/vellum/types/search_request_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .search_weights_request import SearchWeightsRequest
 
 
-class ModelVersionExecConfigParameters(pydantic.BaseModel):
-    temperature: float
-    max_tokens: int
-    stop: typing.Optional[typing.List[str]]
-    top_p: float
-    top_k: typing.Optional[float]
-    frequency_penalty: float
-    presence_penalty: float
+class SearchRequestOptions(pydantic.BaseModel):
+    limit: typing.Optional[int]
+    weights: typing.Optional[SearchWeightsRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/model_version_exec_config_read.py` & `vellumdev-0.0.8/src/vellum/resources/completion_actuals/types/submit_completion_actual_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
-from .model_version_exec_config_parameters import ModelVersionExecConfigParameters
+from ....core.datetime_utils import serialize_datetime
 
 
-class ModelVersionExecConfigRead(pydantic.BaseModel):
-    prompt_template: str = pydantic.Field(
-        description=("The template used to generate prompts for this model version.\n")
-    )
-    parameters: ModelVersionExecConfigParameters
-    input_variables: typing.List[str] = pydantic.Field(
-        description=("Names of the template variables specified in the prompt template.\n")
-    )
+class SubmitCompletionActualRequest(pydantic.BaseModel):
+    id: typing.Optional[str]
+    external_id: typing.Optional[str]
+    text: typing.Optional[str]
+    quality: typing.Optional[float]
+    timestamp: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/normalized_log_probs.py` & `vellumdev-0.0.8/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellumdev-0.0.3/src/vellum/api/types/normalized_token_log_probs.py` & `vellumdev-0.0.8/src/vellum/types/search_weights_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class NormalizedTokenLogProbs(pydantic.BaseModel):
-    token: str
-    logprob: typing.Optional[float]
-    top_logprobs: typing.Optional[typing.Dict[str, float]]
-    text_offset: int
+class SearchWeightsRequest(pydantic.BaseModel):
+    semantic_similarity: float
+    keywords: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/search_request_options_request.py` & `vellumdev-0.0.8/src/vellum/resources/document/types/upload_document_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
+import uuid
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
-from .search_result_merging_request import SearchResultMergingRequest
-from .search_weights_request import SearchWeightsRequest
+from ....core.datetime_utils import serialize_datetime
 
 
-class SearchRequestOptionsRequest(pydantic.BaseModel):
-    limit: typing.Optional[int] = pydantic.Field(description=("The maximum number of results to return.\n"))
-    weights: typing.Optional[SearchWeightsRequest]
-    result_merging: typing.Optional[SearchResultMergingRequest]
+class UploadDocumentResponse(pydantic.BaseModel):
+    document_id: uuid.UUID
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellumdev-0.0.3/src/vellum/api/types/search_response.py` & `vellumdev-0.0.8/src/vellum/types/search_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .search_result import SearchResult
 
 
 class SearchResponse(pydantic.BaseModel):
-    results: typing.List[SearchResult] = pydantic.Field(
-        description=("The results of the search. Each result represents a chunk that matches the search query.\n")
-    )
+    results: typing.List[SearchResult]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

