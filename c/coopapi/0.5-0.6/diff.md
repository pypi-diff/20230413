# Comparing `tmp/coopapi-0.5.tar.gz` & `tmp/coopapi-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopapi-0.5.tar", last modified: Thu Apr 13 17:37:33 2023, max compression
+gzip compressed data, was "coopapi-0.6.tar", last modified: Thu Apr 13 18:19:53 2023, max compression
```

## Comparing `coopapi-0.5.tar` & `coopapi-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.080935 coopapi-0.5/
--rw-rw-rw-   0        0        0     2838 2023-04-13 17:37:33.079902 coopapi-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.051928 coopapi-0.5/coopapi/
--rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.5/coopapi/__init__.py
--rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.5/coopapi/apiShell.py
--rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.5/coopapi/enums.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.5/coopapi/errors.py
--rw-rw-rw-   0        0        0     4536 2023-02-28 17:55:46.000000 coopapi-0.5/coopapi/http_request.py
--rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.5/coopapi/http_request_handlers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:33.077926 coopapi-0.5/coopapi.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-04-13 17:37:33.000000 coopapi-0.5/coopapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.5/coopapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      279 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 17:37:32.000000 coopapi-0.5/coopapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:37:33.080935 coopapi-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-04-13 17:37:25.000000 coopapi-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.108485 coopapi-0.6/
+-rw-rw-rw-   0        0        0     2838 2023-04-13 18:19:53.107494 coopapi-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.096465 coopapi-0.6/coopapi/
+-rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.6/coopapi/__init__.py
+-rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.6/coopapi/apiShell.py
+-rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.6/coopapi/enums.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.6/coopapi/errors.py
+-rw-rw-rw-   0        0        0     4883 2023-04-13 18:18:49.000000 coopapi-0.6/coopapi/http_request.py
+-rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.6/coopapi/http_request_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.106494 coopapi-0.6/coopapi.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.6/coopapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      279 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:19:53.108485 coopapi-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-04-13 18:19:29.000000 coopapi-0.6/setup.py
```

### Comparing `coopapi-0.5/PKG-INFO` & `coopapi-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.5
+Version: 0.6
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.5/README.md` & `coopapi-0.6/README.md`

 * *Files identical despite different names*

### Comparing `coopapi-0.5/coopapi/apiShell.py` & `coopapi-0.6/coopapi/apiShell.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.5/coopapi/http_request.py` & `coopapi-0.6/coopapi/http_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 import logging
 import uuid
 
 import requests
-from typing import Dict
+from typing import Dict, Any
 from fastapi import Request, HTTPException, status, Response
 from coopapi.enums import RequestType
-
+import json
+import pprint
 logger = logging.getLogger('coop.http')
 
 
 def _response_handler(response: Response):
     pass
 
-def _log_send(id:str, lvl: int, method: RequestType, url, label: str = None):
+def _log_send(id:str, lvl: int, method: RequestType, url, label: str = None, **kwargs):
     _lbl_txt = f"[{label}]: " if label else ""
-    logger.log(lvl, f"{_lbl_txt}{method.name} @URL: {url} [{id}]")
+    _txt = f"{_lbl_txt}{method.name} @URL: {url} [{id}]"
+    if kwargs.get('data', None) is not None:
+        _txt += f"\ndata: {pprint.pformat(kwargs['data'])}"
+    if kwargs.get('json', None) is not None:
+        _txt += f"\njson: {pprint.pformat(kwargs['json'])}"
+
+    logger.log(lvl, _txt)
 
 def _log_receive(id:str, lvl:int , method: RequestType, response: Response, url, label: str = None):
     _lbl_txt = f"[{label}]: " if label else ""
-    resp_dict = {'content': response.content}
-    logger.log(lvl, f"{_lbl_txt}{method.name} @URL: {url} returned {response.status_code} [{id}] in {int(response.elapsed.microseconds / 1000)} ms\n"
-                     f"{resp_dict}")
+    logger.log(lvl, f"{_lbl_txt}{method.name} @URL: {url} returned [{response.status_code}] [{id}] in {int(response.elapsed.microseconds / 1000)} ms\n"
+                     f"{pprint.pformat(json.loads(response.content.decode(response.encoding)))}")
 
 def request(url: str,
             method: RequestType,
-            bearer_token:str,
+            bearer_token:str=None,
             loggingLvl=logging.INFO,
             label: str = None,
             request_id: str = None,
             **kwargs) -> Response:
     headers = {}
     if bearer_token is not None:
         headers['Authorization'] = f"Bearer {bearer_token}"
 
     if request_id is None:
         request_id = str(uuid.uuid4())
-    _log_send(id=request_id, lvl=loggingLvl, method=method, url=url, label=label)
+    _log_send(id=request_id, lvl=loggingLvl, method=method, url=url, label=label, **kwargs)
     response: Response = requests.request(method=method.value, url=url, verify=True, headers=headers, **kwargs)
     _log_receive(id=request_id, lvl=loggingLvl, method=method, url=url, label=label, response=response)
     return response
 
 
 def get(url: str,
         bearer_token:str = None,
@@ -50,26 +56,27 @@
                    method=RequestType.GET,
                    bearer_token=bearer_token,
                    loggingLvl=loggingLvl,
                    label=label,
                    **kwargs)
 
 def post(url: str,
-         data: Dict,
-         json: str,
+         data: Dict = None,
+         json_serializable: Any = None,
          label: str = None,
          loggingLvl=logging.INFO,
          bearer_token: str = None) -> Response:
+
     return request(url=url,
                    method=RequestType.POST,
                    bearer_token=bearer_token,
                    loggingLvl=loggingLvl,
                    label=label,
                    data=data,
-                   json=json)
+                   json=json_serializable)
 
 def put(url: str,
          data: Dict = None,
          label: str = None,
          loggingLvl=logging.INFO,
          bearer_token: str = None) -> Response:
     return request(url=url,
```

### Comparing `coopapi-0.5/coopapi/http_request_handlers.py` & `coopapi-0.6/coopapi/http_request_handlers.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.5/coopapi.egg-info/PKG-INFO` & `coopapi-0.6/coopapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.5
+Version: 0.6
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.5/setup.py` & `coopapi-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopapi',
-      version='0.05',
+      version='0.06',
       description='Tools for setting up an API. Built on the FastAPI framework',
       url='https://github.com/tylertjburns/coopapi',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

