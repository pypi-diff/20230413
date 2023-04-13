# Comparing `tmp/ar_ex_sys_worker-1.5.61-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.5.62-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15658 bytes, number of entries: 11
+Zip file size: 15701 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    26388 b- defN 23-Apr-05 10:21 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    18799 b- defN 23-Apr-05 10:05 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    26484 b- defN 23-Apr-13 05:56 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    18861 b- defN 23-Apr-13 05:53 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    10214 b- defN 23-Mar-29 11:51 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1127 b- defN 22-Sep-14 11:20 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-05 10:22 ar_ex_sys_worker-1.5.61.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-05 10:22 ar_ex_sys_worker-1.5.61.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-05 10:22 ar_ex_sys_worker-1.5.61.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-05 10:22 ar_ex_sys_worker-1.5.61.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Apr-05 10:22 ar_ex_sys_worker-1.5.61.dist-info/RECORD
-11 files, 59072 bytes uncompressed, 13942 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Apr-13 05:57 ar_ex_sys_worker-1.5.62.dist-info/RECORD
+11 files, 59230 bytes uncompressed, 13985 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.61.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.5.62.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.61.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.5.62.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.61.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.5.62.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.61.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.5.62.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.5.61.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.5.62.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -87,18 +87,18 @@
         self.mutex = allocate_lock()
         if auto_auth:
             self.auth()
 
     def auth(self):
         self.set_headers(self.get_headers())
 
-    def send_unsend_acts(self, record_id=None):
+    def send_unsend_acts(self, record_id=None, limit=None):
         self.mutex.acquire()
         try:
-            data = self.get_unsend_acts(record_id=record_id)
+            data = self.get_unsend_acts(record_id=record_id, limit=limit)
             if not data:
                 self.mutex.release()
                 return {'error': 'no acts to send'}
             for act in data:
                 self.send_data(act)
         except:
             print(traceback.format_exc())
@@ -453,17 +453,19 @@
         platform_info = self.get_platform_info()[0]
         self.inn, self.kpp = platform_info['inn'], platform_info['kpp']
         if test:
             self.link_host = 'https://signalltestdev.qodex.tech'
 
     def resend_unget_acts(self):
         unsend_acts = self.get_unget_by_signall_acts()
+        if not unsend_acts:
+            return
         for act in unsend_acts:
             self.delete_act_from_send_reports(act['local_id'])
-        self.send_unsend_acts()
+        self.send_unsend_acts(limit=len(unsend_acts))
 
     @wsqluse.wsqluse.getTableDictStripper
     def get_platform_info(self):
         return self.sql_shell.get_table_dict(
             command=f"SELECT inn, kpp FROM duo_pol_owners "
                     f"WHERE id={self.platform_id}")
```

## ar_external_sys_worker/mixins.py

```diff
@@ -429,23 +429,25 @@
 
     def get_acts_period(self, start_date, end_date, smth_else):
         command = self.get_acts_all_command() + " and time_in >= '{}' and time_out::date <= '{}' {}".format(
             start_date, end_date, smth_else)
         return self.sql_shell.get_table_dict(command)
 
     @wsqluse.wsqluse.getTableDictStripper
-    def get_unsend_acts(self, record_id=None):
+    def get_unsend_acts(self, record_id=None, limit=None):
         command = self.get_acts_all_command()
+        if not limit:
+            limit = self.limit
         if record_id:
             command += f' and r.id={record_id} '
         command += "  and r.id NOT IN (SELECT local_id FROM " \
                   "ex_sys_data_send_reports WHERE table_id={} and ex_sys_id = {} and not get is null) " \
                   "and tc.name in {} and time_in::date>'{}' LIMIT {} ".format(
                       self.table_id, self.ex_sys_id, self.trash_cats_to_send,
-                      self.time_start, self.limit)
+                      self.time_start, limit)
         return self.sql_shell.get_table_dict(command)
 
     def get_one_unsend_act(self):
         try:
             return self.get_unsend_acts()[0]
         except:
             pass
```

## Comparing `ar_ex_sys_worker-1.5.61.dist-info/LICENSE` & `ar_ex_sys_worker-1.5.62.dist-info/LICENSE`

 * *Files identical despite different names*

