# Comparing `tmp/fastapi_casdoor-0.1.7-py3.8.egg` & `tmp/fastapi_casdoor-0.1.8-py3.10.egg`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1476 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1338 b- defN 23-Apr-13 12:38 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      250 b- defN 23-Apr-13 12:38 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       39 b- defN 23-Apr-13 12:38 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/zip-safe
-6 files, 1630 bytes uncompressed, 746 bytes compressed:  54.2%
+Zip file size: 1465 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1152 b- defN 23-Apr-13 23:06 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      250 b- defN 23-Apr-13 23:06 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 23:06 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       39 b- defN 23-Apr-13 23:06 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 23:06 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 23:06 EGG-INFO/zip-safe
+6 files, 1444 bytes uncompressed, 735 bytes compressed:  49.1%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: fastapi-casdoor
-Version: 0.1.7
+Version: 0.1.8
 Summary: Integration Casdoor with FastAPI
 Home-page: https://github.com/winrey/python-fastapi-casdoor
 Author: Winrey
 Author-email: i@iaside.com
-License: UNKNOWN
-Description: # fastAPI Casdoor
-        Integration Casdoor with FastAPI
-        
-        ## Installation
-        
-        ```bash
-        pip install fastapi-casdoor
-        ```
-        
-        ## Usage
-        
-        ```python
-        from typing import Annotated, Depends
-        from fastapi import FastAPI
-        from fastapi_casdoor.deps import get_current_user
-        from fastapi_casdoor.models import User
-        
-        
-        @app.get("/")
-        async def root(user: Annotated[User, Depends(get_current_user)]):
-            return {
-                "user": user,
-            }
-        ```
-        
 Keywords: auth,casdoor,fastapi,dependency
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: FastAPI
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fastAPI Casdoor
+Integration Casdoor with FastAPI
+
+## Installation
+
+```bash
+pip install fastapi-casdoor
+```
+
+## Usage
+
+```python
+from typing import Annotated, Depends
+from fastapi import FastAPI
+from fastapi_casdoor.deps import get_current_user
+from fastapi_casdoor.models import User
+
+
+@app.get("/")
+async def root(user: Annotated[User, Depends(get_current_user)]):
+    return {
+        "user": user,
+    }
+```
```

