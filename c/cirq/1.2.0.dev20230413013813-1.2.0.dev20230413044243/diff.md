# Comparing `tmp/cirq-1.2.0.dev20230413013813-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230413044243-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7973 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 01:38 cirq-1.2.0.dev20230413013813.dist-info/LICENSE
--rw-r--r--  2.0 unx     7773 b- defN 23-Apr-13 01:38 cirq-1.2.0.dev20230413013813.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 01:38 cirq-1.2.0.dev20230413013813.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 01:38 cirq-1.2.0.dev20230413013813.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      461 b- defN 23-Apr-13 01:38 cirq-1.2.0.dev20230413013813.dist-info/RECORD
-5 files, 19684 bytes uncompressed, 7103 bytes compressed:  63.9%
+Zip file size: 7970 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 04:42 cirq-1.2.0.dev20230413044243.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7771 b- defN 23-Apr-13 04:42 cirq-1.2.0.dev20230413044243.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 04:42 cirq-1.2.0.dev20230413044243.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-13 04:42 cirq-1.2.0.dev20230413044243.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      461 b- defN 23-Apr-13 04:42 cirq-1.2.0.dev20230413044243.dist-info/RECORD
+5 files, 19682 bytes uncompressed, 7100 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: cirq-1.2.0.dev20230413013813.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230413044243.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230413013813.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230413044243.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230413013813.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230413044243.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230413013813.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230413044243.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230413013813.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230413044243.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230413013813.dist-info/LICENSE` & `cirq-1.2.0.dev20230413044243.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230413013813.dist-info/METADATA` & `cirq-1.2.0.dev20230413044243.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230413013813
+Version: 1.2.0.dev20230413044243
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-core (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-google (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230413013813)
-Requires-Dist: cirq-web (==1.2.0.dev20230413013813)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-core (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-google (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230413044243)
+Requires-Dist: cirq-web (==1.2.0.dev20230413044243)
 Provides-Extra: dev_env
-Requires-Dist: mypy (==0.961.0) ; extra == 'dev_env'
+Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
 Requires-Dist: pytest ; extra == 'dev_env'
 Requires-Dist: pytest-asyncio ; extra == 'dev_env'
 Requires-Dist: pytest-cov ; extra == 'dev_env'
```

