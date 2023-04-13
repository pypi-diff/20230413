# Comparing `tmp/ar_ex_sys_worker-1.5.62-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.5.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15701 bytes, number of entries: 11
+Zip file size: 15887 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    26484 b- defN 23-Apr-13 05:56 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    18861 b- defN 23-Apr-13 05:53 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    26635 b- defN 23-Apr-13 06:51 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19415 b- defN 23-Apr-13 07:00 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
--rw-rw-rw-  2.0 fat    10214 b- defN 23-Mar-29 11:51 ar_external_sys_worker/tests/main_test.py
+-rw-rw-rw-  2.0 fat    10331 b- defN 23-Apr-13 07:02 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1127 b- defN 22-Sep-14 11:20 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/RECORD
-11 files, 59230 bytes uncompressed, 13985 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      343 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 23-Apr-13 07:04 ar_ex_sys_worker-1.5.7.dist-info/RECORD
+11 files, 60046 bytes uncompressed, 14181 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.62.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.62.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.5.7.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.62.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.62.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.62.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -326,21 +326,24 @@
 
     def convert_time_to_msk(self, date, new_timezone, *args, **kwargs):
         date = date.astimezone(timezone(new_timezone))
         return date
 
 
 class SignallActWorker(mixins.SignallMixin, ActsWorker,
-                       mixins.SignallPhotoEncoderMixin):
+                       mixins.SignallPhotoEncoderMixin,
+                       mixins.SignallGetCarriersPO):
     def __init__(self, sql_shell, trash_cats_list, time_start, acts_limit=5,
                  login=None, password=None, auto_auth=True):
         super().__init__(sql_shell=sql_shell, trash_cats=trash_cats_list,
                          time_start=time_start, acts_limit=acts_limit,
                          login=login, password=password, auto_auth=auto_auth)
         self.working_link = self.get_full_endpoint(self.link_create_act)
+        self.get_carriers_po_link = self.get_full_endpoint(
+            self.link_get_po_links)
         self.act_id_from_response = 'act_id'
         self.mutex = allocate_lock()
 
     def format_file_before_logging(self, data):
         data = json.loads(data)
         data.pop('photo_in')
         data.pop('photo_out')
```

## ar_external_sys_worker/mixins.py

```diff
@@ -26,16 +26,18 @@
     link_auth = None
     port = None
     link_create_act = None
     ex_sys_id = None
 
 
 class SignallMixin:
-    link_host = "https://signall.qodex.tech"
+    #link_host = "https://signall.qodex.tech"
+    link_host = "https://signalltestdev.qodex.tech"
     link_auth = '/v1/user/login'
+    link_get_po_links = "/v1/gravity/get_po_clients"
     port = None
     link_create_act = '/v1/acts/create_act'
     ex_sys_id = 1
     auth_key_in_headers = 'Authorization'
     response_token_key = 'token'
     login_key_to_ex_sys = 'email'
     pass_key_to_ex_sys = 'password'
@@ -145,14 +147,15 @@
                 self.pass_key_to_ex_sys: self.password}
         return data
 
     def extract_token(self, auth_result_json):
         response = auth_result_json.json()
         # if 'error' in response:
         #    return response
+        #print(response)
         token = response[self.response_token_key]
         return token
 
     def get_token(self, **kwargs):
         response = self.auth_me()
         token = self.extract_token(response)
         return token
@@ -206,14 +209,27 @@
         data_json = json.dumps(data_json)
         response = requests.post(self.working_link.format(signall_id),
                                  headers=self.headers,
                                  data=data_json)
         return response
 
 
+class SignallGetCarriersPO:
+    headers = None
+    get_carriers_po_link = None
+
+    def get_carriers_po(self):
+        if not self.get_carriers_po_link:
+            return {'error': 'There are not link for route get_carriers'}
+        print(self.get_carriers_po_link)
+        response = requests.get(self.get_carriers_po_link,
+                                headers=self.headers)
+        return response
+
+
 class SignAllCarsGetter:
     headers = None
     working_link = None
 
     def get_cars(self):
         response = requests.get(self.working_link,
                                 headers=self.headers)
```

## ar_external_sys_worker/tests/main_test.py

```diff
@@ -219,15 +219,17 @@
                                            '2021.05.05',
                                            1,
                                            gravity_ip='172.16.9.20',
                                            test=True)
         #inst.link_host = 'https://signalltestdev.qodex.tech'
         inst.auth()
        # print(inst.link_host)
-        inst.send_unsend_acts()
+        #inst.send_unsend_acts()
+        res = inst.get_carriers_po().json()
+        print(f"PO_CARRIERS: {res}\nLen: {len(res['transporters'])}")
 
     @unittest.SkipTest
     def test_send_acts(self):
         self.inst.send_unsend_acts()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `ar_ex_sys_worker-1.5.62.dist-info/LICENSE` & `ar_ex_sys_worker-1.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.5.62.dist-info/RECORD` & `ar_ex_sys_worker-1.5.7.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/main.py,sha256=Ys7MbRmMpz9EBdjAUOmXMFVqoxJ1gjhpGN4run_kjx8,26484
-ar_external_sys_worker/mixins.py,sha256=b0ehBavr3mD4Wnvq6MUlI5XLL5US8ajgB1ZQnIoj2wM,18861
+ar_external_sys_worker/main.py,sha256=yy0341VtS7ms441adGYsTUXXuJAcrv0WNHEnIPRttA4,26635
+ar_external_sys_worker/mixins.py,sha256=oGqpBgPGhrRk9wLtkk0rnsrc1_bPRsVqSppjKaMAyqY,19415
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/tests/main_test.py,sha256=XWdINoaJvqmILef4DxY-PcE3fqZONLF_k1vf8teKet8,10214
+ar_external_sys_worker/tests/main_test.py,sha256=3vl6MXEf9ET7T1scONzRK9NnjCy2SeweqV84qUmWLa4,10331
 ar_external_sys_worker/tests/mixins_test.py,sha256=9gyYIATJV5y7tdOc2PuyqYmYjCATGjfxFNGaa5YKdnY,1127
-ar_ex_sys_worker-1.5.62.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.5.62.dist-info/METADATA,sha256=CWsHuEZjRp4vMke5F-HzAz0AwiSEcnKr6Ww7Fvdbtgo,344
-ar_ex_sys_worker-1.5.62.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ar_ex_sys_worker-1.5.62.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.5.62.dist-info/RECORD,,
+ar_ex_sys_worker-1.5.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.5.7.dist-info/METADATA,sha256=eFvFAusLIMALmgHTv8_P3LiQRzFFBDwbzFr28vAy0M0,343
+ar_ex_sys_worker-1.5.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_ex_sys_worker-1.5.7.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.5.7.dist-info/RECORD,,
```

