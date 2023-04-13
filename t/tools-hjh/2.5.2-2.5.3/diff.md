# Comparing `tmp/tools_hjh-2.5.2.tar.gz` & `tmp/tools_hjh-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.5.2.tar", last modified: Thu Apr 13 07:54:19 2023, max compression
+gzip compressed data, was "dist\tools_hjh-2.5.3.tar", last modified: Thu Apr 13 09:32:15 2023, max compression
```

## Comparing `tools_hjh-2.5.2.tar` & `tools_hjh-2.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.2/LICENSE
--rw-rw-rw-   0        0        0      207 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-04-13 07:54:05.000000 tools_hjh-2.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:54:18.000000 tools_hjh-2.5.2/tools_hjh/
--rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.2/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     8245 2023-03-23 07:55:14.000000 tools_hjh-2.5.2/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.2/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.2/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.2/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.2/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    32853 2023-04-13 07:48:52.000000 tools_hjh-2.5.2/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.2/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.2/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.2/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.2/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:54:19.000000 tools_hjh-2.5.2/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2023-04-13 07:54:17.000000 tools_hjh-2.5.2/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 07:54:16.000000 tools_hjh-2.5.2/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-04-13 09:32:02.000000 tools_hjh-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/tools_hjh/
+-rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.3/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9420 2023-04-13 09:26:36.000000 tools_hjh-2.5.3/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.3/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.3/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.3/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.3/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    32863 2023-04-13 09:27:34.000000 tools_hjh-2.5.3/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.3/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.3/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.3/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.3/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      453 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.5.2/tools_hjh/Chrome.py` & `tools_hjh-2.5.3/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/DBConn.py` & `tools_hjh-2.5.3/tools_hjh/DBConn.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,16 @@
             elif param is None:
                 cur.execute(sql)
             conn.commit()
             rownum = cur.rowcount
             cur.close()
             conn.close()
             return rownum
-    
+
+        '''
         # 执行SELECT语句，会一次性把结果全拿到内存里，数据量大慎用
         if sql.lower().strip().startswith("select"):
             sql = sql.strip()
             col = []
             if param is None:
                 cur.execute(sql)
             elif type(param) == tuple:
@@ -139,15 +140,26 @@
                     cell_new = str(cell)
                     row_new.append(cell_new)
                 rows_new.append(row_new)
             qrs = QueryResults(tuple(col), rows_new)
             cur.close()
             conn.close()
             return qrs
-        
+        '''
+       
+        # 执行SELECT语句
+        if sql.lower().strip().startswith("select"):
+            sql = sql.strip()
+            if param is None:
+                cur.execute(sql)
+            elif type(param) == tuple:
+                cur.execute(sql, param)
+            qrs = QueryResults(cur, conn)
+            return qrs
+
     def run(self, sql, param=None, wait=False):
         """ 执行点什么
         sql中的占位符可以统一使用“?”
         wait为True则会等待当前正在执行的sql，有bug，暂不处理，自用规避"""
         if wait == True:
             tpnum = self.runtp.run(self.__run, (sql, param))
             self.runtp.wait()
@@ -199,26 +211,59 @@
         except:
             pass
         finally:
             self.dbpool = None
     
     def __del__(self):
         self.close()
+    
         
-
 class QueryResults:
 
-    def __init__(self, cols=(), rows=[]):
-        self.cols = cols
-        self.rows = rows
+    def __init__(self, cur, conn):
+        self.cur = cur
+        self.conn = conn
+        self.row = ''
 
-    def get_cols(self):
-        return self.cols
+    def get_cols(self, end_close=False):
+        col = []
+        for c in self.cur.description:
+            col.append(c[0])
+        if end_close:
+            self.close()
+        return tuple(col)
 
-    def get_rows(self):
-        return self.rows
+    def get_rows(self, end_close=False):
+        rows = self.cur.fetchall()
+        rows_new = []
+        for row in rows:
+            row_new = []
+            for cell in row:
+                cell_new = str(cell)
+                row_new.append(cell_new)
+            rows_new.append(row_new)
+        if end_close:
+            self.close()
+        return rows_new
     
-    def set_cols(self, cols):
-        self.cols = cols
+    def next(self):
+        self.row = self.cur.fetchone()
+        if self.row == None:
+            return False
+        else:
+            return True
+
+    def get_row(self):
+        return self.row
+    
+    def close(self):
+        try:
+            self.cur.close()
+        except:
+            pass
+        try:
+            self.conn.close()
+        except:
+            pass
         
-    def set_rows(self, rows):
-        self.rows = rows
+    def __del__(self):
+        self.close()
```

### Comparing `tools_hjh-2.5.2/tools_hjh/HTTPRequest.py` & `tools_hjh-2.5.3/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/HTTPTools.py` & `tools_hjh-2.5.3/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/Log.py` & `tools_hjh-2.5.3/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/MemoryDB.py` & `tools_hjh-2.5.3/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/OracleTools.py` & `tools_hjh-2.5.3/tools_hjh/OracleTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         data_type || '(' || data_precision || ')'
                     when data_type = 'NUMBER' and data_precision = 0 and data_scale = 0 then 
                         data_type
                     else data_type 
                 end column_type, nullable, data_default
             from dba_tab_cols where owner = ? and table_name = ? and column_name not like '%$%' order by column_id
         '''
-        cols_ = ora_conn.run(sql, (username, table)).get_rows()
+        cols_ = ora_conn.run(sql, (username, table)).get_rows(True)
         lenNum = 0
         for col_ in cols_:
             if lenNum < len(col_[0]):
                 lenNum = len(col_[0])
         for col_ in cols_:
             colstr = col_[0]
             typestr = col_[1]
@@ -58,15 +58,15 @@
             else:
                 nullable = ''
             if col_[3] != 'None':
                 data_default = ' default ' + col_[3].strip('\n')
             else:
                 data_default = ''
             mess = mess + 'column: ' + colstr.lower() + nullable + data_default + '\n'
-            
+        
         # 索引 类型 列和列排序
         sql = '''
             select t.index_name
             , t.index_type
             , t2.column_name
             , t3.column_expression
             , t2.descend
@@ -82,17 +82,18 @@
             and t2.index_owner = t3.index_owner(+)
             and t2.table_owner = t3.table_owner(+)
             and t2.index_name = t3.index_name(+)
             and t2.table_name = t3.table_name(+)
             and t2.column_position = t3.column_position(+)
             order by t.index_type, t2.column_position
         '''
-        rows = ora_conn.run(sql, (username, table)).get_rows()
+        qrs = ora_conn.run(sql, (username, table))
+        rows = qrs.get_rows()
+        col = qrs.get_cols(True)
         if len(rows) > 0:
-            col = ora_conn.run(sql, (username, table)).get_cols()
             mdb = MemoryDB()
             mdb.set('t_idx', col, rows)
             # 降序索引也体现为函数索引，列名会用"col_name"，而字符串用'str'
             sql = '''
                 select distinct index_name
                 , group_concat(
                     replace(case when column_name like 'SYS_%$' then column_expression else column_name end, '"', '')
@@ -101,15 +102,15 @@
                     partition by index_name 
                     order by column_position 
                     rows between unbounded preceding and unbounded following
                 ) index_str
                 , uniqueness, index_type
                 from t_idx 
             '''
-            rss = mdb.db_conn.run(sql).get_rows()
+            rss = mdb.db_conn.run(sql).get_rows(True)
             mdb.close()
             for rs in rss:
                 name = rs[0]
                 col = rs[1].lower()
                 if rs[3] == 'BITMAP':
                     idx_type = ' bitmap'
                 elif rs[2] == 'UNIQUE':
@@ -138,15 +139,15 @@
                 and t.owner = t2.owner
                 and t.constraint_name = t2.constraint_name
                 and t.table_name = t2.table_name
                 and t.constraint_type in('P','U')
             ) group by constraint_name, constraint_type
             order by constraint_name, constraint_type
         '''
-        rss = ora_conn.run(sql, (username, table)).get_rows()
+        rss = ora_conn.run(sql, (username, table)).get_rows(True)
         for rs in rss:
             name = rs[0]
             c_type = rs[1]
             cols = rs[2].lower()
             if c_type == 'U':
                 constraint_type = ' unique'
             elif c_type == 'P':
@@ -177,15 +178,15 @@
         """得到某个对象的ddl语言"""
         username = username.upper()
         obj_name = obj_name.upper()
         type_ = type_.upper()
         sql = '''
             select dbms_metadata.get_ddl(?, ?, ?) from dual
         '''
-        return dba_conn.run(sql, (type_, obj_name, username)).get_rows()[0][0]
+        return dba_conn.run(sql, (type_, obj_name, username)).get_rows(True)[0][0]
 
     @staticmethod
     def get_table_ddl(dba_conn, username, table):
         """得到某个表的全部ddl语言，包含表、索引和列注释的ddl"""
         ddl_sqls = ''
         sql = '''
             select * from (
@@ -194,15 +195,15 @@
                 where index_type != 'LOB' and owner = ? and table_name = ?
                 union all
                 select owner, table_name, table_name, 'TABLE' obj_type 
                 from dba_tables
                 where owner = ? and table_name = ?
             ) t order by decode(obj_type, 'TABLE', 0, 'INDEX', 1), obj_name
         '''
-        rows = dba_conn.run(sql, (username, table, username, table)).get_rows()
+        rows = dba_conn.run(sql, (username, table, username, table)).get_rows(True)
         for row in rows:
             type_ = row[3]
             name = row[2]
             ddl_sql = OracleTools.get_ddl(dba_conn, username, type_, name) + ';'
             ddl_sqls = ddl_sqls + '-- ' + type_ + ' ' + name + '\n'
             ddl_sql = ddl_sql.lstrip().replace('"', '')
             ddl_sqls = ddl_sqls + ddl_sql + '\n\n'
@@ -213,15 +214,15 @@
             from dba_col_comments
             where owner = ? 
             and table_name = ? 
             and comments is not null
         '''
         
         ddl_sqls = ddl_sqls + '-- 注释' + '\n'
-        for r in dba_conn.run(sql, (username, table)).get_rows():
+        for r in dba_conn.run(sql, (username, table)).get_rows(True):
             ddl_sqls = ddl_sqls + "comment on column " + username + "." + table + "." + r[0] + " is '" + r[1] + "';\n"
             
         return ddl_sqls    
     
     @staticmethod
     def get_table_size(dba_conn, username, table):
         """得到一个表相关对象的容量分布情况"""
@@ -257,15 +258,15 @@
             from dba_indexes t, dba_segments t2
             where t.owner = t2.owner
             and t.index_name = t2.segment_name
             and t.owner = ?
             and t.table_name = ?
             group by t.owner, t.table_name, t.index_name, t2.segment_type
         '''
-        rows = dba_conn.run(sql, (username, table, username, table, username, table)).get_rows()
+        rows = dba_conn.run(sql, (username, table, username, table, username, table)).get_rows(True)
         return rows
     
     @staticmethod
     def get_sids_by_host(host_conn):
         """ 根据给入的tools_hjh.SSHConn对象获取这台主机运行的全部SID实例名称 """
         sids = []
         pros = host_conn.exec_command("ps -ef | grep ora_smon | grep -v grep | awk '{print $8}'").split('\n')
```

### Comparing `tools_hjh-2.5.2/tools_hjh/SSHConn.py` & `tools_hjh-2.5.3/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/ThreadPool.py` & `tools_hjh-2.5.3/tools_hjh/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.2/tools_hjh/Tools.py` & `tools_hjh-2.5.3/tools_hjh/Tools.py`

 * *Files identical despite different names*

