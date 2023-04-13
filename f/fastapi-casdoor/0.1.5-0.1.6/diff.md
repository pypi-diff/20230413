# Comparing `tmp/fastapi_casdoor-0.1.5-py3.8.egg` & `tmp/fastapi_casdoor-0.1.6-py3.8.egg`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 902 bytes, number of entries: 5
--rw-r--r--  2.0 unx      284 b- defN 23-Apr-13 12:02 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      174 b- defN 23-Apr-13 12:02 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:02 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:02 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:02 EGG-INFO/zip-safe
-5 files, 461 bytes uncompressed, 290 bytes compressed:  37.1%
+Zip file size: 1479 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1338 b- defN 23-Apr-13 12:32 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      250 b- defN 23-Apr-13 12:32 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       44 b- defN 23-Apr-13 12:32 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/zip-safe
+6 files, 1635 bytes uncompressed, 749 bytes compressed:  54.2%
```

## zipnote «TEMP»/diffoscope_fsizqor4_/tmpvo8dam9k_.zip

```diff
@@ -3,14 +3,17 @@
 
 Filename: EGG-INFO/SOURCES.txt
 Comment: 
 
 Filename: EGG-INFO/dependency_links.txt
 Comment: 
 
+Filename: EGG-INFO/requires.txt
+Comment: 
+
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,45 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: fastapi-casdoor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Integration Casdoor with FastAPI
 Home-page: https://github.com/winrey/python-fastapi-casdoor
-Author: winrey
+Author: Winrey
 Author-email: i@iaside.com
-License: MIT Licence
-Description: Integration Casdoor with FastAPI
-Platform: any
+License: UNKNOWN
+Description: # fastAPI Casdoor
+        Integration Casdoor with FastAPI
+        
+        ## Installation
+        
+        ```bash
+        pip install fastapi-casdoor
+        ```
+        
+        ## Usage
+        
+        ```python
+        from typing import Annotated, Depends
+        from fastapi import FastAPI
+        from fastapi_casdoor.deps import get_current_user
+        from fastapi_casdoor.models import User
+        
+        
+        @app.get("/")
+        async def root(user: Annotated[User, Depends(get_current_user)]):
+            return {
+                "user": user,
+            }
+        ```
+        
+Keywords: auth,casdoor,fastapi,dependency
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,6 +1,9 @@
+LICENSE
 README.md
+setup.cfg
 setup.py
-fastapi_casdoor.egg-info/PKG-INFO
-fastapi_casdoor.egg-info/SOURCES.txt
-fastapi_casdoor.egg-info/dependency_links.txt
-fastapi_casdoor.egg-info/top_level.txt
+src/fastapi_casdoor.egg-info/PKG-INFO
+src/fastapi_casdoor.egg-info/SOURCES.txt
+src/fastapi_casdoor.egg-info/dependency_links.txt
+src/fastapi_casdoor.egg-info/requires.txt
+src/fastapi_casdoor.egg-info/top_level.txt
```

