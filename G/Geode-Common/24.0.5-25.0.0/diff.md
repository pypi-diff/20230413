# Comparing `tmp/Geode_Common-24.0.5-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Common-25.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 4148 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      261 b- defN 23-Apr-13 08:22 geode_common/__init__.py
--rw-rw-rw-  2.0 fat      161 b- defN 23-Apr-13 08:22 geode_common/core.py
--rw-rw-rw-  2.0 fat      176 b- defN 23-Apr-13 08:22 geode_common/cutter_solid.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Apr-13 08:22 geode_common/cutter_surface.py
--rw-rw-rw-  2.0 fat      191 b- defN 23-Apr-13 08:22 geode_common/modifier_edged_curve.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Apr-13 08:22 geode_common/modifier_model.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Apr-13 08:22 geode_common/modifier_solid.py
--rw-rw-rw-  2.0 fat      184 b- defN 23-Apr-13 08:22 geode_common/modifier_surface.py
--rw-rw-rw-  2.0 fat     1813 b- defN 23-Apr-13 08:24 Geode_Common-24.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 08:24 Geode_Common-24.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-13 08:24 Geode_Common-24.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1001 b- defN 23-Apr-13 08:24 Geode_Common-24.0.5.dist-info/RECORD
-12 files, 4440 bytes uncompressed, 2450 bytes compressed:  44.8%
+Zip file size: 4185 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      261 b- defN 23-Apr-13 12:09 geode_common/__init__.py
+-rw-rw-rw-  2.0 fat      168 b- defN 23-Apr-13 12:09 geode_common/core.py
+-rw-rw-rw-  2.0 fat      183 b- defN 23-Apr-13 12:09 geode_common/cutter_solid.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-13 12:09 geode_common/cutter_surface.py
+-rw-rw-rw-  2.0 fat      198 b- defN 23-Apr-13 12:09 geode_common/modifier_edged_curve.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-13 12:09 geode_common/modifier_model.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-13 12:09 geode_common/modifier_solid.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Apr-13 12:09 geode_common/modifier_surface.py
+-rw-rw-rw-  2.0 fat     1812 b- defN 23-Apr-13 12:11 Geode_Common-25.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 12:11 Geode_Common-25.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-13 12:11 Geode_Common-25.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1001 b- defN 23-Apr-13 12:11 Geode_Common-25.0.0.dist-info/RECORD
+12 files, 4488 bytes uncompressed, 2487 bytes compressed:  44.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_common/modifier_solid.py
 Comment: 
 
 Filename: geode_common/modifier_surface.py
 Comment: 
 
-Filename: Geode_Common-24.0.5.dist-info/METADATA
+Filename: Geode_Common-25.0.0.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Common-24.0.5.dist-info/WHEEL
+Filename: Geode_Common-25.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Common-24.0.5.dist-info/top_level.txt
+Filename: Geode_Common-25.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Common-24.0.5.dist-info/RECORD
+Filename: Geode_Common-25.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_common/core.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_core import *
-CommonCore.initialize()
+CommonCoreLibrary.initialize()
```

## geode_common/cutter_solid.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_cutter_solid import *
-CommonCutterSolid.initialize()
+CommonCutterSolidLibrary.initialize()
```

## geode_common/cutter_surface.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_cutter_surface import *
-CommonCutterSurface.initialize()
+CommonCutterSurfaceLibrary.initialize()
```

## geode_common/modifier_edged_curve.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_modifier_edged_curve import *
-CommonModifierEdgedCurve.initialize()
+CommonModifierEdgedCurveLibrary.initialize()
```

## geode_common/modifier_model.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_modifier_model import *
-CommonModifierModel.initialize()
+CommonModifierModelLibrary.initialize()
```

## geode_common/modifier_solid.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_modifier_solid import *
-CommonModifierSolid.initialize()
+CommonModifierSolidLibrary.initialize()
```

## geode_common/modifier_surface.py

```diff
@@ -1,8 +1,8 @@
 #
 # Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
 #
 
 import opengeode
 
 from .bin.geode_common_py_modifier_surface import *
-CommonModifierSurface.initialize()
+CommonModifierSurfaceLibrary.initialize()
```

## Comparing `Geode_Common-24.0.5.dist-info/METADATA` & `Geode_Common-25.0.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Geode-Common
-Version: 24.0.5
+Version: 25.0.0
 Summary: Common module for licensed Geode-solutions modules
 Home-page: https://github.com/Geode-solutions/Geode-Common
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==13.*,>=13.4.15)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
 
 <h1 align="center">Geode-Common<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Common module for proprietary Geode-solutions modules</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Common_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Common_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: Geode-Common Version: 24.0.5 Summary: Common module
+Metadata-Version: 2.1 Name: Geode-Common Version: 25.0.0 Summary: Common module
 for licensed Geode-solutions modules Home-page: https://github.com/Geode-
 solutions/Geode-Common Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: opengeode-core (==13.*,>=13.4.15)
+text/markdown Requires-Dist: opengeode-core (==14.*,>=14.0.0)
                  ****** Geode-Commonby Geode-solutions ******
         **** Common module for proprietary Geode-solutions modules ****
                 [Build Status] [Deploy Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
                  [Language] [Semantic-release] [Slack_invite]
```

