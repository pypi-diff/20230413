# Comparing `tmp/dagster-snowflake-pyspark-0.18.6.tar.gz` & `tmp/dagster-snowflake-pyspark-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pyspark-0.18.6.tar", last modified: Thu Apr  6 00:30:15 2023, max compression
+gzip compressed data, was "dagster-snowflake-pyspark-0.18.7.tar", last modified: Thu Apr 13 15:12:14 2023, max compression
```

## Comparing `dagster-snowflake-pyspark-0.18.6.tar` & `dagster-snowflake-pyspark-0.18.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:30:15.857028 dagster-snowflake-pyspark-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-06 00:30:15.857028 dagster-snowflake-pyspark-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:30:15.857028 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)     6079 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:30:15.857028 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-06 00:30:15.000000 dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-06 00:30:15.857028 dagster-snowflake-pyspark-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2023-04-05 23:51:52.000000 dagster-snowflake-pyspark-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:14.693472 dagster-snowflake-pyspark-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:12:14.693472 dagster-snowflake-pyspark-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:14.693472 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9146 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:14.693472 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 15:12:14.000000 dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-13 15:12:14.697472 dagster-snowflake-pyspark-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-13 15:03:07.000000 dagster-snowflake-pyspark-0.18.7/setup.py
```

### Comparing `dagster-snowflake-pyspark-0.18.6/LICENSE` & `dagster-snowflake-pyspark-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.18.6/PKG-INFO` & `dagster-snowflake-pyspark-0.18.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py` & `dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Mapping
+from typing import Mapping, Optional, Sequence, Type
 
 import dagster._check as check
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.definitions.metadata import RawMetadataValue
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
-from dagster_snowflake import build_snowflake_io_manager
+from dagster_snowflake import SnowflakeIOManager, build_snowflake_io_manager
 from dagster_snowflake.snowflake_io_manager import SnowflakeDbClient
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
 
 SNOWFLAKE_CONNECTOR = "net.snowflake.spark.snowflake"
 
 
@@ -32,38 +32,37 @@
 
 class SnowflakePySparkTypeHandler(DbTypeHandler[DataFrame]):
     """Plugin for the Snowflake I/O Manager that can store and load PySpark DataFrames as Snowflake tables.
 
     Examples:
         .. code-block:: python
 
-            from dagster_snowflake import build_snowflake_io_manager
+            from dagster_snowflake import SnowflakeIOManager
+            from dagster_snowflake_pandas import SnowflakePandasTypeHandler
             from dagster_snowflake_pyspark import SnowflakePySparkTypeHandler
-            from pyspark.sql import DataFrame
-            from dagster import Definitions
+            from dagster import Definitions, EnvVar
 
-            snowflake_io_manager = build_snowflake_io_manager([SnowflakePySparkTypeHandler()])
+            class MySnowflakeIOManager(SnowflakeIOManager):
+                @staticmethod
+                def type_handlers() -> Sequence[DbTypeHandler]:
+                    return [SnowflakePandasTypeHandler(), SnowflakePySparkTypeHandler()]
 
-            @asset
-            def my_asset() -> DataFrame:
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in snowflake
+            )
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
                 ...
 
             defs = Definitions(
-                assets=[my_asset],
+                assets=[my_table],
                 resources={
-                    "io_manager": snowflake_io_manager.configured(...)
+                    "io_manager": MySnowflakeIOManager(database="MY_DATABASE", account=EnvVar("SNOWFLAKE_ACCOUNT"), warehouse="my_warehouse", ...)
                 }
             )
 
-            # OR
-
-            @job(resource_defs={'io_manager': snowflake_io_manager})
-            def my_job():
-                ...
-
     """
 
     def handle_output(
         self, context: OutputContext, table_slice: TableSlice, obj: DataFrame, _
     ) -> Mapping[str, RawMetadataValue]:
         options = _get_snowflake_options(context.resource_config, table_slice)
 
@@ -104,15 +103,15 @@
         return [DataFrame]
 
 
 snowflake_pyspark_io_manager = build_snowflake_io_manager(
     [SnowflakePySparkTypeHandler()], default_load_type=DataFrame
 )
 snowflake_pyspark_io_manager.__doc__ = """
-An IO manager definition that reads inputs from and writes PySpark DataFrames to Snowflake. When
+An I/O manager definition that reads inputs from and writes PySpark DataFrames to Snowflake. When
 using the snowflake_pyspark_io_manager, any inputs and outputs without type annotations will be loaded
 as PySpark DataFrames.
 
 Returns:
     IOManagerDefinition
 
 Examples:
@@ -141,15 +140,15 @@
                 })
             }
         )
 
     Note that the warehouse configuration value is required when using the snowflake_pyspark_io_manager
 
     If you do not provide a schema, Dagster will determine a schema based on the assets and ops using
-    the IO Manager. For assets, the schema will be determined from the asset key.
+    the I/O Manager. For assets, the schema will be determined from the asset key.
     For ops, the schema can be specified by including a "schema" entry in output metadata. If "schema" is not provided
     via config or on the asset/op, "public" will be used for the schema.
 
     .. code-block:: python
 
         @op(
             out={"my_table": Out(metadata={"schema": "my_schema"})}
@@ -167,7 +166,80 @@
             ins={"my_table": AssetIn("my_table", metadata={"columns": ["a"]})}
         )
         def my_table_a(my_table: DataFrame) -> DataFrame:
             # my_table will just contain the data from column "a"
             ...
 
 """
+
+
+class SnowflakePySparkIOManager(SnowflakeIOManager):
+    """An I/O manager definition that reads inputs from and writes PySpark DataFrames to Snowflake. When
+    using the SnowflakePySparkIOManager, any inputs and outputs without type annotations will be loaded
+    as PySpark DataFrames.
+
+    Returns:
+        IOManagerDefinition
+
+    Examples:
+        .. code-block:: python
+
+            from dagster_snowflake_pyspark import SnowflakePySparkIOManager
+            from pyspark.sql import DataFrame
+            from dagster import Definitions, EnvVar
+
+            @asset(
+                key_prefix=["my_schema"]  # will be used as the schema in snowflake
+            )
+            def my_table() -> DataFrame:  # the name of the asset will be the table name
+                ...
+
+            defs = Definitions(
+                assets=[my_table],
+                resources={
+                    "io_manager": SnowflakePySparkIOManager(
+                        database="my_database",
+                        warehouse="my_warehouse", # required for SnowflakePySparkIOManager
+                        account=EnvVar("SNOWFLAKE_ACCOUNT"),
+                        password=EnvVar("SNOWFLAKE_PASSWORD"),
+                        ...
+                    )
+                }
+            )
+
+        Note that the warehouse configuration value is required when using the SnowflakePySparkIOManager
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
+            def make_my_table() -> DataFrame:
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
+            def my_table_a(my_table: DataFrame) -> DataFrame:
+                # my_table will just contain the data from column "a"
+                ...
+
+    """
+
+    @staticmethod
+    def type_handlers() -> Sequence[DbTypeHandler]:
+        return [SnowflakePySparkTypeHandler()]
+
+    @staticmethod
+    def default_load_type() -> Optional[Type]:
+        return DataFrame
```

### Comparing `dagster-snowflake-pyspark-0.18.6/dagster_snowflake_pyspark.egg-info/PKG-INFO` & `dagster-snowflake-pyspark-0.18.7/dagster_snowflake_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.18.6/setup.py` & `dagster-snowflake-pyspark-0.18.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-snowflake==0.18.6",
+        "dagster==1.2.7",
+        "dagster-snowflake==0.18.7",
         "pyspark",
         "requests",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
 )
```

