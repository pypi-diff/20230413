# Comparing `tmp/climify_api-0.0.3.tar.gz` & `tmp/climify_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-0.0.3.tar", last modified: Mon Apr  3 11:28:11 2023, max compression
+gzip compressed data, was "climify_api-1.0.0.tar", last modified: Thu Apr 13 08:44:16 2023, max compression
```

## Comparing `climify_api-0.0.3.tar` & `climify_api-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 11:28:11.072155 climify_api-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      932 2023-04-03 11:28:11.068163 climify_api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 11:28:11.054591 climify_api-0.0.3/climify_api/
--rw-rw-rw-   0        0        0       70 2023-03-21 09:44:28.000000 climify_api-0.0.3/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10815 2023-03-31 14:47:44.000000 climify_api-0.0.3/climify_api/REST.py
--rw-rw-rw-   0        0        0     1044 2023-04-03 11:27:34.000000 climify_api-0.0.3/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57606 2023-04-03 10:30:44.000000 climify_api-0.0.3/climify_api/api_client.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-0.0.3/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-0.0.3/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5277 2023-03-31 14:47:44.000000 climify_api-0.0.3/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:28:11.065151 climify_api-0.0.3/climify_api/models/
--rw-rw-rw-   0        0        0     5383 2023-03-28 07:08:37.000000 climify_api-0.0.3/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-0.0.3/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:28:11.063151 climify_api-0.0.3/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-04-03 11:28:10.000000 climify_api-0.0.3/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-03 11:28:11.000000 climify_api-0.0.3/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 11:28:10.000000 climify_api-0.0.3/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-04-03 11:28:10.000000 climify_api-0.0.3/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-03 11:28:10.000000 climify_api-0.0.3/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1429 2023-04-03 11:27:26.000000 climify_api-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 11:28:11.072775 climify_api-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.007822 climify_api-1.0.0/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-04-13 08:44:16.006823 climify_api-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 08:44:15.993706 climify_api-1.0.0/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.0/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.0/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-04-13 08:43:41.000000 climify_api-1.0.0/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.0/climify_api/api_client.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.0/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.0/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.0/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.005824 climify_api-1.0.0/climify_api/models/
+-rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.0/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.0/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.003806 climify_api-1.0.0/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1429 2023-04-13 08:43:29.000000 climify_api-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 08:44:16.007822 climify_api-1.0.0/setup.cfg
```

### Comparing `climify_api-0.0.3/LICENSE` & `climify_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-0.0.3/PKG-INFO` & `climify_api-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 0.0.3
+Version: 1.0.0
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-0.0.3/climify_api/REST.py` & `climify_api-1.0.0/climify_api/REST.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from urllib.parse import urlencode
 import typing
 
 import certifi
 import urllib3
 from urllib3._collections import HTTPHeaderDict
 
-from climify_api.exceptions import climify_apiException, ApiValueError
+from climify_api.exceptions import ClimifyApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTClient(object):
 
@@ -176,24 +176,24 @@
                         timeout=timeout,
                         headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
-                    raise climify_apiException(status=0, reason=msg)
+                    raise ClimifyApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
                 r = self.pool_manager.request(method, url,
                                               preload_content=not stream,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
-            raise climify_apiException(status=0, reason=msg)
+            raise ClimifyApiException(status=0, reason=msg)
 
         if not stream:
             # log response body
             logger.debug("response body: %s", r.data)
 
         return r
```

### Comparing `climify_api-0.0.3/climify_api/api_client.py` & `climify_api-1.0.0/climify_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -785,28 +785,26 @@
         self.style = style
         self.explode = explode
         self.allow_reserved = allow_reserved
 
 
 @dataclass
 class MediaType:
-    """
-    Used to store request and response body schema information
-    encoding:
-        A map between a property name and its encoding information.
-        The key, being the property name, MUST exist in the schema as a property.
-        The encoding object SHALL only apply to requestBody objects when the media type is
-        multipart or application/x-www-form-urlencoded.
+    """Used to store request and response body schema information encoding:
+    A map between a property name and its encoding information.
+    The key, being the property name, MUST exist in the schema as a property.
+    The encoding object SHALL only apply to requestBody objects when the media type is
+    multipart or application/x-www-form-urlencoded.
     """
     schema: typing.Optional[typing.Type[Schema]] = None
     encoding: typing.Optional[typing.Dict[str, Encoding]] = None
 
 
 @dataclass
-class climify_apiResponse(Generic[T]):
+class ClimifyApiResponse(Generic[T]):
     response: urllib3.HTTPResponse
     body: typing.Union[Unset, T] = unset
     headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset
 
     def __init__(
         self,
         response: urllib3.HTTPResponse,
@@ -818,26 +816,26 @@
         """
         self.response = response
         self.body = body
         self.headers = headers
 
 
 @dataclass
-class climify_apiResponseWithoutDeserialization(climify_apiResponse):
+class ClimifyApiResponseWithoutDeserialization(ClimifyApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[Unset, typing.Type[Schema]] = unset
     headers: typing.Union[Unset, typing.List[HeaderParameter]] = unset
 
 
 class OpenApiResponse(JSONDetector):
     __filename_content_disposition_pattern = re.compile('filename="(.+?)"')
 
     def __init__(
         self,
-        response_cls: typing.Type[climify_apiResponse] = climify_apiResponse,
+        response_cls: typing.Type[ClimifyApiResponse] = ClimifyApiResponse,
         content: typing.Optional[typing.Dict[str, MediaType]] = None,
         headers: typing.Optional[typing.List[HeaderParameter]] = None,
     ):
         self.headers = headers
         if content is not None and len(content) == 0:
             raise ValueError('Invalid value for content, the content dict must have >= 1 entry')
         self.content = content
@@ -914,15 +912,15 @@
                 decode=True
             ).decode(part.get_content_charset())
             if part.get_content_charset()
             else part.get_payload()
             for part in msg.get_payload()
         }
 
-    def deserialize(self, response: urllib3.HTTPResponse, configuration: Configuration) -> climify_apiResponse:
+    def deserialize(self, response: urllib3.HTTPResponse, configuration: Configuration) -> ClimifyApiResponse:
         content_type = response.getheader('content-type')
         deserialized_body = unset
         streamed = response.supports_chunked_reads()
 
         deserialized_headers = unset
         if self.headers is not None:
             # TODO add header deserialiation here
```

### Comparing `climify_api-0.0.3/climify_api/auth.py` & `climify_api-1.0.0/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-0.0.3/climify_api/configuration.py` & `climify_api-1.0.0/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-0.0.3/climify_api/exceptions.py` & `climify_api-1.0.0/climify_api/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,30 +120,30 @@
         super(ApiKeyError, self).__init__(full_msg)
 
 
 T = typing.TypeVar("T")
 
 
 @dataclasses.dataclass
-class climify_apiException(OpenApiException, typing.Generic[T]):
+class ClimifyApiException(OpenApiException, typing.Generic[T]):
     status: int
     reason: str
     api_response: typing.Optional[T] = None
 
     @property
     def body(self) -> typing.Union[str, bytes, None]:
         if not self.api_response:
             return None
-        return self.api_response.response.data
+        return self.api_response.data
 
     @property
     def headers(self) -> typing.Optional[HTTPHeaderDict]:
         if not self.api_response:
             return None
-        return self.api_response.response.getheaders()
+        return self.api_response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
```

### Comparing `climify_api-0.0.3/climify_api/schemas.py` & `climify_api-1.0.0/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-0.0.3/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.0/climify_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 0.0.3
+Version: 1.0.0
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-0.0.3/pyproject.toml` & `climify_api-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climify_api"
-version = "0.0.3"
+version = "1.0.0"
 keywords=['Climify','Environmental engineering']
 authors = [
   { name="Climify Aps", email="info@climify.com" },
 ]
 description = "A wrapper library for the Climify REST API"
 #long_description = "A wrapper library for the Climify REST API, used to query sensor data and interact with Climify systems programmatically"
 readme = "README.md"
```

