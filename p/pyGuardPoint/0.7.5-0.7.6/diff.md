# Comparing `tmp/pyGuardPoint-0.7.5.tar.gz` & `tmp/pyGuardPoint-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.7.5.tar", last modified: Thu Apr 13 11:44:59 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.7.6.tar", last modified: Thu Apr 13 12:30:38 2023, max compression
```

## Comparing `pyGuardPoint-0.7.5.tar` & `pyGuardPoint-0.7.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:44:59.250779 pyGuardPoint-0.7.5/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.5/LICENSE.txt
--rw-rw-rw-   0        0        0      199 2023-04-13 11:44:59.249784 pyGuardPoint-0.7.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 11:44:59.239779 pyGuardPoint-0.7.5/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.5/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11334 2023-04-13 11:43:20.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.5/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.5/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     2942 2023-04-13 11:41:21.000000 pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:44:59.248783 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-13 11:44:59.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2023-04-13 11:44:59.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:44:59.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-13 11:44:59.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 11:44:59.000000 pyGuardPoint-0.7.5/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:44:59.250779 pyGuardPoint-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-13 11:44:46.000000 pyGuardPoint-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.045609 pyGuardPoint-0.7.6/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      199 2023-04-13 12:30:38.044608 pyGuardPoint-0.7.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.036375 pyGuardPoint-0.7.6/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.6/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11334 2023-04-13 11:43:20.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.6/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.6/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:30:38.044608 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 12:30:37.000000 pyGuardPoint-0.7.6/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 12:30:38.045609 pyGuardPoint-0.7.6/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.6/setup.py
```

### Comparing `pyGuardPoint-0.7.5/LICENSE.txt` & `pyGuardPoint-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.7.6/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.7.6/pyGuardPoint/guardpoint_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,18 +46,21 @@
     def check_odata_body_structure(response_body):
         if not isinstance(response_body, dict):
             raise GuardPointError("Non-JSON Response Body")
         if '@odata.context' not in response_body:
             raise GuardPointError("Non-ODATA Response Body")
         if not str(response_body['@odata.context']).endswith("$entity"):
             # Non entities seem to always appear to contain 'value'
-            if 'value' or 'errorMessages' not in response_body:
-                raise GuardPointError("Response Body does not contain 'value' or 'errorMessages'")
-            if not isinstance(response_body['value'], list):
-                raise GuardPointError("Malformed Value in Response Body")
+            check = False
+            for item in response_body:
+                if item in ['value', 'errorMessages', 'message', 'error']:
+                    check = True
+            if not check:
+                raise GuardPointError("Response Body does not contain either('value', 'errorMessages', 'message', "
+                                      "'error')")
 
         return response_body
 
 
 class Stopwatch:
 
     def __init__(self):
```

### Comparing `pyGuardPoint-0.7.5/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.7.6/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

