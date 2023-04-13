# Comparing `tmp/salure_helpers_sap-1.5.3.tar.gz` & `tmp/salure_helpers_sap-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_sap-1.5.3.tar", last modified: Thu Mar 16 16:14:38 2023, max compression
+gzip compressed data, was "dist/salure_helpers_sap-1.5.4.tar", last modified: Thu Apr 13 13:12:02 2023, max compression
```

## Comparing `salure_helpers_sap-1.5.3.tar` & `salure_helpers_sap-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/
--rw-r--r--   0 root         (0) root         (0)      253 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10581 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/base_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     7670 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/delimit_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/get_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    22851 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/post_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/salure_helpers/sap/sap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/salure_helpers_sap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 16:14:38.000000 salure_helpers_sap-1.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-03-16 16:14:24.000000 salure_helpers_sap-1.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10581 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/base_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7670 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/delimit_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/get_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    22850 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/post_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/salure_helpers/sap/sap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/salure_helpers_sap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:12:02.000000 salure_helpers_sap-1.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-04-13 13:11:48.000000 salure_helpers_sap-1.5.4/setup.py
```

### Comparing `salure_helpers_sap-1.5.3/salure_helpers/sap/base_functions.py` & `salure_helpers_sap-1.5.4/salure_helpers/sap/base_functions.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.3/salure_helpers/sap/delimit_endpoints.py` & `salure_helpers_sap-1.5.4/salure_helpers/sap/delimit_endpoints.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.3/salure_helpers/sap/get_endpoints.py` & `salure_helpers_sap-1.5.4/salure_helpers/sap/get_endpoints.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.3/salure_helpers/sap/post_endpoints.py` & `salure_helpers_sap-1.5.4/salure_helpers/sap/post_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         fields_to_update.update({"UserIdLong": data['user_id_long']}) if 'user_id_long' in data else fields_to_update
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body.update(fields_to_update)
 
-        response = self.base_class.post_data(uri='CommunicationsPost/*', data=base_body, return_key='UserId')
+        response = self.base_class.post_data(uri='CommunicationPost/*', data=base_body, return_key='UserId')
         return response
 
     def post_organisational_unit(self, data: dict, overload_fields: dict = None):
         """
         Post OrgUnits to SAP
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Give the guid and value from a free field if wanted
```

### Comparing `salure_helpers_sap-1.5.3/salure_helpers/sap/sap.py` & `salure_helpers_sap-1.5.4/salure_helpers/sap/sap.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_sap-1.5.3/setup.py` & `salure_helpers_sap-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='salure_helpers_sap',
-    version='1.5.3',
+    version='1.5.4',
     description='SAP wrapper from Salure',
     long_description='SAP wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.sap"],
     license='Salure License',
     install_requires=[
```

