# Comparing `tmp/pyGuardPoint-0.7.3.tar.gz` & `tmp/pyGuardPoint-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.7.3.tar", last modified: Thu Apr  6 12:01:29 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.7.4.tar", last modified: Thu Apr 13 10:36:26 2023, max compression
```

## Comparing `pyGuardPoint-0.7.3.tar` & `pyGuardPoint-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 12:01:29.094828 pyGuardPoint-0.7.3/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.3/LICENSE.txt
--rw-rw-rw-   0        0        0      199 2023-04-06 12:01:29.094828 pyGuardPoint-0.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 12:01:29.081241 pyGuardPoint-0.7.3/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.3/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11201 2023-04-06 12:00:47.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     4902 2023-04-05 10:42:09.000000 pyGuardPoint-0.7.3/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.3/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     2885 2023-04-03 15:08:05.000000 pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:01:29.093828 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-06 12:01:29.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2023-04-06 12:01:29.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 12:01:29.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-06 12:01:29.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-06 12:01:29.000000 pyGuardPoint-0.7.3/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 12:01:29.094828 pyGuardPoint-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-06 12:01:13.000000 pyGuardPoint-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:36:26.051014 pyGuardPoint-0.7.4/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      199 2023-04-13 10:36:26.050020 pyGuardPoint-0.7.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 10:36:26.038012 pyGuardPoint-0.7.4/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.4/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11201 2023-04-06 12:00:47.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.4/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.4/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     2885 2023-04-03 15:08:05.000000 pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:36:26.049027 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-04-13 10:36:26.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2023-04-13 10:36:26.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:36:26.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-13 10:36:26.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 10:36:26.000000 pyGuardPoint-0.7.4/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:36:26.051014 pyGuardPoint-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-04-13 10:36:14.000000 pyGuardPoint-0.7.4/setup.py
```

### Comparing `pyGuardPoint-0.7.3/LICENSE.txt` & `pyGuardPoint-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_odata_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from .guardpoint_dataclasses import Area, Cardholder
+from .guardpoint_dataclasses import Area, Cardholder, CardholderPersonalDetail
 from urllib.parse import quote
 
 
 def _compose_expand(ignore_list, include_list):
     expand_attribs = ['cardholderType', 'cards', 'cardholderPersonalDetail', 'cardholderCustomizedField', 'insideArea',
                       'securityGroup']
     expand_str = ""
@@ -76,15 +76,20 @@
                     earliest_last_pass=None,
                     exact_match=None):
     filter_phrases = []
 
     if exact_match:
         if isinstance(exact_match, dict):
             for k,v in exact_match.items():
-                filter_phrases.append(f"({k}%20eq%20'{quote(v)}')")
+                if isinstance(v, (str, bool, int)):
+                    filter_phrases.append(f"({k}%20eq%20'{quote(v)}')")
+                if k == "cardholderPersonalDetail" and v.__class__.__name__ == "CardholderPersonalDetail":
+                    details = v.dict(changed_only=True)
+                    for dk, dv in details.items():
+                        filter_phrases.append(f"(CardholderPersonalDetail/{dk}%20eq%20'{quote(dv)}')")
 
     if earliest_last_pass:
         if isinstance(earliest_last_pass, datetime):
             last_pass_date = earliest_last_pass.strftime('%Y-%m-%dT%H:%M:%SZ')
             filter_phrases.append(f'(lastPassDate%20ge%20{last_pass_date})')
 
     # Filter out expired cardholders
```

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.7.4/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.7.4/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.7.4/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.3/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.7.4/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

