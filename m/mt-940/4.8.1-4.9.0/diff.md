# Comparing `tmp/mt-940-4.8.1.tar.gz` & `tmp/mt-940-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mt-940-4.8.1.tar", last modified: Tue Sep 12 20:01:27 2017, max compression
+gzip compressed data, was "dist/mt-940-4.9.0.tar", last modified: Mon Oct 30 01:52:01 2017, max compression
```

## Comparing `mt-940-4.8.1.tar` & `mt-940-4.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/
--rw-rw-r--   0 rick       (501) staff       (20)      275 2017-03-28 20:48:12.000000 mt-940-4.8.1/AUTHORS.rst
--rw-r--r--   0 rick       (501) staff       (20)     1513 2017-09-07 22:38:08.000000 mt-940-4.8.1/CHANGES
--rw-rw-r--   0 rick       (501) staff       (20)     3524 2017-03-28 20:48:12.000000 mt-940-4.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 rick       (501) staff       (20)     1490 2017-03-28 20:48:12.000000 mt-940-4.8.1/LICENSE
--rw-rw-r--   0 rick       (501) staff       (20)      121 2017-03-28 20:48:12.000000 mt-940-4.8.1/MANIFEST.in
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt940/
--rw-r--r--   0 rick       (501) staff       (20)      409 2017-09-12 20:01:16.000000 mt-940-4.8.1/mt940/__about__.py
--rw-r--r--   0 rick       (501) staff       (20)      267 2017-09-12 20:01:01.000000 mt-940-4.8.1/mt940/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     2578 2017-09-07 22:38:08.000000 mt-940-4.8.1/mt940/_compat.py
--rw-r--r--   0 rick       (501) staff       (20)    13698 2017-09-07 22:38:08.000000 mt-940-4.8.1/mt940/models.py
--rw-r--r--   0 rick       (501) staff       (20)     1213 2017-09-07 22:38:08.000000 mt-940-4.8.1/mt940/parser.py
--rw-r--r--   0 rick       (501) staff       (20)     6123 2017-09-12 20:01:16.000000 mt-940-4.8.1/mt940/processors.py
--rw-r--r--   0 rick       (501) staff       (20)    10028 2017-09-07 22:38:08.000000 mt-940-4.8.1/mt940/tags.py
--rw-r--r--   0 rick       (501) staff       (20)      693 2017-09-07 22:38:08.000000 mt-940-4.8.1/mt940/utils.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/
--rw-rw-r--   0 rick       (501) staff       (20)        1 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/dependency_links.txt
--rw-rw-r--   0 rick       (501) staff       (20)        1 2017-03-28 21:28:00.000000 mt-940-4.8.1/mt_940.egg-info/not-zip-safe
--rw-rw-r--   0 rick       (501) staff       (20)     8523 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/PKG-INFO
--rw-rw-r--   0 rick       (501) staff       (20)        7 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/requires.txt
--rw-rw-r--   0 rick       (501) staff       (20)      623 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/SOURCES.txt
--rw-rw-r--   0 rick       (501) staff       (20)       12 2017-09-12 20:01:27.000000 mt-940-4.8.1/mt_940.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)     8523 2017-09-12 20:01:27.000000 mt-940-4.8.1/PKG-INFO
--rw-rw-r--   0 rick       (501) staff       (20)     4227 2017-03-28 20:48:12.000000 mt-940-4.8.1/README.rst
--rw-rw-r--   0 rick       (501) staff       (20)        7 2017-03-28 20:48:12.000000 mt-940-4.8.1/requirements.txt
--rw-rw-r--   0 rick       (501) staff       (20)      299 2017-09-12 20:01:27.000000 mt-940-4.8.1/setup.cfg
--rwxrwxr-x   0 rick       (501) staff       (20)     2815 2017-03-28 20:48:12.000000 mt-940-4.8.1/setup.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/tests/
--rw-rw-r--   0 rick       (501) staff       (20)        0 2017-09-12 20:01:01.000000 mt-940-4.8.1/tests/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/tests/betterplace/
--rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/betterplace/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/tests/cmxl/
--rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/cmxl/__init__.py
--rw-rw-r--   0 rick       (501) staff       (20)      256 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/conftest.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-09-12 20:01:27.000000 mt-940-4.8.1/tests/jejik/
--rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/jejik/__init__.py
--rw-rw-r--   0 rick       (501) staff       (20)      558 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/test_metadata.py
--rw-rw-r--   0 rick       (501) staff       (20)     2901 2017-03-28 20:48:12.000000 mt-940-4.8.1/tests/test_processors.py
--rw-r--r--   0 rick       (501) staff       (20)     2702 2017-09-07 22:38:08.000000 mt-940-4.8.1/tests/test_sta_parsing.py
--rw-r--r--   0 rick       (501) staff       (20)      443 2017-09-07 22:38:08.000000 mt-940-4.8.1/tests/test_utils.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/
+-rw-rw-r--   0 rick       (501) staff       (20)      275 2017-03-28 20:48:12.000000 mt-940-4.9.0/AUTHORS.rst
+-rw-r--r--   0 rick       (501) staff       (20)     1513 2017-09-07 22:38:08.000000 mt-940-4.9.0/CHANGES
+-rw-rw-r--   0 rick       (501) staff       (20)     3524 2017-03-28 20:48:12.000000 mt-940-4.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 rick       (501) staff       (20)     1490 2017-03-28 20:48:12.000000 mt-940-4.9.0/LICENSE
+-rw-rw-r--   0 rick       (501) staff       (20)      121 2017-03-28 20:48:12.000000 mt-940-4.9.0/MANIFEST.in
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt940/
+-rw-r--r--   0 rick       (501) staff       (20)      409 2017-10-30 01:51:04.000000 mt-940-4.9.0/mt940/__about__.py
+-rw-r--r--   0 rick       (501) staff       (20)      267 2017-10-30 01:50:20.000000 mt-940-4.9.0/mt940/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     2578 2017-09-07 22:38:08.000000 mt-940-4.9.0/mt940/_compat.py
+-rw-r--r--   0 rick       (501) staff       (20)    13698 2017-09-07 22:38:08.000000 mt-940-4.9.0/mt940/models.py
+-rw-r--r--   0 rick       (501) staff       (20)     1213 2017-09-07 22:38:08.000000 mt-940-4.9.0/mt940/parser.py
+-rw-r--r--   0 rick       (501) staff       (20)     6259 2017-10-30 01:50:25.000000 mt-940-4.9.0/mt940/processors.py
+-rw-r--r--   0 rick       (501) staff       (20)    10028 2017-10-30 01:50:25.000000 mt-940-4.9.0/mt940/tags.py
+-rw-r--r--   0 rick       (501) staff       (20)      693 2017-09-07 22:38:08.000000 mt-940-4.9.0/mt940/utils.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/
+-rw-rw-r--   0 rick       (501) staff       (20)        1 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/dependency_links.txt
+-rw-rw-r--   0 rick       (501) staff       (20)        1 2017-03-28 21:28:00.000000 mt-940-4.9.0/mt_940.egg-info/not-zip-safe
+-rw-rw-r--   0 rick       (501) staff       (20)     8523 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/PKG-INFO
+-rw-rw-r--   0 rick       (501) staff       (20)        7 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/requires.txt
+-rw-rw-r--   0 rick       (501) staff       (20)      623 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/SOURCES.txt
+-rw-rw-r--   0 rick       (501) staff       (20)       12 2017-10-30 01:52:01.000000 mt-940-4.9.0/mt_940.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)     8523 2017-10-30 01:52:01.000000 mt-940-4.9.0/PKG-INFO
+-rw-rw-r--   0 rick       (501) staff       (20)     4227 2017-03-28 20:48:12.000000 mt-940-4.9.0/README.rst
+-rw-rw-r--   0 rick       (501) staff       (20)        7 2017-03-28 20:48:12.000000 mt-940-4.9.0/requirements.txt
+-rw-rw-r--   0 rick       (501) staff       (20)      299 2017-10-30 01:52:01.000000 mt-940-4.9.0/setup.cfg
+-rwxrwxr-x   0 rick       (501) staff       (20)     2815 2017-03-28 20:48:12.000000 mt-940-4.9.0/setup.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/tests/
+-rw-rw-r--   0 rick       (501) staff       (20)        0 2017-10-30 01:50:20.000000 mt-940-4.9.0/tests/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/tests/betterplace/
+-rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/betterplace/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/tests/cmxl/
+-rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/cmxl/__init__.py
+-rw-rw-r--   0 rick       (501) staff       (20)      256 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/conftest.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2017-10-30 01:52:01.000000 mt-940-4.9.0/tests/jejik/
+-rw-rw-r--   0 rick       (501) staff       (20)        0 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/jejik/__init__.py
+-rw-rw-r--   0 rick       (501) staff       (20)      558 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/test_metadata.py
+-rw-rw-r--   0 rick       (501) staff       (20)     2901 2017-03-28 20:48:12.000000 mt-940-4.9.0/tests/test_processors.py
+-rw-r--r--   0 rick       (501) staff       (20)     2702 2017-09-07 22:38:08.000000 mt-940-4.9.0/tests/test_sta_parsing.py
+-rw-r--r--   0 rick       (501) staff       (20)      443 2017-09-07 22:38:08.000000 mt-940-4.9.0/tests/test_utils.py
```

### Comparing `mt-940-4.8.1/CHANGES` & `mt-940-4.9.0/CHANGES`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/CONTRIBUTING.rst` & `mt-940-4.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/LICENSE` & `mt-940-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/mt940/_compat.py` & `mt-940-4.9.0/mt940/_compat.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/mt940/models.py` & `mt-940-4.9.0/mt940/models.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/mt940/parser.py` & `mt-940-4.9.0/mt940/parser.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/mt940/processors.py` & `mt-940-4.9.0/mt940/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     '31': 'applicant_iban',
     '32': 'applicant_name',
     '34': 'return_debit_notes',
     '35': 'recipient_name',
     '60': 'additional_purpose',
 }
 
-# https://www.hettwer-beratung.de/suepa-spezialwissen/sepa-tecshnische-anforderungen/sepa-geschäftsvorfallcodes-gvct-mt-940c/
+# https://www.hettwer-beratung.de/sepa-spezialwissen/sepa-technische-anforderungen/sepa-gesch%C3%A4ftsvorfallcodes-gvc-mt-940/
 GVC_KEYS = {
     '': 'purpose',
     'IBAN': 'gvc_applicant_iban',
     'BIC ': 'gvc_applicant_bin',
     'EREF': 'end_to_end_reference',
     'MREF': 'additional_position_reference',
     'CRED': 'applicant_creditor_id',
@@ -149,14 +149,17 @@
             result[DETAIL_KEYS[key]] = value
         elif key == '33':
             key32 = DETAIL_KEYS['32']
             result[key32] = (result[key32] or '') + value
         elif key.startswith('2'):
             key20 = DETAIL_KEYS['20']
             result[key20] = (result[key20] or '') + value
+        elif key in ('61', '62', '63'):
+            key60 = DETAIL_KEYS['60']
+            result[key60] = (result[key60] or '') + value
 
     return result
 
 
 def _parse_mt940_gvcodes(purpose):
     result = {}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mt-940-4.8.1/mt940/tags.py` & `mt-940-4.9.0/mt940/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     '''Transaction details
 
     Pattern: 6x65x
     '''
     id = 86
     scope = models.Transaction
     pattern = r'''
-    (?P<transaction_details>(([\s\S]{0,65}\r?\n?){0,5}[\s\S]{0,65}))
+    (?P<transaction_details>(([\s\S]{0,65}\r?\n?){0,8}[\s\S]{0,65}))
     '''
 
 
 class SumEntries(Tag):
     '''Number and Sum of debit Entries
 
     '''
```

### Comparing `mt-940-4.8.1/mt940/utils.py` & `mt-940-4.9.0/mt940/utils.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/mt_940.egg-info/PKG-INFO` & `mt-940-4.9.0/mt_940.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mt-940
-Version: 4.8.1
+Version: 4.9.0
 Summary: A library to parse MT940 files and returns smart Python collections for statistics and manipulation.
 Home-page: https://github.com/WoLpH/mt940
 Author: Rick van Hattem (wolph)
 Author-email: wolph@wol.ph
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: =====
```

### Comparing `mt-940-4.8.1/mt_940.egg-info/SOURCES.txt` & `mt-940-4.9.0/mt_940.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/PKG-INFO` & `mt-940-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mt-940
-Version: 4.8.1
+Version: 4.9.0
 Summary: A library to parse MT940 files and returns smart Python collections for statistics and manipulation.
 Home-page: https://github.com/WoLpH/mt940
 Author: Rick van Hattem (wolph)
 Author-email: wolph@wol.ph
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: =====
```

### Comparing `mt-940-4.8.1/README.rst` & `mt-940-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/setup.py` & `mt-940-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/tests/test_metadata.py` & `mt-940-4.9.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/tests/test_processors.py` & `mt-940-4.9.0/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `mt-940-4.8.1/tests/test_sta_parsing.py` & `mt-940-4.9.0/tests/test_sta_parsing.py`

 * *Files identical despite different names*

