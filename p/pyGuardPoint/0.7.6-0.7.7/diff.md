# Comparing `tmp/pyGuardPoint-0.7.6.tar.gz` & `tmp/pyGuardPoint-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.7.6.tar", last modified: Thu Apr 13 12:30:38 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.7.7.tar", last modified: Thu Apr 13 12:36:22 2023, max compression
```

## Comparing `pyGuardPoint-0.7.6.tar` & `pyGuardPoint-0.7.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.045609 pyGuardPoint-0.7.6/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.6/LICENSE.txt
--rw-rw-rw-   0        0        0      199 2023-04-13 12:30:38.044608 pyGuardPoint-0.7.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.036375 pyGuardPoint-0.7.6/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.6/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11334 2023-04-13 11:43:20.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.6/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.6/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.044608 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 12:30:38.045609 pyGuardPoint-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:36:22.181611 pyGuardPoint-0.7.7/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      199 2023-04-13 12:36:22.180608 pyGuardPoint-0.7.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 12:36:22.172629 pyGuardPoint-0.7.7/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.7/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.7/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.7/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:36:22.179610 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-04-13 12:36:22.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2023-04-13 12:36:22.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:36:22.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-13 12:36:22.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 12:36:22.000000 pyGuardPoint-0.7.7/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 12:36:22.181611 pyGuardPoint-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-04-13 12:36:08.000000 pyGuardPoint-0.7.7/setup.py
```

### Comparing `pyGuardPoint-0.7.6/LICENSE.txt` & `pyGuardPoint-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,24 +19,22 @@
 
         code, json_body = self.gp_json_query("DELETE", url=(url + url_query_params))
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 204:  # HTTP NO_CONTENT
-            try:
-                if "errorMessages" in json_body:
-                    raise GuardPointError(json_body["errorMessages"][0]["other"])
-                if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-                else:
-                    raise GuardPointError(str(code))
-            except Exception:
+            if "errorMessages" in json_body:
+                raise GuardPointError(json_body["errorMessages"][0]["other"])
+            if 'error' in json_body:
+                raise GuardPointError(json_body['error'])
+            else:
                 raise GuardPointError(str(code))
 
+
         return True
 
     def update_card_holder_area(self, cardholder_uid: str, area: Area):
         if not validators.uuid(cardholder_uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
 
         if not validators.uuid(area.uid):
```

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.7.7/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.7.7/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.7.7/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.6/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.7.7/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

