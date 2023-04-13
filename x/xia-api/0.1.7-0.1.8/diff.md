# Comparing `tmp/xia_api-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_api-0.1.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 384647 bytes, number of entries: 9
--rw-r--r--  2.0 unx      497 b- defN 23-Mar-12 08:04 xia_api/__init__.py
--rw-r--r--  2.0 unx   240128 b- defN 23-Mar-12 08:54 xia_api/auth_client.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   286208 b- defN 23-Mar-12 08:55 xia_api/message.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   450560 b- defN 23-Mar-12 08:56 xia_api/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-12 08:56 xia_api-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      675 b- defN 23-Mar-12 08:56 xia_api-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-12 08:56 xia_api-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-12 08:56 xia_api-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      742 b- defN 23-Mar-12 08:56 xia_api-0.1.7.dist-info/RECORD
-9 files, 979069 bytes uncompressed, 383371 bytes compressed:  60.8%
+Zip file size: 384746 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      497 b- defN 23-Apr-13 06:12 xia_api/__init__.py
+-rw-r--r--  2.0 unx   240128 b- defN 23-Apr-13 06:32 xia_api/auth_client.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   286208 b- defN 23-Apr-13 06:33 xia_api/message.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   450560 b- defN 23-Apr-13 06:35 xia_api/rest.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      675 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      742 b- defN 23-Apr-13 06:35 xia_api-0.1.8.dist-info/RECORD
+9 files, 979069 bytes uncompressed, 383470 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_api/message.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_api/rest.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_api-0.1.7.dist-info/LICENSE.txt
+Filename: xia_api-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api-0.1.7.dist-info/METADATA
+Filename: xia_api-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_api-0.1.7.dist-info/WHEEL
+Filename: xia_api-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api-0.1.7.dist-info/top_level.txt
+Filename: xia_api-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api-0.1.7.dist-info/RECORD
+Filename: xia_api-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api/__init__.py

```diff
@@ -7,8 +7,8 @@
 __all__ = [
     "AuthClient",
     "RestApi", "error_handle",
     "XiaCollectionDeleteMsg", "XiaDocumentDeleteMsg", "XiaFileMsg", "XiaRecordBook", "XiaRecordItem",
     "XiaErrorMessage", "XiaActionResult"
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_api-0.1.7.dist-info/METADATA` & `xia_api-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

