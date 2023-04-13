# Comparing `tmp/visier-connector-0.8.6.tar.gz` & `tmp/visier-connector-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.8.6.tar", last modified: Wed Apr  5 22:17:44 2023, max compression
+gzip compressed data, was "visier-connector-0.9.0.tar", last modified: Thu Apr 13 18:14:39 2023, max compression
```

## Comparing `visier-connector-0.8.6.tar` & `visier-connector-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:17:44.633185 visier-connector-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 22:17:34.000000 visier-connector-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-05 22:17:44.633185 visier-connector-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-05 22:17:34.000000 visier-connector-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:17:44.633185 visier-connector-0.8.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-05 22:17:34.000000 visier-connector-0.8.6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-05 22:17:34.000000 visier-connector-0.8.6/examples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 22:17:44.633185 visier-connector-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-05 22:17:34.000000 visier-connector-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:17:44.633185 visier-connector-0.8.6/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-05 22:17:34.000000 visier-connector-0.8.6/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:17:44.633185 visier-connector-0.8.6/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-05 22:17:34.000000 visier-connector-0.8.6/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-05 22:17:34.000000 visier-connector-0.8.6/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-05 22:17:34.000000 visier-connector-0.8.6/visier/connector/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:17:44.633185 visier-connector-0.8.6/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-05 22:17:44.000000 visier-connector-0.8.6/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-05 22:17:44.000000 visier-connector-0.8.6/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:17:44.000000 visier-connector-0.8.6/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 22:17:44.000000 visier-connector-0.8.6/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 22:17:44.000000 visier-connector-0.8.6/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.422876 visier-connector-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 18:14:30.000000 visier-connector-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 18:14:39.418876 visier-connector-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-13 18:14:30.000000 visier-connector-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-13 18:14:30.000000 visier-connector-0.9.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 18:14:30.000000 visier-connector-0.9.0/examples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:14:39.422876 visier-connector-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 18:14:30.000000 visier-connector-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-13 18:14:30.000000 visier-connector-0.9.0/visier/connector/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:14:39.418876 visier-connector-0.9.0/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 18:14:39.000000 visier-connector-0.9.0/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.8.6/LICENSE` & `visier-connector-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/PKG-INFO` & `visier-connector-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.8.6
+Version: 0.9.0
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

### Comparing `visier-connector-0.8.6/README.md` & `visier-connector-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![linting](https://github.com/visier/visier-connector-python/actions/workflows/pylint.yml/badge.svg) ![pypi publishing](https://github.com/visier/visier-connector-python/actions/workflows/publish-to-test-pypi.yml/badge.svg)
+![linting](https://github.com/visier/connector-python/actions/workflows/pylint.yml/badge.svg) ![pypi publishing](https://github.com/visier/connector-python/actions/workflows/publish-to-test-pypi.yml/badge.svg)
 # Visier Python Connector
 Use the Visier Python Connector to query Visier People Data.
 
 The connector enables Python developers to query Visier People Data using Visier's SQL-like query language. 
 
 ## Prerequisites
 The connector acts as middleware between your (typically Pandas-enabled) Python application and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
```

### Comparing `visier-connector-0.8.6/examples/__init__.py` & `visier-connector-0.9.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/examples/util.py` & `visier-connector-0.9.0/examples/util.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/setup.py` & `visier-connector-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/visier/__init__.py` & `visier-connector-0.9.0/visier/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.8.6"
+__version__ = "0.9.0"
```

### Comparing `visier-connector-0.8.6/visier/connector/__init__.py` & `visier-connector-0.9.0/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/visier/connector/authentication.py` & `visier-connector-0.9.0/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.8.6/visier/connector/sessions.py` & `visier-connector-0.9.0/visier/connector/sessions.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 """
 Visier Session object through which JSON as well as SQL-like queries are executed.
 """
 
 import json
 import dataclasses
+from typing import Callable
 import requests
-from requests import Session
+from requests import Session, Response
 from visier.connector.authentication import Authentication
 
 
 @dataclasses.dataclass
 class QueryExecutionError(Exception):
     """Description of error from executing a query"""
     def __init__(self, status_code, message) -> None:
@@ -66,60 +67,63 @@
     """
     HEADER = {"Accept": "application/jsonlines, application/json"}
 
     def __init__(self, auth: Authentication) -> None:
         self._auth = auth
         self._session = None
 
-
     def execute_aggregate(self, query_def: object):
         """Execute a Visier aggregate query and return a tabular result."""
         url = self._auth.host + "/v1/data/query/aggregate"
-        return self._execute_with_retry(url, query_def)
-
+        return self._execute_query_api(url, query_def)
 
     def execute_list(self, query_def: object):
         """Execute a Visier list query and return a tabular result."""
         url = self._auth.host + "/v1/data/query/list"
-        return self._execute_with_retry(url, query_def)
-
+        return self._execute_query_api(url, query_def)
 
     def execute_sqllike(self, sql_query: str, options = None):
         """Execute a Visier SQL-like query statement and return a tabular result."""
         url = self._auth.host + "/v1/data/query/sql"
         body = {"query" : sql_query}
         if options:
             body["options"] = options
-        return self._execute_with_retry(url, body)
-
-
-    def __enter__(self):
-        self._connect()
-        return self
-
-
-    def __exit__(self, ex_type, ex_value, trace_back):
-        self._close()
+        return self._execute_query_api(url, body)
 
+    def execute(self, call_function: Callable[[Session], Response]) -> Response:
+        """Execute a custom function with the current session.
 
-    def _execute_with_retry(self, url: str, body: object):
-        """Generic method for executing a query and retrying if necessary."""
+        Keyword arguments:
+        call_function -- Function that takes a Session object as input and
+                         returns a Response object.
+        """
         num_attempts_left = 2
         is_ok = False
         while not is_ok and num_attempts_left > 0:
-            result = self._session.post(url=url, json=body, headers=self.HEADER)
+            result = call_function(self._session)
             num_attempts_left -= 1
             is_ok = result.ok
             if not is_ok:
                 if result.status_code == 401 and num_attempts_left > 0:
                     self._connect()
                 else:
                     raise QueryExecutionError(result.status_code, result.text)
-        return ResultTable(result.iter_lines())
+        return result
 
+    def __enter__(self):
+        self._connect()
+        return self
+
+    def __exit__(self, ex_type, ex_value, trace_back):
+        self._close()
+
+    def _execute_query_api(self, url: str, body: object):
+        """Helper method for executing a query API with flattened result."""
+        result = self.execute(lambda s: s.post(url=url, json=body, headers=self.HEADER))
+        return ResultTable(result.iter_lines())
 
     def _connect(self):
         url = self._auth.host + "/v1/admin/visierSecureToken"
         body = {'username': self._auth.username, 'password': self._auth.password}
         if self._auth.vanity:
             body["vanityName"] = self._auth.vanity
         result = requests.post(url=url, data=body, timeout=30)
@@ -127,10 +131,9 @@
 
         # Only create a requests.Session once we have a Visier ASID Token
         asid_token = result.text
         self._session = Session()
         self._session.cookies["VisierASIDToken"] = asid_token
         self._session.headers.update({"apikey": self._auth.api_key})
 
-
     def _close(self):
         self._session.close()
```

### Comparing `visier-connector-0.8.6/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.0/visier_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.8.6
+Version: 0.9.0
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

