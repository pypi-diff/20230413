# Comparing `tmp/satellitevu-1.3.0.tar.gz` & `tmp/satellitevu-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellitevu-1.3.0.tar", max compression
+gzip compressed data, was "satellitevu-1.4.0.tar", max compression
```

## Comparing `satellitevu-1.3.0.tar` & `satellitevu-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1080 2023-01-27 11:11:11.781025 satellitevu-1.3.0/LICENSE
--rw-r--r--   0        0        0     3336 2023-01-27 11:11:11.781147 satellitevu-1.3.0/README.md
--rw-r--r--   0        0        0     1031 2023-02-09 11:11:42.859767 satellitevu-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-01-27 11:11:11.782945 satellitevu-1.3.0/satellitevu/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 11:11:11.783058 satellitevu-1.3.0/satellitevu/apis/__init__.py
--rw-r--r--   0        0        0     2838 2023-02-09 11:11:42.860359 satellitevu-1.3.0/satellitevu/apis/archive.py
--rw-r--r--   0        0        0     2440 2023-01-27 11:11:11.783313 satellitevu-1.3.0/satellitevu/apis/archive_test.py
--rw-r--r--   0        0        0     1175 2023-02-08 11:00:34.271093 satellitevu-1.3.0/satellitevu/apis/base.py
--rw-r--r--   0        0        0     1287 2023-02-09 11:11:42.860726 satellitevu-1.3.0/satellitevu/apis/base_test.py
--rw-r--r--   0        0        0     5617 2023-02-27 17:01:35.746721 satellitevu-1.3.0/satellitevu/apis/orders.py
--rw-r--r--   0        0        0    10041 2023-01-27 11:11:11.783652 satellitevu-1.3.0/satellitevu/apis/orders_test.py
--rw-r--r--   0        0        0      149 2023-01-27 11:11:11.783803 satellitevu-1.3.0/satellitevu/auth/__init__.py
--rw-r--r--   0        0        0     2799 2023-01-27 11:11:11.783914 satellitevu-1.3.0/satellitevu/auth/auth.py
--rw-r--r--   0        0        0     1664 2023-02-08 11:18:37.912057 satellitevu-1.3.0/satellitevu/auth/auth_test.py
--rw-r--r--   0        0        0     1956 2023-01-27 11:11:11.784142 satellitevu-1.3.0/satellitevu/auth/cache.py
--rw-r--r--   0        0        0     2144 2023-01-27 11:11:11.784314 satellitevu-1.3.0/satellitevu/auth/cache_test.py
--rw-r--r--   0        0        0      122 2023-01-27 11:11:11.784424 satellitevu-1.3.0/satellitevu/auth/exc.py
--rw-r--r--   0        0        0     1842 2023-01-27 11:11:11.784538 satellitevu-1.3.0/satellitevu/client.py
--rw-r--r--   0        0        0     1363 2023-01-27 11:11:11.784635 satellitevu-1.3.0/satellitevu/config.py
--rw-r--r--   0        0        0     2406 2023-02-07 16:07:46.455658 satellitevu-1.3.0/satellitevu/conftest.py
--rw-r--r--   0        0        0      148 2023-01-27 11:11:11.784875 satellitevu-1.3.0/satellitevu/http/__init__.py
--rw-r--r--   0        0        0     2038 2023-02-27 17:01:32.974560 satellitevu-1.3.0/satellitevu/http/base.py
--rw-r--r--   0        0        0     3327 2023-02-07 16:07:46.456241 satellitevu-1.3.0/satellitevu/http/http_test.py
--rw-r--r--   0        0        0     1305 2023-02-07 16:07:46.456449 satellitevu-1.3.0/satellitevu/http/httpx.py
--rw-r--r--   0        0        0     1334 2023-02-07 16:07:46.456623 satellitevu-1.3.0/satellitevu/http/requests.py
--rw-r--r--   0        0        0     1744 2023-02-07 16:07:46.456798 satellitevu-1.3.0/satellitevu/http/urllib.py
--rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 satellitevu-1.3.0/setup.py
--rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 satellitevu-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-13 07:17:49.629738 satellitevu-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3336 2023-04-13 07:17:49.629738 satellitevu-1.4.0/README.md
+-rw-r--r--   0        0        0     1031 2023-04-13 09:05:24.864379 satellitevu-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/__init__.py
+-rw-r--r--   0        0        0     2838 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/archive.py
+-rw-r--r--   0        0        0     2440 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/archive_test.py
+-rw-r--r--   0        0        0     1175 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/base.py
+-rw-r--r--   0        0        0     1287 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/base_test.py
+-rw-r--r--   0        0        0     5617 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/orders.py
+-rw-r--r--   0        0        0    10041 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/apis/orders_test.py
+-rw-r--r--   0        0        0     1261 2023-04-13 09:05:24.864379 satellitevu-1.4.0/satellitevu/apis/otm.py
+-rw-r--r--   0        0        0      149 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/__init__.py
+-rw-r--r--   0        0        0     2799 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/auth.py
+-rw-r--r--   0        0        0     1664 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/auth_test.py
+-rw-r--r--   0        0        0     1956 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/cache.py
+-rw-r--r--   0        0        0     2144 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/cache_test.py
+-rw-r--r--   0        0        0      122 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/auth/exc.py
+-rw-r--r--   0        0        0     2622 2023-04-13 09:05:24.864379 satellitevu-1.4.0/satellitevu/client.py
+-rw-r--r--   0        0        0     1363 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/config.py
+-rw-r--r--   0        0        0     2406 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/conftest.py
+-rw-r--r--   0        0        0      148 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/__init__.py
+-rw-r--r--   0        0        0     2038 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/base.py
+-rw-r--r--   0        0        0     3327 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/http_test.py
+-rw-r--r--   0        0        0     1305 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/httpx.py
+-rw-r--r--   0        0        0     1334 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/requests.py
+-rw-r--r--   0        0        0     1744 2023-04-13 07:17:49.633738 satellitevu-1.4.0/satellitevu/http/urllib.py
+-rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 satellitevu-1.4.0/PKG-INFO
```

### Comparing `satellitevu-1.3.0/LICENSE` & `satellitevu-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/README.md` & `satellitevu-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/pyproject.toml` & `satellitevu-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satellitevu"
-version = "1.3.0"
+version = "1.4.0"
 description = "Client SDK for SatelliteVu's platform APIs"
 authors = ["Christian Wygoda <christian.wygoda@satellitevu.com>", "Zhelini Sivanesan <zhelini.sivanesan@satellitevu.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `satellitevu-1.3.0/satellitevu/apis/archive.py` & `satellitevu-1.4.0/satellitevu/apis/archive.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/apis/archive_test.py` & `satellitevu-1.4.0/satellitevu/apis/archive_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/apis/base.py` & `satellitevu-1.4.0/satellitevu/apis/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/apis/base_test.py` & `satellitevu-1.4.0/satellitevu/apis/base_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/apis/orders.py` & `satellitevu-1.4.0/satellitevu/apis/orders.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/apis/orders_test.py` & `satellitevu-1.4.0/satellitevu/apis/orders_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/auth/auth.py` & `satellitevu-1.4.0/satellitevu/auth/auth.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/auth/auth_test.py` & `satellitevu-1.4.0/satellitevu/auth/auth_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/auth/cache.py` & `satellitevu-1.4.0/satellitevu/auth/cache.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/auth/cache_test.py` & `satellitevu-1.4.0/satellitevu/auth/cache_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/client.py` & `satellitevu-1.4.0/satellitevu/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,50 @@
-from typing import Optional, Union
+from typing import Dict, Optional, Union
+from warnings import warn
 
 from satellitevu.apis.archive import ArchiveV1
 from satellitevu.apis.orders import OrdersV1
+from satellitevu.apis.otm import OtmV1
 from satellitevu.auth import AbstractCache, Auth
 from satellitevu.config import GATEWAY
 from satellitevu.http import AbstractClient, UrllibClient
 
 
+class FutureApis:
+    otm: OtmV1
+
+    _called: Dict[str, bool] = {}
+
+    def __init__(self, client: AbstractClient, gateway_url: str):
+        self.otm = OtmV1(client, gateway_url)
+
+    def __getattribute__(self, __name: str):
+        attr = super().__getattribute__(__name)
+        if __name != "_called":
+            has_been_called = self._called.get(__name, False)
+            self._called[__name] = True
+            if not has_been_called:
+                warn(
+                    f"{__name} is a not yet a stable API. Use at own risk",
+                    FutureWarning,
+                )
+        return attr
+
+
 class Client:
     _client: AbstractClient
     _gateway_url: str
 
     auth: Auth
 
     archive_v1: ArchiveV1
     orders_v1: OrdersV1
 
+    future: FutureApis
+
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         *,
         audience: Optional[str] = None,
         cache: Optional[AbstractCache] = None,
@@ -39,14 +64,16 @@
             client=self._client,
         )
         self._client.set_auth(self._gateway_url, self.auth)
 
         self.archive_v1 = ArchiveV1(self._client, self._gateway_url)
         self.orders_v1 = OrdersV1(self._client, self._gateway_url)
 
+        self.future = FutureApis(self._client, self._gateway_url)
+
     def _setup_client(self) -> AbstractClient:
         client = self._setup_requests_session()
         if client is None:
             client = UrllibClient()
         return client
 
     def _setup_requests_session(self) -> Union[AbstractClient, None]:
```

### Comparing `satellitevu-1.3.0/satellitevu/config.py` & `satellitevu-1.4.0/satellitevu/config.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/conftest.py` & `satellitevu-1.4.0/satellitevu/conftest.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/http/base.py` & `satellitevu-1.4.0/satellitevu/http/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/http/http_test.py` & `satellitevu-1.4.0/satellitevu/http/http_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/http/httpx.py` & `satellitevu-1.4.0/satellitevu/http/httpx.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/http/requests.py` & `satellitevu-1.4.0/satellitevu/http/requests.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/satellitevu/http/urllib.py` & `satellitevu-1.4.0/satellitevu/http/urllib.py`

 * *Files identical despite different names*

### Comparing `satellitevu-1.3.0/setup.py` & `satellitevu-1.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: satellitevu
+Version: 1.4.0
+Summary: Client SDK for SatelliteVu's platform APIs
+License: MIT
+Author: Christian Wygoda
+Author-email: christian.wygoda@satellitevu.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['satellitevu', 'satellitevu.apis', 'satellitevu.auth', 'satellitevu.http']
+# SatelliteVu SDK for Python
 
-package_data = \
-{'': ['*']}
+Lightweight API Client SDK for SatelliteVu's Platform APIs, providing authorization
+handling and convenience methods to interact with the published APIs.
 
-install_requires = \
-['appdirs>=1.4.4,<2.0.0']
-
-setup_kwargs = {
-    'name': 'satellitevu',
-    'version': '1.3.0',
-    'description': "Client SDK for SatelliteVu's platform APIs",
-    'long_description': '# SatelliteVu SDK for Python\n\nLightweight API Client SDK for SatelliteVu\'s Platform APIs, providing authorization\nhandling and convenience methods to interact with the published APIs.\n\n## Installation\n\nThe package is published to [PyPi][pypi] and can be installed with pip:\n\n```\npip install satellitevu\n```\n\nCurrently Python 3.8 and Python 3.10 are supported.\n\n## Usage\n\nA User API Client credential set consisting of an _client id_ and _client secret_ is\nneeded and should be set in your script\'s environment variables.\n\nCheck out the [examples][examples] provided. They can for example be run locally with\n\n```\npoetry run python ./examples/archive.py --example=recent\n```\n\n### Simple Client Usage\n\nThe easiest way to get started is to use the `satellitevu.Client` class, which needs\na client_id and client_secret only:\n\n```\nimport os\n\nfrom satellitevu import Client\n\n\nclient = Client(os.getenv("CLIENT_ID"), os.getenv("CLIENT_SECRET"))\nprint(client.archive_v1.search().json())\n```\n\n`client.archive_v1.search` supports all supported request body parameters documented\nin the [API docs][search-api-docs], with special handling for `datetime` which is\nconstructed from the optional `date_from` and `date_to` parameters and a default result\npage size limit of 25.\n\n### Authentication Handling\n\nThe `satellitevu.Auth` class provides the main interface to retrieve an\nauthorization token required to interact with the API endpoints.\n\n```\nimport os\n\nfrom satellitevu import Auth\n\n\nauth = Auth(os.getenv("CLIENT_ID"), os.getenv("CLIENT_SECRET"))\nprint(auth.token())\n```\n\nThus retrieved token can be used for bearer token authentication in HTTP request\nAuthorization headers.\n\nThe `Auth` class by default uses a file based cache which will store the token in\n\n- `~/.cache/SatelliteVu` on Linux\n- `~/Library/Caches/SatelliteVu` on MacOS\n- `C:\\Documents and Settings\\<username>\\Local Settings\\Application Data\\SatelliteVu\\Cache`\n  on Windows\n\nOther cache implementations must implement the `satellitevu.auth.cache.AbstractCache`\nclass.\n\n### HTTP Client Wrappers\n\nConvenience wrapper classes for common HTTP client implementations are provided as\nimplementations of `satellitevu.http.AbstractClient`, which provides an `request` method\nwith an interface similar to `requests.request` and returning an\n`satellitevu.http.ResponseWrapper` instance, where the response object of the underlying\nimplementation is available in the `raw` property.\n\nCommonly used properties and methods are exposed on both `AbstractClient` and\n`ResponseWrapper`.\n\n- `satellitevu.http.UrllibClient` for Python standard lib\'s `urllib`\n- `satellitevu.http.requests.RequestsSession` using `requests.Session` class\n- `satellitevu.http.httpx.HttpxClient` using `httpx.Client` (Todo)\n\nImplementations based on `requests` and `httpx` allow setting an instance of the\nunderlying implementation, but will provide a default instance if not.\n\n[pyenv]: https://github.com/pyenv/pyenv\n[poetry]: https://python-poetry.org\n[pipx]: https://pypa.github.io/pipx/\n[nox]: https://nox.thea.codes/en/stable/\n[nox-poetry]: https://nox-poetry.readthedocs.io/en/stable/\n[search-api-docs]: https://api.satellitevu.com/archive/v1/docs#operation/Search_search_post\n[pypi]: https://pypi.org/project/satellitevu/\n[examples]: https://github.com/SatelliteVu/satellitevu-client-python/tree/main/examples\n',
-    'author': 'Christian Wygoda',
-    'author_email': 'christian.wygoda@satellitevu.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Installation
 
+The package is published to [PyPi][pypi] and can be installed with pip:
+
+```
+pip install satellitevu
+```
+
+Currently Python 3.8 and Python 3.10 are supported.
+
+## Usage
+
+A User API Client credential set consisting of an _client id_ and _client secret_ is
+needed and should be set in your script's environment variables.
+
+Check out the [examples][examples] provided. They can for example be run locally with
+
+```
+poetry run python ./examples/archive.py --example=recent
+```
+
+### Simple Client Usage
+
+The easiest way to get started is to use the `satellitevu.Client` class, which needs
+a client_id and client_secret only:
+
+```
+import os
+
+from satellitevu import Client
+
+
+client = Client(os.getenv("CLIENT_ID"), os.getenv("CLIENT_SECRET"))
+print(client.archive_v1.search().json())
+```
+
+`client.archive_v1.search` supports all supported request body parameters documented
+in the [API docs][search-api-docs], with special handling for `datetime` which is
+constructed from the optional `date_from` and `date_to` parameters and a default result
+page size limit of 25.
+
+### Authentication Handling
+
+The `satellitevu.Auth` class provides the main interface to retrieve an
+authorization token required to interact with the API endpoints.
+
+```
+import os
+
+from satellitevu import Auth
+
+
+auth = Auth(os.getenv("CLIENT_ID"), os.getenv("CLIENT_SECRET"))
+print(auth.token())
+```
+
+Thus retrieved token can be used for bearer token authentication in HTTP request
+Authorization headers.
+
+The `Auth` class by default uses a file based cache which will store the token in
+
+- `~/.cache/SatelliteVu` on Linux
+- `~/Library/Caches/SatelliteVu` on MacOS
+- `C:\Documents and Settings\<username>\Local Settings\Application Data\SatelliteVu\Cache`
+  on Windows
+
+Other cache implementations must implement the `satellitevu.auth.cache.AbstractCache`
+class.
+
+### HTTP Client Wrappers
+
+Convenience wrapper classes for common HTTP client implementations are provided as
+implementations of `satellitevu.http.AbstractClient`, which provides an `request` method
+with an interface similar to `requests.request` and returning an
+`satellitevu.http.ResponseWrapper` instance, where the response object of the underlying
+implementation is available in the `raw` property.
+
+Commonly used properties and methods are exposed on both `AbstractClient` and
+`ResponseWrapper`.
+
+- `satellitevu.http.UrllibClient` for Python standard lib's `urllib`
+- `satellitevu.http.requests.RequestsSession` using `requests.Session` class
+- `satellitevu.http.httpx.HttpxClient` using `httpx.Client` (Todo)
+
+Implementations based on `requests` and `httpx` allow setting an instance of the
+underlying implementation, but will provide a default instance if not.
+
+[pyenv]: https://github.com/pyenv/pyenv
+[poetry]: https://python-poetry.org
+[pipx]: https://pypa.github.io/pipx/
+[nox]: https://nox.thea.codes/en/stable/
+[nox-poetry]: https://nox-poetry.readthedocs.io/en/stable/
+[search-api-docs]: https://api.satellitevu.com/archive/v1/docs#operation/Search_search_post
+[pypi]: https://pypi.org/project/satellitevu/
+[examples]: https://github.com/SatelliteVu/satellitevu-client-python/tree/main/examples
 
-setup(**setup_kwargs)
```

