# Comparing `tmp/openapify-0.3.3.tar.gz` & `tmp/openapify-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.3.tar", last modified: Wed Apr 12 18:57:10 2023, max compression
+gzip compressed data, was "openapify-0.3.4.tar", last modified: Thu Apr 13 11:18:36 2023, max compression
```

## Comparing `openapify-0.3.3.tar` & `openapify-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.147448 openapify-0.3.3/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.3/LICENSE
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-12 18:57:10.147319 openapify-0.3.3/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    29397 2023-04-12 18:43:50.000000 openapify-0.3.3/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.144357 openapify-0.3.3/openapify/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      488 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146237 openapify-0.3.3/openapify/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.3/openapify/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    14809 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/core/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3.3/openapify/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2018 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/core/document.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.3/openapify/core/jsonschema.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.3/openapify/core/models.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146533 openapify-0.3.3/openapify/core/openapi/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.3/openapify/core/openapi/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5264 2023-04-12 18:44:38.000000 openapify-0.3.3/openapify/core/openapi/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5197 2023-04-12 18:41:02.000000 openapify-0.3.3/openapify/decorators.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146725 openapify-0.3.3/openapify/ext/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.3/openapify/ext/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.146899 openapify-0.3.3/openapify/ext/web/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.3/openapify/ext/web/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.3/openapify/ext/web/aiohttp.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.3/openapify/py.typed
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-12 18:57:10.145158 openapify-0.3.3/openapify.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.3/openapify.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-12 18:57:10.000000 openapify-0.3.3/openapify.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.3/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-12 18:57:10.147487 openapify-0.3.3/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1298 2023-04-12 18:56:24.000000 openapify-0.3.3/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.663397 openapify-0.3.4/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.4/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-13 11:18:36.663248 openapify-0.3.4/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    29397 2023-04-12 18:43:50.000000 openapify-0.3.4/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.660069 openapify-0.3.4/openapify/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      488 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662005 openapify-0.3.4/openapify/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.4/openapify/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    15575 2023-04-13 11:17:48.000000 openapify-0.3.4/openapify/core/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2120 2023-04-13 11:17:48.000000 openapify-0.3.4/openapify/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2018 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/core/document.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.4/openapify/core/jsonschema.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.4/openapify/core/models.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662345 openapify-0.3.4/openapify/core/openapi/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.4/openapify/core/openapi/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5261 2023-04-13 10:15:38.000000 openapify-0.3.4/openapify/core/openapi/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5197 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/decorators.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662562 openapify-0.3.4/openapify/ext/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.4/openapify/ext/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662735 openapify-0.3.4/openapify/ext/web/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.4/openapify/ext/web/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.4/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.4/openapify/py.typed
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.660891 openapify-0.3.4/openapify.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.4/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.4/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-13 11:18:36.663433 openapify-0.3.4/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1298 2023-04-13 11:18:03.000000 openapify-0.3.4/setup.py
```

### Comparing `openapify-0.3.3/LICENSE` & `openapify-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/PKG-INFO` & `openapify-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openapify-0.3.3/README.md` & `openapify-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify/core/builder.py` & `openapify-0.3.4/openapify/core/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import apispec
 from typing_extensions import TypeAlias
 
 from openapify.core.const import (
     DEFAULT_OPENAPI_VERSION,
     DEFAULT_SPEC_TITLE,
     DEFAULT_SPEC_VERSION,
+    RESPONSE_DESCRIPTIONS,
 )
 from openapify.core.document import OpenAPIDocument
 from openapify.core.jsonschema import ComponentType, build_json_schema
 from openapify.core.models import (
     Body,
     Cookie,
     Header,
@@ -44,14 +45,22 @@
     "delete",
     "head",
     "options",
     "trace",
 ]
 
 
+def default_response_description(http_code: str) -> str:
+    result = RESPONSE_DESCRIPTIONS.get(http_code)
+    if result:
+        return result
+    else:
+        return RESPONSE_DESCRIPTIONS[f"{http_code[0]}XX"]
+
+
 def _merge_parameters(
     old_parameters: Sequence[openapi.Parameter], new_parameters: Dict[str, str]
 ) -> Sequence[openapi.Parameter]:
     for parameter in old_parameters or []:
         parameter_description = new_parameters.get(parameter.name)
         if parameter_description:
             parameter.description = parameter_description
@@ -90,15 +99,15 @@
             key=lambda r: (r.path, METHOD_ORDER.index(r.method.lower())),
         ):
             self._process_route(route)
 
     def _process_route(self, route: RouteDef) -> None:
         method = route.method.lower()
         meta = getattr(route.handler, "__openapify__", [])
-        responses = openapi.Responses()
+        responses: Optional[openapi.Responses] = None
         summary = route.summary
         description = route.description
         tags = route.tags.copy() if route.tags else []
         deprecated = None
         external_docs = None
         security = None
         parameters = route.parameters.copy() if route.parameters else []
@@ -117,15 +126,16 @@
                     body_value_type = body
                     media_type = args.get("media_type")
                     body_required = args.get("body_required")
                     body_description = args.get("body_description")
                     body_example = args.get("body_example")
                     body_examples = args.get("body_examples")
                 if body is not None:
-                    request_body = self._build_request_body(
+                    request_body = self._update_request_body(
+                        body=request_body,
                         value_type=body_value_type,
                         media_type=media_type,
                         required=body_required,
                         description=body_description,
                         example=body_example,
                         examples=body_examples,
                     )
@@ -136,15 +146,15 @@
                 if headers:
                     parameters.extend(self._build_request_headers(headers))
                 cookies = args.get("cookies")
                 if cookies:
                     parameters.extend(self._build_cookies(cookies))
 
             elif args_type == "response":
-                self._update_responses(responses=responses, **args)
+                responses = self._update_responses(responses=responses, **args)
             elif args_type == "path_docs":
                 args = args.copy()
                 summary = args.get("summary")
                 description = args.get("description")
                 tags.extend(args.get("tags") or [])
                 # _merge_parameters(parameters, args.get("parameters") or {})
                 external_docs = self._build_external_docs(
@@ -270,65 +280,75 @@
                     schema=parameter_schema,
                     example=cookie.example,
                     examples=self._build_examples(cookie.examples),
                 )
             )
         return result
 
-    def _build_request_body(
+    def _update_request_body(
         self,
+        body: Optional[openapi.RequestBody],
         value_type: Type,
         media_type: str = "application/json",
         required: Optional[bool] = None,
         description: Optional[str] = None,
         example: Optional[Any] = None,
         examples: Optional[Mapping[str, Union[openapi.Example, Any]]] = None,
     ) -> openapi.RequestBody:
-        return openapi.RequestBody(
-            description=description,
-            content={
-                media_type: openapi.MediaType(
-                    schema=build_json_schema(value_type, self.spec),
-                    example=example,
-                    examples=self._build_examples(examples),
-                )
-            },
-            required=required,
-        )
+        if body is None:
+            body = openapi.RequestBody()
+        if description:
+            body.description = description
+        if required is not None:
+            body.required = required
+        if value_type is not None:
+            if body.content is None:
+                body.content = {}
+            body.content[media_type] = openapi.MediaType(
+                schema=build_json_schema(value_type, self.spec),
+                example=example,
+                examples=self._build_examples(examples),
+            )
+        return body
 
     def _update_responses(
         self,
-        responses: openapi.Responses,
+        responses: Optional[openapi.Responses],
         http_code: openapi.HttpCode,
         body: Optional[Type] = None,
         media_type: str = "application/json",
         description: Optional[str] = None,
         headers: Optional[Dict[str, Union[str, Header]]] = None,
         example: Optional[Any] = None,
         examples: Optional[Dict[str, Union[openapi.Example, Any]]] = None,
-    ) -> None:
+    ) -> openapi.Responses:
         http_code = str(http_code)
+        if responses is None:
+            responses = openapi.Responses()
         if responses.codes is None:
             responses.codes = {}
         response = responses.codes.get(http_code)
         if not response:
             response = openapi.Response()
             responses.codes[http_code] = response
         if headers:
             response.headers = self._build_response_headers(headers)
         if description:
             response.description = description
+        elif not response.description:
+            response.description = default_response_description(http_code)
         if body is not None:
             if response.content is None:
                 response.content = {}
             response.content[media_type] = openapi.MediaType(
                 schema=build_json_schema(body, self.spec),
                 example=example,
                 examples=self._build_examples(examples),
             )
+        return responses
 
     @staticmethod
     def _build_external_docs(
         data: Union[str, Tuple[str, str]]
     ) -> Optional[openapi.ExternalDocumentation]:
         if not data:
             return None
```

### Comparing `openapify-0.3.3/openapify/core/document.py` & `openapify-0.3.4/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify/core/jsonschema.py` & `openapify-0.3.4/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify/core/models.py` & `openapify-0.3.4/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify/core/openapi/models.py` & `openapify-0.3.4/openapify/core/openapi/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     examples: Optional[Mapping[str, Example]] = None
     encoding: Optional[str] = None
 
 
 @dataclass
 class RequestBody(Object):
     description: Optional[str] = None
-    content: Optional[Mapping[str, MediaType]] = None
+    content: Optional[Dict[str, MediaType]] = None
     required: Optional[bool] = None
 
 
 @dataclass
 class Response(Object):
     description: Optional[str] = None
     headers: Optional[Mapping[str, Header]] = None
```

### Comparing `openapify-0.3.3/openapify/decorators.py` & `openapify-0.3.4/openapify/decorators.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify/ext/web/aiohttp.py` & `openapify-0.3.4/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/openapify.egg-info/PKG-INFO` & `openapify-0.3.4/openapify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openapify-0.3.3/openapify.egg-info/SOURCES.txt` & `openapify-0.3.4/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.3/setup.py` & `openapify-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.3",
+    version="0.3.4",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
```

