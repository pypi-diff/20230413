# Comparing `tmp/yotpy-0.0.61.tar.gz` & `tmp/yotpy-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.61.tar", last modified: Wed Apr 12 23:16:04 2023, max compression
+gzip compressed data, was "yotpy-0.0.62.tar", last modified: Thu Apr 13 15:04:03 2023, max compression
```

## Comparing `yotpy-0.0.61.tar` & `yotpy-0.0.62.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.61/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.61/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.61/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.61/README.md
--rw-r--r--   0        0        0        0 2023-04-12 23:07:55.942421 yotpy-0.0.61/__init__.py
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.61/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.61/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.61/docs/yotpy.html
--rw-r--r--   0        0        0     1883 2023-04-12 22:50:16.599595 yotpy-0.0.61/exceptions.py
--rw-r--r--   0        0        0      830 2023-04-12 22:19:29.450917 yotpy-0.0.61/pyproject.toml
--rw-r--r--   0        0        0    30803 2023-04-12 23:08:26.829890 yotpy-0.0.61/yotpy.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.61/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.62/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.62/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.62/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.62/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 23:07:55.942421 yotpy-0.0.62/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.62/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.62/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.62/docs/yotpy.html
+-rw-r--r--   0        0        0     1883 2023-04-12 22:50:16.599595 yotpy-0.0.62/exceptions.py
+-rw-r--r--   0        0        0      830 2023-04-12 22:19:29.450917 yotpy-0.0.62/pyproject.toml
+-rw-r--r--   0        0        0    30725 2023-04-13 15:03:16.110425 yotpy-0.0.62/yotpy.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.62/PKG-INFO
```

### Comparing `yotpy-0.0.61/.github/workflows/static.yml` & `yotpy-0.0.62/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/LICENSE` & `yotpy-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/docs/search.js` & `yotpy-0.0.62/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/docs/yotpy.html` & `yotpy-0.0.62/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/exceptions.py` & `yotpy-0.0.62/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/pyproject.toml` & `yotpy-0.0.62/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.61/yotpy.py` & `yotpy-0.0.62/yotpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 """
 
-__version__ = "0.0.61"
+__version__ = "0.0.62"
 
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
@@ -14,16 +14,14 @@
 from html import unescape
 from urllib.parse import urlencode
 from math import ceil
 from itertools import chain
 from .exceptions import CustomException, SessionNotCreatedError, FailedToGetTokenError, PreflightException, UploadException, SendException, UserNotFound, AppNotFound
 
 
-# TODO: Give better error messages for bad requests
-
 class JSONTransformer:
     """
     A utility class for transforming JSON data into various formats.
     """
 
     @staticmethod
     def stream_json_data(json: dict, keys: tuple) -> Iterator[dict[str, Union[tuple, str]]]:
@@ -244,18 +242,17 @@
         """
         schema = list(iterator.schema)
         headers = {field.name for field in schema if (
             include and field.name in include) or (exclude and field.name not in exclude)}
 
         rows = []
         for row in iterator:
-            [row.pop(field.name, None)
-             for field in schema if field.name not in headers]
+            row = {field.name : row[field.name] for field in schema if field.name in headers}
             rows.append(row)
-
+        
         return headers, rows
 
     @staticmethod
     def to_rows(json_list: list[dict], sep: str, exclude: list[str] = [], include: list[str] = []) -> tuple[list, set]:
         """
         Flatten a list of JSON objects into a list of rows and a set of headers.
 
@@ -369,15 +366,15 @@
             app_key (str): The target app you want authenticated.
             secret (str): The client secret to authenticate the request.
 
         Returns:
             str: The user access token.
 
         Raises:
-            Exception: If the response status is not OK (200).
+            FailedToGetTokenError: If the response status is not OK (200).
         """
         url = "https://api.yotpo.com/oauth/token"
         data = {
             "grant_type": "client_credentials",
             "client_id": self._app_key,
             "client_secret": self._secret,
         }
@@ -419,14 +416,15 @@
             exception_type (Union[CustomException, Exception]): The type of exception to raise when an error occurs. Defaults to CustomException.
             **kwargs: Additional keyword arguments to be passed to the request object.
 
         Returns:
             dict: The parsed JSON response.
 
         Raises:
+            SessionNotCreatedError: If the aiohttp session has not been created.
             exception_type: If the response status is not 200, an instance of the specified exception_type is raised with an error message.
         """
         if not hasattr(self, 'aiohttp_session'):
             raise SessionNotCreatedError()
 
         async with self.aiohttp_session.get(url, **kwargs) as response:
             if response.status == 200:
@@ -449,14 +447,15 @@
             exception_type (Union[CustomException, Exception]): The type of exception to raise when an error occurs. Defaults to CustomException.
             **kwargs: Additional keyword arguments to be passed to the request object.
 
         Returns:
             dict: The parsed JSON response.
 
         Raises:
+            SessionNotCreatedError: If the aiohttp session has not been created.
             exception_type: If the response status is not 200, an instance of the specified exception_type is raised with an error message.
         """
         if not hasattr(self, 'aiohttp_session'):
             raise SessionNotCreatedError()
 
         async with self.aiohttp_session.post(url, data=data, **kwargs) as response:
             if response.status == 200:
@@ -501,15 +500,15 @@
             ```python
             >>> yotpo = YotpoAPIWrapper(app_key, secret)
             >>> async with yotpo as yp:
             >>>     user = await yp.get_user()
             ```
 
         Raises:
-            Exception: If the request to the user endpoint returns a non-OK status.
+            UserNotFound: If the request to the user endpoint returns a non-OK status.
         """
         url = self.write_user_endpoint
 
         return await self._get_request(url, parser=lambda data: data['response']['user'], exception_type=UserNotFound)
 
     async def get_app(self) -> dict:
         """
@@ -524,17 +523,14 @@
 
         Raises:
             AppDataNotFound: If the request to the app endpoint returns a non-OK status.
         """
         # NOTE: The user_id does not appear to actually matter at all, as it still returns data even if it is not a valid user ID.
         # I suspect `user_id` is just used to track which user is making the request.
 
-        # TODO: If the above is true, we can probably abstract away the `user_id` parameter and just use the user ID from the user endpoint.
-        # And if need be we can add some configuration to allow the user to specify a user ID if they want to.
-
         url = f"https://api-write.yotpo.com/apps/{self._app_key}?user_id={self.user_id}&utoken={self._utoken}"
 
         return await self._get_request(url, parser=lambda data: data['response']['app'], exception_type=AppNotFound)
 
     async def get_total_reviews(self) -> int:
         """
         Asynchronously fetches the total number of reviews for an app.
@@ -660,14 +656,15 @@
 
         Returns:
             dict: A dictionary containing the response data.
 
         Raises:
             Exception: If any response status is not 200.
             UploadException: If the uploaded file is not valid.
+            SendException: If the send request fails.
         """
         upload_url = f"{self.write_app_endpoint}/{self._app_key}/account_emails/{template_id}/upload_mailing_list"
         send_url = f"{self.write_app_endpoint}/{self._app_key}/account_emails/{template_id}/send_burst_email"
 
         upload_response = await self._post_request(upload_url, {"file": csv_stringio, "utoken": self._utoken}, exception_type=UploadException)
         upload_data = upload_response['response']['response']
```

### Comparing `yotpy-0.0.61/PKG-INFO` & `yotpy-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.61
+Version: 0.0.62
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

