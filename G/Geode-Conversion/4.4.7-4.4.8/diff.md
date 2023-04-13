# Comparing `tmp/Geode_Conversion-4.4.7-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-4.4.8-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 2839 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-07 12:40 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat       85 b- defN 23-Apr-07 12:41 geode_conversion/geode_conversion.py
--rw-rw-rw-  2.0 fat      197 b- defN 23-Apr-07 12:41 geode_conversion/geode_conversion_model.py
--rw-rw-rw-  2.0 fat      198 b- defN 23-Apr-07 12:40 geode_conversion/model.py
--rw-rw-rw-  2.0 fat     1952 b- defN 23-Apr-07 12:41 Geode_Conversion-4.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-07 12:41 Geode_Conversion-4.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-07 12:41 Geode_Conversion-4.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      688 b- defN 23-Apr-07 12:41 Geode_Conversion-4.4.7.dist-info/RECORD
-8 files, 3307 bytes uncompressed, 1619 bytes compressed:  51.0%
+Zip file size: 2267 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-13 08:46 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-13 08:46 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat     2049 b- defN 23-Apr-13 08:47 Geode_Conversion-4.4.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 08:47 Geode_Conversion-4.4.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-13 08:47 Geode_Conversion-4.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      499 b- defN 23-Apr-13 08:47 Geode_Conversion-4.4.8.dist-info/RECORD
+6 files, 2927 bytes uncompressed, 1355 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
-Filename: geode_conversion/geode_conversion.py
-Comment: 
-
-Filename: geode_conversion/geode_conversion_model.py
-Comment: 
-
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: Geode_Conversion-4.4.7.dist-info/METADATA
+Filename: Geode_Conversion-4.4.8.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-4.4.7.dist-info/WHEEL
+Filename: Geode_Conversion-4.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-4.4.7.dist-info/top_level.txt
+Filename: Geode_Conversion-4.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-4.4.7.dist-info/RECORD
+Filename: Geode_Conversion-4.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/model.py

```diff
@@ -1,9 +1,9 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
-from geode_common import core
+import geode_common
 
-from .geode_conversion_py_model import *
+from .bin.geode_conversion_py_model import *
 ConversionModel.initialize()
```

## Comparing `Geode_Conversion-4.4.7.dist-info/METADATA` & `Geode_Conversion-4.4.8.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 4.4.7
+Version: 4.4.8
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: geode-common (==24.*,>=24.0.5)
+Requires-Dist: opengeode-core (==13.*,>=13.4.15)
 
 <h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Conversion OpenGeode module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 4.4.7 Summary: Conversion
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 4.4.8 Summary: Conversion
 module for Geode-solutions OpenGeode modules Home-page: https://github.com/
 Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown
+Content-Type: text/markdown Requires-Dist: geode-common (==24.*,>=24.0.5)
+Requires-Dist: opengeode-core (==13.*,>=13.4.15)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

