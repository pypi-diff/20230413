# Comparing `tmp/finolog-sdk-1.0.6.4.tar.gz` & `tmp/finolog-sdk-1.0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finolog-sdk-1.0.6.4.tar", last modified: Mon Feb 20 14:51:14 2023, max compression
+gzip compressed data, was "finolog-sdk-1.0.6.5.tar", last modified: Thu Apr 13 06:53:08 2023, max compression
```

## Comparing `finolog-sdk-1.0.6.4.tar` & `finolog-sdk-1.0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 14:51:14.050958 finolog-sdk-1.0.6.4/
--rw-rw-rw-   0        0        0     2074 2023-02-20 14:51:14.049959 finolog-sdk-1.0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2023-02-13 15:13:59.000000 finolog-sdk-1.0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 14:51:14.018958 finolog-sdk-1.0.6.4/finolog/
--rw-rw-rw-   0        0        0        0 2023-02-10 14:28:44.000000 finolog-sdk-1.0.6.4/finolog/__init__.py
--rw-rw-rw-   0        0        0       25 2023-02-20 14:50:58.000000 finolog-sdk-1.0.6.4/finolog/_version.py
--rw-rw-rw-   0        0        0      843 2023-02-15 06:46:51.000000 finolog-sdk-1.0.6.4/finolog/client.py
--rw-rw-rw-   0        0        0     2356 2023-02-13 14:52:57.000000 finolog-sdk-1.0.6.4/finolog/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:51:14.023958 finolog-sdk-1.0.6.4/finolog/services/
--rw-rw-rw-   0        0        0        2 2023-02-13 08:08:30.000000 finolog-sdk-1.0.6.4/finolog/services/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-02-13 15:07:19.000000 finolog-sdk-1.0.6.4/finolog/services/api_service.py
--rw-rw-rw-   0        0        0     5151 2023-02-15 07:57:49.000000 finolog-sdk-1.0.6.4/finolog/services/contractor_service.py
--rw-rw-rw-   0        0        0      433 2023-02-15 06:46:51.000000 finolog-sdk-1.0.6.4/finolog/services/country_service.py
--rw-rw-rw-   0        0        0     7869 2023-02-13 07:56:13.000000 finolog-sdk-1.0.6.4/finolog/services/document_service.py
--rw-rw-rw-   0        0        0     5544 2023-02-13 15:00:32.000000 finolog-sdk-1.0.6.4/finolog/services/requisite_service.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:51:14.028958 finolog-sdk-1.0.6.4/finolog/types/
--rw-rw-rw-   0        0        0        0 2023-02-10 14:16:17.000000 finolog-sdk-1.0.6.4/finolog/types/__init__.py
--rw-rw-rw-   0        0        0      972 2023-02-15 07:46:30.000000 finolog-sdk-1.0.6.4/finolog/types/contractor_types.py
--rw-rw-rw-   0        0        0      136 2023-02-15 06:45:33.000000 finolog-sdk-1.0.6.4/finolog/types/country_types.py
--rw-rw-rw-   0        0        0     4590 2023-02-13 07:18:07.000000 finolog-sdk-1.0.6.4/finolog/types/document_types.py
--rw-rw-rw-   0        0        0      727 2023-02-13 11:18:39.000000 finolog-sdk-1.0.6.4/finolog/types/requisite_types.py
--rw-rw-rw-   0        0        0      359 2023-02-13 15:04:48.000000 finolog-sdk-1.0.6.4/finolog/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:51:14.048987 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/
--rw-rw-rw-   0        0        0     2074 2023-02-20 14:51:13.000000 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      656 2023-02-20 14:51:13.000000 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 14:51:13.000000 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-20 14:51:13.000000 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-20 14:51:13.000000 finolog-sdk-1.0.6.4/finolog_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-20 14:51:14.050958 finolog-sdk-1.0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     2300 2023-02-20 14:50:23.000000 finolog-sdk-1.0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:08.500075 finolog-sdk-1.0.6.5/
+-rw-rw-rw-   0        0        0     2074 2023-04-13 06:53:08.495076 finolog-sdk-1.0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2023-02-13 15:13:59.000000 finolog-sdk-1.0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:08.355078 finolog-sdk-1.0.6.5/finolog/
+-rw-rw-rw-   0        0        0        0 2023-02-10 14:28:44.000000 finolog-sdk-1.0.6.5/finolog/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-04-13 06:52:08.000000 finolog-sdk-1.0.6.5/finolog/_version.py
+-rw-rw-rw-   0        0        0      843 2023-02-15 06:46:51.000000 finolog-sdk-1.0.6.5/finolog/client.py
+-rw-rw-rw-   0        0        0     2356 2023-02-13 14:52:57.000000 finolog-sdk-1.0.6.5/finolog/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:08.382076 finolog-sdk-1.0.6.5/finolog/services/
+-rw-rw-rw-   0        0        0        2 2023-02-13 08:08:30.000000 finolog-sdk-1.0.6.5/finolog/services/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-02-13 15:07:19.000000 finolog-sdk-1.0.6.5/finolog/services/api_service.py
+-rw-rw-rw-   0        0        0     5237 2023-04-13 06:51:53.000000 finolog-sdk-1.0.6.5/finolog/services/contractor_service.py
+-rw-rw-rw-   0        0        0      433 2023-02-15 06:46:51.000000 finolog-sdk-1.0.6.5/finolog/services/country_service.py
+-rw-rw-rw-   0        0        0     7869 2023-02-13 07:56:13.000000 finolog-sdk-1.0.6.5/finolog/services/document_service.py
+-rw-rw-rw-   0        0        0     5544 2023-02-13 15:00:32.000000 finolog-sdk-1.0.6.5/finolog/services/requisite_service.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:08.425077 finolog-sdk-1.0.6.5/finolog/types/
+-rw-rw-rw-   0        0        0        0 2023-02-10 14:16:17.000000 finolog-sdk-1.0.6.5/finolog/types/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-02-15 07:46:30.000000 finolog-sdk-1.0.6.5/finolog/types/contractor_types.py
+-rw-rw-rw-   0        0        0      136 2023-02-15 06:45:33.000000 finolog-sdk-1.0.6.5/finolog/types/country_types.py
+-rw-rw-rw-   0        0        0     4590 2023-02-13 07:18:07.000000 finolog-sdk-1.0.6.5/finolog/types/document_types.py
+-rw-rw-rw-   0        0        0      727 2023-02-13 11:18:39.000000 finolog-sdk-1.0.6.5/finolog/types/requisite_types.py
+-rw-rw-rw-   0        0        0      359 2023-02-13 15:04:48.000000 finolog-sdk-1.0.6.5/finolog/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:08.487076 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2074 2023-04-13 06:53:08.000000 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2023-04-13 06:53:08.000000 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:53:08.000000 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-13 06:53:08.000000 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 06:53:08.000000 finolog-sdk-1.0.6.5/finolog_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:53:08.503078 finolog-sdk-1.0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     2300 2023-02-20 14:50:23.000000 finolog-sdk-1.0.6.5/setup.py
```

### Comparing `finolog-sdk-1.0.6.4/PKG-INFO` & `finolog-sdk-1.0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finolog-sdk
-Version: 1.0.6.4
+Version: 1.0.6.5
 Summary: Wrapper for working with Finolog service API
 Home-page: https://github.com/RTHeLL/finolog-sdk
 Download-URL: https://github.com/RTHeLL/finolog-sdk/archive/master.zip
 Author: Kinder (RTHeLL)
 Author-email: k1ndermail@ya.ru
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: wrapper,finance,finolog
```

### Comparing `finolog-sdk-1.0.6.4/README.md` & `finolog-sdk-1.0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/client.py` & `finolog-sdk-1.0.6.5/finolog/client.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/exceptions.py` & `finolog-sdk-1.0.6.5/finolog/exceptions.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/services/api_service.py` & `finolog-sdk-1.0.6.5/finolog/services/api_service.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/services/contractor_service.py` & `finolog-sdk-1.0.6.5/finolog/services/contractor_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,19 @@
         if 'inn' in payload:
             validate_string_length('inn', payload['inn'], min_l=10, max_l=12)
 
         if 'is_bizzed' in payload:
             payload['is_bizzed'] = 'true' if payload['is_bizzed'] is True else 'false'
 
         response = self.request('GET', self.uri, payload)
-        return [Contractor(**obj) for obj in response]
+
+        try:
+            return [Contractor(**obj) for obj in response]
+        except TypeError:
+            raise TypeError(response)
 
     def get_contractor(self, contractor_id: int) -> Contractor:
         self.validate_payload(
             payload={'id': contractor_id},
             types={
                 'id': int
             }
```

### Comparing `finolog-sdk-1.0.6.4/finolog/services/document_service.py` & `finolog-sdk-1.0.6.5/finolog/services/document_service.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/services/requisite_service.py` & `finolog-sdk-1.0.6.5/finolog/services/requisite_service.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/types/contractor_types.py` & `finolog-sdk-1.0.6.5/finolog/types/contractor_types.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/types/document_types.py` & `finolog-sdk-1.0.6.5/finolog/types/document_types.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog/types/requisite_types.py` & `finolog-sdk-1.0.6.5/finolog/types/requisite_types.py`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/finolog_sdk.egg-info/PKG-INFO` & `finolog-sdk-1.0.6.5/finolog_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finolog-sdk
-Version: 1.0.6.4
+Version: 1.0.6.5
 Summary: Wrapper for working with Finolog service API
 Home-page: https://github.com/RTHeLL/finolog-sdk
 Download-URL: https://github.com/RTHeLL/finolog-sdk/archive/master.zip
 Author: Kinder (RTHeLL)
 Author-email: k1ndermail@ya.ru
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: wrapper,finance,finolog
```

### Comparing `finolog-sdk-1.0.6.4/finolog_sdk.egg-info/SOURCES.txt` & `finolog-sdk-1.0.6.5/finolog_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finolog-sdk-1.0.6.4/setup.py` & `finolog-sdk-1.0.6.5/setup.py`

 * *Files identical despite different names*

