# Comparing `tmp/sdkpoc-1.0-py3-none-any.whl.zip` & `tmp/sdkpoc-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1761 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-13 09:16 example/__init__.py
--rw-rw-r--  2.0 unx      519 b- defN 23-Apr-13 11:26 example/example.py
--rw-rw-r--  2.0 unx      449 b- defN 23-Apr-13 11:53 sdkpoc-1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 11:53 sdkpoc-1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-13 11:53 sdkpoc-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      432 b- defN 23-Apr-13 11:53 sdkpoc-1.0.dist-info/RECORD
-6 files, 1516 bytes uncompressed, 977 bytes compressed:  35.6%
+Zip file size: 1758 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-13 12:29 example/__init__.py
+-rw-rw-r--  2.0 unx      519 b- defN 23-Apr-13 12:25 example/example.py
+-rw-rw-r--  2.0 unx      449 b- defN 23-Apr-13 12:29 sdkpoc-1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 12:29 sdkpoc-1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-13 12:29 sdkpoc-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      432 b- defN 23-Apr-13 12:29 sdkpoc-1.1.dist-info/RECORD
+6 files, 1515 bytes uncompressed, 974 bytes compressed:  35.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: example/__init__.py
 Comment: 
 
 Filename: example/example.py
 Comment: 
 
-Filename: sdkpoc-1.0.dist-info/METADATA
+Filename: sdkpoc-1.1.dist-info/METADATA
 Comment: 
 
-Filename: sdkpoc-1.0.dist-info/WHEEL
+Filename: sdkpoc-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sdkpoc-1.0.dist-info/top_level.txt
+Filename: sdkpoc-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sdkpoc-1.0.dist-info/RECORD
+Filename: sdkpoc-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## example/__init__.py

```diff
@@ -1 +1 @@
-name = "example"
+name = "sdkpoc"
```

