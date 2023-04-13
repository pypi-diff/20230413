# Comparing `tmp/tools_hjh-2.5.1.tar.gz` & `tmp/tools_hjh-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.5.1.tar", last modified: Thu Mar 30 09:15:29 2023, max compression
+gzip compressed data, was "dist\tools_hjh-2.5.2.tar", last modified: Thu Apr 13 07:54:19 2023, max compression
```

## Comparing `tools_hjh-2.5.1.tar` & `tools_hjh-2.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 09:15:29.000000 tools_hjh-2.5.1/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.1/LICENSE
--rw-rw-rw-   0        0        0      207 2023-03-30 09:15:29.000000 tools_hjh-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-30 09:15:29.000000 tools_hjh-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-03-30 09:15:22.000000 tools_hjh-2.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh/
--rw-rw-rw-   0        0        0     2832 2023-01-13 02:55:02.000000 tools_hjh-2.5.1/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     8245 2023-03-23 07:55:14.000000 tools_hjh-2.5.1/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.1/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.1/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.1/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.1/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    32439 2023-03-30 09:14:13.000000 tools_hjh-2.5.1/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2022-12-27 02:34:09.000000 tools_hjh-2.5.1/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.1/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.1/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.1/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:15:29.000000 tools_hjh-2.5.1/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-03-30 09:15:28.000000 tools_hjh-2.5.1/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-04-13 07:54:05.000000 tools_hjh-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:54:18.000000 tools_hjh-2.5.2/tools_hjh/
+-rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.2/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     8245 2023-03-23 07:55:14.000000 tools_hjh-2.5.2/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.2/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.2/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.2/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.2/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    32853 2023-04-13 07:48:52.000000 tools_hjh-2.5.2/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.2/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.2/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.2/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.2/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      453 2023-04-13 07:54:17.000000 tools_hjh-2.5.2/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.5.1/tools_hjh/Chrome.py` & `tools_hjh-2.5.2/tools_hjh/Chrome.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def get(self, url, headers=None, data=None):
         while self.openSize == self.maxSize:
             time.sleep(0.2)
         for chrome in self.pool:
             if chrome.get_status() == 0:
                 self.openSize = self.openSize + 1
                 text = chrome.get(url, headers, data)
-                chrome.get(url='data:,')
+                # chrome.get(url='data:,')
                 self.openSize = self.openSize - 1
                 return text
         time.sleep(0.2)
         return self.get(url, headers, data)
     
     def close(self):
         while self.openSize > 0:
```

### Comparing `tools_hjh-2.5.1/tools_hjh/DBConn.py` & `tools_hjh-2.5.2/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/HTTPRequest.py` & `tools_hjh-2.5.2/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/HTTPTools.py` & `tools_hjh-2.5.2/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/Log.py` & `tools_hjh-2.5.2/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/MemoryDB.py` & `tools_hjh-2.5.2/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/OracleTools.py` & `tools_hjh-2.5.2/tools_hjh/OracleTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # coding:utf-8
-from tools_hjh.Log import Log
 from tools_hjh.DBConn import DBConn
 from tools_hjh.DBConn import QueryResults
 from tools_hjh.MemoryDB import MemoryDB
-from tools_hjh.Tools import line_merge_align, locatdate, merge_spaces, \
-    analysis_hosts, locattime, remove_leading_space
-from numpy.core.defchararray import upper
+from tools_hjh.Tools import line_merge_align, locatdate, merge_spaces, analysis_hosts, locattime
 
 
 def main():
     rows = []
     for idx in range(0, 10):
         row = (idx, idx, idx)
         rows.append(row)
@@ -19,19 +16,19 @@
     testDB.close()
 
 
 class OracleTools:
     """ 用于Oracle的工具类 """
     
     @staticmethod
-    def desc(ora_conn, username, table):
+    def desc(ora_conn, username, table, simple_mode=True):
         """得到表结构，包括索引、约束和默认值情况"""
         username = username.upper()
         table = table.upper()
-        mess = 'table: ' + username.lower() + '.' + table.lower() + '\n'
+        mess = 'table: ' + table.lower() + '\n'
         
         # 列 类型 非空约束 默认值
         sql = '''
             select column_name, 
                 case 
                     when data_type = 'VARCHAR2' or data_type = 'CHAR' then 
                         data_type || '(' || data_length || ')'
@@ -107,22 +104,26 @@
                 ) index_str
                 , uniqueness, index_type
                 from t_idx 
             '''
             rss = mdb.db_conn.run(sql).get_rows()
             mdb.close()
             for rs in rss:
+                name = rs[0]
                 col = rs[1].lower()
                 if rs[3] == 'BITMAP':
                     idx_type = ' bitmap'
                 elif rs[2] == 'UNIQUE':
                     idx_type = ' unique'
                 else:
                     idx_type = ''
-                ss = 'index: (' + col.replace(' asc', '').replace(',', ', ') + ')' + idx_type
+                if simple_mode:
+                    ss = 'index: (' + col.replace(' asc', '').replace(',', ', ') + ')' + idx_type
+                else:
+                    ss = 'index: ' + name.lower() + ' (' + col.replace(' asc', '').replace(',', ', ') + ')' + idx_type
                 mess = mess + ss + '\n'
                 
         # 约束 类型 列和列排序
         sql = '''
             select constraint_name, constraint_type
             , max(cols)
             from (
@@ -139,23 +140,27 @@
                 and t.table_name = t2.table_name
                 and t.constraint_type in('P','U')
             ) group by constraint_name, constraint_type
             order by constraint_name, constraint_type
         '''
         rss = ora_conn.run(sql, (username, table)).get_rows()
         for rs in rss:
+            name = rs[0]
             c_type = rs[1]
             cols = rs[2].lower()
             if c_type == 'U':
                 constraint_type = ' unique'
             elif c_type == 'P':
                 constraint_type = ' pk'
             else:
                 constraint_type = ''
-            mess = mess + 'constraint: (' + cols + ')' + constraint_type + '\n'
+            if simple_mode:
+                mess = mess + 'constraint: (' + cols + ')' + constraint_type + '\n'
+            else:
+                mess = mess + 'constraint: ' + name.lower() + ' (' + cols + ')' + constraint_type + '\n'
         return mess.strip('\n')
 
     @staticmethod
     def compare_table(src_conn, src_username, src_table_name, dst_conn, dst_username, dst_table_name):
         """ 比较两个表，根据desc方法得到的字符串去比较 """
         src_username = src_username.upper()
         dst_username = dst_username.upper()
@@ -180,21 +185,24 @@
 
     @staticmethod
     def get_table_ddl(dba_conn, username, table):
         """得到某个表的全部ddl语言，包含表、索引和列注释的ddl"""
         ddl_sqls = ''
         sql = '''
             select * from (
-                select table_owner owner, table_name, index_name obj_name, 'INDEX' obj_type from dba_indexes
+                select table_owner owner, table_name, index_name obj_name, 'INDEX' obj_type 
+                from dba_indexes
+                where index_type != 'LOB' and owner = ? and table_name = ?
                 union all
-                select owner, table_name, table_name, 'TABLE' obj_type from dba_tables
-            ) t where t.owner = ? and t.table_name = ?
-            order by decode(obj_type, 'TABLE', 0, 'INDEX', 1), obj_name
+                select owner, table_name, table_name, 'TABLE' obj_type 
+                from dba_tables
+                where owner = ? and table_name = ?
+            ) t order by decode(obj_type, 'TABLE', 0, 'INDEX', 1), obj_name
         '''
-        rows = dba_conn.run(sql, (username, table)).get_rows()
+        rows = dba_conn.run(sql, (username, table, username, table)).get_rows()
         for row in rows:
             type_ = row[3]
             name = row[2]
             ddl_sql = OracleTools.get_ddl(dba_conn, username, type_, name) + ';'
             ddl_sqls = ddl_sqls + '-- ' + type_ + ' ' + name + '\n'
             ddl_sql = ddl_sql.lstrip().replace('"', '')
             ddl_sqls = ddl_sqls + ddl_sql + '\n\n'
@@ -206,15 +214,15 @@
             where owner = ? 
             and table_name = ? 
             and comments is not null
         '''
         
         ddl_sqls = ddl_sqls + '-- 注释' + '\n'
         for r in dba_conn.run(sql, (username, table)).get_rows():
-            ddl_sqls = ddl_sqls + "comment on column " + username + "." + table + "." + r[0] + " is '" + r[1] + "'\n"
+            ddl_sqls = ddl_sqls + "comment on column " + username + "." + table + "." + r[0] + " is '" + r[1] + "';\n"
             
         return ddl_sqls    
     
     @staticmethod
     def get_table_size(dba_conn, username, table):
         """得到一个表相关对象的容量分布情况"""
         sql = '''
```

### Comparing `tools_hjh-2.5.1/tools_hjh/SSHConn.py` & `tools_hjh-2.5.2/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/ThreadPool.py` & `tools_hjh-2.5.2/tools_hjh/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.1/tools_hjh/Tools.py` & `tools_hjh-2.5.2/tools_hjh/Tools.py`

 * *Files identical despite different names*

