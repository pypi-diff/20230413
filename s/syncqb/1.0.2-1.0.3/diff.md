# Comparing `tmp/syncqb-1.0.2.tar.gz` & `tmp/syncqb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.2.tar", last modified: Fri Apr  7 17:11:54 2023, max compression
+gzip compressed data, was "syncqb-1.0.3.tar", last modified: Thu Apr 13 17:32:09 2023, max compression
```

## Comparing `syncqb-1.0.2.tar` & `syncqb-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-07 17:11:54.517650 syncqb-1.0.2/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.2/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-07 17:11:54.517650 syncqb-1.0.2/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.2/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      643 2023-04-07 15:48:21.000000 syncqb-1.0.2/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-07 17:11:54.517650 syncqb-1.0.2/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.2/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-07 17:11:54.487650 syncqb-1.0.2/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-07 17:11:54.507650 syncqb-1.0.2/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.2/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.2/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    17643 2023-04-06 20:19:05.000000 syncqb-1.0.2/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10547 2023-04-07 14:19:04.000000 syncqb-1.0.2/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2123 2023-04-07 17:06:19.000000 syncqb-1.0.2/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1392 2023-04-07 14:15:23.000000 syncqb-1.0.2/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.2/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.2/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)      618 2023-04-06 18:45:19.000000 syncqb-1.0.2/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.2/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    26718 2023-04-06 20:21:34.000000 syncqb-1.0.2/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.2/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-07 17:11:54.517650 syncqb-1.0.2/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-07 17:11:54.000000 syncqb-1.0.2/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      538 2023-04-07 17:11:54.000000 syncqb-1.0.2/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-07 17:11:54.000000 syncqb-1.0.2/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-07 17:11:54.000000 syncqb-1.0.2/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-07 17:11:54.000000 syncqb-1.0.2/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-07 17:11:54.517650 syncqb-1.0.2/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1424 2023-04-07 16:32:23.000000 syncqb-1.0.2/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.397101 syncqb-1.0.3/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.3/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-13 17:32:09.387101 syncqb-1.0.3/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.3/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-13 17:29:22.000000 syncqb-1.0.3/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-13 17:32:09.397101 syncqb-1.0.3/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.3/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.377101 syncqb-1.0.3/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.377101 syncqb-1.0.3/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.3/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.3/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    15814 2023-04-13 17:16:51.000000 syncqb-1.0.3/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11313 2023-04-13 17:00:56.000000 syncqb-1.0.3/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.3/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.3/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.3/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.3/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2639 2023-04-13 17:16:03.000000 syncqb-1.0.3/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.3/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.3/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.3/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.387101 syncqb-1.0.3/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.387101 syncqb-1.0.3/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1296 2023-04-13 17:21:46.000000 syncqb-1.0.3/tests/test.py
```

### Comparing `syncqb-1.0.2/LICENSE` & `syncqb-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/PKG-INFO` & `syncqb-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.2/README.md` & `syncqb-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/src/syncqb/json_quickbase.py` & `syncqb-1.0.3/src/syncqb/json_quickbase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,52 @@
-
-
 from .quickbase import QuickbaseClient
 from .qb_errors import *
 import requests
-import time
 import json
 import xml.etree.ElementTree as ET
 
 class JsonQuickbaseClient(QuickbaseClient):
-    def __init__(self, credentials=None, timeout=None, **kwargs):
+    def __init__(self, credentials=None, timeout=None, default=None, **kwargs):
         if not credentials:
             credentials = kwargs
         super().__init__(credentials, timeout)
         self.headers = {
             'QB-Realm-Hostname': self.realmhost,
             'Content-Type': 'application/json',
         }
         if self.user_token is not None:
             self.headers.update(
                 {'Authorization': f'QB-USER-TOKEN {self.user_token}'})
         else:
             raise QBAuthError("In order to use this SDK, you must provide a Quickbase user token.")
-
-    # ---------------------------------------- core request functions ----------------------------------------
-    def _attempt_request(self, url, action, params=None, body=None, json=True):
-        tries = 0
-
-        while tries < 10:
-            try:
-                return self._request(url, action, params=params, body=body, json=json)
-            except requests.exceptions.Timeout or QBResponseError:
-                tries += 1
-                time.sleep(1)
-                pass
-        raise QBConnectionError('Connection Error: Timeout')
-
-    def _request(self, url, action, params=None, body=None, json=True):
-        kwargs = {
-            'headers': self.headers,
-            'timeout': self.timeout,
-        }
-        if params:
-            kwargs['params'] = params
-        if body:
-            kwargs['json'] = body
-
-        if action == 'get':
-            response: requests.models.Response = requests.get(url, **kwargs)
-        elif action == 'post':
-            response: requests.models.Response = requests.post(url, **kwargs)
-        elif action == 'delete':
-            response: requests.models.Response = requests.delete(url, **kwargs)
-        else:
-            raise ValueError('Invalid action')        
-
-        if response.status_code == 401 or response.status_code == 403:
-            raise QBAuthError('Invalid credentials')
-        elif response.status_code == 404:
-            raise QBConnectionError('Connection Error: Invalid URL')
-        elif response.status_code == 400:
-            raise QBResponseError('Response Error: Invalid request', response)
-        elif response.status_code == 429:
-            raise QBResponseError('Response Error: Too many requests', response)
-        elif response.status_code == 500:
-            raise QBResponseError('Response Error: Internal Quickbase Server Error', response)
         
-        if json:
-            return response.json()
-        else:
-            return response
-
-    def _get(self, url, params=None):
-        return self._request(url, 'get', params=params)
+        self.default = default
 
-    def _post(self, url, params=None, body=None):
-        return self._request(url, 'post', params=params, body=body)
-
-    def _delete(self, url, params=None):
-        return self._request(url, 'delete', params=params)
     # ---------------------------------------- formatting functions ----------------------------------------
     def nest(self, data_list):
         for index, data in enumerate(data_list):
             data_list[index] = {key: {'value': value} for key, value in data.items()}
 
         return data_list
 
     def denest(self, data_list):
         for index, data in enumerate(data_list):
             data_list[index] = {key: value['value'] for key, value in data.items()}
 
         return data_list
-
-    def none_to_0(self, data_list):
+    
+    def replace_empty_values(self, data_list, default_value):
         for index, data in enumerate(data_list):
-            data_list[index] = {key: 0 if value is None else value for key, value in data.items()}
+            data_list[index] = {key: default_value if value is None else value for key, value in data.items()}
 
         return data_list
 
+    def none_to_0(self, data_list):
+        return self.replace_empty_values(data_list, 0)
+
     def round_ints(self, data_list):
         for index, data in enumerate(data_list):
             for key, value in data.items():
                 if isinstance(value, float) and value.is_integer():
                     data_list[index][key] = int(value)
 
         return data_list
@@ -118,43 +64,45 @@
 
     def get_schema(self, database=None, include_permissions=False):
         params = {
             'tableId': database or self.database,
             'includeFieldPerms': 'true' if include_permissions else 'false'
         }
 
-        response = self._attempt_request(
+        response = self._request(
             'https://api.quickbase.com/v1/fields',
             'get',
-            params=params
+            self.headers,
+            params=params,
+            json=True
         )
         return response
 
     def get_primary_key(self, database=None):
         schema = self.get_schema(database)
         for record in schema:
             if record['properties']['primaryKey']:
                 return str(record['id'])
 
     def _get_report_query(self, qid, database=None):
         params = {
             'tableId': database or self.database,
         }
         url = f"https://api.quickbase.com/v1/reports/{qid}"
-        response = self._attempt_request(url, 'get', params=params)
+        response = self._request(url, 'get', self.headers, params=params, json=True)
 
         return {
             'where': response['query']['filter'],
             'sortBy': response['query']['sortBy'],
             'groupBy': response['query']['groupBy'],
         }
     # ---------------------------------------- query functions ----------------------------------------
     def do_query(self, query=None, qid=None, columns=None, sort=None,
                  num=None, skip=None, ascending=True,
-                 database=None, round_ints=True, require_all=False):
+                 database=None, round_ints=True, require_all=False, default=None):
         
         
         if sort == None:
             sort = [3]
         
         if query:
 
@@ -190,41 +138,44 @@
             if query_info.get('groupBy'):
                 body['groupBy'] = query_info['groupBy']
 
             response = self._get_data(body, skip, num, require_all)
         else:
             raise ValueError('Must provide either a query or a qid')
 
-        data = self.none_to_0(response['data'])
+        if default == None:
+            default = self.default
+        
 
-        data = self.denest(data)
+        data = self.denest(response.get('data'))
+        data = self.replace_empty_values(data, default)
 
         if round_ints:
             data = self.round_ints(data)
 
         return data
 
     def _run_report(self, qid, database=None, skip=None, top=None):
         params = {
             'tableId': database or self.database,
             'skip': skip,
             'top': top,
         }
         url = f"https://api.quickbase.com/v1/reports/{qid}/run"
-        response = self._attempt_request(url, 'post', params=params)
+        response = self._request(url, 'post', self.headers, params=params, json=True)
 
         return response
 
     def _run_query(self, body, skip=None, top=None):
         url = 'https://api.quickbase.com/v1/records/query'
         body.update({'options': {
             'skip': int(skip or 0),
             'top': int(top or 0)
         }})
-        response = self._attempt_request(url, 'post', body=body)
+        response = self._request(url, 'post', self.headers, data=body, json=True)
 
         return response
 
     def _get_data(self, body, skip=None, top=None, require_all=False, report=False):
         if require_all:
             return self._get_all_data(body, skip, top, report)
         else:
@@ -345,15 +296,15 @@
 
     def delete_record(self, rid, database=None):
         body = {
             'from': database or self.database,
             'where': "{3.EX.'%s'}" % rid
         }
         url = 'https://api.quickbase.com/v1/records'
-        response = self._attempt_request(url, 'delete', body=body)
+        response = self._request(url, 'delete', self.headers, data=body, json=True)
 
         return response
     # ---------------------------------------- multiple record functions ----------------------------------------
     def add_multiple_records(self, data, database=None, return_fields=None, round_ints=False, safemode=False):
 
         if safemode:
             pk = self.get_primary_key(database)
@@ -393,15 +344,15 @@
 
         url = 'https://api.quickbase.com/v1/records'
         body = {
             'to': database or self.database,
             'data': records,
             'fieldsToReturn': return_fields
         }
-        response = self._attempt_request(url, 'post', body=body)
+        response = self._request(url, 'post', self.headers, data=body, json=True)
 
         return response
 
     def purge_records(self, database=None, rids=None, query=None):
         if not rids and not query:
             raise ValueError('Must provide either a list of rids or a query')
         
@@ -410,15 +361,15 @@
             query = 'OR'.join(["{3.EX.'%s'}" % rid for rid in rids])
         
         body = {
             'from': database or self.database,
             'where': query
         }
         url = 'https://api.quickbase.com/v1/records'
-        response = self._attempt_request(url, 'delete', body=body)
+        response = self._request(url, 'delete', self.headers, data=body, json=True)
 
         return response
     # ---------------------------------------- file functions ----------------------------------------
     def upload_file(self, rid, upload, database=None):
         record = {
             '3': rid,
             upload['field']: {
@@ -432,15 +383,15 @@
 
     def get_file(self, url=None, database=None, record=None, field=None, version=0):
         if record and field:
             url = f"https://api.quickbase.com/v1/files/{database or self.database}/{record}/{field}/{version}"
         else:
             url = f"https://api.quickbase.com/v1{url}"
 
-        response = self._attempt_request(url, 'get', json=False)
+        response = self._request(url, 'get', self.headers, json=False)
 
         return response, response.content
     # ---------------------------------------- misc functions ----------------------------------------
     def import_from_csv(self, records_csv, clist, database=None):
         csv = records_csv.splitlines()
         data = []
```

### Comparing `syncqb-1.0.2/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.3/src/syncqb/json_quickbase.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from .qb_errors import *
 from .quickbase import QuickbaseClient
 from typing import Any
 
 class JsonQuickbaseClient(QuickbaseClient):
     headers: dict[str, str] | None = ...
 
-    def __init__(self, credentials: dict[str, str] | None = None, timeout: int | None = None, **kwargs: Any) -> None: 
+    def __init__(self, credentials: dict[str, str] | None = None, timeout: int | None = None, default: Any | None = None, **kwargs: Any) -> None: 
         """
         Client for Quickbase JSON API
         :param credentials: (dict or None) a dictionary of credentials (default: None) 
             username (optional)
             password (optional)
             realmhost (optional)
             base_url (required)
             user_token (required)
-        :param timeout: The number of seconds to wait before timing out a request
+        :param timeout: (int or None) The number of seconds to wait before timing out a request (default: None)
+        :param default: (Any or None) The default value to use for empty fields (default: None)
         :param kwargs: Additional keyword arguments (used if credentials is None)
         """
         ...
     def nest(self, data_list: list[dict[str, Any]]) ->  list[dict[str, Any]]:
         """
         Takes a list of dictionaries and nests the values in a dictionary with a 'value' key.
         This is necessary for Quickbase to accept the data.
@@ -29,21 +30,31 @@
     def denest(self, data_list: list[dict[str, Any]]) ->  list[dict[str, Any]]: 
         """
         Takes a list of dictionaries and removes the 'value' key from the values.
         :param data_list: (list of dict) your list of record data
         :return: (list of dict) your list of record data
         """
         ...
+    def replace_empty_values(self, data_list: list[dict[str, Any]], default_value: Any) ->  list[dict[str, Any]]:
+        """
+        Takes a list of dictionaries and replaces None values with a given default value.
+        :param data_list: (list of dict) your list of record data
+        :param default_value: (any) the value to replace None with
+        :return: (list of dict) your list of record data
+        """
+        ...
     def none_to_0(self, data_list: list[dict[str, Any]]) ->  list[dict[str, Any]]: 
         """
+        DEPRECATED: Use replace_empty_values instead.
         Takes a list of dictionaries and replaces None values with 0.
         :param data_list: (list of dict) your list of record data
         :return: (list of dict) your list of record data
         """
         ...
+    
     def round_ints(self, data_list: list[dict[str, Any]]) ->  list[dict[str, Any]]: 
         """
         Takes a list of dictionaries and rounds all float values that are actually integers.
         :param data_list: (list of dict) your list of record data
         :return: (list of dict) your list of record data
         """
         ...
@@ -60,27 +71,28 @@
         Get the primary key of a Quickbase table.
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :return: (str) the primary key field ID
         """
         ...
     def do_query(self, query: str | None = None, qid: int | None = None, columns: list[str | int] | None = None, sort: list[str | int] | None = None, 
                  num: int | None = None, skip: int | None = None, ascending: bool = True, database: str | None = None, round_ints: bool = True, 
-                 require_all: bool = False) -> list[dict[str, Any]]: 
+                 require_all: bool = False, default: Any | None = None) -> list[dict[str, Any]]: 
         """
         Query a Quickbase table.
         :param query: (str or None) Quickbase query string (default None)
         :param qid: (int or None) Quickbase report ID (default None)
         :param columns: (None or list of str or int) List of column IDs to return (default None)
         :param sort: (None or list of str or int) List of column IDs to sort by (default None)
         :param num: (int or None) Max number of records to return (default None)
         :param skip: (int or None) Number of records to skip (default None)
         :param ascending: (bool) Whether to sort ascending (default True)
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :param round_ints: (bool) Whether to round integers (default True)
         :param require_all: (bool) Whether to require all records be returned (default False, risk of performance issues if True - USES MULTPLE API CALLS)
+        :param default: (Any or None) The default value to use for empty fields (default None)
         :return: (list of dict) your list of record data
         """
         ...
     def add_record(self, fields: dict[str, Any], database: str | None = None, uploads: list[dict[str, str | bytes]] | None = None, 
                    safemode: bool = False, return_fields: list[str | int] | None = None) -> int | dict[str, Any]: 
         """
         Add a record to a Quickbase table.
```

### Comparing `syncqb-1.0.2/src/syncqb/qb_client.py` & `syncqb-1.0.3/src/syncqb/qb_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import getpass
 from dotenv import find_dotenv, load_dotenv
 from . import json_quickbase, xml_quickbase
 from .qb_errors import QBError
 
-def get_client(json_sdk=False, creds=None):
+def get_client(json_sdk=False, creds=None, **kwargs):
     if creds:
         url = creds.get('QB_URL')
         user_token = creds.get('QB_USERTOKEN')
         username = creds.get('QB_USERNAME')
         password = creds.get('QB_PASSWORD')
     else:
         load_dotenv(find_dotenv(usecwd=True))
@@ -20,28 +20,28 @@
         if not url and not user_token and not username and not password:
             raise QBError('No credentials found, your .env file may be missing or in the wrong directory.')
             
 
     if json_sdk:
         new_qb_client = json_quickbase.JsonQuickbaseClient(
             # realmhost=realmhost, base_url=url, user_token=user_token)
-            credentials={'base_url': url, 'user_token': user_token})
+            credentials={'base_url': url, 'user_token': user_token}, **kwargs)
         return new_qb_client
     else:
         qb_client = xml_quickbase.XmlQuickbaseClient(hours=25,
-            credentials={'username': username, 'password': password, 'base_url': url}
+            credentials={'username': username, 'password': password, 'base_url': url}, **kwargs
                 # username, password, base_url=url, hours=25
         )
         return qb_client
     
-def get_json_client(creds=None):
-    return get_client(True, creds)
+def get_json_client(creds=None, **kwargs):
+    return get_client(True, creds, **kwargs)
 
-def get_xml_client(creds=None):
-    return get_client(False, creds)
+def get_xml_client(creds=None, **kwargs):
+    return get_client(False, creds, **kwargs)
        
 
 def set_qb_info():
     
     path = os.path.join(os.getcwd())
     input_path = input('Enter path to .env file (or leave blank for your cwd): ')
     path = os.path.join(input_path if input_path else path, '.env')
```

### Comparing `syncqb-1.0.2/src/syncqb/qb_errors.py` & `syncqb-1.0.3/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/src/syncqb/qb_errors.pyi` & `syncqb-1.0.3/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/src/syncqb/quickbase.pyi` & `syncqb-1.0.3/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/src/syncqb/xml_quickbase.py` & `syncqb-1.0.3/src/syncqb/xml_quickbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,49 +24,24 @@
         super().__init__(credentials, timeout, database)
 
         if authenticate:
             self.authenticate()
         elif ticket is not None:
             self.ticket = ticket
 
-    def _request(self, url, data, action, type):
-        if action == 'files':
+    def _request(self, url, data, method, action):
+
+        if method == 'files':
             headers = {'cookie': f'ticket={self.ticket}'}
         else:
             headers = {
                 'content-type': 'application/xml',
-                'QUICKBASE-ACTION': f'API_{action}',
+                'QUICKBASE-ACTION': f'API_{method}',
             }
-        tries = 0
-        while tries < 10:
-            try:
-                return self._make_request(url, data, headers, type)
-            except requests.exceptions.Timeout or QBConnectionError:
-                print('Timeout error, retrying...')
-                tries += 1
-                time.sleep(1)
-        raise QBConnectionError('Connection Error: Timeout')
-
-    def _make_request(self, url, data, headers, type):
-        if type == 'POST':
-            response =  requests.post(url, data=data, headers=headers, timeout=self.timeout)
-        elif type == 'GET':
-            response = requests.get(url, headers=headers, timeout=self.timeout)
-
-        if response.status_code == 401 or response.status_code == 403:
-            raise QBAuthError('Invalid credentials')
-        elif response.status_code == 404:
-            raise QBConnectionError('Connection Error: Invalid URL')
-        elif response.status_code == 400:
-            raise QBResponseError('Response Error: Invalid request', response)
-        elif response.status_code == 429:
-            raise QBResponseError('Response Error: Too many requests', response)
-        elif response.status_code == 500:
-            raise QBResponseError('Response Error: Internal Quickbase Server Error', response)
-        
+        response = super()._request(url, action, headers, data=data, json=False)
         return response.content
 
     def _build_xml(self, data):
         if self.ticket:
             data['ticket'] = self.ticket
         if self.apptoken:
             data['apptoken'] = self.apptoken
```

### Comparing `syncqb-1.0.2/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.3/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.2/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.3/src/syncqb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.2/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.3/src/syncqb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 src/syncqb/quickbase.pyi
 src/syncqb/xml_quickbase.py
 src/syncqb/xml_quickbase.pyi
 src/syncqb.egg-info/PKG-INFO
 src/syncqb.egg-info/SOURCES.txt
 src/syncqb.egg-info/dependency_links.txt
 src/syncqb.egg-info/entry_points.txt
+src/syncqb.egg-info/requires.txt
 src/syncqb.egg-info/top_level.txt
 tests/test.py
```

### Comparing `syncqb-1.0.2/tests/test.py` & `syncqb-1.0.3/tests/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,27 +30,21 @@
             'field': '19',
             'filename': 'test.txt',
             'value': 'MjM='
         }
     ]
 
     client = qb_client.get_xml_client()
-    client2 = qb_client.get_json_client()
+    client2 = qb_client.get_json_client(default='NOT APPLICABLE')
 
-    xml_res = client.do_query(
-        # query='{3.EX.128}',
-        qid=10, 
-        columns=[3, 6, 9], 
-        database='bnsucj684', 
-        structured=True,
-        qid_custom_headers=True
-    )
-    # xml_res = 'N/A'
-    # json_res = client2.get_file(database='bnsucj684', field=19, record=69036)
-    json_res = 'N/A'
+    # xml_res = client.get_f
+    xml_res = 'N/A'
+    json_res = client2.do_query(
+        qid=13, database="bpxua87ct", sort=[22], ascending=False)
+    # json_res = 'N/A'
 
     print('xml_res:', xml_res)
     print('json_res:', json_res)
```

