# Comparing `tmp/dagster-duckdb-polars-0.18.6.tar.gz` & `tmp/dagster-duckdb-polars-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.18.6.tar", last modified: Thu Apr  6 00:28:25 2023, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.18.7.tar", last modified: Thu Apr 13 15:13:57 2023, max compression
```

## Comparing `dagster-duckdb-polars-0.18.6.tar` & `dagster-duckdb-polars-0.18.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:25.876330 dagster-duckdb-polars-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-06 00:28:25.876330 dagster-duckdb-polars-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:25.876330 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4847 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:25.876330 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-06 00:28:25.000000 dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-06 00:28:25.876330 dagster-duckdb-polars-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-05 23:51:52.000000 dagster-duckdb-polars-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/setup.py
```

### Comparing `dagster-duckdb-polars-0.18.6/LICENSE` & `dagster-duckdb-polars-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.18.6/PKG-INFO` & `dagster-duckdb-polars-0.18.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.18.6/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+from typing import Optional, Sequence, Type
+
 import polars as pl
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
-from dagster_duckdb.io_manager import DuckDbClient, build_duckdb_io_manager
+from dagster_duckdb.io_manager import DuckDbClient, DuckDBIOManager, build_duckdb_io_manager
 
 
 class DuckDBPolarsTypeHandler(DbTypeHandler[pl.DataFrame]):
     """Stores and loads Polars DataFrames in DuckDB.
 
-    To use this type handler, pass it to ``build_duckdb_io_manager``
+    To use this type handler, return it from the ``type_handlers` method of an I/O manager that inherits from ``DuckDBIOManager``.
 
     Example:
         .. code-block:: python
 
-            from dagster_duckdb import build_duckdb_io_manager
+            from dagster_duckdb import DuckDBIOManager
             from dagster_duckdb_polars import DuckDBPolarsTypeHandler
 
-            @asset
-            def my_table():
-                ...
+            class MyDuckDBIOManager(DuckDBIOManager):
+                @staticmethod
+                def type_handlers() -> Sequence[DbTypeHandler]:
+                    return [DuckDBPolarsTypeHandler()]
 
-            duckdb_io_manager = build_duckdb_io_manager([DuckDBPolarsTypeHandler()])
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in duckdb
+            )
+            def my_table() -> pl.DataFrame:  # the name of the asset will be the table name
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
         self, context: OutputContext, table_slice: TableSlice, obj: pl.DataFrame, connection
     ):
         """Stores the polars DataFrame in duckdb."""
@@ -77,15 +82,15 @@
         return [pl.DataFrame]
 
 
 duckdb_polars_io_manager = build_duckdb_io_manager(
     [DuckDBPolarsTypeHandler()], default_load_type=pl.DataFrame
 )
 duckdb_polars_io_manager.__doc__ = """
-An IO manager definition that reads inputs from and writes polars dataframes to DuckDB. When
+An I/O manager definition that reads inputs from and writes polars dataframes to DuckDB. When
 using the duckdb_polars_io_manager, any inputs and outputs without type annotations will be loaded
 as Polars DataFrames.
 
 Returns:
     IOManagerDefinition
 
 Examples:
@@ -104,15 +109,15 @@
         def my_repo():
             return with_resources(
                 [my_table],
                 {"io_manager": duckdb_polars_io_manager.configured({"database": "my_db.duckdb"})}
             )
 
     If you do not provide a schema, Dagster will determine a schema based on the assets and ops using
-    the IO Manager. For assets, the schema will be determined from the asset key.
+    the I/O Manager. For assets, the schema will be determined from the asset key.
     For ops, the schema can be specified by including a "schema" entry in output metadata. If "schema" is not provided
     via config or on the asset/op, "public" will be used for the schema.
 
     .. code-block:: python
 
         @op(
             out={"my_table": Out(metadata={"schema": "my_schema"})}
@@ -130,7 +135,68 @@
             ins={"my_table": AssetIn("my_table", metadata={"columns": ["a"]})}
         )
         def my_table_a(my_table: pl.DataFrame) -> pl.DataFrame:
             # my_table will just contain the data from column "a"
             ...
 
 """
+
+
+class DuckDBPolarsIOManager(DuckDBIOManager):
+    """An I/O manager definition that reads inputs from and writes Polars DataFrames to DuckDB. When
+    using the DuckDBPolarsIOManager, any inputs and outputs without type annotations will be loaded
+    as Polars DataFrames.
+
+    Returns:
+        IOManagerDefinition
+
+    Examples:
+        .. code-block:: python
+
+            from dagster_duckdb_polars import DuckDBPolarsIOManager
+
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in DuckDB
+            )
+            def my_table() -> pl.DataFrame:  # the name of the asset will be the table name
+                ...
+
+            defs = Definitions(
+                assets=[my_table],
+                resources={"io_manager": DuckDBPolarsIOManager(database="my_db.duckdb")}
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
+            def make_my_table() -> pl.DataFrame:
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
+            def my_table_a(my_table: pl.DataFrame) -> pl.DataFrame:
+                # my_table will just contain the data from column "a"
+                ...
+
+    """
+
+    @staticmethod
+    def type_handlers() -> Sequence[DbTypeHandler]:
+        return [DuckDBPolarsTypeHandler()]
+
+    @staticmethod
+    def default_load_type() -> Optional[Type]:
+        return pl.DataFrame
```

### Comparing `dagster-duckdb-polars-0.18.6/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.18.6/setup.py` & `dagster-duckdb-polars-0.18.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-duckdb==0.18.6",
+        "dagster==1.2.7",
+        "dagster-duckdb==0.18.7",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

