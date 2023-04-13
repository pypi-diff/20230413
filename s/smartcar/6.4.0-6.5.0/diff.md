# Comparing `tmp/smartcar-6.4.0.tar.gz` & `tmp/smartcar-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartcar-6.4.0.tar", last modified: Wed Mar 22 22:39:51 2023, max compression
+gzip compressed data, was "dist/smartcar-6.5.0.tar", last modified: Thu Apr 13 20:19:03 2023, max compression
```

## Comparing `smartcar-6.4.0.tar` & `smartcar-6.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-22 22:39:51.177414 smartcar-6.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-03-22 22:38:44.000000 smartcar-6.4.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-03-22 22:39:51.177414 smartcar-6.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2023-03-22 22:38:44.000000 smartcar-6.4.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-03-22 22:39:51.177414 smartcar-6.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-03-22 22:38:44.000000 smartcar-6.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-22 22:39:51.173413 smartcar-6.4.0/smartcar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-03-22 22:39:10.000000 smartcar-6.4.0/smartcar/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/auth_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3587 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9064 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/smartcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10800 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18452 2023-03-22 22:38:44.000000 smartcar-6.4.0/smartcar/vehicle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-22 22:39:51.173413 smartcar-6.4.0/smartcar.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-03-22 22:39:51.000000 smartcar-6.4.0/smartcar.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-03-22 22:39:51.000000 smartcar-6.4.0/smartcar.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-22 22:39:51.000000 smartcar-6.4.0/smartcar.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-03-22 22:39:51.000000 smartcar-6.4.0/smartcar.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-03-22 22:39:51.000000 smartcar-6.4.0/smartcar.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2023-04-13 20:18:12.000000 smartcar-6.5.0/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-04-13 20:19:03.239466 smartcar-6.5.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6355 2023-04-13 20:18:12.000000 smartcar-6.5.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-04-13 20:19:03.243466 smartcar-6.5.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1215 2023-04-13 20:18:12.000000 smartcar-6.5.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/smartcar/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-04-13 20:18:38.000000 smartcar-6.5.0/smartcar/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9282 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/auth_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4118 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3587 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9064 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/smartcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11006 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19528 2023-04-13 20:18:12.000000 smartcar-6.5.0/smartcar/vehicle.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-13 20:19:03.239466 smartcar-6.5.0/smartcar.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6635 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      363 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-04-13 20:19:03.000000 smartcar-6.5.0/smartcar.egg-info/top_level.txt
```

### Comparing `smartcar-6.4.0/LICENSE.md` & `smartcar-6.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/PKG-INFO` & `smartcar-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.4.0
+Version: 6.5.0
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `smartcar-6.4.0/README.md` & `smartcar-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/setup.py` & `smartcar-6.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/smartcar/auth_client.py` & `smartcar-6.5.0/smartcar/auth_client.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/smartcar/exception.py` & `smartcar-6.5.0/smartcar/exception.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/smartcar/helpers.py` & `smartcar-6.5.0/smartcar/helpers.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/smartcar/smartcar.py` & `smartcar-6.5.0/smartcar/smartcar.py`

 * *Files identical despite different names*

### Comparing `smartcar-6.4.0/smartcar/types.py` & `smartcar-6.5.0/smartcar/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,14 +178,16 @@
 Vin = NamedTuple("Vin", [("vin", str), ("meta", namedtuple)])
 
 Charge = NamedTuple(
     "Charge",
     [("is_plugged_in", bool), ("state", str), ("meta", namedtuple)],
 )
 
+ChargeLimit = NamedTuple("ChargeLimit", [("limit", float), ("meta", namedtuple)])
+
 Battery = NamedTuple(
     "Battery",
     [("percent_remaining", float), ("range", float), ("meta", namedtuple)],
 )
 
 BatteryCapacity = NamedTuple(
     "BatteryCapacity", [("capacity", float), ("meta", namedtuple)]
@@ -346,14 +348,17 @@
 
     elif path == "odometer":
         return Odometer(data["distance"], headers)
 
     elif path == "location":
         return Location(data["latitude"], data["longitude"], headers)
 
+    elif path == "charge/limit":
+        return ChargeLimit(data["limit"], headers)
+
     elif path == "permissions":
         return Permissions(
             data["permissions"],
             Paging(data["paging"]["count"], data["paging"]["offset"]),
             headers,
         )
 
@@ -361,14 +366,15 @@
         return Subscribe(data["webhookId"], data["vehicleId"], headers)
 
     elif (
         path == "lock"
         or path == "unlock"
         or path == "start_charge"
         or path == "stop_charge"
+        or path == "set_charge_limit"
     ):
         return Action(data["status"], data["message"], headers)
 
     elif path == "disconnect" or path == "unsubscribe":
         return Status(data["status"], headers)
 
     elif path == "":
```

### Comparing `smartcar-6.4.0/smartcar/vehicle.py` & `smartcar-6.5.0/smartcar/vehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,30 @@
         """
         path = ""
         url = self._format_url(path)
         headers = self._get_headers()
         response = helpers.requester("GET", url, headers=headers)
         return types.select_named_tuple(path, response)
 
+    def get_charge_limit(self) -> types.ChargeLimit:
+        """
+        GET Vehicle.get_charge_limit
+
+        Returns:
+            ChargeLimit = NamedTuple("ChargeLimit", [("limit", float), ("meta", namedtuple)])
+
+        Raises:
+            SmartcarException
+        """
+        path = "charge/limit"
+        url = self._format_url(path)
+        headers = self._get_headers()
+        response = helpers.requester("GET", url, headers=headers)
+        return types.select_named_tuple(path, response)
+
     # ===========================================
     # Action (POST) Requests
     # ===========================================
 
     def lock(self) -> types.Status:
         """
         POST Vehicle.lock
@@ -316,14 +332,31 @@
         url = self._format_url("charge")
         headers = self._get_headers(need_unit_system=False)
         response = helpers.requester(
             "POST", url, headers=headers, json={"action": "STOP"}
         )
         return types.select_named_tuple("stop_charge", response)
 
+    def set_charge_limit(self, limit) -> types.Status:
+        """
+        POST Vehicle.set_charge_limit
+
+        Returns:
+            Action: NamedTuple("Action", [("status", str), ("message", str), ("meta", rs.namedtuple)])
+
+        Raises:
+            SmartcarException
+        """
+        url = self._format_url("charge/limit")
+        headers = self._get_headers(need_unit_system=False)
+        response = helpers.requester(
+            "POST", url, headers=headers, json={"limit": limit}
+        )
+        return types.select_named_tuple("set_charge_limit", response)
+
     def batch(self, paths: List[str]) -> namedtuple:
         """
         POST Vehicle.batch
 
         This method follows a series of steps:
         1. Format and send request to Smartcar API batch endpoint
         2. Store each response in a batch dictionary.
```

### Comparing `smartcar-6.4.0/smartcar.egg-info/PKG-INFO` & `smartcar-6.5.0/smartcar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcar
-Version: 6.4.0
+Version: 6.5.0
 Summary: Smartcar Python SDK
 Home-page: https://github.com/smartcar/python-sdk
 Author: Smartcar
 Author-email: hello@smartcar.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

