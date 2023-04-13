# Comparing `tmp/tap_exact-0.1.0.tar.gz` & `tmp/tap_exact-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.1.0.tar", max compression
+gzip compressed data, was "tap_exact-0.1.1.tar", max compression
```

## Comparing `tap_exact-0.1.0.tar` & `tap_exact-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-13 07:17:41.445248 tap_exact-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.0/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.0/tap_exact/client.py
--rw-r--r--   0        0        0    24892 2023-04-13 08:13:29.985247 tap_exact-0.1.0/tap_exact/streams.py
--rw-r--r--   0        0        0     1643 2023-04-13 08:15:22.125248 tap_exact-0.1.0/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.0/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.0/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.0/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-13 09:22:16.735247 tap_exact-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.1/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.1/tap_exact/client.py
+-rw-r--r--   0        0        0    24904 2023-04-13 09:22:12.055247 tap_exact-0.1.1/tap_exact/streams.py
+-rw-r--r--   0        0        0     1643 2023-04-13 08:15:22.125248 tap_exact-0.1.1/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.1/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.1/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.1/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.1/PKG-INFO
```

### Comparing `tap_exact-0.1.0/pyproject.toml` & `tap_exact-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.1.0"
+version = "0.1.1"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.1.0/tap_exact/client.py` & `tap_exact-0.1.1/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.0/tap_exact/streams.py` & `tap_exact-0.1.1/tap_exact/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # TODO: - Override `UsersStream` and `GroupsStream` with your own stream definition.
 #       - Copy-paste as many times as needed to create multiple stream types.
 
 
 class SalesInvoicesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "sales-invoices"
+    name = "sales_invoices"
     primary_keys = ["InvoiceID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "InvoiceID",
@@ -103,15 +103,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class PurchaseInvoicesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "purchase-invoices"
+    name = "purchase_invoices"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -201,15 +201,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class GeneralLedgerAccountsStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "gl-accounts"
+    name = "general_ledger_accounts"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -279,15 +279,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class BankEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "bank-entry-lines"
+    name = "bank_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -372,15 +372,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class CashEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "cash-entry-lines"
+    name = "cash_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -465,15 +465,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class GeneralJournalEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "general-journal-entry-lines"
+    name = "general_journal_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -563,15 +563,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class PurchaseEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "purchase-entry-lines"
+    name = "purchase_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
@@ -651,15 +651,15 @@
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
 class SalesEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "sales-entry-lines"
+    name = "sales_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
```

### Comparing `tap_exact-0.1.0/tap_exact/tap.py` & `tap_exact-0.1.1/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.0/tap_exact/tests/test_core.py` & `tap_exact-0.1.1/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.0/setup.py` & `tap_exact-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.1.0/PKG-INFO` & `tap_exact-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.1.0
+Version: 0.1.1
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

