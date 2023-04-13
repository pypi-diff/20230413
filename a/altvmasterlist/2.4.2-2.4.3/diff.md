# Comparing `tmp/altvmasterlist-2.4.2.tar.gz` & `tmp/altvmasterlist-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-2.4.2.tar", max compression
+gzip compressed data, was "altvmasterlist-2.4.3.tar", max compression
```

## Comparing `altvmasterlist-2.4.2.tar` & `altvmasterlist-2.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-01 09:27:36.080216 altvmasterlist-2.4.2/LICENSE
--rw-r--r--   0        0        0      425 2023-04-01 09:27:36.080216 altvmasterlist-2.4.2/README.md
--rw-r--r--   0        0        0     1033 2023-04-01 09:27:36.080216 altvmasterlist-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      402 2023-04-01 09:27:36.084216 altvmasterlist-2.4.2/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     6982 2023-04-01 09:27:36.084216 altvmasterlist-2.4.2/src/altvmasterlist/altstats.py
--rw-r--r--   0        0        0     8327 2023-04-01 09:27:36.084216 altvmasterlist-2.4.2/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0    10138 2023-04-01 09:27:36.084216 altvmasterlist-2.4.2/src/altvmasterlist/shared.py
--rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 altvmasterlist-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/LICENSE
+-rw-r--r--   0        0        0      425 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/README.md
+-rw-r--r--   0        0        0     1052 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     6982 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/altstats.py
+-rw-r--r--   0        0        0     8327 2023-04-13 13:23:07.300956 altvmasterlist-2.4.3/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0    10238 2023-04-13 13:23:07.304956 altvmasterlist-2.4.3/src/altvmasterlist/shared.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.3/PKG-INFO
```

### Comparing `altvmasterlist-2.4.2/LICENSE` & `altvmasterlist-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.2/pyproject.toml` & `altvmasterlist-2.4.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "2.4.2"
+version = "2.4.3"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
@@ -14,17 +14,18 @@
     "Operating System :: OS Independent"
 ]
 packages = [
     { include = "altvmasterlist", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-requests = "^2.28.2"
-Brotli = "^1.0.9"
+python = "^3.11"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.3.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `altvmasterlist-2.4.2/src/altvmasterlist/altstats.py` & `altvmasterlist-2.4.3/src/altvmasterlist/altstats.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.2/src/altvmasterlist/masterlist.py` & `altvmasterlist-2.4.3/src/altvmasterlist/masterlist.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.2/src/altvmasterlist/shared.py` & `altvmasterlist-2.4.3/src/altvmasterlist/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
+from urllib.request import urlopen, Request
 from dataclasses import dataclass
 from json import dumps, loads
 from io import StringIO
-import requests
 import logging
 import secrets
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger().setLevel(logging.INFO)
 
 
@@ -87,21 +87,21 @@
     else:
         req_headers = {
             'User-Agent': 'AltPublicAgent',
             'content-type': 'application/json; charset=utf-8'
         }
 
     try:
-        api_data = requests.get(url, headers=req_headers, timeout=60)
-
-        if api_data.status_code != 200:
-            logging.warning(f"the request returned nothing.")
-            return None
-        else:
-            return loads(api_data.content.decode("utf-8", errors='ignore'))
+        api_request = Request(url, headers=req_headers, method="GET")
+        with urlopen(api_request, timeout=60) as api_data:
+            if api_data.status != 200:
+                logging.warning(f"the request returned nothing.")
+                return None
+            else:
+                return loads(api_data.read().decode("utf-8", errors='ignore'))
     except Exception as e:
         logging.error(e)
         return None
 
 
 def get_dtc_url(use_cdn: bool, cdn_url: str, host: str, port: int, locked: bool, password: str = None) -> str | None:
     """This function gets the direct connect protocol url of an alt:V Server.
```

