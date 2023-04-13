# Comparing `tmp/scrapy-zyte-api-0.8.0.tar.gz` & `tmp/scrapy-zyte-api-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-zyte-api-0.8.0.tar", last modified: Tue Mar 28 11:24:42 2023, max compression
+gzip compressed data, was "scrapy-zyte-api-0.8.1.tar", last modified: Thu Apr 13 06:30:08 2023, max compression
```

## Comparing `scrapy-zyte-api-0.8.0.tar` & `scrapy-zyte-api-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 11:24:42.384907 scrapy-zyte-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-03-28 11:24:42.384907 scrapy-zyte-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28662 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 11:24:42.384907 scrapy-zyte-api-0.8.0/scrapy_zyte_api/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/_downloader_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/_request_fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 11:24:42.384907 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-03-28 11:24:42.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-28 11:24:42.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 11:24:42.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 11:24:42.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 11:24:42.000000 scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-28 11:24:42.388907 scrapy-zyte-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-28 11:24:27.000000 scrapy-zyte-api-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28567 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/scrapy_zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_downloader_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/_request_fingerprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29333 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 06:30:08.000000 scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 06:30:08.621831 scrapy-zyte-api-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-13 06:29:59.000000 scrapy-zyte-api-0.8.1/setup.py
```

### Comparing `scrapy-zyte-api-0.8.0/PKG-INFO` & `scrapy-zyte-api-0.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: scrapy-zyte-api
-Version: 0.8.0
-Summary: Client library to process URLs through Zyte API
-Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
-Author: Zyte Group Ltd
-Author-email: info@zyte.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst
-
 ===============
 scrapy-zyte-api
 ===============
 
 .. image:: https://img.shields.io/pypi/v/scrapy-zyte-api.svg
    :target: https://pypi.python.org/pypi/scrapy-zyte-api
    :alt: PyPI Version
@@ -108,47 +89,47 @@
 Usage
 =====
 
 You can send requests through Zyte API in one of the following ways:
 
 -   Send all request through Zyte API by default, letting Zyte API parameters
     be chosen automatically based on your Scrapy request parameters. See
-    **Using transparent mode** below.
+    `Using transparent mode`_.
 
 -   Send specific requests through Zyte API, setting all Zyte API parameters
-    manually, keeping full control of what is sent to Zyte API. See **Sending
-    requests with manually-defined parameters** below.
+    manually, keeping full control of what is sent to Zyte API.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Send specific requests through Zyte API, letting Zyte API parameters be
-    chosen automatically based on your Scrapy request parameters. See **Sending
-    requests with automatically-mapped parameters** below.
+    chosen automatically based on your Scrapy request parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 Zyte API response parameters are mapped into Scrapy response parameters where
-possible. See **Response mapping** below for details.
+possible. See `Response mapping`_ for details.
 
 
 Using transparent mode
 ----------------------
 
 Set the ``ZYTE_API_TRANSPARENT_MODE`` `Scrapy setting`_ to ``True`` to handle
 Scrapy requests as follows:
 
 .. _Scrapy setting: https://docs.scrapy.org/en/latest/topics/settings.html
 
 -   By default, requests are sent through Zyte API with automatically-mapped
-    parameters. See **Sending requests with automatically-mapped parameters**
-    below for details about automatic request parameter mapping.
+    parameters. See `Sending requests with automatically-mapped parameters`_
+    for details about automatic request parameter mapping.
 
     You do not need to set the ``zyte_api_automap`` request meta key to
     ``True``, but you can set it to a dictionary to extend your Zyte API
     request parameters.
 
 -   Requests with the ``zyte_api`` request meta key set to a ``dict`` are sent
-    through Zyte API with manually-defined parameters. See **Sending requests
-    with manually-defined parameters** below.
+    through Zyte API with manually-defined parameters.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Requests with the ``zyte_api_automap`` request meta key set to ``False``
     are *not* sent through Zyte API.
 
 For example:
 
 .. code-block:: python
@@ -266,16 +247,15 @@
                 },
             )
 
         def parse(self, response):
             print(response.text)
             # "<html>…</html>"
 
-See also **Using transparent mode** above and **Automated request parameter
-mapping** below.
+See also `Using transparent mode`_ and `Automated request parameter mapping`_.
 
 
 Response mapping
 ----------------
 
 Zyte API responses are mapped with one of the following classes:
 
@@ -365,16 +345,16 @@
         # b'\x89PNG\r\n\x1a\n\x00\x00\x00\r…'
 
 
 Automated request parameter mapping
 -----------------------------------
 
 When you enable automated request parameter mapping, be it through transparent
-mode (see **Using transparent mode** above) or for a specific request (see
-**Sending requests with automatically-mapped parameters** above), Zyte API
+mode (see `Using transparent mode`_) or for a specific request (see
+`Sending requests with automatically-mapped parameters`_), Zyte API
 parameters are chosen as follows by default:
 
 -   ``Request.url`` becomes ``url``, same as in requests with manually-defined
     parameters.
 
 -   If ``Request.method`` is something other than ``"GET"``, it becomes
     ``httpRequestMethod``.
@@ -589,36 +569,35 @@
 example, all requests may need to set the same geolocation, or the spider only
 uses ``browserHtml`` requests.
 
 The following settings allow you to define Zyte API parameters to be included
 in all requests:
 
 -   ``ZYTE_API_DEFAULT_PARAMS`` is a ``dict`` of parameters to be combined with
-    manually-defined parameters. See **Sending requests with manually-defined
-    parameters** above.
+    manually-defined parameters. See `Sending requests with manually-defined parameters`_.
 
     You may set the ``zyte_api`` request meta key to an empty ``dict`` to only
     use default parameters for that request.
 
 -   ``ZYTE_API_AUTOMAP_PARAMS`` is a ``dict`` of parameters to be combined with
-    automatically-mapped parameters. See **Sending requests with
-    automatically-mapped parameters** above.
+    automatically-mapped parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 For example, if you set ``ZYTE_API_DEFAULT_PARAMS`` to
 ``{"geolocation": "US"}`` and ``zyte_api`` to ``{"browserHtml": True}``,
 ``{"url: "…", "geolocation": "US", "browserHtml": True}`` is sent to Zyte API.
 
 Parameters in these settings are merged with request-specific parameters, with
 request-specific parameters taking precedence.
 
 ``ZYTE_API_DEFAULT_PARAMS`` has no effect on requests that use automated
 request parameter mapping, and ``ZYTE_API_AUTOMAP_PARAMS`` has no effect on
 requests that use manually-defined parameters.
 
-When using transparent mode (see **Using transparent mode** above), be careful
+When using transparent mode (see `Using transparent mode`_), be careful
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
```

### Comparing `scrapy-zyte-api-0.8.0/README.rst` & `scrapy-zyte-api-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: scrapy-zyte-api
+Version: 0.8.1
+Summary: Client library to process URLs through Zyte API
+Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
+Author: Zyte Group Ltd
+Author-email: info@zyte.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 ===============
 scrapy-zyte-api
 ===============
 
 .. image:: https://img.shields.io/pypi/v/scrapy-zyte-api.svg
    :target: https://pypi.python.org/pypi/scrapy-zyte-api
    :alt: PyPI Version
@@ -89,47 +109,47 @@
 Usage
 =====
 
 You can send requests through Zyte API in one of the following ways:
 
 -   Send all request through Zyte API by default, letting Zyte API parameters
     be chosen automatically based on your Scrapy request parameters. See
-    **Using transparent mode** below.
+    `Using transparent mode`_.
 
 -   Send specific requests through Zyte API, setting all Zyte API parameters
-    manually, keeping full control of what is sent to Zyte API. See **Sending
-    requests with manually-defined parameters** below.
+    manually, keeping full control of what is sent to Zyte API.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Send specific requests through Zyte API, letting Zyte API parameters be
-    chosen automatically based on your Scrapy request parameters. See **Sending
-    requests with automatically-mapped parameters** below.
+    chosen automatically based on your Scrapy request parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 Zyte API response parameters are mapped into Scrapy response parameters where
-possible. See **Response mapping** below for details.
+possible. See `Response mapping`_ for details.
 
 
 Using transparent mode
 ----------------------
 
 Set the ``ZYTE_API_TRANSPARENT_MODE`` `Scrapy setting`_ to ``True`` to handle
 Scrapy requests as follows:
 
 .. _Scrapy setting: https://docs.scrapy.org/en/latest/topics/settings.html
 
 -   By default, requests are sent through Zyte API with automatically-mapped
-    parameters. See **Sending requests with automatically-mapped parameters**
-    below for details about automatic request parameter mapping.
+    parameters. See `Sending requests with automatically-mapped parameters`_
+    for details about automatic request parameter mapping.
 
     You do not need to set the ``zyte_api_automap`` request meta key to
     ``True``, but you can set it to a dictionary to extend your Zyte API
     request parameters.
 
 -   Requests with the ``zyte_api`` request meta key set to a ``dict`` are sent
-    through Zyte API with manually-defined parameters. See **Sending requests
-    with manually-defined parameters** below.
+    through Zyte API with manually-defined parameters.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Requests with the ``zyte_api_automap`` request meta key set to ``False``
     are *not* sent through Zyte API.
 
 For example:
 
 .. code-block:: python
@@ -247,16 +267,15 @@
                 },
             )
 
         def parse(self, response):
             print(response.text)
             # "<html>…</html>"
 
-See also **Using transparent mode** above and **Automated request parameter
-mapping** below.
+See also `Using transparent mode`_ and `Automated request parameter mapping`_.
 
 
 Response mapping
 ----------------
 
 Zyte API responses are mapped with one of the following classes:
 
@@ -346,16 +365,16 @@
         # b'\x89PNG\r\n\x1a\n\x00\x00\x00\r…'
 
 
 Automated request parameter mapping
 -----------------------------------
 
 When you enable automated request parameter mapping, be it through transparent
-mode (see **Using transparent mode** above) or for a specific request (see
-**Sending requests with automatically-mapped parameters** above), Zyte API
+mode (see `Using transparent mode`_) or for a specific request (see
+`Sending requests with automatically-mapped parameters`_), Zyte API
 parameters are chosen as follows by default:
 
 -   ``Request.url`` becomes ``url``, same as in requests with manually-defined
     parameters.
 
 -   If ``Request.method`` is something other than ``"GET"``, it becomes
     ``httpRequestMethod``.
@@ -570,36 +589,35 @@
 example, all requests may need to set the same geolocation, or the spider only
 uses ``browserHtml`` requests.
 
 The following settings allow you to define Zyte API parameters to be included
 in all requests:
 
 -   ``ZYTE_API_DEFAULT_PARAMS`` is a ``dict`` of parameters to be combined with
-    manually-defined parameters. See **Sending requests with manually-defined
-    parameters** above.
+    manually-defined parameters. See `Sending requests with manually-defined parameters`_.
 
     You may set the ``zyte_api`` request meta key to an empty ``dict`` to only
     use default parameters for that request.
 
 -   ``ZYTE_API_AUTOMAP_PARAMS`` is a ``dict`` of parameters to be combined with
-    automatically-mapped parameters. See **Sending requests with
-    automatically-mapped parameters** above.
+    automatically-mapped parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 For example, if you set ``ZYTE_API_DEFAULT_PARAMS`` to
 ``{"geolocation": "US"}`` and ``zyte_api`` to ``{"browserHtml": True}``,
 ``{"url: "…", "geolocation": "US", "browserHtml": True}`` is sent to Zyte API.
 
 Parameters in these settings are merged with request-specific parameters, with
 request-specific parameters taking precedence.
 
 ``ZYTE_API_DEFAULT_PARAMS`` has no effect on requests that use automated
 request parameter mapping, and ``ZYTE_API_AUTOMAP_PARAMS`` has no effect on
 requests that use manually-defined parameters.
 
-When using transparent mode (see **Using transparent mode** above), be careful
+When using transparent mode (see `Using transparent mode`_), be careful
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
```

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/_cookies.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_cookies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from http.cookiejar import Cookie
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from scrapy.http import Request
 from scrapy.http.cookies import CookieJar
 
 
 def _get_cookie_jar(request: Request, cookie_jars: Dict[Any, CookieJar]) -> CookieJar:
     jar_id = request.meta.get("cookiejar")
     return cookie_jars[jar_id]
 
 
 def _process_cookies(
-    api_response: Dict[str, Any], request: Request, cookie_jars: Dict[Any, CookieJar]
+    api_response: Dict[str, Any],
+    request: Request,
+    cookie_jars: Optional[Dict[Any, CookieJar]],
 ):
+    if not cookie_jars:
+        return
     response_cookies = api_response.get("experimental", {}).get("responseCookies")
     if not response_cookies:
         return
     cookie_jar = _get_cookie_jar(request, cookie_jars)
     for response_cookie in response_cookies:
         rest = {}
         http_only = response_cookie.get("httpOnly", None)
```

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/_downloader_middleware.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_downloader_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ._params import _ParamParser
 
 
 class ScrapyZyteAPIDownloaderMiddleware:
-
     _slot_prefix = "zyte-api@"
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls(crawler)
 
     def __init__(self, crawler) -> None:
```

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/_params.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_params.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/_request_fingerprinter.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/_request_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/handler.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,14 @@
             logger.error(
                 f"Got an error when processing Zyte API request ({request.url}): {er}"
             )
             raise
         finally:
             self._update_stats()
 
-        assert self._cookie_jars is not None  # typing
         return _process_response(api_response, request, self._cookie_jars)
 
     def _log_request(self, params):
         if not self._must_log_request:
             return
         params = self._truncate_params(params)
         logger.debug(f"Sending Zyte API extract request: {json.dumps(params)}")
```

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/responses.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     _RESPONSE_HAS_PROTOCOL,
 )
 
 _DEFAULT_ENCODING = "utf-8"
 
 
 class ZyteAPIMixin:
-
     REMOVE_HEADERS = {
         # Zyte API already decompresses the HTTP Response Body. Scrapy's
         # HttpCompressionMiddleware will error out when it attempts to
         # decompress an already decompressed body based on this header.
         "content-encoding"
     }
 
@@ -158,15 +157,17 @@
 _JSON = Union[
     None, str, int, float, bool, List["_JSON"], Dict[_IMMUTABLE_JSON, "_JSON"]
 ]
 _API_RESPONSE = Dict[str, _JSON]
 
 
 def _process_response(
-    api_response: _API_RESPONSE, request: Request, cookie_jars: Dict[Any, CookieJar]
+    api_response: _API_RESPONSE,
+    request: Request,
+    cookie_jars: Optional[Dict[Any, CookieJar]],
 ) -> Optional[Union[ZyteAPITextResponse, ZyteAPIResponse]]:
     """Given a Zyte API Response and the ``scrapy.Request`` that asked for it,
     this returns either a ``ZyteAPITextResponse`` or ``ZyteAPIResponse`` depending
     on which if it can properly decode the HTTP Body or have access to browserHtml.
     """
 
     # NOTES: Currently, Zyte API does NOT only allow both 'browserHtml' and
```

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api/utils.py` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.0/scrapy_zyte_api.egg-info/PKG-INFO` & `scrapy-zyte-api-0.8.1/scrapy_zyte_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 ===============
 scrapy-zyte-api
 ===============
 
 .. image:: https://img.shields.io/pypi/v/scrapy-zyte-api.svg
    :target: https://pypi.python.org/pypi/scrapy-zyte-api
@@ -108,47 +109,47 @@
 Usage
 =====
 
 You can send requests through Zyte API in one of the following ways:
 
 -   Send all request through Zyte API by default, letting Zyte API parameters
     be chosen automatically based on your Scrapy request parameters. See
-    **Using transparent mode** below.
+    `Using transparent mode`_.
 
 -   Send specific requests through Zyte API, setting all Zyte API parameters
-    manually, keeping full control of what is sent to Zyte API. See **Sending
-    requests with manually-defined parameters** below.
+    manually, keeping full control of what is sent to Zyte API.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Send specific requests through Zyte API, letting Zyte API parameters be
-    chosen automatically based on your Scrapy request parameters. See **Sending
-    requests with automatically-mapped parameters** below.
+    chosen automatically based on your Scrapy request parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 Zyte API response parameters are mapped into Scrapy response parameters where
-possible. See **Response mapping** below for details.
+possible. See `Response mapping`_ for details.
 
 
 Using transparent mode
 ----------------------
 
 Set the ``ZYTE_API_TRANSPARENT_MODE`` `Scrapy setting`_ to ``True`` to handle
 Scrapy requests as follows:
 
 .. _Scrapy setting: https://docs.scrapy.org/en/latest/topics/settings.html
 
 -   By default, requests are sent through Zyte API with automatically-mapped
-    parameters. See **Sending requests with automatically-mapped parameters**
-    below for details about automatic request parameter mapping.
+    parameters. See `Sending requests with automatically-mapped parameters`_
+    for details about automatic request parameter mapping.
 
     You do not need to set the ``zyte_api_automap`` request meta key to
     ``True``, but you can set it to a dictionary to extend your Zyte API
     request parameters.
 
 -   Requests with the ``zyte_api`` request meta key set to a ``dict`` are sent
-    through Zyte API with manually-defined parameters. See **Sending requests
-    with manually-defined parameters** below.
+    through Zyte API with manually-defined parameters.
+    See `Sending requests with manually-defined parameters`_.
 
 -   Requests with the ``zyte_api_automap`` request meta key set to ``False``
     are *not* sent through Zyte API.
 
 For example:
 
 .. code-block:: python
@@ -266,16 +267,15 @@
                 },
             )
 
         def parse(self, response):
             print(response.text)
             # "<html>…</html>"
 
-See also **Using transparent mode** above and **Automated request parameter
-mapping** below.
+See also `Using transparent mode`_ and `Automated request parameter mapping`_.
 
 
 Response mapping
 ----------------
 
 Zyte API responses are mapped with one of the following classes:
 
@@ -365,16 +365,16 @@
         # b'\x89PNG\r\n\x1a\n\x00\x00\x00\r…'
 
 
 Automated request parameter mapping
 -----------------------------------
 
 When you enable automated request parameter mapping, be it through transparent
-mode (see **Using transparent mode** above) or for a specific request (see
-**Sending requests with automatically-mapped parameters** above), Zyte API
+mode (see `Using transparent mode`_) or for a specific request (see
+`Sending requests with automatically-mapped parameters`_), Zyte API
 parameters are chosen as follows by default:
 
 -   ``Request.url`` becomes ``url``, same as in requests with manually-defined
     parameters.
 
 -   If ``Request.method`` is something other than ``"GET"``, it becomes
     ``httpRequestMethod``.
@@ -589,36 +589,35 @@
 example, all requests may need to set the same geolocation, or the spider only
 uses ``browserHtml`` requests.
 
 The following settings allow you to define Zyte API parameters to be included
 in all requests:
 
 -   ``ZYTE_API_DEFAULT_PARAMS`` is a ``dict`` of parameters to be combined with
-    manually-defined parameters. See **Sending requests with manually-defined
-    parameters** above.
+    manually-defined parameters. See `Sending requests with manually-defined parameters`_.
 
     You may set the ``zyte_api`` request meta key to an empty ``dict`` to only
     use default parameters for that request.
 
 -   ``ZYTE_API_AUTOMAP_PARAMS`` is a ``dict`` of parameters to be combined with
-    automatically-mapped parameters. See **Sending requests with
-    automatically-mapped parameters** above.
+    automatically-mapped parameters.
+    See `Sending requests with automatically-mapped parameters`_.
 
 For example, if you set ``ZYTE_API_DEFAULT_PARAMS`` to
 ``{"geolocation": "US"}`` and ``zyte_api`` to ``{"browserHtml": True}``,
 ``{"url: "…", "geolocation": "US", "browserHtml": True}`` is sent to Zyte API.
 
 Parameters in these settings are merged with request-specific parameters, with
 request-specific parameters taking precedence.
 
 ``ZYTE_API_DEFAULT_PARAMS`` has no effect on requests that use automated
 request parameter mapping, and ``ZYTE_API_AUTOMAP_PARAMS`` has no effect on
 requests that use manually-defined parameters.
 
-When using transparent mode (see **Using transparent mode** above), be careful
+When using transparent mode (see `Using transparent mode`_), be careful
 of which parameters you define through ``ZYTE_API_AUTOMAP_PARAMS``. In
 transparent mode, all Scrapy requests go through Zyte API, even requests that
 Scrapy sends automatically, such as those for ``robots.txt`` files when
 ROBOTSTXT_OBEY_ is ``True``, or those for sitemaps when using a `sitemap
 spider`_. Certain parameters, like ``browserHtml`` or ``screenshot``, are not
 meant to be used for every single request.
```

### Comparing `scrapy-zyte-api-0.8.0/setup.py` & `scrapy-zyte-api-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="scrapy-zyte-api",
-    version="0.8.0",
+    version="0.8.1",
     description="Client library to process URLs through Zyte API",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="info@zyte.com",
     url="https://github.com/scrapy-plugins/scrapy-zyte-api",
     packages=["scrapy_zyte_api"],
```

