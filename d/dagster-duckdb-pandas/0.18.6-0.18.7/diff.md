# Comparing `tmp/dagster-duckdb-pandas-0.18.6.tar.gz` & `tmp/dagster-duckdb-pandas-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.18.6.tar", last modified: Thu Apr  6 00:31:49 2023, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.18.7.tar", last modified: Thu Apr 13 15:15:49 2023, max compression
```

## Comparing `dagster-duckdb-pandas-0.18.6.tar` & `dagster-duckdb-pandas-0.18.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:31:49.617628 dagster-duckdb-pandas-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-06 00:31:49.617628 dagster-duckdb-pandas-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:31:49.617628 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4516 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:31:49.617628 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-06 00:31:49.000000 dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-06 00:31:49.617628 dagster-duckdb-pandas-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-05 23:51:52.000000 dagster-duckdb-pandas-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:49.605836 dagster-duckdb-pandas-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:15:49.605836 dagster-duckdb-pandas-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:49.605836 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:15:49.605836 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:15:49.000000 dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-13 15:15:49.605836 dagster-duckdb-pandas-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-13 15:03:07.000000 dagster-duckdb-pandas-0.18.7/setup.py
```

### Comparing `dagster-duckdb-pandas-0.18.6/LICENSE` & `dagster-duckdb-pandas-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.18.6/PKG-INFO` & `dagster-duckdb-pandas-0.18.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,45 @@
+from typing import Optional, Sequence, Type
+
 import pandas as pd
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
-from dagster_duckdb.io_manager import DuckDbClient, build_duckdb_io_manager
+from dagster_duckdb.io_manager import (
+    DuckDbClient,
+    DuckDBIOManager,
+    build_duckdb_io_manager,
+)
 
 
 class DuckDBPandasTypeHandler(DbTypeHandler[pd.DataFrame]):
     """Stores and loads Pandas DataFrames in DuckDB.
 
-    To use this type handler, pass it to ``build_duckdb_io_manager``
+    To use this type handler, return it from the ``type_handlers` method of an I/O manager that inherits from ``DuckDBIOManager``.
 
     Example:
         .. code-block:: python
 
-            from dagster_duckdb import build_duckdb_io_manager
+            from dagster_duckdb import DuckDBIOManager
             from dagster_duckdb_pandas import DuckDBPandasTypeHandler
 
-            @asset
-            def my_table():
-                ...
+            class MyDuckDBIOManager(DuckDBIOManager):
+                @staticmethod
+                def type_handlers() -> Sequence[DbTypeHandler]:
+                    return [DuckDBPandasTypeHandler()]
 
-            duckdb_io_manager = build_duckdb_io_manager([DuckDBPandasTypeHandler()])
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in duckdb
+            )
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
+                ...
 
-            @repository
-            def my_repo():
-                return with_resources(
-                    [my_table],
-                    {"io_manager": duckdb_io_manager.configured({"database": "my_db.duckdb"})}
-                )
+            defs = Definitions(
+                assets=[my_table],
+                resources={"io_manager": MyDuckDBIOManager(database="my_db.duckdb")}
+            )
 
     """
 
     def handle_output(
         self, context: OutputContext, table_slice: TableSlice, obj: pd.DataFrame, connection
     ):
         """Stores the pandas DataFrame in duckdb."""
@@ -71,15 +80,15 @@
         return [pd.DataFrame]
 
 
 duckdb_pandas_io_manager = build_duckdb_io_manager(
     [DuckDBPandasTypeHandler()], default_load_type=pd.DataFrame
 )
 duckdb_pandas_io_manager.__doc__ = """
-An IO manager definition that reads inputs from and writes Pandas DataFrames to DuckDB. When
+An I/O manager definition that reads inputs from and writes Pandas DataFrames to DuckDB. When
 using the duckdb_pandas_io_manager, any inputs and outputs without type annotations will be loaded
 as Pandas DataFrames.
 
 Returns:
     IOManagerDefinition
 
 Examples:
@@ -98,15 +107,15 @@
         def my_repo():
             return with_resources(
                 [my_table],
                 {"io_manager": duckdb_pandas_io_manager.configured({"database": "my_db.duckdb"})}
             )
 
     If you do not provide a schema, Dagster will determine a schema based on the assets and ops using
-    the IO Manager. For assets, the schema will be determined from the asset key.
+    the I/O Manager. For assets, the schema will be determined from the asset key.
     For ops, the schema can be specified by including a "schema" entry in output metadata. If "schema" is not provided
     via config or on the asset/op, "public" will be used for the schema.
 
     .. code-block:: python
 
         @op(
             out={"my_table": Out(metadata={"schema": "my_schema"})}
@@ -124,7 +133,68 @@
             ins={"my_table": AssetIn("my_table", metadata={"columns": ["a"]})}
         )
         def my_table_a(my_table: pd.DataFrame) -> pd.DataFrame:
             # my_table will just contain the data from column "a"
             ...
 
 """
+
+
+class DuckDBPandasIOManager(DuckDBIOManager):
+    """An I/O manager definition that reads inputs from and writes Pandas DataFrames to DuckDB. When
+    using the DuckDBPandasIOManager, any inputs and outputs without type annotations will be loaded
+    as Pandas DataFrames.
+
+    Returns:
+        IOManagerDefinition
+
+    Examples:
+        .. code-block:: python
+
+            from dagster_duckdb_pandas import DuckDBPandasIOManager
+
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in DuckDB
+            )
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
+                ...
+
+            defs = Definitions(
+                assets=[my_table],
+                resources={"io_manager": DuckDBPandasIOManager(database="my_db.duckdb")}
+            )
+
+        If you do not provide a schema, Dagster will determine a schema based on the assets and ops using
+        the I/O Manager. For assets, the schema will be determined from the asset key, as in the above example.
+        For ops, the schema can be specified by including a "schema" entry in output metadata. If "schema" is not provided
+        via config or on the asset/op, "public" will be used for the schema.
+
+        .. code-block:: python
+
+            @op(
+                out={"my_table": Out(metadata={"schema": "my_schema"})}
+            )
+            def make_my_table() -> pd.DataFrame:
+                # the returned value will be stored at my_schema.my_table
+                ...
+
+        To only use specific columns of a table as input to a downstream op or asset, add the metadata "columns" to the
+        In or AssetIn.
+
+        .. code-block:: python
+
+            @asset(
+                ins={"my_table": AssetIn("my_table", metadata={"columns": ["a"]})}
+            )
+            def my_table_a(my_table: pd.DataFrame) -> pd.DataFrame:
+                # my_table will just contain the data from column "a"
+                ...
+
+    """
+
+    @staticmethod
+    def type_handlers() -> Sequence[DbTypeHandler]:
+        return [DuckDBPandasTypeHandler()]
+
+    @staticmethod
+    def default_load_type() -> Optional[Type]:
+        return pd.DataFrame
```

### Comparing `dagster-duckdb-pandas-0.18.6/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.18.7/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pandas-0.18.6/setup.py` & `dagster-duckdb-pandas-0.18.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-duckdb==0.18.6",
+        "dagster==1.2.7",
+        "dagster-duckdb==0.18.7",
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     zip_safe=False,
 )
```

