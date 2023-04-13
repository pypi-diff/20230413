# Comparing `tmp/ar_ex_sys_worker-1.5.7-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.5.71-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15887 bytes, number of entries: 11
+Zip file size: 15896 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
 -rw-rw-rw-  2.0 fat    26635 b- defN 23-Apr-13 06:51 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19415 b- defN 23-Apr-13 07:00 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    19415 b- defN 23-Apr-13 07:06 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    10331 b- defN 23-Apr-13 07:02 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1127 b- defN 22-Sep-14 11:20 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      343 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      989 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/RECORD
-11 files, 60046 bytes uncompressed, 14181 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Apr-13 07:07 ar_ex_sys_worker-1.5.71.dist-info/RECORD
+11 files, 60052 bytes uncompressed, 14180 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.7.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.5.71.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.7.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.5.71.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.7.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.5.71.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.7.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.5.71.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.7.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.5.71.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/mixins.py

```diff
@@ -26,16 +26,16 @@
     link_auth = None
     port = None
     link_create_act = None
     ex_sys_id = None
 
 
 class SignallMixin:
-    #link_host = "https://signall.qodex.tech"
-    link_host = "https://signalltestdev.qodex.tech"
+    link_host = "https://signall.qodex.tech"
+    #link_host = "https://signalltestdev.qodex.tech"
     link_auth = '/v1/user/login'
     link_get_po_links = "/v1/gravity/get_po_clients"
     port = None
     link_create_act = '/v1/acts/create_act'
     ex_sys_id = 1
     auth_key_in_headers = 'Authorization'
     response_token_key = 'token'
```

## Comparing `ar_ex_sys_worker-1.5.7.dist-info/LICENSE` & `ar_ex_sys_worker-1.5.71.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.5.7.dist-info/RECORD` & `ar_ex_sys_worker-1.5.71.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/main.py,sha256=yy0341VtS7ms441adGYsTUXXuJAcrv0WNHEnIPRttA4,26635
-ar_external_sys_worker/mixins.py,sha256=oGqpBgPGhrRk9wLtkk0rnsrc1_bPRsVqSppjKaMAyqY,19415
+ar_external_sys_worker/mixins.py,sha256=5ipUbvwnG_QanPeGsC6472OpeergyvYpao2dX0aK9HM,19415
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/tests/main_test.py,sha256=3vl6MXEf9ET7T1scONzRK9NnjCy2SeweqV84qUmWLa4,10331
 ar_external_sys_worker/tests/mixins_test.py,sha256=9gyYIATJV5y7tdOc2PuyqYmYjCATGjfxFNGaa5YKdnY,1127
-ar_ex_sys_worker-1.5.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.5.7.dist-info/METADATA,sha256=eFvFAusLIMALmgHTv8_P3LiQRzFFBDwbzFr28vAy0M0,343
-ar_ex_sys_worker-1.5.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ar_ex_sys_worker-1.5.7.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.5.7.dist-info/RECORD,,
+ar_ex_sys_worker-1.5.71.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.5.71.dist-info/METADATA,sha256=i12vwoBwuDtczhbK47zGhegryhuqI34FOIx5ZwTGIkM,344
+ar_ex_sys_worker-1.5.71.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_ex_sys_worker-1.5.71.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.5.71.dist-info/RECORD,,
```

