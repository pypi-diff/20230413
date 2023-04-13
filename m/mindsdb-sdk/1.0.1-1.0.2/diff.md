# Comparing `tmp/mindsdb_sdk-1.0.1.tar.gz` & `tmp/mindsdb_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_sdk-1.0.1.tar", last modified: Mon Apr  3 15:15:45 2023, max compression
+gzip compressed data, was "dist/mindsdb_sdk-1.0.2.tar", last modified: Thu Apr 13 15:09:53 2023, max compression
```

## Comparing `mindsdb_sdk-1.0.1.tar` & `mindsdb_sdk-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/connectors/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/mindsdb_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:15:45.000000 mindsdb_sdk-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-03 15:15:31.000000 mindsdb_sdk-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/setup.py
```

### Comparing `mindsdb_sdk-1.0.1/PKG-INFO` & `mindsdb_sdk-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: mindsdb_sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
-        It enables you to connect to a midnsDB server and use it in a similar way to mindsb_native.
+        It enables you to connect to a MidnsDB server from python using HTTP API.
         
         ## Install
         ```
         pip install mindsdb_sdk
         ```
         
-        ## Example 
+        ## Example
         
         Connect:
         ```python
         import mindsdb_sdk
         
         # Connect to local server 
         
         server = mindsdb_sdk.connect()
         server = mindsdb_sdk.connect('http://127.0.0.1:47334')
         
         # Connect to cloud server
         
         server = mindsdb_sdk.connect(email='a@b.com', password='-')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='a@b.com', password='-')
+        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
+        
+        # Connect to MindsDB Pro
+        
+        server = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
+        
         ```
         
         Base usage:
         ```python
         
         # database
         databases = server.list_databases()
@@ -78,14 +83,18 @@
               'rentals_model',
               predict='price',
               query=query,
         )
         
         ```
         
+        More examples in [Google colab notebook](
+        https://colab.research.google.com/drive/1QouwAR3saFb9ffthrIs1LSH5COzyQa11#scrollTo=k6IbwsKRPQCR
+        )
+        
         ## API documentation
         
         Generating:
         
         ```commandline
         pip install sphinx
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/__init__.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 
 from mindsdb_sdk.__about__ import __package_name__ as name, __version__
 
 from .server import Server
 
 
-def connect(url: str = None, email: str = None, password: str = None) -> Server:
+def connect(url: str = None, login: str = None, password: str = None, is_managed: bool = False) -> Server:
     """
     Create connection to mindsdb server
 
     :param url: url to mindsdb server
-    :param email: user email to login (for cloud version)
+    :param login: user login, for cloud version it contents email
     :param password: user password to login (for cloud version)
+    :param is_managed: whether or not the URL points to a managed instance
     :return: Server object
 
     Examples
     --------
 
     >>> import mindsdb_sdk
 
     Connect to local server
 
     >>> server = mindsdb_sdk.connect()
     >>> server = mindsdb_sdk.connect('http://127.0.0.1:47334')
 
     Connect to cloud server
 
-    >>> server = mindsdb_sdk.connect(email='a@b.com', password='-')
-    >>> server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='a@b.com', password='-')
+    >>> server = mindsdb_sdk.connect(login='a@b.com', password='-')
+    >>> server = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
 
-    """
+    Connect to MindsDB pro
+
+    >>> server = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
 
+    """
     if url is None:
-        if email is not None:
+        if login is not None:
             # default is cloud
             url = 'https://cloud.mindsdb.com'
         else:
             # is local
             url = 'http://127.0.0.1:47334'
 
-    return Server(url=url, email=email, password=password)
+    return Server(url=url, login=login, password=password, is_managed=is_managed)
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/connectors/rest_api.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/rest_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import wraps
 
 import requests
 import pandas as pd
 
 
 def _try_relogin(fnc):
-    wraps(fnc)
+    @wraps(fnc)
     def wrapper(self, *args, **kwargs):
         try:
             return fnc(self, *args, **kwargs)
         except requests.HTTPError as e:
             if e.response.status_code != 401:
                 raise e
 
@@ -20,28 +20,45 @@
                 raise e
             # call once more
             return fnc(self, *args, **kwargs)
     return wrapper
 
 
 class RestAPI:
-    def __init__(self, url=None, email=None, password=None):
+    def __init__(self, url=None, login=None, password=None, is_managed=False):
 
         self.url = url
-        self.email = email
+        self.username = login
         self.password = password
+        self.is_managed = is_managed
         self.session = requests.Session()
 
-        if email is not None:
+        if login is not None:
             self.login()
 
     def login(self):
-        url = self.url + '/cloud/login'
-        json = {'email': self.email, 'password': self.password}
+        managed_endpoint = '/api/login'
+        cloud_endpoint = '/cloud/login'
+
+        if self.is_managed:
+            json = {'password': self.password, 'username': self.username}
+            url = self.url + managed_endpoint
+        else:
+            json = {'password': self.password, 'email': self.username}
+            url = self.url + cloud_endpoint
         r = self.session.post(url, json=json)
+
+        # failback when is using managed instance with is_managed=False
+        if r.status_code in (405, 404) and self.is_managed is False:
+            # try managed instance login
+
+            json = {'password': self.password, 'username': self.username}
+            url = self.url + managed_endpoint
+            r = self.session.post(url, json=json)
+
         r.raise_for_status()
 
     @_try_relogin
     def sql_query(self, sql, database=None, lowercase_columns=False):
         if database is None:
             database = 'mindsdb'
         url = self.url + '/api/sql/query'
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/database.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     Wortking with tables:
     Get table as Query object
 
     >>> table = database.get_table('table1')
 
     Filter and limit
 
-    >>> table.filter(a=1, b='2')
-    >>> table.limit(3)
+    >>> table = table.filter(a=1, b='2')
+    >>> table = table.limit(3)
 
     Get content of table as dataframe. At that moment query will be sent on server and executed
 
     >>> df = table.fetch()
 
     Creating table
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/model.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Union
 
 import pandas as pd
 
-from mindsdb_sql.parser.dialects.mindsdb import RetrainPredictor, AdjustPredictor
+from mindsdb_sql.parser.dialects.mindsdb import RetrainPredictor, FinetunePredictor
 from mindsdb_sql.parser.ast import Identifier, Select, Star, Join, Update, Describe, Constant
 from mindsdb_sql import parse_sql
 from mindsdb_sql.planner.utils import query_traversal
 
 from mindsdb_sdk.utils import dict_to_binary_op
 from mindsdb_sdk.query import Query
 
@@ -47,47 +47,59 @@
         :param data: dataframe or Query object as input to predictor
         :param params: parameters for predictor, optional
         :return: dataframe with result of prediction
         """
         if isinstance(data, Query):
             # create join from select if it is simple select
             ast_query = parse_sql(data.sql, dialect='mindsdb')
-            if isinstance(ast_query, Select) and isinstance(ast_query.from_table, Identifier):
-                # inject aliases
-                if ast_query.from_table.alias is None:
-                    alias = 't'
-                    ast_query.from_table.alias = Identifier(alias)
-                else:
-                    alias = ast_query.from_table.alias.parts[-1]
-
-                def inject_alias(node, is_table, **kwargs):
-                    if not is_table:
-                        if isinstance(node, Identifier):
-                            if node.parts[0] != alias:
-                                node.parts.insert(0, alias)
 
-                query_traversal(ast_query, inject_alias)
-
-                # replace table with join
-                ast_query.from_table = Join(
+            # injection of join disabled yet
+            # if isinstance(ast_query, Select) and isinstance(ast_query.from_table, Identifier):
+            #     # inject aliases
+            #     if ast_query.from_table.alias is None:
+            #         alias = 't'
+            #         ast_query.from_table.alias = Identifier(alias)
+            #     else:
+            #         alias = ast_query.from_table.alias.parts[-1]
+            #
+            #     def inject_alias(node, is_table, **kwargs):
+            #         if not is_table:
+            #             if isinstance(node, Identifier):
+            #                 if node.parts[0] != alias:
+            #                     node.parts.insert(0, alias)
+            #
+            #     query_traversal(ast_query, inject_alias)
+            #
+            #     # replace table with join
+            #     model_identifier = self._get_identifier()
+            #     model_identifier.alias = Identifier('m')
+            #
+            #     ast_query.from_table = Join(
+            #         join_type='join',
+            #         left=ast_query.from_table,
+            #         right=model_identifier
+            #     )
+            #
+            #     # select only model columns
+            #     ast_query.targets = [Identifier(parts=['m', Star()])]
+            #
+
+            # wrap query to subselect
+            model_identifier = self._get_identifier()
+            model_identifier.alias = Identifier('m')
+
+            ast_query.parentheses = True
+            ast_query = Select(
+                targets=[Identifier(parts=['m', Star()])],
+                from_table=Join(
                     join_type='join',
-                    left=ast_query.from_table,
-                    right=self._get_identifier()
-                )
-            else:
-                # wrap query to subselect
-                ast_query.parentheses = True
-                ast_query = Select(
-                    targets=[Star()],
-                    from_table=Join(
-                        join_type='join',
-                        left=ast_query,
-                        right=self._get_identifier()
-                    )
+                    left=ast_query,
+                    right=model_identifier
                 )
+            )
             if params is not None:
                 ast_query.using = params
             # execute in query's database
             return self.project.api.sql_query(ast_query.to_string(), database=data.database)
 
         elif isinstance(data, pd.DataFrame):
             return self.project.api.model_predict(self.project.name, self.name, data,
@@ -111,29 +123,29 @@
 
         :return: model data
         """
         model = self.project.get_model(self.name, self.version)
         self.data = model.data
         return self.data
 
-    def adjust(self,
+    def finetune(self,
                query: Union[str, Query] = None,
                database: str = None,
                options: dict = None,
                engine: str = None) -> Union[Model, ModelVersion]:
         """
-        Call adjust of the model
+        Call finetune of the model
 
-        :param query: sql string or Query object to get data for adjusting, optional
-        :param database: database to get data for adjusting, optional
-        :param options: parameters for adjusting model, optional
+        :param query: sql string or Query object to get data for fine-tuning, optional
+        :param database: database to get data for fine-tuning, optional
+        :param options: parameters for fine-tuning model, optional
         :param engine: ml engine, optional
         :return: Model object
         """
-        return self._retrain(ast_class=AdjustPredictor,
+        return self._retrain(ast_class=FinetunePredictor,
                              query=query, database=database,
                              options=options, engine=engine)
 
     def retrain(self,
                query: Union[str, Query] = None,
                database: str = None,
                options: dict = None,
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/project.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     >>> view = project.create_view(
     ...   'view1',
     ...   query=database.query('select * from table1')
     ...)
 
     Getting data:
 
-    >>> view.filter(a=1, b=2)
-    >>> view.limit(100)
+    >>> view = view.filter(a=1, b=2)
+    >>> view = view.limit(100)
     >>> df = view.fetch()
 
     Drop view:
 
     >>> project.drop_view('view1')
 
 
@@ -191,19 +191,19 @@
     ...   AND t.bedrooms=2
     ...  LIMIT 4;
     ...''').fetch()
 
 
     Model managing
 
-    Adjusting
+    Fine-tuning
 
-    >>> model.adjust(query)
-    >>> model.adjust('select * from demo_data.house_sales', database='example_db')
-    >>> model.adjust(query, params={'x': 2})
+    >>> model.finetune(query)
+    >>> model.finetune('select * from demo_data.house_sales', database='example_db')
+    >>> model.finetune(query, params={'x': 2})
 
     Retraining
 
     >>> model.retrain(query)
     >>> model.retrain('select * from demo_data.house_sales', database='example_db')
     >>> model.retrain(query, params={'x': 2})
 
@@ -342,15 +342,15 @@
         df = df.rename(columns=cols_map)
 
         return [
             model_class(self, item)
             for item in df.to_dict('records')
         ]
 
-    def create_model(self, name: str, predict: str, engine: str = None,
+    def create_model(self, name: str, predict: str = None, engine: str = None,
                      query: Union[str, Query] = None, database: str = None,
                      options: dict = None, timeseries_options: dict = None) -> Model:
         """
         Create new model in project and return it
 
         If query/database is passed, it will be executed on mindsdb side
 
@@ -368,19 +368,23 @@
             query = query.sql
         elif isinstance(query, pd.DataFrame):
             raise NotImplementedError('Dataframe as input for training model is not supported yet')
 
         if database is not None:
             database = Identifier(database)
 
+        if predict is not None:
+            targets = [Identifier(predict)]
+        else:
+            targets = None
         ast_query = CreatePredictor(
             name=Identifier(name),
             query_str=query,
             integration_name=database,
-            targets=[Identifier(predict)],
+            targets=targets,
         )
 
         if timeseries_options is not None:
             if 'group' in timeseries_options:
                 group = timeseries_options['group']
                 if not isinstance(group, list):
                     group = [group]
@@ -391,15 +395,15 @@
                 ast_query.window = timeseries_options['window']
             if 'horizon' in timeseries_options:
                 ast_query.horizon = timeseries_options['horizon']
         if options is None:
             options = {}
         if engine is not None:
             options['engine'] = engine
-
+        ast_query.using = options
         df = self.query(ast_query.to_string()).fetch()
         if len(df) > 0:
             data = dict(df.iloc[0])
             # to lowercase
             data = {k.lower(): v for k,v in data.items()}
 
             return Model(self, data)
@@ -485,15 +489,15 @@
         if len(jobs) == 1:
             return jobs[0]
         elif len(jobs) == 0:
             raise AttributeError("Job doesn't exist")
         else:
             raise RuntimeError("Several jobs with the same name")
 
-    def create_job(self, name: str, query_str:str,
+    def create_job(self, name: str, query_str: str,
                    start_at: dt.datetime = None, end_at: dt.datetime = None,
                    repeat_str: str = None) -> Union[Job, None]:
         """
         Create new job in project and return it.
         If it is not possible (job executed and not accessible anymore): return None
         More info: https://docs.mindsdb.com/sql/create/jobs
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/query.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import copy
+
 import pandas as pd
 
 from mindsdb_sql.parser.ast import Select, Star, Identifier, Constant
 
 from mindsdb_sdk.utils import dict_to_binary_op
 
 
@@ -53,25 +55,30 @@
         """
         Applies filters on table
         table.filter(a=1, b=2) adds where condition to table:
         'select * from table1 where a=1 and b=2'
 
         :param kwargs: filter
         """
-        self._filters.update(kwargs)
-        self._update_query()
+        # creates new object
+        query = copy.deepcopy(self)
+        query._filters.update(kwargs)
+        query._update_query()
+        return query
 
     def limit(self, val: int):
         """
         Applies limit condition to table query
 
         :param val: limit size
         """
-        self._limit = val
-        self._update_query()
+        query = copy.deepcopy(self)
+        query._limit = val
+        query._update_query()
+        return query
 
     def _update_query(self):
         ast_query = Select(
             targets=[Star()],
             from_table=Identifier(self.name),
             where=dict_to_binary_op(self._filters)
         )
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk/server.py` & `mindsdb_sdk-1.0.2/mindsdb_sdk/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
     >>> project = server.get_project('proj')
 
     >>> project = server.get_project()  # default is mindsdb project
 
     """
 
-    def __init__(self, url: str = None, email: str = None, password: str = None):
-        self.api = RestAPI(url, email, password)
+    def __init__(self, url: str = None, login: str = None, password: str = None, is_managed: bool = False):
+        self.api = RestAPI(url, login, password, is_managed)
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.api.url})'
 
     def _list_databases(self):
         data = self.api.sql_query(
             "select NAME from information_schema.databases where TYPE='data'"
```

### Comparing `mindsdb_sdk-1.0.1/mindsdb_sdk.egg-info/PKG-INFO` & `mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: mindsdb-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
-        It enables you to connect to a midnsDB server and use it in a similar way to mindsb_native.
+        It enables you to connect to a MidnsDB server from python using HTTP API.
         
         ## Install
         ```
         pip install mindsdb_sdk
         ```
         
-        ## Example 
+        ## Example
         
         Connect:
         ```python
         import mindsdb_sdk
         
         # Connect to local server 
         
         server = mindsdb_sdk.connect()
         server = mindsdb_sdk.connect('http://127.0.0.1:47334')
         
         # Connect to cloud server
         
         server = mindsdb_sdk.connect(email='a@b.com', password='-')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='a@b.com', password='-')
+        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
+        
+        # Connect to MindsDB Pro
+        
+        server = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
+        
         ```
         
         Base usage:
         ```python
         
         # database
         databases = server.list_databases()
@@ -78,14 +83,18 @@
               'rentals_model',
               predict='price',
               query=query,
         )
         
         ```
         
+        More examples in [Google colab notebook](
+        https://colab.research.google.com/drive/1QouwAR3saFb9ffthrIs1LSH5COzyQa11#scrollTo=k6IbwsKRPQCR
+        )
+        
         ## API documentation
         
         Generating:
         
         ```commandline
         pip install sphinx
```

### Comparing `mindsdb_sdk-1.0.1/setup.py` & `mindsdb_sdk-1.0.2/setup.py`

 * *Files identical despite different names*

