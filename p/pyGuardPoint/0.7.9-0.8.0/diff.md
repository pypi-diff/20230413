# Comparing `tmp/pyGuardPoint-0.7.9.tar.gz` & `tmp/pyGuardPoint-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.7.9.tar", last modified: Thu Apr 13 14:20:48 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.8.0.tar", last modified: Thu Apr 13 14:22:47 2023, max compression
```

## Comparing `pyGuardPoint-0.7.9.tar` & `pyGuardPoint-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:48.723716 pyGuardPoint-0.7.9/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.7.9/LICENSE.txt
--rw-rw-rw-   0        0        0     1106 2023-04-13 14:20:48.723716 pyGuardPoint-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-04-13 14:19:28.000000 pyGuardPoint-0.7.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:48.714695 pyGuardPoint-0.7.9/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.7.9/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.7.9/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.7.9/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:20:48.722709 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     1106 2023-04-13 14:20:48.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-13 14:20:48.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:20:48.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-13 14:20:48.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 14:20:48.000000 pyGuardPoint-0.7.9/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 14:20:48.723716 pyGuardPoint-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-13 14:20:36.000000 pyGuardPoint-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:47.863777 pyGuardPoint-0.8.0/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-13 14:22:47.862735 pyGuardPoint-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2023-04-13 14:22:21.000000 pyGuardPoint-0.8.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:47.852375 pyGuardPoint-0.8.0/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.0/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.0/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.0/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:22:47.862230 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     1089 2023-04-13 14:22:47.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-13 14:22:47.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:22:47.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-13 14:22:47.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 14:22:47.000000 pyGuardPoint-0.8.0/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:22:47.863777 pyGuardPoint-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-13 14:22:36.000000 pyGuardPoint-0.8.0/setup.py
```

### Comparing `pyGuardPoint-0.7.9/LICENSE.txt` & `pyGuardPoint-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/PKG-INFO` & `pyGuardPoint-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.7.9
+Version: 0.8.0
 Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-===============
 pyGuardPoint
 ===============
 
 pyGuardPoint providers pythonic programming interface to GuardPoint-10.
 GuardPoint-10 is an Access Control System(ACS) - Learn more about GuardPoint-10 here https://www.sensoraccess.co.uk/guardpoint10/
 
 What is it good for?
```

### Comparing `pyGuardPoint-0.7.9/README.rst` & `pyGuardPoint-0.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-===============
 pyGuardPoint
 ===============
 
 pyGuardPoint providers pythonic programming interface to GuardPoint-10.
 GuardPoint-10 is an Access Control System(ACS) - Learn more about GuardPoint-10 here https://www.sensoraccess.co.uk/guardpoint10/
 
 What is it good for?
```

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.8.0/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.8.0/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.8.0/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.8.0/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.7.9
+Version: 0.8.0
 Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-===============
 pyGuardPoint
 ===============
 
 pyGuardPoint providers pythonic programming interface to GuardPoint-10.
 GuardPoint-10 is an Access Control System(ACS) - Learn more about GuardPoint-10 here https://www.sensoraccess.co.uk/guardpoint10/
 
 What is it good for?
```

### Comparing `pyGuardPoint-0.7.9/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.8.0/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.7.9/setup.py` & `pyGuardPoint-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.7.9",
+      version="0.8.0",
       author="John Owen",
       description="Easy-to-use Python module implementing GuardPoint's WebAPI",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

