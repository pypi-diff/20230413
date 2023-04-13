# Comparing `tmp/dagster_gcp_pyspark-0.18.6.tar.gz` & `tmp/dagster_gcp_pyspark-0.18.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.18.6.tar", last modified: Thu Apr  6 00:28:31 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.18.7.tar", last modified: Thu Apr 13 15:13:00 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.18.6.tar` & `dagster_gcp_pyspark-0.18.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:31.964368 dagster_gcp_pyspark-0.18.6/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-06 00:28:31.964368 dagster_gcp_pyspark-0.18.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:31.960368 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      344 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:31.964368 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:28:31.964368 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-06 00:28:31.000000 dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-06 00:28:31.968368 dagster_gcp_pyspark-0.18.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-05 23:51:52.000000 dagster_gcp_pyspark-0.18.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:00.681546 dagster_gcp_pyspark-0.18.7/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-13 15:13:00.681546 dagster_gcp_pyspark-0.18.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:00.677546 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:00.677546 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:00.677546 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-13 15:13:00.000000 dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-13 15:13:00.681546 dagster_gcp_pyspark-0.18.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-13 15:03:07.000000 dagster_gcp_pyspark-0.18.7/setup.py
```

### Comparing `dagster_gcp_pyspark-0.18.6/LICENSE` & `dagster_gcp_pyspark-0.18.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.18.6/PKG-INFO` & `dagster_gcp_pyspark-0.18.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping, Optional, Sequence, Type
 
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.definitions.metadata import RawMetadataValue
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
-from dagster_gcp import build_bigquery_io_manager
+from dagster_gcp import BigQueryIOManager, build_bigquery_io_manager
 from dagster_gcp.bigquery.io_manager import BigQueryClient
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
 
 
 def _get_bigquery_write_options(
     config: Optional[Mapping[str, Any]], table_slice: TableSlice
@@ -29,32 +29,33 @@
 
 class BigQueryPySparkTypeHandler(DbTypeHandler[DataFrame]):
     """Plugin for the BigQuery I/O Manager that can store and load PySpark DataFrames as BigQuery tables.
 
     Examples:
         .. code-block:: python
 
-            from dagster_gcp import build_bigquery_io_manager
-            from dagster_bigquery_pyspark import BigQueryPySparkTypeHandler
-            from dagster import asset, Definitions
+            from dagster_gcp import BigQueryIOManager
+            from dagster_bigquery_pandas import BigQueryPySparkTypeHandler
+            from dagster import Definitions, EnvVar
+
+            class MyBigQueryIOManager(BigQueryIOManager):
+                @staticmethod
+                def type_handlers() -> Sequence[DbTypeHandler]:
+                    return [BigQueryPySparkTypeHandler()]
 
             @asset(
-                key_prefix=["my_dataset"]  # will be used as the dataset in BigQuery
+                key_prefix=["my_dataset"]  # my_dataset will be used as the dataset in BigQuery
             )
-            def my_table():
+            def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
                 ...
 
-            bigquery_io_manager = build_bigquery_io_manager([BigQueryPySparkTypeHandler()])
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
         self, context: OutputContext, table_slice: TableSlice, obj: DataFrame, _
@@ -105,15 +106,15 @@
 Returns:
     IOManagerDefinition
 
 Examples:
 
     .. code-block:: python
 
-        from dagster_bigquery_pyspark import bigquery_pyspark_io_manager
+        from dagster_gcp_pyspark import bigquery_pyspark_io_manager
         from dagster import Definitions
 
         @asset(
             key_prefix=["my_dataset"]  # will be used as the dataset in BigQuery
         )
         def my_table() -> pd.DataFrame:  # the name of the asset will be the table name
             ...
@@ -161,7 +162,80 @@
     via a standard method, you can provide a service account key as the "gcp_credentials" configuration.
     Dagster will store this key in a temporary file and set GOOGLE_APPLICATION_CREDENTIALS to point to the file.
     After the run completes, the file will be deleted, and GOOGLE_APPLICATION_CREDENTIALS will be
     unset. The key must be base64 encoded to avoid issues with newlines in the keys. You can retrieve
     the base64 encoded key with this shell command: cat $GOOGLE_APPLICATION_CREDENTIALS | base64
 
 """
+
+
+class BigQueryPySparkIOManager(BigQueryIOManager):
+    """An I/O manager definition that reads inputs from and writes PySpark DataFrames to BigQuery.
+
+    Returns:
+        IOManagerDefinition
+
+    Examples:
+        .. code-block:: python
+
+            from dagster_gcp_pyspark import BigQueryPySparkIOManager
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
+                    "io_manager": BigQueryPySparkIOManager(project=EnvVar("GCP_PROJECT"))
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
+        return [BigQueryPySparkTypeHandler()]
+
+    @staticmethod
+    def default_load_type() -> Optional[Type]:
+        return DataFrame
```

### Comparing `dagster_gcp_pyspark-0.18.6/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.18.7/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.18.6
+Version: 0.18.7
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.18.6/setup.py` & `dagster_gcp_pyspark-0.18.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-gcp==0.18.6",
+        "dagster==1.2.7",
+        "dagster-gcp==0.18.7",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

