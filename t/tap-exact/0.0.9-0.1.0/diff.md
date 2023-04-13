# Comparing `tmp/tap_exact-0.0.9.tar.gz` & `tmp/tap_exact-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.0.9.tar", max compression
+gzip compressed data, was "tap_exact-0.1.0.tar", max compression
```

## Comparing `tap_exact-0.0.9.tar` & `tap_exact-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-02-28 18:32:44.466873 tap_exact-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.0.9/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.0.9/tap_exact/client.py
--rw-r--r--   0        0        0     3162 2023-02-28 18:32:21.896873 tap_exact-0.0.9/tap_exact/streams.py
--rw-r--r--   0        0        0     1233 2022-12-28 16:09:09.953613 tap_exact-0.0.9/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.0.9/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.0.9/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.0.9/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-13 07:17:41.445248 tap_exact-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.0/tap_exact/client.py
+-rw-r--r--   0        0        0    24892 2023-04-13 08:13:29.985247 tap_exact-0.1.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1643 2023-04-13 08:15:22.125248 tap_exact-0.1.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.0/PKG-INFO
```

### Comparing `tap_exact-0.0.9/pyproject.toml` & `tap_exact-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.0.9"
+version = "0.1.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.0.9/tap_exact/client.py` & `tap_exact-0.1.0/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.0.9/tap_exact/tap.py` & `tap_exact-0.1.0/tap_exact/tap.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,33 @@
 
 from singer_sdk import Tap, Stream
 from singer_sdk import typing as th  # JSON schema typing helpers
 # TODO: Import your custom stream types here:
 from tap_exact.streams import (
     ExactOnlineStream,
     SalesInvoicesStream,
+    PurchaseInvoicesStream,
+    GeneralLedgerAccountsStream,
+    BankEntryLinesStream,
+    CashEntryLinesStream,
+    GeneralJournalEntryLinesStream,
+    PurchaseEntryLinesStream,
+    SalesEntryLinesStream
 )
 # TODO: Compile a list of custom stream types here
 #       OR rewrite discover_streams() below with your custom logic.
 STREAM_TYPES = [
     SalesInvoicesStream,
+    PurchaseInvoicesStream,
+    GeneralLedgerAccountsStream,
+    BankEntryLinesStream,
+    CashEntryLinesStream,
+    GeneralJournalEntryLinesStream,
+    PurchaseEntryLinesStream,
+    SalesEntryLinesStream
 ]
 
 
 class TapExactOnline(Tap):
     """ExactOnline tap class."""
     name = "tap-exact"
```

### Comparing `tap_exact-0.0.9/tap_exact/tests/test_core.py` & `tap_exact-0.1.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.0.9/setup.py` & `tap_exact-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.0.9',
+    'version': '0.1.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.0.9/PKG-INFO` & `tap_exact-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.0.9
+Version: 0.1.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

