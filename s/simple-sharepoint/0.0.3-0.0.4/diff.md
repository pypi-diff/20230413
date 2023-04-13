# Comparing `tmp/simple_sharepoint-0.0.3-py3-none-any.whl.zip` & `tmp/simple_sharepoint-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4862 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:22 simple_sharepoint/__init__.py
+Zip file size: 4870 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:26 simple_sharepoint/__init__.py
 -rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/client.py
 -rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/sharepoint.py
--rw-rw-rw-  2.0 fat     3831 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      594 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/RECORD
-7 files, 11094 bytes uncompressed, 3798 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat     3924 b- defN 23-Apr-13 09:26 simple_sharepoint-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:26 simple_sharepoint-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:26 simple_sharepoint-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      594 b- defN 23-Apr-13 09:26 simple_sharepoint-0.0.4.dist-info/RECORD
+7 files, 11187 bytes uncompressed, 3806 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: simple_sharepoint/client.py
 Comment: 
 
 Filename: simple_sharepoint/sharepoint.py
 Comment: 
 
-Filename: simple_sharepoint-0.0.3.dist-info/METADATA
+Filename: simple_sharepoint-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: simple_sharepoint-0.0.3.dist-info/WHEEL
+Filename: simple_sharepoint-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: simple_sharepoint-0.0.3.dist-info/top_level.txt
+Filename: simple_sharepoint-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_sharepoint-0.0.3.dist-info/RECORD
+Filename: simple_sharepoint-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_sharepoint/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.3'
+__version__ = '0.0.4'
```

## Comparing `simple_sharepoint-0.0.3.dist-info/METADATA` & `simple_sharepoint-0.0.4.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-sharepoint
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple way to handle sharepoint with python
 Home-page: UNKNOWN
 Author: sprumin
 Author-email: sprumin@wellbia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -56,61 +56,62 @@
 default_path = < SHAREPOINT_BASE_PATH >
 src = < LOCAL_FILE_PATH >
 dst = default_path + < SHAREPOINT_TARGET_PATH >
 
 upload_file(src, dst)
 ```
 
-<b>SHAREPOINT_BASE_PATH</b> refers to the default path for a sharepoint document entry.<br>
+<b><i>SHAREPOINT_BASE_PATH</i></b> refers to the default path for a sharepoint document entry.<br>
 ( format ) /sites/<SHAREPOINT_SITE>/Shared Documents<br>
 ( ex ) `/sites/testsite/Shared Documents`
 
-<b>LOCAL_FILE_PATH</b> means the path to the file to be uploaded.<br>
+<b><i>LOCAL_FILE_PATH</i></b> means the path to the file to be uploaded.<br>
 ( ex ) `/home/ubuntu/test.txt`
 
-<b>SHAREPOINT_TARGET_PATH</b> means the actual path to be uploaded to sharepoint.<br>
+<b><i>SHAREPOINT_TARGET_PATH</i></b> means the actual path to be uploaded to sharepoint.<br>
 Think of the document menu in sharepoint as the root directory and enter the path thereafter.<br>
 You do not need to include the file name.<br>
 ( ex ) `excel/example`
 
 If you run it as above, it will be uploaded as below.<br>
 `/sites/testsite/Shared Documents/excel/example/test.txt`
 
+
 ### upload_dir
 
 A function that uploads a particular directory and all its contents under the directory to sharepoint.
 
 ```python
 default_path = < SHAREPOINT_BASE_PATH >
 src = < LOCAL_DIR_PATH >
 dst = default_path + < SHAREPOINT_TARGET_PATH >
 
 upload_dir(src, dst)
 ```
 
-<b>SHAREPOINT_BASE_PATH</b>, <b>SHAREPIONT_TARGET_PATH</b> See item upload_file
+<b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b> See item upload_file
 
-<b>LOCAL_DIR_PATH</b> means the path to the directory to be uploaded.<br>
+<b><i>LOCAL_DIR_PATH</i></b> means the path to the directory to be uploaded.<br>
 ( ex ) `/home/ubuntu/files`
 
 ### download_file
 
 A function that downloads a specific file from the sharepoint.
 
 ```python
 default_path = < SHAREPOINT_BASE_PATH >
 src = default_path + < SHAREPOINT_TARGET_PATH >
 dst = < LOCAL_FILE_PATH >
 
 download_file(src, dst)
 ```
 
-<b>SHAREPOINT_BASE_PATH</b>, <b>SHAREPIONT_TARGET_PATH</b>, <b>LOCAL_FILE_PATH</b> See item upload_file
+<b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b>, <b><i>LOCAL_FILE_PATH</i></b> See item upload_file
 
-The download_file function requires you to specify the file name to be stored in <b>LOCAL_FILE_PATH</b>.
+The download_file function requires you to specify the file name to be stored in <b><i>LOCAL_FILE_PATH</i></b>.
 ( ex ) `/home/ubuntu/files/test.txt`
 
 
 ### download_dir
 
 A function that downloads a particular directory in the sharepoint and all the contents under it.
 
@@ -118,14 +119,14 @@
 default_path = < SHAREPOINT_BASE_PATH >
 src = default_path + < SHAREPOINT_TARGET_PATH >
 dst = < LOCAL_DIR_PATH >
 
 download_dir(src, dst)
 ```
 
-<b>SHAREPOINT_BASE_PATH</b>, <b>SHAREPIONT_TARGET_PATH</b>, <b>LOCAL_DIR_PATH</b> See item upload_dir
+<b><i>SHAREPOINT_BASE_PATH</i></b>, <b><i>SHAREPIONT_TARGET_PATH</i></b>, <b><i>LOCAL_DIR_PATH</i></b> See item upload_dir
 
 
 ## Third Party Libraries and Dependencies
 
 [Office365-REST-Python-Client](https://pypi.org/project/Office365-REST-Python-Client/)
```

## Comparing `simple_sharepoint-0.0.3.dist-info/RECORD` & `simple_sharepoint-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-simple_sharepoint/__init__.py,sha256=kQOJvtmpbHGE0oVJv6oubUfigE6lAOQFBGPyh3SkWZI,21
+simple_sharepoint/__init__.py,sha256=Qkdiz6Ybn1PE1SlWhKAQBmETf7pQ0yr5HmkqLVDxsqE,21
 simple_sharepoint/client.py,sha256=Dj6AF-ou9StogucoxtGjlaJiNYFUhZAT6VxY2KLSwF0,3269
 simple_sharepoint/sharepoint.py,sha256=Dj6AF-ou9StogucoxtGjlaJiNYFUhZAT6VxY2KLSwF0,3269
-simple_sharepoint-0.0.3.dist-info/METADATA,sha256=65mLhkbgRFRtn2T2oZn2F2s6GvE7SZoVeTDXsI-8W_U,3831
-simple_sharepoint-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simple_sharepoint-0.0.3.dist-info/top_level.txt,sha256=OKT7wofvYfR9RTWMF85SbimTyz2ze7zwkCxMzuxgmv4,18
-simple_sharepoint-0.0.3.dist-info/RECORD,,
+simple_sharepoint-0.0.4.dist-info/METADATA,sha256=yo2tzmgPLecY0PNW3I9zPKvTuB-9z-ZjIGTQ_W_ynZY,3924
+simple_sharepoint-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simple_sharepoint-0.0.4.dist-info/top_level.txt,sha256=OKT7wofvYfR9RTWMF85SbimTyz2ze7zwkCxMzuxgmv4,18
+simple_sharepoint-0.0.4.dist-info/RECORD,,
```

