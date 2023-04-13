# Comparing `tmp/tpds_manifest-1.0.3-py3-none-any.whl.zip` & `tmp/tpds_manifest-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4336 bytes, number of entries: 8
--rw-r--r--  2.0 unx       65 b- defN 23-Mar-10 16:13 tpds/__init__.py
--rw-r--r--  2.0 unx      147 b- defN 23-Mar-10 16:13 tpds/packages/__init__.py
--rw-r--r--  2.0 unx     3445 b- defN 23-Mar-10 16:13 tpds/packages/packages.yaml
--rw-r--r--  2.0 unx     1322 b- defN 23-Mar-10 16:14 tpds_manifest-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2191 b- defN 23-Mar-10 16:14 tpds_manifest-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-10 16:14 tpds_manifest-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-10 16:14 tpds_manifest-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Mar-10 16:14 tpds_manifest-1.0.3.dist-info/RECORD
-8 files, 7918 bytes uncompressed, 3192 bytes compressed:  59.7%
+Zip file size: 4351 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       65 b- defN 23-Apr-13 16:59 tpds/__init__.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Apr-13 16:59 tpds/packages/__init__.py
+-rw-r--r--  2.0 unx     3608 b- defN 23-Apr-13 16:59 tpds/packages/packages.yaml
+-rw-r--r--  2.0 unx     1322 b- defN 23-Apr-13 17:00 tpds_manifest-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2191 b- defN 23-Apr-13 17:00 tpds_manifest-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 17:00 tpds_manifest-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-13 17:00 tpds_manifest-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-Apr-13 17:00 tpds_manifest-1.0.4.dist-info/RECORD
+8 files, 8081 bytes uncompressed, 3207 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: tpds/packages/__init__.py
 Comment: 
 
 Filename: tpds/packages/packages.yaml
 Comment: 
 
-Filename: tpds_manifest-1.0.3.dist-info/LICENSE
+Filename: tpds_manifest-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: tpds_manifest-1.0.3.dist-info/METADATA
+Filename: tpds_manifest-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: tpds_manifest-1.0.3.dist-info/WHEEL
+Filename: tpds_manifest-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: tpds_manifest-1.0.3.dist-info/top_level.txt
+Filename: tpds_manifest-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tpds_manifest-1.0.3.dist-info/RECORD
+Filename: tpds_manifest-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpds/packages/packages.yaml

```diff
@@ -123,7 +123,13 @@
         - tpds-extension-ta010-support
 
   tpds-extension-ecc204-support:
     description: "Microchip(SPG) Trust Platform - ECC204 Device Support"
     source:
       pypi:
         - tpds-extension-ecc204-support
+
+  tpds-extension-secureboot:
+    description: "Microchip(SPG) Trust Platform - ECC204 Device Support"
+    source:
+      pypi:
+        - tpds-extension-secureboot
```

## Comparing `tpds_manifest-1.0.3.dist-info/LICENSE` & `tpds_manifest-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpds_manifest-1.0.3.dist-info/METADATA` & `tpds_manifest-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpds-manifest
-Version: 1.0.3
+Version: 1.0.4
 Summary: Microchip(SPG) Trust Platform Approved Package List
 Maintainer-email: Microchip Technology <SPG.Tools@microchip.com>
 License: (c) 2015-2023 Microchip Technology Inc. and its subsidiaries.
         
         Subject to your compliance with these terms, you may use the Microchip Software
         and any derivatives exclusively with Microchip products. It is your
         responsibility to comply with third party license terms applicable to your
```

## Comparing `tpds_manifest-1.0.3.dist-info/RECORD` & `tpds_manifest-1.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 tpds/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 tpds/packages/__init__.py,sha256=9k_fIxiyh_h0ny4zratu79y9cCHY5N2mNBBgdY-iF-E,147
-tpds/packages/packages.yaml,sha256=iS3C-lasHtQNpS7mEQculu9YTr8r9jnI00z3Utp30sU,3445
-tpds_manifest-1.0.3.dist-info/LICENSE,sha256=F_itoJVw8BueLDyZXyIPzgH_thxrjAGZ9vasLzVc19I,1322
-tpds_manifest-1.0.3.dist-info/METADATA,sha256=qZqYhTq-mpF4pA941Y1ASqpeCxku-qNNtpC1_3JNeqc,2191
-tpds_manifest-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tpds_manifest-1.0.3.dist-info/top_level.txt,sha256=Tl4GsItOlkTwS5kMrk7oOjlZsRztkeFRTneAJ5ZBOjQ,5
-tpds_manifest-1.0.3.dist-info/RECORD,,
+tpds/packages/packages.yaml,sha256=N43XnPhynJDFNBcSc1Fk8SkC8on_OmmpFenKjMEWzTM,3608
+tpds_manifest-1.0.4.dist-info/LICENSE,sha256=F_itoJVw8BueLDyZXyIPzgH_thxrjAGZ9vasLzVc19I,1322
+tpds_manifest-1.0.4.dist-info/METADATA,sha256=AXNlBI9OqVXUmm0AHq6kS4Exb632A1lod2xVzvtfZM8,2191
+tpds_manifest-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tpds_manifest-1.0.4.dist-info/top_level.txt,sha256=Tl4GsItOlkTwS5kMrk7oOjlZsRztkeFRTneAJ5ZBOjQ,5
+tpds_manifest-1.0.4.dist-info/RECORD,,
```

