# Comparing `tmp/scrapingant-client-1.0.1.tar.gz` & `tmp/scrapingant-client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scrapingant-client-python/scrapingant-client-python/dist/tmpoaqbqsfb/scrapingant-client-1.0.1.tar", last modified: Sun Oct 23 15:01:44 2022, max compression
+gzip compressed data, was "/home/runner/work/scrapingant-client-python/scrapingant-client-python/dist/.tmp-7gvksitd/scrapingant-client-2.0.0.tar", last modified: Thu Apr 13 08:18:02 2023, max compression
```

## Comparing `scrapingant-client-1.0.1.tar` & `scrapingant-client-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     8695 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7793 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/cookie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/response.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/scrapingant_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8695 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/scrapingant_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 15:01:44.000000 scrapingant-client-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-10-23 15:01:36.000000 scrapingant-client-1.0.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/scrapingant_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/scrapingant_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:18:02.000000 scrapingant-client-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-13 08:17:52.000000 scrapingant-client-2.0.0/tests/test_integration.py
```

### Comparing `scrapingant-client-1.0.1/PKG-INFO` & `scrapingant-client-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: scrapingant-client
-Version: 1.0.1
-Summary: Official python client for the ScrapingAnt API.
-Home-page: https://github.com/ScrapingAnt/scrapingant-client-python
-Author: andrii.kovalenko
-Author-email: adrekoval@gmail.com
-License: Apache-2.0
-Keywords: scrapingant api scraper scraping
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: ~=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: async
-
 # ScrapingAnt API client for Python
 
 [![PyPI version](https://badge.fury.io/py/scrapingant-client.svg)](https://badge.fury.io/py/scrapingant-client)
 
 `scrapingant-client` is the official library to access [ScrapingAnt API](https://docs.scrapingant.com) from your Python
 applications. It provides useful features like parameters encoding to improve the ScrapingAnt usage experience. Requires
 python 3.6+.
@@ -42,15 +19,15 @@
 
 ## Quick Start
 
 ```python3
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
-# Scrape the example.com site.
+# Scrape the example.com site
 result = client.general_request('https://example.com')
 print(result.content)
 ```
 
 ## Install
 
 ```shell
@@ -81,50 +58,52 @@
 
 * * *
 
 #### ScrapingAntClient.general_request and ScrapingAntClient.general_request_async
 
 https://docs.scrapingant.com/request-response-format#available-parameters
 
-| Param             | Type                              | Default    |
-|-------------------|-----------------------------------|------------|
-| url               | <code>string</code>               |            |
-| cookies           | <code>List[Cookie]</code>         | None       |
-| headers           | <code>List[Dict[str, str]]</code> | None       |
-| js_snippet        | <code>string</code>               | None       |
-| proxy_type        | <code>ProxyType</code>            | datacenter | 
-| proxy_country     | <code>str</code>                  | None       | 
-| return_text       | <code>boolean</code>              | False      |
-| wait_for_selector | <code>str</code>                  | None       |
-| browser           | <code>boolean</code>              | True       |
+| Param             | Type                                                                                                                       | Default    |
+|-------------------|----------------------------------------------------------------------------------------------------------------------------|------------|
+| url               | <code>string</code>                                                                                                        |            |
+| method            | <code>string</code>                                                                                                        | GET        |
+| cookies           | <code>List[Cookie]</code>                                                                                                  | None       |
+| headers           | <code>List[Dict[str, str]]</code>                                                                                          | None       |
+| js_snippet        | <code>string</code>                                                                                                        | None       |
+| proxy_type        | <code>ProxyType</code>                                                                                                     | datacenter | 
+| proxy_country     | <code>str</code>                                                                                                           | None       | 
+| wait_for_selector | <code>str</code>                                                                                                           | None       |
+| browser           | <code>boolean</code>                                                                                                       | True       |
+| data              | same as [requests param 'data'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
+| json              | same as [requests param 'json'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
 
 **IMPORTANT NOTE:** <code>js_snippet</code> will be encoded to Base64 automatically by the ScrapingAnt client library.
 
 * * *
 
 #### Cookie
 
 Class defining cookie. Currently it supports only name and value
 
-| Param | Type                | 
+| Param |  Type               | 
 |-------|---------------------|
 | name  | <code>string</code> | 
 | value | <code>string</code> |
 
 * * *
 
 #### Response
 
 Class defining response from API.
-
-| Param       | Type                      |
-|-------------|---------------------------|
-| content     | <code>string</code>       |
-| cookies     | <code>List[Cookie]</code> |
-| status_code | <code>int</code>          |
+| Param       | Type                       |
+|-------------|----------------------------|
+| content     | <code>string</code>        |
+| cookies     | <code>List[Cookie]</code>  |
+| status_code | <code>int</code>           |
+| text        | <code>string</code>        |
 
 ## Exceptions
 
 `ScrapingantClientException` is base Exception class, used for all errors.
 
 | Exception                            | Reason                                                                                                                       |
 |--------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
@@ -250,19 +229,43 @@
 
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
 
 
 async def main():
-    # Scrape the example.com site.
+    # Scrape the example.com site
     result = await client.general_request_async('https://example.com')
     print(result.content)
 
 
 asyncio.run(main())
 ```
 
+### Sending POST request
+
+```python3
+from scrapingant_client import ScrapingAntClient
+
+client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
+
+# Sending POST request with json data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    json={"test": "test"},
+)
+print(result.content)
+
+# Sending POST request with bytes data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    data=b'test_bytes',
+)
+print(result.content)
+```
+
 ## Useful links
 
 - [Scrapingant API doumentation](https://docs.scrapingant.com)
 - [Scrapingant JS Client](https://github.com/scrapingant/scrapingant-client-js)
```

### Comparing `scrapingant-client-1.0.1/README.md` & `scrapingant-client-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: scrapingant-client
+Version: 2.0.0
+Summary: Official python client for the ScrapingAnt API.
+Home-page: https://github.com/ScrapingAnt/scrapingant-client-python
+Author: andrii.kovalenko
+Author-email: adrekoval@gmail.com
+License: Apache-2.0
+Keywords: scrapingant api scraper scraping
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: async
+
 # ScrapingAnt API client for Python
 
 [![PyPI version](https://badge.fury.io/py/scrapingant-client.svg)](https://badge.fury.io/py/scrapingant-client)
 
 `scrapingant-client` is the official library to access [ScrapingAnt API](https://docs.scrapingant.com) from your Python
 applications. It provides useful features like parameters encoding to improve the ScrapingAnt usage experience. Requires
 python 3.6+.
@@ -19,15 +42,15 @@
 
 ## Quick Start
 
 ```python3
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
-# Scrape the example.com site.
+# Scrape the example.com site
 result = client.general_request('https://example.com')
 print(result.content)
 ```
 
 ## Install
 
 ```shell
@@ -58,50 +81,52 @@
 
 * * *
 
 #### ScrapingAntClient.general_request and ScrapingAntClient.general_request_async
 
 https://docs.scrapingant.com/request-response-format#available-parameters
 
-| Param             | Type                              | Default    |
-|-------------------|-----------------------------------|------------|
-| url               | <code>string</code>               |            |
-| cookies           | <code>List[Cookie]</code>         | None       |
-| headers           | <code>List[Dict[str, str]]</code> | None       |
-| js_snippet        | <code>string</code>               | None       |
-| proxy_type        | <code>ProxyType</code>            | datacenter | 
-| proxy_country     | <code>str</code>                  | None       | 
-| return_text       | <code>boolean</code>              | False      |
-| wait_for_selector | <code>str</code>                  | None       |
-| browser           | <code>boolean</code>              | True       |
+| Param             | Type                                                                                                                       | Default    |
+|-------------------|----------------------------------------------------------------------------------------------------------------------------|------------|
+| url               | <code>string</code>                                                                                                        |            |
+| method            | <code>string</code>                                                                                                        | GET        |
+| cookies           | <code>List[Cookie]</code>                                                                                                  | None       |
+| headers           | <code>List[Dict[str, str]]</code>                                                                                          | None       |
+| js_snippet        | <code>string</code>                                                                                                        | None       |
+| proxy_type        | <code>ProxyType</code>                                                                                                     | datacenter | 
+| proxy_country     | <code>str</code>                                                                                                           | None       | 
+| wait_for_selector | <code>str</code>                                                                                                           | None       |
+| browser           | <code>boolean</code>                                                                                                       | True       |
+| data              | same as [requests param 'data'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
+| json              | same as [requests param 'json'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
 
 **IMPORTANT NOTE:** <code>js_snippet</code> will be encoded to Base64 automatically by the ScrapingAnt client library.
 
 * * *
 
 #### Cookie
 
 Class defining cookie. Currently it supports only name and value
 
-| Param | Type                | 
+| Param |  Type               | 
 |-------|---------------------|
 | name  | <code>string</code> | 
 | value | <code>string</code> |
 
 * * *
 
 #### Response
 
 Class defining response from API.
-
-| Param       | Type                      |
-|-------------|---------------------------|
-| content     | <code>string</code>       |
-| cookies     | <code>List[Cookie]</code> |
-| status_code | <code>int</code>          |
+| Param       | Type                       |
+|-------------|----------------------------|
+| content     | <code>string</code>        |
+| cookies     | <code>List[Cookie]</code>  |
+| status_code | <code>int</code>           |
+| text        | <code>string</code>        |
 
 ## Exceptions
 
 `ScrapingantClientException` is base Exception class, used for all errors.
 
 | Exception                            | Reason                                                                                                                       |
 |--------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
@@ -227,19 +252,43 @@
 
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
 
 
 async def main():
-    # Scrape the example.com site.
+    # Scrape the example.com site
     result = await client.general_request_async('https://example.com')
     print(result.content)
 
 
 asyncio.run(main())
 ```
 
+### Sending POST request
+
+```python3
+from scrapingant_client import ScrapingAntClient
+
+client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
+
+# Sending POST request with json data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    json={"test": "test"},
+)
+print(result.content)
+
+# Sending POST request with bytes data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    data=b'test_bytes',
+)
+print(result.content)
+```
+
 ## Useful links
 
 - [Scrapingant API doumentation](https://docs.scrapingant.com)
 - [Scrapingant JS Client](https://github.com/scrapingant/scrapingant-client-js)
```

### Comparing `scrapingant-client-1.0.1/scrapingant_client/__init__.py` & `scrapingant-client-2.0.0/scrapingant_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.1"
+__version__ = "2.0.0"
 
 from scrapingant_client.client import ScrapingAntClient
 from scrapingant_client.cookie import Cookie
 from scrapingant_client.errors import (
     ScrapingantClientException,
     ScrapingantInvalidTokenException,
     ScrapingantInvalidInputException,
```

### Comparing `scrapingant-client-1.0.1/scrapingant_client/client.py` & `scrapingant-client-2.0.0/scrapingant_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,127 +35,133 @@
     def _form_payload(
             self,
             url: str,
             cookies: Optional[List[Cookie]] = None,
             js_snippet: Optional[str] = None,
             proxy_type: ProxyType = ProxyType.datacenter,
             proxy_country: Optional[str] = None,
-            return_text: bool = False,
             wait_for_selector: Optional[str] = None,
             browser: bool = True,
     ) -> Dict:
         request_data = {'url': url}
         if cookies is not None:
             request_data['cookies'] = cookies_list_to_string(cookies)
         if js_snippet is not None:
             encoded_js_snippet = base64_encode_string(js_snippet)
             request_data['js_snippet'] = encoded_js_snippet
         request_data['proxy_type'] = proxy_type
         if proxy_country is not None:
             request_data['proxy_country'] = proxy_country.lower()
         if wait_for_selector is not None:
             request_data['wait_for_selector'] = wait_for_selector
-        request_data['return_text'] = return_text
         request_data['browser'] = browser
         return request_data
 
     def _parse_response(self, response_status_code: int, response_data: Dict, url: str) -> Response:
         if response_status_code == 403:
             raise ScrapingantInvalidTokenException()
         elif response_status_code == 404:
             raise ScrapingantSiteNotReachableException(url)
         elif response_status_code == 422:
             raise ScrapingantInvalidInputException(response_data)
         elif response_status_code == 423:
             raise ScrapingantDetectedException()
         elif response_status_code == 500:
             raise ScrapingantInternalException()
-        content = response_data['content']
+        content = response_data['html']
         cookies_string = response_data['cookies']
+        text = response_data['text']
         status_code = response_data['status_code']
         cookies_list = cookies_list_from_string(cookies_string)
         return Response(
             content=content,
             cookies=cookies_list,
+            text=text,
             status_code=status_code
         )
 
     def general_request(
             self,
             url: str,
+            method: str = 'GET',
             cookies: Optional[List[Cookie]] = None,
             headers: Optional[Dict[str, str]] = None,
             js_snippet: Optional[str] = None,
             proxy_type: ProxyType = ProxyType.datacenter,
             proxy_country: Optional[str] = None,
-            return_text: bool = False,
             wait_for_selector: Optional[str] = None,
             browser: bool = True,
+            data=None,
+            json=None,
     ) -> Response:
         request_data = self._form_payload(
             url=url,
             cookies=cookies,
             js_snippet=js_snippet,
             proxy_type=proxy_type,
             proxy_country=proxy_country,
-            return_text=return_text,
             wait_for_selector=wait_for_selector,
             browser=browser,
         )
         try:
-            response = self.requests_session.post(
-                SCRAPINGANT_API_BASE_URL + '/general',
-                json=request_data,
+            response = self.requests_session.request(
+                method=method,
+                url=SCRAPINGANT_API_BASE_URL + '/extended',
+                params=request_data,
                 headers=convert_headers(headers),
-                timeout=TIMEOUT_SECONDS
+                data=data,
+                json=json,
             )
         except requests.exceptions.Timeout:
             raise ScrapingantTimeoutException()
         response_status_code = response.status_code
         response_data = response.json()
         parsed_response: Response = self._parse_response(response_status_code, response_data, url)
         return parsed_response
 
     async def general_request_async(
             self,
             url: str,
+            method: str = 'GET',
             cookies: Optional[List[Cookie]] = None,
             headers: Optional[Dict[str, str]] = None,
             js_snippet: Optional[str] = None,
             proxy_type: ProxyType = ProxyType.datacenter,
             proxy_country: Optional[str] = None,
-            return_text: bool = False,
             wait_for_selector: Optional[str] = None,
             browser: bool = True,
+            data=None,
+            json=None,
     ) -> Response:
         import httpx
 
         request_data = self._form_payload(
             url=url,
             cookies=cookies,
             js_snippet=js_snippet,
             proxy_type=proxy_type,
             proxy_country=proxy_country,
-            return_text=return_text,
             wait_for_selector=wait_for_selector,
             browser=browser,
         )
         async with httpx.AsyncClient(
                 headers={
                     'x-api-key': self.token,
                     'User-Agent': self.user_agent,
                 },
                 timeout=TIMEOUT_SECONDS,
         ) as client:
             try:
-                response = await client.post(
-                    SCRAPINGANT_API_BASE_URL + '/general',
-                    json=request_data,
+                response = await client.request(
+                    method=method,
+                    url=SCRAPINGANT_API_BASE_URL + '/extended',
+                    params=request_data,
                     headers=convert_headers(headers),
+                    data=data,
+                    json=json,
                 )
             except httpx.TimeoutException:
                 raise ScrapingantTimeoutException()
-
         response_status_code = response.status_code
         response_data = response.json()
         parsed_response: Response = self._parse_response(response_status_code, response_data, url)
         return parsed_response
```

### Comparing `scrapingant-client-1.0.1/scrapingant_client/cookie.py` & `scrapingant-client-2.0.0/scrapingant_client/cookie.py`

 * *Files identical despite different names*

### Comparing `scrapingant-client-1.0.1/scrapingant_client/errors.py` & `scrapingant-client-2.0.0/scrapingant_client/errors.py`

 * *Files identical despite different names*

### Comparing `scrapingant-client-1.0.1/scrapingant_client.egg-info/PKG-INFO` & `scrapingant-client-2.0.0/scrapingant_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapingant-client
-Version: 1.0.1
+Version: 2.0.0
 Summary: Official python client for the ScrapingAnt API.
 Home-page: https://github.com/ScrapingAnt/scrapingant-client-python
 Author: andrii.kovalenko
 Author-email: adrekoval@gmail.com
 License: Apache-2.0
 Keywords: scrapingant api scraper scraping
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: ~=3.5
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: async
 
 # ScrapingAnt API client for Python
 
 [![PyPI version](https://badge.fury.io/py/scrapingant-client.svg)](https://badge.fury.io/py/scrapingant-client)
@@ -42,15 +42,15 @@
 
 ## Quick Start
 
 ```python3
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
-# Scrape the example.com site.
+# Scrape the example.com site
 result = client.general_request('https://example.com')
 print(result.content)
 ```
 
 ## Install
 
 ```shell
@@ -81,50 +81,52 @@
 
 * * *
 
 #### ScrapingAntClient.general_request and ScrapingAntClient.general_request_async
 
 https://docs.scrapingant.com/request-response-format#available-parameters
 
-| Param             | Type                              | Default    |
-|-------------------|-----------------------------------|------------|
-| url               | <code>string</code>               |            |
-| cookies           | <code>List[Cookie]</code>         | None       |
-| headers           | <code>List[Dict[str, str]]</code> | None       |
-| js_snippet        | <code>string</code>               | None       |
-| proxy_type        | <code>ProxyType</code>            | datacenter | 
-| proxy_country     | <code>str</code>                  | None       | 
-| return_text       | <code>boolean</code>              | False      |
-| wait_for_selector | <code>str</code>                  | None       |
-| browser           | <code>boolean</code>              | True       |
+| Param             | Type                                                                                                                       | Default    |
+|-------------------|----------------------------------------------------------------------------------------------------------------------------|------------|
+| url               | <code>string</code>                                                                                                        |            |
+| method            | <code>string</code>                                                                                                        | GET        |
+| cookies           | <code>List[Cookie]</code>                                                                                                  | None       |
+| headers           | <code>List[Dict[str, str]]</code>                                                                                          | None       |
+| js_snippet        | <code>string</code>                                                                                                        | None       |
+| proxy_type        | <code>ProxyType</code>                                                                                                     | datacenter | 
+| proxy_country     | <code>str</code>                                                                                                           | None       | 
+| wait_for_selector | <code>str</code>                                                                                                           | None       |
+| browser           | <code>boolean</code>                                                                                                       | True       |
+| data              | same as [requests param 'data'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
+| json              | same as [requests param 'json'](https://requests.readthedocs.io/en/latest/user/quickstart/#more-complicated-post-requests) | None       |
 
 **IMPORTANT NOTE:** <code>js_snippet</code> will be encoded to Base64 automatically by the ScrapingAnt client library.
 
 * * *
 
 #### Cookie
 
 Class defining cookie. Currently it supports only name and value
 
-| Param | Type                | 
+| Param |  Type               | 
 |-------|---------------------|
 | name  | <code>string</code> | 
 | value | <code>string</code> |
 
 * * *
 
 #### Response
 
 Class defining response from API.
-
-| Param       | Type                      |
-|-------------|---------------------------|
-| content     | <code>string</code>       |
-| cookies     | <code>List[Cookie]</code> |
-| status_code | <code>int</code>          |
+| Param       | Type                       |
+|-------------|----------------------------|
+| content     | <code>string</code>        |
+| cookies     | <code>List[Cookie]</code>  |
+| status_code | <code>int</code>           |
+| text        | <code>string</code>        |
 
 ## Exceptions
 
 `ScrapingantClientException` is base Exception class, used for all errors.
 
 | Exception                            | Reason                                                                                                                       |
 |--------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
@@ -250,19 +252,43 @@
 
 from scrapingant_client import ScrapingAntClient
 
 client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
 
 
 async def main():
-    # Scrape the example.com site.
+    # Scrape the example.com site
     result = await client.general_request_async('https://example.com')
     print(result.content)
 
 
 asyncio.run(main())
 ```
 
+### Sending POST request
+
+```python3
+from scrapingant_client import ScrapingAntClient
+
+client = ScrapingAntClient(token='<YOUR-SCRAPINGANT-API-TOKEN>')
+
+# Sending POST request with json data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    json={"test": "test"},
+)
+print(result.content)
+
+# Sending POST request with bytes data
+result = client.general_request(
+    url="https://httpbin.org/post",
+    method="POST",
+    data=b'test_bytes',
+)
+print(result.content)
+```
+
 ## Useful links
 
 - [Scrapingant API doumentation](https://docs.scrapingant.com)
 - [Scrapingant JS Client](https://github.com/scrapingant/scrapingant-client-js)
```

### Comparing `scrapingant-client-1.0.1/scrapingant_client.egg-info/SOURCES.txt` & `scrapingant-client-2.0.0/scrapingant_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapingant-client-1.0.1/setup.py` & `scrapingant-client-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP :: Browsers",
         "License :: OSI Approved :: Apache Software License",
     ],
     keywords="scrapingant api scraper scraping",
-    python_requires='~=3.5',
+    python_requires='~=3.7',
     install_requires=['requests>=2,<3'],
     extras_require={
         'dev': [
             'pytest>=7,<8',
             'flake8>=4,<5',
             'responses>=0,<1',
             'pytest-httpx>=0,<1',
```

### Comparing `scrapingant-client-1.0.1/tests/test_cookies.py` & `scrapingant-client-2.0.0/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `scrapingant-client-1.0.1/tests/test_exceptions.py` & `scrapingant-client-2.0.0/tests/test_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,61 +12,61 @@
     ScrapingantTimeoutException,
 )
 from scrapingant_client.constants import SCRAPINGANT_API_BASE_URL
 
 
 @responses.activate
 def test_invalid_token():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   json={'detail': 'wrong token'}, status=403)
     client = ScrapingAntClient(token='invalid_token')
     with pytest.raises(ScrapingantInvalidTokenException):
         client.general_request('example.com')
 
 
 @responses.activate
 def test_invalid_input():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   json={'detail': 'wrong url'}, status=422)
     client = ScrapingAntClient(token='some_token')
     with pytest.raises(ScrapingantInvalidInputException) as e:
         client.general_request('bad_url')
     assert 'wrong url' in str(e)
 
 
 @responses.activate
 def test_internal_server_error():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   json={}, status=500)
     client = ScrapingAntClient(token='some_token')
     with pytest.raises(ScrapingantInternalException):
         client.general_request('bad_url')
 
 
 @responses.activate
 def test_not_reachable():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   json={}, status=404)
     client = ScrapingAntClient(token='some_token')
     with pytest.raises(ScrapingantSiteNotReachableException) as e:
         client.general_request('example.com')
     assert 'The requested URL is not reachable (example.com)' in str(e)
 
 
 @responses.activate
 def test_detected():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   json={}, status=423)
     client = ScrapingAntClient(token='some_token')
     with pytest.raises(ScrapingantDetectedException) as e:
         client.general_request('example.com')
     assert 'The anti-bot detection system has detected the request' in str(e)
 
 
 @responses.activate
 def test_timeout():
-    responses.add(responses.POST, SCRAPINGANT_API_BASE_URL + '/general',
+    responses.add(responses.GET, SCRAPINGANT_API_BASE_URL + '/extended',
                   body=requests.exceptions.ReadTimeout())
     client = ScrapingAntClient(token='some_token')
     with pytest.raises(ScrapingantTimeoutException) as e:
         client.general_request('example.com')
     assert 'Got timeout' in str(e)
```

### Comparing `scrapingant-client-1.0.1/tests/test_integration.py` & `scrapingant-client-2.0.0/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,99 +8,130 @@
 from scrapingant_client.constants import SCRAPINGANT_API_BASE_URL
 
 
 @responses.activate
 def test_integration():
     client = ScrapingAntClient(token='test_token')
     responses.add(
-        responses.POST,
-        url=SCRAPINGANT_API_BASE_URL + '/general',
+        responses.GET,
+        url=SCRAPINGANT_API_BASE_URL +
+        '/extended'
+        '?url=http%3A%2F%2Fexample.com'
+        '&cookies=test_name%3Dtest_value'
+        '&js_snippet=dGVzdF9qc19zdHJpbmc%3D'
+        '&proxy_type=datacenter'
+        '&proxy_country=test_country'
+        '&wait_for_selector=test_selector'
+        '&browser=True',
         json={
-            "content": "test_content",
+            "html": "test_content",
             "cookies": "test_key1=test_value1;test_key2=test_value2",
+            "text": "test_text",
             "status_code": 200,
         },
         status=200,
     )
     response = client.general_request(
         url='http://example.com',
         cookies=[Cookie('test_name', 'test_value')],
-        headers={'testheader': 'test_header_value'},
+        headers={
+            'testheader': 'test_header_value'},
         js_snippet='test_js_string',
         proxy_type=ProxyType.datacenter,
         proxy_country='test_country',
-        return_text=True,
         wait_for_selector='test_selector',
         browser=True,
     )
     expected = {
         'content': 'test_content',
         'cookies': [Cookie('test_key1', 'test_value1'), Cookie('test_key2', 'test_value2')],
-        'status_code': 200
+        "text": "test_text",
+        'status_code': 200,
     }
     assert response.__dict__ == expected
     assert len(responses.calls) == 1
 
-    expected_body = {
-        'browser': True,
-        'cookies': 'test_name=test_value',
-        'js_snippet': 'dGVzdF9qc19zdHJpbmc=',
-        'proxy_country': 'test_country',
-        'proxy_type': 'datacenter',
-        'return_text': True,
-        'url': 'http://example.com',
-        'wait_for_selector': 'test_selector',
-    }
-    assert json.loads(responses.calls[0].request.body) == expected_body
-
     headers = responses.calls[0].request.headers
     assert headers['ant-testheader'] == 'test_header_value'
     assert headers['x-api-key'] == 'test_token'
 
 
 @pytest.mark.asyncio
 async def test_integration_async(httpx_mock: HTTPXMock):
     client = ScrapingAntClient(token='test_token')
     httpx_mock.add_response(
-        method="POST",
-        url=SCRAPINGANT_API_BASE_URL + '/general',
+        method="GET",
+        url=SCRAPINGANT_API_BASE_URL +
+        '/extended'
+        '?url=http%3A%2F%2Fexample.com'
+        '&cookies=test_name%3Dtest_value'
+        '&js_snippet=dGVzdF9qc19zdHJpbmc%3D'
+        '&proxy_type=datacenter'
+        '&proxy_country=test_country'
+        '&wait_for_selector=test_selector'
+        '&browser=true',
         json={
-            "content": "test_content",
+            "html": "test_content",
             "cookies": "test_key1=test_value1;test_key2=test_value2",
+            "text": "test_text",
             "status_code": 200,
         },
         status_code=200,
     )
     response = await client.general_request_async(
         url='http://example.com',
         cookies=[Cookie('test_name', 'test_value')],
-        headers={'testheader': 'test_header_value'},
+        headers={
+            'testheader': 'test_header_value'},
         js_snippet='test_js_string',
         proxy_type=ProxyType.datacenter,
         proxy_country='test_country',
-        return_text=True,
         wait_for_selector='test_selector',
         browser=True,
     )
     expected = {
         'content': 'test_content',
         'cookies': [Cookie('test_key1', 'test_value1'), Cookie('test_key2', 'test_value2')],
-        'status_code': 200
+        "text": "test_text",
+        'status_code': 200,
     }
     assert response.__dict__ == expected
     assert len(httpx_mock.get_requests()) == 1
 
-    expected_body = {
-        'browser': True,
-        'cookies': 'test_name=test_value',
-        'js_snippet': 'dGVzdF9qc19zdHJpbmc=',
-        'proxy_country': 'test_country',
+    headers = httpx_mock.get_requests()[0].headers
+    assert headers['ant-testheader'] == 'test_header_value'
+    assert headers['x-api-key'] == 'test_token'
+
+
+@responses.activate
+def test_post():
+    client = ScrapingAntClient(token='test_token')
+    responses.add(
+        responses.POST,
+        url=SCRAPINGANT_API_BASE_URL + '/extended',
+        json={
+            "html": "test_content",
+            "cookies": "",
+            "text": "test_text",
+            "status_code": 200,
+        },
+        status=200,
+    )
+    client.general_request(
+        url='http://example.com',
+        method='POST',
+        json={
+            'test_key': 'test_value'},
+    )
+
+    assert len(responses.calls) == 1
+    assert responses.calls[0].request.method == 'POST'
+    assert json.loads(responses.calls[0].request.body) == {
+        'test_key': 'test_value'}
+    assert responses.calls[0].request.params == {
+        'browser': 'True',
         'proxy_type': 'datacenter',
-        'return_text': True,
         'url': 'http://example.com',
-        'wait_for_selector': 'test_selector',
     }
-    assert json.loads(httpx_mock.get_requests()[0].content) == expected_body
 
-    headers = httpx_mock.get_requests()[0].headers
-    assert headers['ant-testheader'] == 'test_header_value'
+    headers = responses.calls[0].request.headers
     assert headers['x-api-key'] == 'test_token'
```

