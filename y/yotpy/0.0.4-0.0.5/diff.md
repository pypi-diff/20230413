# Comparing `tmp/yotpy-0.0.4.tar.gz` & `tmp/yotpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.4.tar", last modified: Wed Apr 12 01:04:32 2023, max compression
+gzip compressed data, was "yotpy-0.0.5.tar", last modified: Wed Apr 12 19:49:57 2023, max compression
```

## Comparing `yotpy-0.0.4.tar` & `yotpy-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      298 2023-04-12 00:26:21.499743 yotpy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.4/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.4/README.md
--rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    28570 2023-04-12 01:03:49.147051 yotpy-0.0.4/yotpy.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      298 2023-04-12 00:26:21.499743 yotpy-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.5/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.5/README.md
+-rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    31441 2023-04-12 19:48:36.694873 yotpy-0.0.5/yotpy.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.5/PKG-INFO
```

### Comparing `yotpy-0.0.4/LICENSE` & `yotpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.4/pyproject.toml` & `yotpy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.4/yotpy.py` & `yotpy-0.0.5/yotpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 """
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 import asyncio
 import aiohttp
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
-from requests import post as requests_post
 from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
 from html import unescape
 from urllib.parse import urlencode
 from math import ceil
 from itertools import chain
 
 
@@ -253,14 +252,43 @@
 
         Returns:
             set[str]: A set of headers.
         """
         return {key for item in json_list for key in item.keys()}
 
     @staticmethod
+    def from_bigquery_iterator(iterator: Iterator, exclude: set[str] = {}, include: set[str] = {}) -> tuple[set, list]:
+        """
+        Convert a BigQuery RowIterator into a set of headers and a list of rows.
+
+        Args:
+            iterator (Iterator): A BigQuery RowIterator object.
+            exclude (set[str], optional): A set of field names to exclude from the output. Defaults to an empty set.
+            include (set[str], optional): A set of field names to include in the output. If provided, only these fields
+                                          will be included. Defaults to an empty set.
+
+        Returns:
+            tuple[set, list]: A tuple containing a set of headers and a list of rows as dictionaries.
+                              Headers are the field names included in the output, and rows are dictionaries
+                              containing field values for each row in the RowIterator.
+
+        Note:
+            If both `exclude` and `include` are provided, the `include` set takes precedence.
+        """
+        schema = list(iterator.schema)
+        headers = {field.name for field in schema if (include and field.name in include) or (exclude and field.name not in exclude)}
+
+        rows = []
+        for row in iterator:
+            [row.pop(field.name, None) for field in schema if field.name not in headers]
+            rows.append(row)
+
+        return headers, rows
+
+    @staticmethod
     def to_rows(json_list: list[dict], sep: str, exclude: list[str] = [], include: list[str] = []) -> tuple[list, set]:
         """
         Flatten a list of JSON objects into a list of rows and a set of headers.
         
         This method takes a list of nested JSON objects and converts each JSON object into a
         dictionary with keys representing the nested structure using a specified separator. 
         It then creates a list of rows, where each row contains the values from the flattened
@@ -548,17 +576,49 @@
             AppDataNotFound: If unable to get the app data.
         """
         app = await self.get_app()
 
         return app['data_for_events']['total_reviews']
     
     async def get_templates(self) -> dict:
+        """
+        Asynchronously fetch the email templates associated with the Yotpo account.
+
+        This method retrieves the app data, extracts the email templates, and returns them as a dictionary.
+        The primary use case for this function is to obtain the template IDs required for the 'send_review_request' method.
+
+        The returned dictionary contains template objects with properties such as 'id' (template_id),
+        'email_type', 'data', and others. For example:
+        ```python
+            {
+                'id': 10291872,
+                'account_id': 9092811,
+                'email_type_id': 31,
+                'email_type': {
+                    'id': 31,
+                    'name': 'mail_post_service',
+                    'template': 'testimonials_request'
+                },
+                'data': {
+                    'subject': 'Tell us what you think - {company_name}',
+                    'header': 'Hello {user},\\n We love having you as a customer and would really appreciate it if you filled out the form below.',
+                    'bottom': 'Thanks so much! <br> - {company_name}'
+                },
+                'formless_call_to_action': '',
+                'days_delay': 3,
+                'email_submission_type_id': 9
+            }
+        ```
+        Returns:
+            dict: A dictionary containing the email templates, keyed by their names.
+        """
         app = await self.get_app()
         templates = app['account_emails']
         return templates
+
         
     async def fetch_review_page(self, url: str) -> list[dict]:
         """
         Asynchronously fetch a single review page from the specified URL.
 
         This function fetches review data from the provided URL and parses the response based on whether
         the URL is for the widget endpoint or not.
```

### Comparing `yotpy-0.0.4/PKG-INFO` & `yotpy-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

