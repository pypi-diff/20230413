# Comparing `tmp/pycallrail-0.5.2.tar.gz` & `tmp/pycallrail-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycallrail-0.5.2.tar", last modified: Mon Mar 27 07:41:12 2023, max compression
+gzip compressed data, was "pycallrail-0.5.3.tar", last modified: Mon Mar 27 08:02:12 2023, max compression
```

## Comparing `pycallrail-0.5.2.tar` & `pycallrail-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:12.160972 pycallrail-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 07:41:12.160972 pycallrail-0.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:12.156973 pycallrail-0.5.2/pycallrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:12.160972 pycallrail-0.5.2/pycallrail/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/companies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/form_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/api/textmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/callrail.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:12.160972 pycallrail-0.5.2/pycallrail/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/tests/testbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-27 07:41:01.000000 pycallrail-0.5.2/pycallrail/tests/testcall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:41:12.156973 pycallrail-0.5.2/pycallrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 07:41:12.000000 pycallrail-0.5.2/pycallrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-27 07:41:12.000000 pycallrail-0.5.2/pycallrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 07:41:12.000000 pycallrail-0.5.2/pycallrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 07:41:12.000000 pycallrail-0.5.2/pycallrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 07:41:12.000000 pycallrail-0.5.2/pycallrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 07:41:12.160972 pycallrail-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-27 07:41:01.000000 pycallrail-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:02:12.275301 pycallrail-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 08:02:12.275301 pycallrail-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:02:12.271301 pycallrail-0.5.3/pycallrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:02:12.275301 pycallrail-0.5.3/pycallrail/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/companies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/form_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/api/textmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/callrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:02:12.275301 pycallrail-0.5.3/pycallrail/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/tests/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-27 08:01:59.000000 pycallrail-0.5.3/pycallrail/tests/testcall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:02:12.271301 pycallrail-0.5.3/pycallrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 08:02:12.000000 pycallrail-0.5.3/pycallrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-27 08:02:12.000000 pycallrail-0.5.3/pycallrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 08:02:12.000000 pycallrail-0.5.3/pycallrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 08:02:12.000000 pycallrail-0.5.3/pycallrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 08:02:12.000000 pycallrail-0.5.3/pycallrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 08:02:12.275301 pycallrail-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-27 08:01:59.000000 pycallrail-0.5.3/setup.py
```

### Comparing `pycallrail-0.5.2/pycallrail/api/accounts.py` & `pycallrail-0.5.3/pycallrail/api/accounts.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/api/call.py` & `pycallrail-0.5.3/pycallrail/api/call.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/api/companies.py` & `pycallrail-0.5.3/pycallrail/api/companies.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/api/form_submissions.py` & `pycallrail-0.5.3/pycallrail/api/form_submissions.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/api/tag.py` & `pycallrail-0.5.3/pycallrail/api/tag.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/api/textmessage.py` & `pycallrail-0.5.3/pycallrail/api/textmessage.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/callrail.py` & `pycallrail-0.5.3/pycallrail/callrail.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             'relative_pagination': 'true'
         }
 
     def _relative_paginator(
             self,
             response: requests.Response,
             response_data_key: str = None
-    ) -> Iterable | AsyncIterable | Generator | AsyncGenerator:
+    ) -> Iterable:
         """
         Base relative pagination function for the CallRail API.
         """
         pagination_list = []
         while True:
             try:
                 pagination_list.extend(response.json()[response_data_key])
@@ -116,15 +116,15 @@
                 raise e
         return pagination_list
     
     def _offset_paginator(
             self,
             response: requests.Response,
             response_data_key: str = None
-    ) -> Iterable | AsyncIterable | Generator | AsyncGenerator:
+    ) -> Iterable :
         """
         Base offset pagination function for the CallRail API.
         """
         pagination_list = []
         current_page = response.json()['page']
         total_pages = response.json()['total_pages']
```

### Comparing `pycallrail-0.5.2/pycallrail/exceptions.py` & `pycallrail-0.5.3/pycallrail/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail/tests/testbase.py` & `pycallrail-0.5.3/pycallrail/tests/testbase.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
         },
         parent=self.cr)
 
         account = self.cr.get_account("ACCfc800e85eba74b62ae02ef58fd76b0db")
         mock_get_account.assert_called_once()
 
         self.assertIsInstance(account, Account)
-        self.assertEqual(account.id, "ACCfc800e85eba74b62ae02ef58fd76b0db")
+        self.assertEqual(account.id, "ACCfc800e85eba74b62ae02ef58fd76b0db")
```

### Comparing `pycallrail-0.5.2/pycallrail/tests/testcall.py` & `pycallrail-0.5.3/pycallrail/tests/testcall.py`

 * *Files identical despite different names*

### Comparing `pycallrail-0.5.2/pycallrail.egg-info/SOURCES.txt` & `pycallrail-0.5.3/pycallrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

