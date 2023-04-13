# Comparing `tmp/ops_channel-0.5.4.tar.gz` & `tmp/ops_channel-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_channel-0.5.4.tar", last modified: Sat Mar 18 01:44:08 2023, max compression
+gzip compressed data, was "ops_channel-0.5.5.tar", last modified: Thu Apr 13 03:27:11 2023, max compression
```

## Comparing `ops_channel-0.5.4.tar` & `ops_channel-0.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-03-18 01:44:08.410436 ops_channel-0.5.4/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-03-18 01:44:08.409716 ops_channel-0.5.4/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.4/README.md
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-03-18 01:44:08.403431 ops_channel-0.5.4/ops_channel/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      127 2022-10-20 02:06:16.000000 ops_channel-0.5.4/ops_channel/__init__.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    97491 2023-03-18 01:17:33.000000 ops_channel-0.5.4/ops_channel/base.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    25141 2023-03-18 01:12:44.000000 ops_channel-0.5.4/ops_channel/test.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-03-18 01:44:08.407477 ops_channel-0.5.4/ops_channel.egg-info/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-03-18 01:44:08.000000 ops_channel-0.5.4/ops_channel.egg-info/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-03-18 01:44:08.000000 ops_channel-0.5.4/ops_channel.egg-info/SOURCES.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-03-18 01:44:08.000000 ops_channel-0.5.4/ops_channel.egg-info/dependency_links.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-03-18 01:44:08.000000 ops_channel-0.5.4/ops_channel.egg-info/top_level.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-03-18 01:44:08.410660 ops_channel-0.5.4/setup.cfg
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-03-18 01:43:30.000000 ops_channel-0.5.4/setup.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.984755 ops_channel-0.5.5/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-04-13 03:27:11.984302 ops_channel-0.5.5/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.5/README.md
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.980323 ops_channel-0.5.5/ops_channel/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      127 2022-10-20 02:06:16.000000 ops_channel-0.5.5/ops_channel/__init__.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)    97625 2023-04-13 03:19:35.000000 ops_channel-0.5.5/ops_channel/base.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)    25301 2023-04-13 03:10:36.000000 ops_channel-0.5.5/ops_channel/test.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.983002 ops_channel-0.5.5/ops_channel.egg-info/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/top_level.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-04-13 03:27:11.984965 ops_channel-0.5.5/setup.cfg
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-04-13 03:26:45.000000 ops_channel-0.5.5/setup.py
```

### Comparing `ops_channel-0.5.4/README.md` & `ops_channel-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.4/ops_channel/base.py` & `ops_channel-0.5.5/ops_channel/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1076,14 +1076,15 @@
         '''
         :param dsn_str='mysql://root:root@localhost:3306/ferry':
         :return:
         '''
         import dsnparse
         dsn = dsnparse.parse(dsn_str)
         import pymysql
+        from pymysql.constants import CLIENT
         try:
             from collections import OrderedDict
             from pymysql.cursors import DictCursorMixin, Cursor
             class OrderedDictCursor(DictCursorMixin, Cursor):
                 dict_type = OrderedDict
         except Exception as er:
             OrderedDictCursor = pymysql.cursors.DictCursor
@@ -1091,14 +1092,15 @@
                                      user=dsn.user,
                                      port=dsn.port,
                                      password=dsn.password,
                                      database=dsn.database,
                                      charset='utf8mb4',
                                      cursorclass=OrderedDictCursor,
                                      # local_infile=True,
+                                     client_flag=CLIENT.MULTI_STATEMENTS,
                                      max_allowed_packet=1024 * 1024 * 1024)
         connection.autocommit(True)
         # try:
         #     self.mysql_query(connection, 'set  global max_allowed_packet=1073741824;')
         # except Exception as er:
         #     pass
 
@@ -1477,29 +1479,29 @@
         sql_files = []
         for root, dirs, files in os.walk(sql_dir):
             for file in files:
                 if file.endswith('.sql'):
                     sql_files.append(os.path.join(root, file))
         for sql_file in sql_files:
             with open(sql_file, 'r') as f:
-                lines = f.read()
-                lines = re.split(r'[\r\n]+$', lines)
+                content = f.read()
+                lines = re.split(r'[\r\n]+', content, flags=re.MULTILINE)
                 sql=[]
                 for line in lines:
-                    # if line.startswith('--') or line.startswith('#'):
-                    #     continue
+                    if line.startswith('--') or line.startswith('#'):
+                        continue
                     sql.append(line)
                     if len(sql) > 0 and line.strip().endswith(';'):
                         try:
                             self.mysql_query(conn,"\n".join(sql))
                             sql=[]
                         except Exception as e:
                             print(e)
-                            # s="\n".join(sql)
-                            # print("\n".join(sql))
+                            s="\n".join(sql)
+                            print("\n".join(sql))
                             sql=[]
 
     # merge same file name in different directory
     def merge_sql_files(self, from_dir, to_dir):
         import os
         import shutil
         files1 = self.find_files(from_dir, '.sql')
```

### Comparing `ops_channel-0.5.4/ops_channel/test.py` & `ops_channel-0.5.5/ops_channel/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,8 +660,13 @@
 
 # print(cli.convert_markdown_to_baidu_naotu(md))
 
 
 
 # cli.load_sql_to_mysql(conn_mock_db,'/Users/junqiang.zhang/Downloads/hr')
 
-cli.merge_sql_files('/Users/junqiang.zhang/repo/go/dms/db','/Users/junqiang.zhang/repo/go/dms/mock/db')
+# cli.merge_sql_files('/Users/junqiang.zhang/repo/go/dms/db','/Users/junqiang.zhang/repo/go/dms/mock/db')
+
+
+dsn='mysql://root:mock@localhost:63307/mock'
+conn_mock_db=cli.get_mysql_connection(dsn)
+cli.load_sql_to_mysql(conn_mock_db,'/Users/junqiang.zhang/dbs/dms')
```

### Comparing `ops_channel-0.5.4/setup.py` & `ops_channel-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2018-11-27 19:17:34
 #############################################
 
 from setuptools import setup, find_packages
 
 setup(
     name="ops_channel",
-    version="0.5.4",
+    version="0.5.5",
     keywords=("pip", "ops_channel"),
     description="ops_channel util",
     long_description="ops_channel util",
     license="MIT Licence",
     packages=find_packages(),
     url="https://github.com/sjqzhang/ops_channel",
     author="jqzhang",
```

