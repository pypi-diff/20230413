# Comparing `tmp/xia_api_flask-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_api_flask-0.1.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 171981 bytes, number of entries: 7
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 06:41 xia_api_flask/__init__.py
--rw-r--r--  2.0 unx   450560 b- defN 23-Mar-12 09:03 xia_api_flask/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-12 09:03 xia_api_flask-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      737 b- defN 23-Mar-12 09:03 xia_api_flask-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-12 09:03 xia_api_flask-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-12 09:03 xia_api_flask-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      594 b- defN 23-Mar-12 09:03 xia_api_flask-0.1.7.dist-info/RECORD
-7 files, 452248 bytes uncompressed, 170917 bytes compressed:  62.2%
+Zip file size: 171983 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 07:56 xia_api_flask/__init__.py
+-rw-r--r--  2.0 unx   450560 b- defN 23-Apr-13 07:59 xia_api_flask/rest.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      737 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      594 b- defN 23-Apr-13 07:59 xia_api_flask-0.1.8.dist-info/RECORD
+7 files, 452248 bytes uncompressed, 170919 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_api_flask/__init__.py
 Comment: 
 
 Filename: xia_api_flask/rest.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_api_flask-0.1.7.dist-info/LICENSE.txt
+Filename: xia_api_flask-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.7.dist-info/METADATA
+Filename: xia_api_flask-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_api_flask-0.1.7.dist-info/WHEEL
+Filename: xia_api_flask-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api_flask-0.1.7.dist-info/top_level.txt
+Filename: xia_api_flask-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.7.dist-info/RECORD
+Filename: xia_api_flask-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_api_flask.rest import Restful
 
 __all__ = [
     "Restful",
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_api_flask-0.1.7.dist-info/METADATA` & `xia_api_flask-0.1.8.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api-flask
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_api_flask-0.1.7.dist-info/RECORD` & `xia_api_flask-0.1.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_api_flask/__init__.py,sha256=CH5xe5xy1PX-V80-lxL_BoxuItyt3Ee8hzSu8O3Q0fU,92
-xia_api_flask/rest.cp39-win_amd64.pyd,sha256=Ux6QsV7LUincJ7niwifTaTa7xwoT8sk15_TVZLMckA8,450560
-xia_api_flask-0.1.7.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
-xia_api_flask-0.1.7.dist-info/METADATA,sha256=eRQ80bP7KHVAIQc_cGjccrpibeO683duWA8ipV02HK4,737
-xia_api_flask-0.1.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_api_flask-0.1.7.dist-info/top_level.txt,sha256=riUnMW32w4zoQkF1U4a8gVUOwFM03-zYNtfKi8tzG6c,14
-xia_api_flask-0.1.7.dist-info/RECORD,,
+xia_api_flask/__init__.py,sha256=LXs0HhaaEPNod7VJ0k96qUspJ1LKTaShkQ-yL5PZ_ok,92
+xia_api_flask/rest.cp39-win_amd64.pyd,sha256=kFKP9LG8X4xJUwWL44MTf55q5smUDq0lyT6QZs8kQ4w,450560
+xia_api_flask-0.1.8.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
+xia_api_flask-0.1.8.dist-info/METADATA,sha256=TiiDssftT_aMQ3e5va_4ry7ssxsVhr_Yx6JuDShvMAk,737
+xia_api_flask-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_api_flask-0.1.8.dist-info/top_level.txt,sha256=riUnMW32w4zoQkF1U4a8gVUOwFM03-zYNtfKi8tzG6c,14
+xia_api_flask-0.1.8.dist-info/RECORD,,
```

