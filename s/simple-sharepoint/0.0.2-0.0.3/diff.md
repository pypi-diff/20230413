# Comparing `tmp/simple_sharepoint-0.0.2-py3-none-any.whl.zip` & `tmp/simple_sharepoint-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3986 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 07:55 simple_sharepoint/__init__.py
+Zip file size: 4862 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-13 09:22 simple_sharepoint/__init__.py
 -rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/client.py
 -rw-rw-rw-  2.0 fat     3269 b- defN 23-Apr-13 06:33 simple_sharepoint/sharepoint.py
--rw-rw-rw-  2.0 fat      795 b- defN 23-Apr-13 07:55 simple_sharepoint-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 07:55 simple_sharepoint-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 07:55 simple_sharepoint-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      593 b- defN 23-Apr-13 07:55 simple_sharepoint-0.0.2.dist-info/RECORD
-7 files, 8057 bytes uncompressed, 2922 bytes compressed:  63.7%
+-rw-rw-rw-  2.0 fat     3831 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      594 b- defN 23-Apr-13 09:22 simple_sharepoint-0.0.3.dist-info/RECORD
+7 files, 11094 bytes uncompressed, 3798 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: simple_sharepoint/client.py
 Comment: 
 
 Filename: simple_sharepoint/sharepoint.py
 Comment: 
 
-Filename: simple_sharepoint-0.0.2.dist-info/METADATA
+Filename: simple_sharepoint-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: simple_sharepoint-0.0.2.dist-info/WHEEL
+Filename: simple_sharepoint-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: simple_sharepoint-0.0.2.dist-info/top_level.txt
+Filename: simple_sharepoint-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_sharepoint-0.0.2.dist-info/RECORD
+Filename: simple_sharepoint-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_sharepoint/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.2'
+__version__ = '0.0.3'
```

## Comparing `simple_sharepoint-0.0.2.dist-info/RECORD` & `simple_sharepoint-0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-simple_sharepoint/__init__.py,sha256=ZkJ4YFnqff5CwHnqUupPsAVatqD4aozkrh1u-iQrvMc,21
+simple_sharepoint/__init__.py,sha256=kQOJvtmpbHGE0oVJv6oubUfigE6lAOQFBGPyh3SkWZI,21
 simple_sharepoint/client.py,sha256=Dj6AF-ou9StogucoxtGjlaJiNYFUhZAT6VxY2KLSwF0,3269
 simple_sharepoint/sharepoint.py,sha256=Dj6AF-ou9StogucoxtGjlaJiNYFUhZAT6VxY2KLSwF0,3269
-simple_sharepoint-0.0.2.dist-info/METADATA,sha256=v17wZwE23axLKRMg8Uu3EwqYxEM0HYMKqADELBgcHPI,795
-simple_sharepoint-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simple_sharepoint-0.0.2.dist-info/top_level.txt,sha256=OKT7wofvYfR9RTWMF85SbimTyz2ze7zwkCxMzuxgmv4,18
-simple_sharepoint-0.0.2.dist-info/RECORD,,
+simple_sharepoint-0.0.3.dist-info/METADATA,sha256=65mLhkbgRFRtn2T2oZn2F2s6GvE7SZoVeTDXsI-8W_U,3831
+simple_sharepoint-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simple_sharepoint-0.0.3.dist-info/top_level.txt,sha256=OKT7wofvYfR9RTWMF85SbimTyz2ze7zwkCxMzuxgmv4,18
+simple_sharepoint-0.0.3.dist-info/RECORD,,
```

