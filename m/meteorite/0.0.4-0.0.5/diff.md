# Comparing `tmp/meteorite-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/meteorite-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2499448 bytes, number of entries: 6
--rw-r--r--  4.6 unx     2072 b- defN 23-Apr-01 08:24 meteorite-0.0.4.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-01 08:24 meteorite-0.0.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     1101 b- defN 23-Apr-01 08:24 meteorite-0.0.4.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      119 b- defN 23-Apr-01 08:24 meteorite/__init__.py
--rwxr-xr-x  4.6 unx  6608384 b- defN 23-Apr-01 08:24 meteorite/meteorite.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      491 b- defN 23-Apr-01 08:24 meteorite-0.0.4.dist-info/RECORD
-6 files, 6612263 bytes uncompressed, 2498564 bytes compressed:  62.2%
+Zip file size: 2499669 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     2097 b- defN 23-Apr-13 18:30 meteorite-0.0.5.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-13 18:30 meteorite-0.0.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1101 b- defN 23-Apr-13 18:30 meteorite-0.0.5.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      119 b- defN 23-Apr-13 18:30 meteorite/__init__.py
+-rwxr-xr-x  4.6 unx  6611968 b- defN 23-Apr-13 18:30 meteorite/meteorite.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      491 b- defN 23-Apr-13 18:30 meteorite-0.0.5.dist-info/RECORD
+6 files, 6615872 bytes uncompressed, 2498785 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: meteorite-0.0.4.dist-info/METADATA
+Filename: meteorite-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: meteorite-0.0.4.dist-info/WHEEL
+Filename: meteorite-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: meteorite-0.0.4.dist-info/license_files/LICENSE
+Filename: meteorite-0.0.5.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: meteorite/__init__.py
 Comment: 
 
 Filename: meteorite/meteorite.cp39-win_amd64.pyd
 Comment: 
 
-Filename: meteorite-0.0.4.dist-info/RECORD
+Filename: meteorite-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `meteorite-0.0.4.dist-info/METADATA` & `meteorite-0.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: meteorite
-Version: 0.0.4
+Version: 0.0.5
 License-File: LICENSE
 Summary: A fast and simple web server for machine learning models
 Keywords: model,server,api,hosting
 Maintainer-email: Utkarsh Goel <utkarsh@deploif.ai>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ☄️ Meteorite
+
 A fast and simple web server to host your Machine Learning model.
 
 <!-- TOC -->
-* [☄️ Meteorite](#-meteorite)
-  * [Install the pip package](#install-the-pip-package)
-  * [Write your server](#write-your-server)
-  * [Project status](#project-status)
-  * [Contribute to ☄️ Meteorite](#contribute-to--meteorite)
-<!-- TOC -->
+
+- [☄️ Meteorite](#-meteorite)
+  - [Install the pip package](#install-the-pip-package)
+  - [Write your server](#write-your-server)
+  - [Project status](#project-status)
+  - [Contribute to ☄️ Meteorite](#contribute-to--meteorite)
+  <!-- TOC -->
 
 ## Install the pip package
 
 ```shell
 pip install meteorite
 ```
 
@@ -37,33 +39,33 @@
 def predict(data):
     body = data.decode("utf-8")
     """
     Run your model on the input
     """
     return body
 
-app.start()
+app.start(port=4000) # port is 4000 by default
 ```
 
 By default, the server starts at port `4000`. The `predict` function will run with GET/POST requests on `/predict`.
 
-You can go to http://localhost:4000/predict on your browser to see the result, or use a REST API client to test the 
+You can go to http://localhost:4000/predict on your browser to see the result, or use a REST API client to test the
 endpoint.
 
 ## Project status
 
-This project is under active development. We will not recommend you to use this package for critical applications. 
+This project is under active development. We will not recommend you to use this package for critical applications.
 We will welcome all contributions! Please refer to the contributions section for more details.
 
 Some of the features we're still working on:
 
 - [x] Pass POST request String and JSON into the Python function.
 - [x] Return String and JSON with the correct content type headers.
-- [ ] Graceful error handling (⚠️ Priority).
-- [ ] Customise the route and port for the main task.
+- [x] Graceful error handling (⚠️ Priority).
+- [x] Customise the port for the server
 - [ ] Allow more datatypes for POST request to the model.
 - [ ] Create more examples.
 
 ## Contribute to ☄️ Meteorite
 
 Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) docs for details.
```

## Comparing `meteorite-0.0.4.dist-info/license_files/LICENSE` & `meteorite-0.0.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

