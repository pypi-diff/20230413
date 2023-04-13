# Comparing `tmp/looker_ingestion-1.2.0.tar.gz` & `tmp/looker_ingestion-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looker_ingestion-1.2.0.tar", last modified: Thu Sep  1 17:51:08 2022, max compression
+gzip compressed data, was "looker_ingestion-1.3.0.tar", last modified: Thu Apr 13 21:48:21 2023, max compression
```

## Comparing `looker_ingestion-1.2.0.tar` & `looker_ingestion-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 17:51:08.603681 looker_ingestion-1.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10198 2022-09-01 17:51:08.603681 looker_ingestion-1.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9823 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 17:51:08.587681 looker_ingestion-1.2.0/looker_ingestion/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/looker_ingestion/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/looker_ingestion/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2758 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/looker_ingestion/load_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10581 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/looker_ingestion/sync_data.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 17:51:08.587681 looker_ingestion-1.2.0/looker_ingestion.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10198 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2022-09-01 17:51:08.000000 looker_ingestion-1.2.0/looker_ingestion.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-09-01 17:51:08.603681 looker_ingestion-1.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      850 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 17:51:08.587681 looker_ingestion-1.2.0/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3573 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/tests/test_load_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2987 2022-09-01 17:50:57.000000 looker_ingestion-1.2.0/tests/test_sync_data.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10198 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/looker_ingestion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/looker_ingestion/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/looker_ingestion/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2758 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/looker_ingestion/load_s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10581 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/looker_ingestion/sync_data.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/looker_ingestion.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10198 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-04-13 21:48:21.000000 looker_ingestion-1.3.0/looker_ingestion.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-13 21:48:21.863750 looker_ingestion-1.3.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3573 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/tests/test_load_s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2023-04-13 21:48:07.000000 looker_ingestion-1.3.0/tests/test_sync_data.py
```

### Comparing `looker_ingestion-1.2.0/LICENSE` & `looker_ingestion-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.2.0/PKG-INFO` & `looker_ingestion-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looker_ingestion
-Version: 1.2.0
+Version: 1.3.0
 Summary: Extracts adhoc queries from the Looker API to S3
 Home-page: https://github.com/open-toast/extract-looker-metadata
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `looker_ingestion-1.2.0/README.md` & `looker_ingestion-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.2.0/looker_ingestion/load_s3.py` & `looker_ingestion-1.3.0/looker_ingestion/load_s3.py`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.2.0/looker_ingestion/sync_data.py` & `looker_ingestion-1.3.0/looker_ingestion/sync_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             model=query_body["model"],
             view=query_body["explore"],
             fields=fields,
             filters=filters,
             sorts=sorts,
             limit=row_limit,
         )
-        sdk = looker_sdk.init31()
+        sdk = looker_sdk.init40()
         query_run = sdk.run_inline_query(result_format, write_query)
         if result_format == "json":
             query_run = json.loads(query_run)
             if query_run != []:
                 if query_run[0].get("looker_error") is not None:
                     logging.error(
                         f"Error {query_run[0].get('looker_error')} returned when attempting to fetch Looker query history for {date_filter}"
```

### Comparing `looker_ingestion-1.2.0/looker_ingestion.egg-info/PKG-INFO` & `looker_ingestion-1.3.0/looker_ingestion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looker-ingestion
-Version: 1.2.0
+Version: 1.3.0
 Summary: Extracts adhoc queries from the Looker API to S3
 Home-page: https://github.com/open-toast/extract-looker-metadata
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `looker_ingestion-1.2.0/setup.py` & `looker_ingestion-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="looker_ingestion",
-    version="1.2.0",
+    version="1.3.0",
     description="Extracts adhoc queries from the Looker API to S3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/open-toast/extract-looker-metadata",
     packages=find_packages(),
     entry_points={
         "console_scripts": ["extract_looker_metadata = looker_ingestion.sync_data:main"]
```

### Comparing `looker_ingestion-1.2.0/tests/test_load_s3.py` & `looker_ingestion-1.3.0/tests/test_load_s3.py`

 * *Files identical despite different names*

### Comparing `looker_ingestion-1.2.0/tests/test_sync_data.py` & `looker_ingestion-1.3.0/tests/test_sync_data.py`

 * *Files identical despite different names*

