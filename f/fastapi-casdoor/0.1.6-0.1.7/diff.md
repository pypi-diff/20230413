# Comparing `tmp/fastapi_casdoor-0.1.6-py3.8.egg` & `tmp/fastapi_casdoor-0.1.7-py3.8.egg`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1479 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1338 b- defN 23-Apr-13 12:32 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      250 b- defN 23-Apr-13 12:32 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       44 b- defN 23-Apr-13 12:32 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:32 EGG-INFO/zip-safe
-6 files, 1635 bytes uncompressed, 749 bytes compressed:  54.2%
+Zip file size: 1476 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1338 b- defN 23-Apr-13 12:38 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      250 b- defN 23-Apr-13 12:38 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       39 b- defN 23-Apr-13 12:38 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 12:38 EGG-INFO/zip-safe
+6 files, 1630 bytes uncompressed, 746 bytes compressed:  54.2%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-casdoor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Integration Casdoor with FastAPI
 Home-page: https://github.com/winrey/python-fastapi-casdoor
 Author: Winrey
 Author-email: i@iaside.com
 License: UNKNOWN
 Description: # fastAPI Casdoor
         Integration Casdoor with FastAPI
```

## EGG-INFO/requires.txt

```diff
@@ -1,4 +1,4 @@
-fastapi[all]
+fastapi
 python-dateutil
-pyjwt
+PyJWT
 pydantic
```

