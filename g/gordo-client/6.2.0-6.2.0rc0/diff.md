# Comparing `tmp/gordo_client-6.2.0-py3-none-any.whl.zip` & `tmp/gordo_client-6.2.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 44983 bytes, number of entries: 16
+Zip file size: 45010 bytes, number of entries: 16
 -rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx      497 b- defN 80-Jan-01 00:00 gordo_client/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 gordo_client/cli/__init__.py
 -rw-r--r--  2.0 unx     8256 b- defN 80-Jan-01 00:00 gordo_client/cli/client.py
 -rw-r--r--  2.0 unx     1308 b- defN 80-Jan-01 00:00 gordo_client/cli/custom_types.py
 -rw-r--r--  2.0 unx    23791 b- defN 80-Jan-01 00:00 gordo_client/client.py
 -rw-r--r--  2.0 unx     5471 b- defN 80-Jan-01 00:00 gordo_client/dataframe.py
 -rw-r--r--  2.0 unx     8715 b- defN 80-Jan-01 00:00 gordo_client/forwarders.py
 -rw-r--r--  2.0 unx     3564 b- defN 80-Jan-01 00:00 gordo_client/io.py
 -rw-r--r--  2.0 unx     1769 b- defN 80-Jan-01 00:00 gordo_client/schemas.py
 -rw-r--r--  2.0 unx     2703 b- defN 80-Jan-01 00:00 gordo_client/utils.py
-?rw-r--r--  2.0 unx       69 b- defN 16-Jan-01 00:00 gordo_client-6.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 gordo_client-6.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3852 b- defN 16-Jan-01 00:00 gordo_client-6.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     1292 b- defN 16-Jan-01 00:00 gordo_client-6.2.0.dist-info/RECORD
-16 files, 129934 bytes uncompressed, 42867 bytes compressed:  67.0%
+?rw-r--r--  2.0 unx       69 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     3842 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1307 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/RECORD
+16 files, 129939 bytes uncompressed, 42864 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: gordo_client/schemas.py
 Comment: 
 
 Filename: gordo_client/utils.py
 Comment: 
 
-Filename: gordo_client-6.2.0.dist-info/entry_points.txt
+Filename: gordo_client-6.2.0rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: gordo_client-6.2.0.dist-info/LICENSE
+Filename: gordo_client-6.2.0rc0.dist-info/LICENSE
 Comment: 
 
-Filename: gordo_client-6.2.0.dist-info/WHEEL
+Filename: gordo_client-6.2.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: gordo_client-6.2.0.dist-info/METADATA
+Filename: gordo_client-6.2.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: gordo_client-6.2.0.dist-info/RECORD
+Filename: gordo_client-6.2.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gordo_client-6.2.0.dist-info/LICENSE` & `gordo_client-6.2.0rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gordo_client-6.2.0.dist-info/METADATA` & `gordo_client-6.2.0rc0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo-client
-Version: 6.2.0
+Version: 6.2.0rc0
 Summary: Gordo client
 Home-page: https://github.com/equinor/gordo-client
 License: AGPL-3.0
 Keywords: gordo-client
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: PyYAML (>=5.3.1,<6.0.0)
 Requires-Dist: click (>=7.0.0,<9.0.0)
-Requires-Dist: gordo-core (>=0.3.0,<0.4.0)
+Requires-Dist: gordo-core (==0.3.0rc0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.20,<3.0)
 Requires-Dist: simplejson (>=3.17.2,<4.0.0)
 Requires-Dist: wrapt (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/equinor/gordo-client
 Description-Content-Type: text/markdown
 
@@ -35,15 +35,15 @@
 * [Installation.](#Installation)
 * [Developers Instructions.](#Developers-Instructions)
     * [Setup.](#Setup)
     * [Run tests.](#Run-tests)
     
 ## Installation
 
-At least python 3.9 need to be installed in the system first.
+Python 3.9 need to be installed in the system first.
 
 In order to install or uninstall this library run following commands.
 ```bash
 # Install
 pip install gordo-client
 
 # Uninstall
```

## Comparing `gordo_client-6.2.0.dist-info/RECORD` & `gordo_client-6.2.0rc0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 gordo_client/cli/custom_types.py,sha256=rE6iT0cuPU8wzvFVm6HSWOka9D_Zxc9w8BcC7eNeIRM,1308
 gordo_client/client.py,sha256=_TvJTpdHZt5ZEIReZDw82yrmL-XYoC-8Tfknb-2fWFE,23791
 gordo_client/dataframe.py,sha256=NIysETom72gGyghpKtCPOYFecuGUwK1o6pb7ZeReXBc,5471
 gordo_client/forwarders.py,sha256=S80fwzAxA-luzxVq82AM4J1ZRz0NrXv12aIpM2JBvCo,8715
 gordo_client/io.py,sha256=Wmv06dwUaYxWIiHjKjBPhH8GBpNCfv7LKqCt1RJAMS8,3564
 gordo_client/schemas.py,sha256=ox7tp1ZgVWBOkmkaz0IScJ-2fozmh6u_Kaax50kp5Kc,1769
 gordo_client/utils.py,sha256=3_x-fbTQt-fOA8CFfkPVdBXhBoKwxFfvyq-dzrrX-CQ,2703
-gordo_client-6.2.0.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
-gordo_client-6.2.0.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
-gordo_client-6.2.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-gordo_client-6.2.0.dist-info/METADATA,sha256=yKR-4YJC3a41MC3asOsuVlMPyaQTx774_Z0Gk73QieI,3852
-gordo_client-6.2.0.dist-info/RECORD,,
+gordo_client-6.2.0rc0.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
+gordo_client-6.2.0rc0.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
+gordo_client-6.2.0rc0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+gordo_client-6.2.0rc0.dist-info/METADATA,sha256=dHjbxt2jyjvx_33L82Qr2DrSVsxdYCocL4ysby7WLZM,3842
+gordo_client-6.2.0rc0.dist-info/RECORD,,
```

