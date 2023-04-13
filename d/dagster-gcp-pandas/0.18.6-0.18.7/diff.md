# Comparing `tmp/dagster-gcp-pandas-0.18.6.tar.gz` & `tmp/dagster-gcp-pandas-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.18.6.tar", last modified: Thu Apr  6 00:27:39 2023, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.18.7.tar", last modified: Thu Apr 13 15:13:46 2023, max compression
```

## Comparing `dagster-gcp-pandas-0.18.6.tar` & `dagster-gcp-pandas-0.18.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-06 00:27:39.000000 dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-06 00:27:39.524037 dagster-gcp-pandas-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-05 23:51:52.000000 dagster-gcp-pandas-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:46.125617 dagster-gcp-pandas-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-13 15:13:46.125617 dagster-gcp-pandas-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:46.125617 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:46.125617 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9688 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:46.125617 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-13 15:13:46.000000 dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-13 15:13:46.129617 dagster-gcp-pandas-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-13 15:03:07.000000 dagster-gcp-pandas-0.18.7/setup.py
```

### Comparing `dagster-gcp-pandas-0.18.6/LICENSE` & `dagster-gcp-pandas-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.18.6/PKG-INFO` & `dagster-gcp-pandas-0.18.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-gcp-pandas-0.18.6/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.18.7/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+from typing import Optional, Sequence, Type
+
 import pandas as pd
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
-from dagster_gcp.bigquery.io_manager import BigQueryClient, build_bigquery_io_manager
+from dagster_gcp.bigquery.io_manager import (
+    BigQueryClient,
+    BigQueryIOManager,
+    build_bigquery_io_manager,
+)
 
 
 class BigQueryPandasTypeHandler(DbTypeHandler[pd.DataFrame]):
     """Plugin for the BigQuery I/O Manager that can store and load Pandas DataFrames as BigQuery tables.
 
     Examples:
         .. code-block:: python
 
-            from dagster_gcp import build_bigquery_io_manager
+            from dagster_gcp import BigQueryIOManager
             from dagster_bigquery_pandas import BigQueryPandasTypeHandler
-            from dagster import asset, Definitions
+            from dagster import Definitions, EnvVar
+
+            class MyBigQueryIOManager(BigQueryIOManager):
+                @staticmethod
+                def type_handlers() -> Sequence[DbTypeHandler]:
+                    return [BigQueryPandasTypeHandler()]
 
             @asset(
-                key_prefix=["my_dataset"]  # will be used as the dataset in BigQuery
+                key_prefix=["my_dataset"]  # my_dataset will be used as the dataset in BigQuery
             )
-            def my_table():
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
                 ...
 
-            bigquery_io_manager = build_bigquery_io_manager([BigQueryPandasTypeHandler()])
-
             defs = Definitions(
                 assets=[my_table],
                 resources={
-                    "io_manager": bigquery_io_manager.configured({
-                        "project" : {"env": "GCP_PROJECT"}
-                    })
+                    "io_manager": MyBigQueryIOManager(project=EnvVar("GCP_PROJECT"))
                 }
             )
 
     """
 
     def handle_output(
         self, context: OutputContext, table_slice: TableSlice, obj: pd.DataFrame, connection
@@ -39,16 +46,16 @@
         """Stores the pandas DataFrame in BigQuery."""
         with_uppercase_cols = obj.rename(str.upper, copy=False, axis="columns")
 
         job = connection.load_table_from_dataframe(
             dataframe=with_uppercase_cols,
             destination=f"{table_slice.schema}.{table_slice.table}",
             project=table_slice.database,
-            location=context.resource_config["location"] if context.resource_config else None,
-            timeout=context.resource_config["timeout"] if context.resource_config else None,
+            location=context.resource_config.get("location") if context.resource_config else None,
+            timeout=context.resource_config.get("timeout") if context.resource_config else None,
         )
         job.result()
 
         context.add_output_metadata(
             {
                 "row_count": obj.shape[0],
                 "dataframe_columns": MetadataValue.table_schema(
@@ -67,16 +74,16 @@
     ) -> pd.DataFrame:
         """Loads the input as a Pandas DataFrame."""
         if table_slice.partition_dimensions and len(context.asset_partition_keys) == 0:
             return pd.DataFrame()
         result = connection.query(
             query=BigQueryClient.get_select_statement(table_slice),
             project=table_slice.database,
-            location=context.resource_config["location"] if context.resource_config else None,
-            timeout=context.resource_config["timeout"] if context.resource_config else None,
+            location=context.resource_config.get("location") if context.resource_config else None,
+            timeout=context.resource_config.get("timeout") if context.resource_config else None,
         ).to_dataframe()
 
         result.columns = map(str.lower, result.columns)
         return result
 
     @property
     def supported_types(self):
@@ -92,15 +99,15 @@
 Returns:
     IOManagerDefinition
 
 Examples:
 
     .. code-block:: python
 
-        from dagster_bigquery_pandas import bigquery_pandas_io_manager
+        from dagster_gcp_pandas import bigquery_pandas_io_manager
         from dagster import Definitions
 
         @asset(
             key_prefix=["my_dataset"]  # will be used as the dataset in BigQuery
         )
         def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
             ...
@@ -148,7 +155,80 @@
     via a standard method, you can provide a service account key as the "gcp_credentials" configuration.
     Dagster will store this key in a temporary file and set GOOGLE_APPLICATION_CREDENTIALS to point to the file.
     After the run completes, the file will be deleted, and GOOGLE_APPLICATION_CREDENTIALS will be
     unset. The key must be base64 encoded to avoid issues with newlines in the keys. You can retrieve
     the base64 encoded key with this shell command: cat $GOOGLE_APPLICATION_CREDENTIALS | base64
 
 """
+
+
+class BigQueryPandasIOManager(BigQueryIOManager):
+    """An I/O manager definition that reads inputs from and writes pandas DataFrames to BigQuery.
+
+    Returns:
+        IOManagerDefinition
+
+    Examples:
+        .. code-block:: python
+
+            from dagster_gcp_pandas import BigQueryPandasIOManager
+            from dagster import Definitions, EnvVar
+
+            @asset(
+                key_prefix=["my_dataset"]  # will be used as the dataset in BigQuery
+            )
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
+                ...
+
+            defs = Definitions(
+                assets=[my_table],
+                resources={
+                    "io_manager": BigQueryPandasIOManager(project=EnvVar("GCP_PROJECT"))
+                }
+            )
+
+        You can tell Dagster in which dataset to create tables by setting the "dataset" configuration value.
+        If you do not provide a dataset as configuration to the I/O manager, Dagster will determine a dataset based
+        on the assets and ops using the I/O Manager. For assets, the dataset will be determined from the asset key,
+        as shown in the above example. The final prefix before the asset name will be used as the dataset. For example,
+        if the asset "my_table" had the key prefix ["gcp", "bigquery", "my_dataset"], the dataset "my_dataset" will be
+        used. For ops, the dataset can be specified by including a "schema" entry in output metadata. If "schema" is not provided
+        via config or on the asset/op, "public" will be used for the dataset.
+
+        .. code-block:: python
+
+            @op(
+                out={"my_table": Out(metadata={"schema": "my_dataset"})}
+            )
+            def make_my_table() -> pd.DataFrame:
+                # the returned value will be stored at my_dataset.my_table
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
+        If you cannot upload a file to your Dagster deployment, or otherwise cannot
+        `authenticate with GCP <https://cloud.google.com/docs/authentication/provide-credentials-adc>`_
+        via a standard method, you can provide a service account key as the "gcp_credentials" configuration.
+        Dagster will store this key in a temporary file and set GOOGLE_APPLICATION_CREDENTIALS to point to the file.
+        After the run completes, the file will be deleted, and GOOGLE_APPLICATION_CREDENTIALS will be
+        unset. The key must be base64 encoded to avoid issues with newlines in the keys. You can retrieve
+        the base64 encoded key with this shell command: cat $GOOGLE_APPLICATION_CREDENTIALS | base64
+
+    """
+
+    @staticmethod
+    def type_handlers() -> Sequence[DbTypeHandler]:
+        return [BigQueryPandasTypeHandler()]
+
+    @staticmethod
+    def default_load_type() -> Optional[Type]:
+        return pd.DataFrame
```

### Comparing `dagster-gcp-pandas-0.18.6/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.18.7/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-gcp-pandas-0.18.6/setup.py` & `dagster-gcp-pandas-0.18.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-gcp==0.18.6",
+        "dagster==1.2.7",
+        "dagster-gcp==0.18.7",
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

