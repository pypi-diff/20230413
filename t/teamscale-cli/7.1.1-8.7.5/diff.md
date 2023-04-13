# Comparing `tmp/teamscale_cli-7.1.1-py3-none-any.whl.zip` & `tmp/teamscale_cli-8.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13802 bytes, number of entries: 11
--rw-r--r--  2.0 unx      153 b- defN 20-Apr-21 06:31 teamscale_precommit_client/__init__.py
--rw-r--r--  2.0 unx     2141 b- defN 20-Apr-21 06:31 teamscale_precommit_client/client_configuration_utils.py
--rw-r--r--  2.0 unx      672 b- defN 20-Apr-21 06:31 teamscale_precommit_client/data.py
--rw-r--r--  2.0 unx     5509 b- defN 22-Oct-20 07:34 teamscale_precommit_client/git_utils.py
--rw-r--r--  2.0 unx    19455 b- defN 22-Oct-20 07:34 teamscale_precommit_client/precommit_client.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      554 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       82 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1014 b- defN 22-Oct-20 07:52 teamscale_cli-7.1.1.dist-info/RECORD
-11 files, 41056 bytes uncompressed, 12048 bytes compressed:  70.7%
+Zip file size: 13809 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      153 b- defN 23-Apr-12 09:15 teamscale_precommit_client/__init__.py
+-rw-r--r--  2.0 unx     2141 b- defN 23-Apr-12 09:15 teamscale_precommit_client/client_configuration_utils.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Apr-12 09:15 teamscale_precommit_client/data.py
+-rw-r--r--  2.0 unx     5509 b- defN 23-Apr-12 09:15 teamscale_precommit_client/git_utils.py
+-rw-r--r--  2.0 unx    19455 b- defN 23-Apr-12 09:15 teamscale_precommit_client/precommit_client.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      554 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       82 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1014 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/RECORD
+11 files, 41056 bytes uncompressed, 12055 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: teamscale_precommit_client/git_utils.py
 Comment: 
 
 Filename: teamscale_precommit_client/precommit_client.py
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/LICENSE
+Filename: teamscale_cli-8.7.5.dist-info/LICENSE
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/METADATA
+Filename: teamscale_cli-8.7.5.dist-info/METADATA
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/WHEEL
+Filename: teamscale_cli-8.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/entry_points.txt
+Filename: teamscale_cli-8.7.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/top_level.txt
+Filename: teamscale_cli-8.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: teamscale_cli-7.1.1.dist-info/RECORD
+Filename: teamscale_cli-8.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `teamscale_cli-7.1.1.dist-info/LICENSE` & `teamscale_cli-8.7.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teamscale_cli-7.1.1.dist-info/METADATA` & `teamscale_cli-8.7.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: teamscale-cli
-Version: 7.1.1
+Version: 8.7.5
 Summary: Client for performing precommit analysis with Teamscale.
 Home-page: https://github.com/cqse/teamscale-cli
 Author: Thomas Kinnen - CQSE GmbH
 Author-email: kinnen@cqse.eu
 License: Apache
 Keywords: teamscale client precommit
 Classifier: Topic :: Utilities
 License-File: LICENSE
 Requires-Dist: teamscale-client (==7.1.1)
-Requires-Dist: gitpython (==2.1.15)
+Requires-Dist: gitpython (==3.1.30)
 Requires-Dist: gitdb2 (==2.0.6)
-Requires-Dist: nuitka (==1.1.5)
+Requires-Dist: nuitka (==1.5.5)
 
 Command line client for performing precommit analysis with Teamscale.
```

## Comparing `teamscale_cli-7.1.1.dist-info/RECORD` & `teamscale_cli-8.7.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 teamscale_precommit_client/__init__.py,sha256=4bzI44HpaakS-k3GJRRTChWa3IItRdskdnoAYBc85bA,153
 teamscale_precommit_client/client_configuration_utils.py,sha256=KYJabL7c8KcliLGKAJePrm49XN7M_b22-juiiX8e8Qg,2141
 teamscale_precommit_client/data.py,sha256=IqmRM1qT2azP1YR9Q569Q7Rt7sLoMC1C9kpOvF9s9kA,672
 teamscale_precommit_client/git_utils.py,sha256=WeYBVtOtQtyf0RwyUsW6PppVS5gFzqUtjVAzURR79PU,5509
 teamscale_precommit_client/precommit_client.py,sha256=krc-mQkMGzeC4hUaVP3NggPU9U9n2rv4WU6Tpni0r_M,19455
-teamscale_cli-7.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-teamscale_cli-7.1.1.dist-info/METADATA,sha256=5FwV1tQKq2x1R2iyqNPlNdC0r3o7ZxMT89q6N1iEf_0,554
-teamscale_cli-7.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-teamscale_cli-7.1.1.dist-info/entry_points.txt,sha256=fhhE5zS36olRi97D3CYpIMHJzA5RUmFXzfBCvZnBCrQ,82
-teamscale_cli-7.1.1.dist-info/top_level.txt,sha256=jDevF26mFjqBdOngIZOvUVnngjCXXlzbLvoZvHc7O0A,27
-teamscale_cli-7.1.1.dist-info/RECORD,,
+teamscale_cli-8.7.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+teamscale_cli-8.7.5.dist-info/METADATA,sha256=WMWDfMSfFJdDYVB5tcsEE_DDmjSVue44glez1SqJG_Y,554
+teamscale_cli-8.7.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teamscale_cli-8.7.5.dist-info/entry_points.txt,sha256=fhhE5zS36olRi97D3CYpIMHJzA5RUmFXzfBCvZnBCrQ,82
+teamscale_cli-8.7.5.dist-info/top_level.txt,sha256=jDevF26mFjqBdOngIZOvUVnngjCXXlzbLvoZvHc7O0A,27
+teamscale_cli-8.7.5.dist-info/RECORD,,
```

