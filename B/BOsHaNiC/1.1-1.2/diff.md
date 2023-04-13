# Comparing `tmp/BOsHaNiC-1.1-py3-none-any.whl.zip` & `tmp/BOsHaNiC-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 1326 bytes, number of entries: 6
--rw-r--r--  2.0 unx       29 b- defN 23-Apr-13 16:27 calculator/__init__.py
--rw-r--r--  2.0 unx       39 b- defN 23-Apr-13 16:26 calculator/adder.py
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-13 16:30 BOsHaNiC-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 16:30 BOsHaNiC-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-13 16:30 BOsHaNiC-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      443 b- defN 23-Apr-13 16:30 BOsHaNiC-1.1.dist-info/RECORD
-6 files, 665 bytes uncompressed, 518 bytes compressed:  22.1%
+Zip file size: 1149 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-13 16:42 calculator/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-13 16:45 BOsHaNiC-1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 16:45 BOsHaNiC-1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-13 16:45 BOsHaNiC-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      369 b- defN 23-Apr-13 16:45 BOsHaNiC-1.2.dist-info/RECORD
+5 files, 599 bytes uncompressed, 455 bytes compressed:  24.0%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
 Filename: calculator/__init__.py
 Comment: 
 
-Filename: calculator/adder.py
+Filename: BOsHaNiC-1.2.dist-info/METADATA
 Comment: 
 
-Filename: BOsHaNiC-1.1.dist-info/METADATA
+Filename: BOsHaNiC-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: BOsHaNiC-1.1.dist-info/WHEEL
+Filename: BOsHaNiC-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: BOsHaNiC-1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: BOsHaNiC-1.1.dist-info/RECORD
+Filename: BOsHaNiC-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## calculator/__init__.py

```diff
@@ -1 +1,5 @@
-from adder import add_numbers
+def add_numbers(a, b):
+    return a+b
+
+def sub_numbers(a, b):
+    return a-b
```

