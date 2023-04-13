# Comparing `tmp/ms_salesforce_to_bigquery-0.0.7.tar.gz` & `tmp/ms_salesforce_to_bigquery-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_to_bigquery-0.0.7.tar", max compression
+gzip compressed data, was "ms_salesforce_to_bigquery-0.0.8.tar", max compression
```

## Comparing `ms_salesforce_to_bigquery-0.0.7.tar` & `ms_salesforce_to_bigquery-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/LICENSE
--rw-r--r--   0        0        0     3396 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/__init__.py
--rw-r--r--   0        0        0     1499 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2083 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2757 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2403 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     3268 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     1419 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0     6900 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     3661 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0      980 2023-04-12 14:28:28.988284 ms_salesforce_to_bigquery-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3396 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/__init__.py
+-rw-r--r--   0        0        0     1499 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2275 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2757 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2403 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     3268 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     1419 2023-04-13 11:32:12.599493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:32:12.603493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0     6900 2023-04-13 11:32:12.603493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     6962 2023-04-13 11:32:12.603493 ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-13 11:32:12.603493 ms_salesforce_to_bigquery-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 ms_salesforce_to_bigquery-0.0.8/PKG-INFO
```

### Comparing `ms_salesforce_to_bigquery-0.0.7/LICENSE` & `ms_salesforce_to_bigquery-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/README.md` & `ms_salesforce_to_bigquery-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/Auth.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/SalesforceQueryExecutor.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             private_key,
             audience,
             session_duration_hours,
         )
         self.endpoint = (
             f"{domain}/{SALESFORCE_QUERY_ENDPOINT.format(api_version)}"
         )
+        self.domain = domain
         self.access_token = self.authenticate()
 
     def fetch_data(self, query: str):
         if not self.access_token:
             logging.error("Authentication failed, cannot fetch data")
             return None
 
@@ -44,15 +45,19 @@
         next_url = f"{self.endpoint}?q={query}"
 
         while next_url:
             response = self._make_request(next_url, headers)
             if response:
                 data = response.json()
                 all_records.extend(data.get("records", []))
-                next_url = data.get("nextRecordsUrl", None)
+                nextRecordsUrl = data.get("nextRecordsUrl", None)
+                if nextRecordsUrl:
+                    next_url = f"{self.domain}{nextRecordsUrl}"
+                else:
+                    next_url = None
             else:
                 next_url = None
 
         return all_records
 
     def _make_request(self, url, headers):
         try:
```

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/__init__.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_to_bigquery-0.0.8/ms_salesforce_to_bigquery/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_to_bigquery-0.0.7/pyproject.toml` & `ms_salesforce_to_bigquery-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-to-bigquery"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_to_bigquery"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_to_bigquery-0.0.7/PKG-INFO` & `ms_salesforce_to_bigquery-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-to-bigquery
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

