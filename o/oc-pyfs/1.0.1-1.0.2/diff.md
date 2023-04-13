# Comparing `tmp/oc_pyfs-1.0.1-py3-none-any.whl.zip` & `tmp/oc_pyfs-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13320 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5133 b- defN 23-Apr-13 08:18 oc_pyfs/NexusFS.py
--rw-r--r--  2.0 unx    19280 b- defN 23-Apr-13 08:18 oc_pyfs/SvnFS.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 08:18 oc_pyfs/__init__.py
--rw-r--r--  2.0 unx      318 b- defN 23-Apr-13 08:18 oc_pyfs/fs_utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 08:18 oc_pyfs-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      268 b- defN 23-Apr-13 08:18 oc_pyfs-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 08:18 oc_pyfs-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-13 08:18 oc_pyfs-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      682 b- defN 23-Apr-13 08:18 oc_pyfs-1.0.1.dist-info/RECORD
-9 files, 37138 bytes uncompressed, 12152 bytes compressed:  67.3%
+Zip file size: 13330 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5133 b- defN 23-Apr-13 08:41 oc_pyfs/NexusFS.py
+-rw-r--r--  2.0 unx    19280 b- defN 23-Apr-13 08:41 oc_pyfs/SvnFS.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 08:41 oc_pyfs/__init__.py
+-rw-r--r--  2.0 unx      318 b- defN 23-Apr-13 08:41 oc_pyfs/fs_utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 08:41 oc_pyfs-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      280 b- defN 23-Apr-13 08:41 oc_pyfs-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 08:41 oc_pyfs-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-13 08:41 oc_pyfs-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      682 b- defN 23-Apr-13 08:41 oc_pyfs-1.0.2.dist-info/RECORD
+9 files, 37150 bytes uncompressed, 12162 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: oc_pyfs/__init__.py
 Comment: 
 
 Filename: oc_pyfs/fs_utils.py
 Comment: 
 
-Filename: oc_pyfs-1.0.1.dist-info/LICENSE
+Filename: oc_pyfs-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: oc_pyfs-1.0.1.dist-info/METADATA
+Filename: oc_pyfs-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: oc_pyfs-1.0.1.dist-info/WHEEL
+Filename: oc_pyfs-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: oc_pyfs-1.0.1.dist-info/top_level.txt
+Filename: oc_pyfs-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_pyfs-1.0.1.dist-info/RECORD
+Filename: oc_pyfs-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `oc_pyfs-1.0.1.dist-info/LICENSE` & `oc_pyfs-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_pyfs-1.0.1.dist-info/RECORD` & `oc_pyfs-1.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oc_pyfs/NexusFS.py,sha256=rKZ5lnCaXWN84nO_SI7XBm9oTWI-SuFbeQUB4ffLE_k,5133
 oc_pyfs/SvnFS.py,sha256=k9cXgaOVuXLxAZlMuv2F3pEZUNYo3xXDCMQGwuy9kcY,19280
 oc_pyfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oc_pyfs/fs_utils.py,sha256=gKjmDalFTZ18xx4xOUqFmHTH4_akVRijvhOoLR3A8dY,318
-oc_pyfs-1.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_pyfs-1.0.1.dist-info/METADATA,sha256=dazniSpwmBq64Sr90lTjsVKAJE7jFnyD6AVFU3oVqGc,268
-oc_pyfs-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-oc_pyfs-1.0.1.dist-info/top_level.txt,sha256=vZ5zzVDnaBgfX3EA9-Q8zwYoE44R2mcua_w56V-7BTM,8
-oc_pyfs-1.0.1.dist-info/RECORD,,
+oc_pyfs-1.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_pyfs-1.0.2.dist-info/METADATA,sha256=KlnN-XdjpQcLsj2BQN2x41Kcg1Qj3Mk_9IEH3a6lCYA,280
+oc_pyfs-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+oc_pyfs-1.0.2.dist-info/top_level.txt,sha256=vZ5zzVDnaBgfX3EA9-Q8zwYoE44R2mcua_w56V-7BTM,8
+oc_pyfs-1.0.2.dist-info/RECORD,,
```

