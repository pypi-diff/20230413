# Comparing `tmp/yourtools-0.4.4.tar.gz` & `tmp/yourtools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.4.4.tar", last modified: Thu Apr 13 10:16:05 2023, max compression
+gzip compressed data, was "dist/yourtools-0.4.5.tar", last modified: Thu Apr 13 10:55:04 2023, max compression
```

## Comparing `yourtools-0.4.4.tar` & `yourtools-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:16:05.000000 yourtools-0.4.4/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2416 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      649 2023-04-13 09:13:14.000000 yourtools-0.4.4/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2893 2023-04-07 10:28:09.000000 yourtools-0.4.4/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.4.4/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-13 10:16:05.000000 yourtools-0.4.4/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.4.4/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.4.4/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.4.4/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 10:16:05.000000 yourtools-0.4.4/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-13 10:16:05.000000 yourtools-0.4.4/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:55:04.000000 yourtools-0.4.5/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.4.5/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.4.5/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.4.5/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.4.5/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.4.5/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      649 2023-04-13 09:13:14.000000 yourtools-0.4.5/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2893 2023-04-07 10:28:09.000000 yourtools-0.4.5/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.4.5/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-13 10:55:04.000000 yourtools-0.4.5/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.4.5/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.4.5/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.4.5/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-13 10:55:04.000000 yourtools-0.4.5/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-13 10:55:04.000000 yourtools-0.4.5/setup.cfg
```

### Comparing `yourtools-0.4.4/yourtools/db/dbutils.py` & `yourtools-0.4.5/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/yourtools/db/hive.py` & `yourtools-0.4.5/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/yourtools/db/mysql.py` & `yourtools-0.4.5/yourtools/db/mysql.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,63 +23,63 @@
             ssh_tunnel.start()
             self.dbconfig.host = ssh_tunnel.local_bind_host
             self.dbconfig.port = ssh_tunnel.local_bind_port
         self._init()
 
     def _init(self):
         try:
-            self._connect = pymysql.connect(
+            self.connect = pymysql.connect(
                 host=str(self.dbconfig.host),
                 port=self.dbconfig.port,
                 user=str(self.dbconfig.username),
                 passwd=str(self.dbconfig.password),
                 db=str(self.dbconfig.db),
                 charset=str(self.dbconfig.charset)
             )
-            self.cursor = self._connect.cursor()
+            self.cursor = self.connect.cursor()
             return True
         except Exception as err:
             raise Exception("MySQL Connection error", err)
             return False
 
     def get_conn(self):
-        if self._connect():
-            return self._connect()
+        if self.connect:
+            return self.connect
         else:
             self._init()
-            return self._connect()
+            return self.connect
 
     def close_conn(self):
-        if self._connect:
-            self._connect.close()
+        if self.connect:
+            self.connect.close()
 
     def query(self, sql, param=None):
         """
         Query data
         :param sql:
         :param param:
         :param size: Number of rows of data you want to return
         :return:
         """
-        cur = self._connect.cursor(cursor=pymysql.cursors.DictCursor)
+        cur = self.connect.cursor(cursor=pymysql.cursors.DictCursor)
         rows = None
         try:
             cur.execute(sql, param)
             rows = cur.fetchall()
         except Exception as e:
             raise Exception(e)
-            self._connect.rollback()
+            self.connect.rollback()
         cur.close()
         return rows
 
     def execute(self, sql):
         """
         exec DML：INSERT、UPDATE、DELETE
         :param sql: dml sql
         :param param: string|list
         :return: Number of rows affected
         """
         try:
             self.cursor.execute(sql)
-            self._connect.commit()
+            self.connect.commit()
         except Exception as e:
-            self._connect.rollback()
+            self.connect.rollback()
```

### Comparing `yourtools-0.4.4/yourtools/Azkaban.py` & `yourtools-0.4.5/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/yourtools/Time.py` & `yourtools-0.4.5/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/yourtools/WeChat.py` & `yourtools-0.4.5/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/yourtools.egg-info/PKG-INFO` & `yourtools-0.4.5/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.4.4/README.md` & `yourtools-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/setup.py` & `yourtools-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.4/PKG-INFO` & `yourtools-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

