# Comparing `tmp/abuscom-libs-0.1.3.tar.gz` & `tmp/abuscom-libs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.3.tar", last modified: Wed Apr  5 15:00:14 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.4.tar", last modified: Thu Apr 13 12:25:29 2023, max compression
```

## Comparing `abuscom-libs-0.1.3.tar` & `abuscom-libs-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-05 15:00:14.413707 abuscom-libs-0.1.3/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-05 15:00:14.413263 abuscom-libs-0.1.3/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.3/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-05 15:00:14.401221 abuscom-libs-0.1.3/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-05 15:00:14.409182 abuscom-libs-0.1.3/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.3/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     1359 2023-02-21 13:45:27.000000 abuscom-libs-0.1.3/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8368 2023-02-02 14:27:02.000000 abuscom-libs-0.1.3/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     4083 2023-04-05 12:19:11.000000 abuscom-libs-0.1.3/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.3/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     3416 2023-04-05 14:58:55.000000 abuscom-libs-0.1.3/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-05 15:00:14.412645 abuscom-libs-0.1.3/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-05 15:00:13.000000 abuscom-libs-0.1.3/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-05 15:00:14.000000 abuscom-libs-0.1.3/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-05 15:00:13.000000 abuscom-libs-0.1.3/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-05 15:00:14.000000 abuscom-libs-0.1.3/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-05 15:00:14.000000 abuscom-libs-0.1.3/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-05 15:00:14.413809 abuscom-libs-0.1.3/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-05 14:59:13.000000 abuscom-libs-0.1.3/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.272921 abuscom-libs-0.1.4/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-13 12:25:29.272547 abuscom-libs-0.1.4/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.4/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.262384 abuscom-libs-0.1.4/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.269010 abuscom-libs-0.1.4/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.4/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     1359 2023-02-21 13:45:27.000000 abuscom-libs-0.1.4/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.4/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5983 2023-04-07 09:46:30.000000 abuscom-libs-0.1.4/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.4/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.4/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.271978 abuscom-libs-0.1.4/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-13 12:25:28.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-13 12:25:28.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-13 12:25:29.273030 abuscom-libs-0.1.4/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-13 12:24:19.000000 abuscom-libs-0.1.4/setup.py
```

### Comparing `abuscom-libs-0.1.3/README.md` & `abuscom-libs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.3/abuscom/connectors/compass.py` & `abuscom-libs-0.1.4/abuscom/connectors/compass.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.3/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.4/abuscom/connectors/hubspot.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,17 @@
         try:
             tuple = tuple + (item['teams'][0]['name'],)
         except KeyError:
             tuple = tuple + ('UNDEFINED',)
         return tuple
 
     def read_deals(self, colNames):
-        dealsEndpoint = "/crm/v4/objects/deals?limit=100&properties=dealname&properties=dealType&properties=dealstage&properties=amount&properties=deal_currency_code&properties=hy2_market&properties=hy2_product&properties=hy2_application&properties=hubspot_owner_id&properties=hs_deal_stage_probability&properties=hs_exchange_rate&properties=of_systems&properties=expected_delivery&properties=h2_kg_&properties=hy2_battery&properties=hy2_storage&properties=hs_object_id&properties=electrolyzer&properties=sales_team&properties=hy_invoice_co_&properties=hy_mfg_co_&associations=companies"
+
+
+        dealsEndpoint = "/crm/v4/objects/deals?limit=100&properties=critical_opp_review&properties=dealname&properties=dealType&properties=dealstage&properties=amount&properties=deal_currency_code&properties=hy2_market&properties=hy2_product&properties=hy2_application&properties=hubspot_owner_id&properties=hs_deal_stage_probability&properties=hs_exchange_rate&properties=of_systems&properties=expected_delivery&properties=h2_kg_&properties=hy2_battery&properties=hy2_storage&properties=hs_object_id&properties=electrolyzer&properties=sales_team&properties=hy_invoice_co_&properties=hy_mfg_co_&associations=companies"
         dealList = self.__read_page(endpoint=dealsEndpoint, resultProperty='results')
         try:
             data = [*map(lambda x: self.__companyToTuple(x, colNames), dealList)]
             return data
 
         except (JSONDecodeError, LookupError, AirflowException) as ex:
             print(ex)
```

### Comparing `abuscom-libs-0.1.3/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.4/abuscom/connectors/oracle.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,30 +56,55 @@
             self.clear_table(tableName=tableName)
         # If there are rows to insert, then bulk-insert them using the OracleHook.
         if tuples:
             self.ora_hook.bulk_insert_rows(tableName, tuples)
         # Return 0 to indicate success.
         return 0
 
-    def load_to_tuples(self, tableName, colNames):
+    def load_to_tuples(self, tableName, colNames,where=[]):
         """
         Reads data from an Oracle table and returns it as a list of tuples.
 
-        :param table_name: The name of the table to read from.
-        :param col_names: A list of strings representing the column names to read.
+        :param tableName: The name of the table to read from.
+        :param colNames: A list of strings representing the column names to read.
+        :param where: OPTIONAL. A list of objects representing the column, symbol, and value to filter by.
+                    Example: [{ 'column': 'bool', 'symbol': '=', 'value': 0 }, { 'column': 'desc', 'symbol': '<>', 'value': 'test' },{
+                                                                                                                                             "column": "desc",
+                                                                                                                                             "symbol": "<>",
+                                                                                                                                             "value": "\"4\""
+                                                                                                                                           }]
+                    ATTENTION: types need to match!
 
         :return: A list of tuples representing the rows in the table.
         """
-        columns = ",".join(colNames)
         if(len(colNames)==0):
             print('No Columns given, return 0')
             return 0
-        df = self.ora_hook.get_pandas_df(f"SELECT {columns} FROM {tableName}")
+        # Create a string with the uppercase column names separated by commas
+        columns = ",".join('"' + columnName.upper() + '"' for columnName in colNames)
+
+        # If a where clause is specified, construct the SQL WHERE clause with the filter conditions + check if value is string or number....
+        if len(where) > 0:
+            whereClause = "WHERE " + " AND ".join('"' + cond['column'].upper() + '"' + ' ' + cond['symbol'] + ' ' +
+                                                (f"'{cond['value']}'" if not str(cond['value']).isdigit() else str(cond['value']))
+                                                for cond in where)
+        else:
+            whereClause = ""
+
+        # Construct the SQL query with the specified table, columns, and WHERE clause
+        sql = f"SELECT {columns} FROM {tableName} {whereClause}"
+
+        # Execute the SQL query and retrieve the data as a Pandas DataFrame
+        df = self.ora_hook.get_pandas_df(sql)
+        print("Used SQL statement: ", sql)
+
+        # Convert the DataFrame to a list of tuples representing the rows in the table
         return list(df.itertuples(index=False))
 
+
     def get_column_names(self, tableName):
         """
         Gets all column names of the given table using COLUMN_NAME
 
         :param table_name: The name of the table to read from.
 
         :return: A list of ColumnNames representing the columns in the table.
@@ -87,7 +112,9 @@
         print(f"Finding Oracle columns with: {tableName}")
         columns_query = f"SELECT COLUMN_NAME FROM ALL_TAB_COLUMNS WHERE TABLE_NAME = '{tableName.upper()}'"
         with self.ora_hook.get_conn() as conn:
             with conn.cursor() as cur:
                 cur.execute(columns_query)
                 column_names = [row[0] for row in cur.fetchall()]
         return column_names
+
+
```

### Comparing `abuscom-libs-0.1.3/abuscom/connectors/planio.py` & `abuscom-libs-0.1.4/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.3/setup.py` & `abuscom-libs-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.3',
+    version='0.1.4',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

