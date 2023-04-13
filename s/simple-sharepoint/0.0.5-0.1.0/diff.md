# Comparing `tmp/simple_sharepoint-0.0.5-py3-none-any.whl.zip` & `tmp/simple_sharepoint-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 4872 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:30 simple_sharepoint/__init__.py
--rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/client.py
+Zip file size: 7788 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:57 simple_sharepoint/__init__.py
+-rw-rw-rw-  2.0 fat     2900 b- defN 23-Apr-12 07:49 simple_sharepoint/api.py
+-rw-rw-rw-  2.0 fat     2807 b- defN 23-Apr-13 09:53 simple_sharepoint/client.py
 -rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/sharepoint.py
--rw-rw-rw-  2.0 fat     3948 b- defN 23-Apr-13 09:30 simple_sharepoint-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:30 simple_sharepoint-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:30 simple_sharepoint-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      594 b- defN 23-Apr-13 09:30 simple_sharepoint-0.0.5.dist-info/RECORD
-7 files, 11211 bytes uncompressed, 3808 bytes compressed:  66.0%
+-rw-rw-rw-  2.0 fat      684 b- defN 23-Apr-13 04:00 simple_sharepoint/test.py
+-rw-rw-rw-  2.0 fat     1412 b- defN 23-Apr-05 09:21 simple_sharepoint/upload.py
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Apr-13 09:54 simple_sharepoint/utils.py
+-rw-rw-rw-  2.0 fat     3948 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      922 b- defN 23-Apr-13 09:57 simple_sharepoint-0.1.0.dist-info/RECORD
+11 files, 16771 bytes uncompressed, 6216 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
 Filename: simple_sharepoint/__init__.py
 Comment: 
 
+Filename: simple_sharepoint/api.py
+Comment: 
+
 Filename: simple_sharepoint/client.py
 Comment: 
 
 Filename: simple_sharepoint/sharepoint.py
 Comment: 
 
-Filename: simple_sharepoint-0.0.5.dist-info/METADATA
+Filename: simple_sharepoint/test.py
+Comment: 
+
+Filename: simple_sharepoint/upload.py
+Comment: 
+
+Filename: simple_sharepoint/utils.py
+Comment: 
+
+Filename: simple_sharepoint-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: simple_sharepoint-0.0.5.dist-info/WHEEL
+Filename: simple_sharepoint-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: simple_sharepoint-0.0.5.dist-info/top_level.txt
+Filename: simple_sharepoint-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_sharepoint-0.0.5.dist-info/RECORD
+Filename: simple_sharepoint-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_sharepoint/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.5'
+__version__ = '0.1.0'
```

## simple_sharepoint/client.py

```diff
@@ -1,11 +1,13 @@
 from office365.runtime.auth.authentication_context import ClientCredential
 from office365.runtime.client_request_exception import ClientRequestException
 from office365.sharepoint.client_context import ClientContext
 
+from .utils import check_path_exists, create_folder, print_upload_progress
+
 import os
 
 
 class Client():
 	def __init__(self, cid: str, csec: str, base_url: str):
 		self.cid = cid
 		self.csec = csec
@@ -16,39 +18,39 @@
 	
 	def upload_file(self, src: str, dst: str, check_dir: bool=True):
 		try:
 			if check_dir:
 				dirs = [d for d in dst.split("/")[3:] if d]
 				for i in range(len(dirs)):
 					path = "/".join(dirs[:i+1])
-					valid = self.check_path_exists(path)
+					valid = check_path_exists(self.ctx, path)
 
 					if valid is None:
-						self.create_folder(path)
+						create_folder(self.ctx, path)
 
 			target_folder = self.ctx.web.get_folder_by_server_relative_url(dst)
 			response = target_folder.files.create_upload_session(
-				src, 10000000, self.print_upload_progress
+				src, 10000000, print_upload_progress
 			)
 
 			self.ctx.execute_query()
 			print(f"[INFO] {response.serverRelativeUrl} Success uploaded")
 		except Exception as e:
 			print(f"[ERROR] Upload Failed")
 			print(e)
 
 	def upload_dir(self, src: str, dst: str):
 		try:
 			dirs = [d for d in dst.split("/")[3:] if d]
 			for i in range(len(dirs)):
 				path = "/".join(dirs[:i+1])
-				valid = self.check_path_exists(path)
+				valid = check_path_exists(self.ctx, path)
 
 				if valid is None:
-					self.create_folder(path)
+					create_folder(self.ctx, path)
 
 			for file in os.listdir(src):
 				path = '%s/%s' % (src, file)
 				
 				if os.path.isdir(path):
 					ndir = f"{dst}/{file}"
 					self.upload_dir(path, ndir)
@@ -84,29 +86,8 @@
 			for item in files:
 				self.download_file(item.properties["ServerRelativeUrl"], os.path.join(dst, item.properties["Name"]))
 			
 			for item in folders:
 				self.download_dir(item.properties["ServerRelativeUrl"], os.path.join(dst, item.properties["Name"]))
 		except Exception as e:
 			print(f"[ERROR] Donwload failed")
-			print(e)
-
-	def check_path_exists(self, path: str) -> bool:
-		if not path:
-			return []
-
-		try:
-			return self.ctx.web.get_folder_by_server_relative_url(path).get().execute_query().exists
-		except ClientRequestException as e:
-			if e.response.status_code == 404:
-				return None
-			else:
-				raise ValueError(e.response.text)
-
-	def create_folder(self, path: str):
-		if not path:
-			return []
-
-		self.ctx.web.folders.add(path).execute_query()
-	
-	def print_upload_progress(self, offset: int):
-		print("Uploaded '{0}' bytes...".format(offset))   
+			print(e)
```

## Comparing `simple_sharepoint-0.0.5.dist-info/METADATA` & `simple_sharepoint-0.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-sharepoint
-Version: 0.0.5
+Version: 0.1.0
 Summary: Simple way to handle sharepoint with python
 Home-page: UNKNOWN
 Author: sprumin
 Author-email: sprumin@wellbia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

