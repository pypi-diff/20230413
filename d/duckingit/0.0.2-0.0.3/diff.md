# Comparing `tmp/duckingit-0.0.2.tar.gz` & `tmp/duckingit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.2.tar", last modified: Mon Apr 10 15:02:09 2023, max compression
+gzip compressed data, was "duckingit-0.0.3.tar", last modified: Thu Apr 13 19:27:53 2023, max compression
```

## Comparing `duckingit-0.0.2.tar` & `duckingit-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-10 15:02:09.624531 duckingit-0.0.2/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3011 2023-04-10 15:02:09.624057 duckingit-0.0.2/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2406 2023-04-10 14:58:02.000000 duckingit-0.0.2/README.md
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-10 15:02:09.620799 duckingit-0.0.2/duckingit/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       34 2023-04-06 07:52:58.000000 duckingit-0.0.2/duckingit/__init__.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2034 2023-04-10 13:51:09.000000 duckingit-0.0.2/duckingit/_controller.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      142 2023-04-07 11:54:32.000000 duckingit-0.0.2/duckingit/_exceptions.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     1994 2023-04-10 09:01:01.000000 duckingit-0.0.2/duckingit/_parser.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3803 2023-04-10 13:23:34.000000 duckingit-0.0.2/duckingit/_planner.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3143 2023-04-10 09:19:32.000000 duckingit-0.0.2/duckingit/_provider.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     5366 2023-04-10 14:00:41.000000 duckingit-0.0.2/duckingit/_session.py
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-10 15:02:09.623407 duckingit-0.0.2/duckingit.egg-info/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3011 2023-04-10 15:02:09.000000 duckingit-0.0.2/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      348 2023-04-10 15:02:09.000000 duckingit-0.0.2/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)        1 2023-04-10 15:02:09.000000 duckingit-0.0.2/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       29 2023-04-10 15:02:09.000000 duckingit-0.0.2/duckingit.egg-info/requires.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       10 2023-04-10 15:02:09.000000 duckingit-0.0.2/duckingit.egg-info/top_level.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      824 2023-04-10 15:01:42.000000 duckingit-0.0.2/pyproject.toml
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       38 2023-04-10 15:02:09.624677 duckingit-0.0.2/setup.cfg
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.604305 duckingit-0.0.3/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3933 2023-04-13 19:27:53.603778 duckingit-0.0.3/PKG-INFO
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3328 2023-04-13 19:09:01.000000 duckingit-0.0.3/README.md
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.598373 duckingit-0.0.3/duckingit/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       66 2023-04-10 18:13:42.000000 duckingit-0.0.3/duckingit/__init__.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     1350 2023-04-13 16:52:25.000000 duckingit-0.0.3/duckingit/_analyze.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     1773 2023-04-13 17:18:52.000000 duckingit-0.0.3/duckingit/_config.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     2104 2023-04-13 17:18:18.000000 duckingit-0.0.3/duckingit/_controller.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      760 2023-04-13 17:02:57.000000 duckingit-0.0.3/duckingit/_encode.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      186 2023-04-12 13:01:34.000000 duckingit-0.0.3/duckingit/_exceptions.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     2322 2023-04-13 17:14:20.000000 duckingit-0.0.3/duckingit/_parser.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     2294 2023-04-13 17:14:14.000000 duckingit-0.0.3/duckingit/_planner.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     5502 2023-04-13 17:18:29.000000 duckingit-0.0.3/duckingit/_session.py
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.602518 duckingit-0.0.3/duckingit.egg-info/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3933 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      389 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)        1 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       29 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/requires.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       10 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      824 2023-04-13 19:25:57.000000 duckingit-0.0.3/pyproject.toml
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       38 2023-04-13 19:27:53.604469 duckingit-0.0.3/setup.cfg
```

### Comparing `duckingit-0.0.2/PKG-INFO` & `duckingit-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-Metadata-Version: 2.1
-Name: duckingit
-Version: 0.0.2
-Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
-Author-email: Tobias Egelund <egelundtobias@gmail.com>
-Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
-Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
-Keywords: Serverless,DuckDB,Data Engineering
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+![logo](logo.png)
 
-# DuckingIt
 A framework to leverage the endless capabilities of serverless computing powered by DuckDB.
 
 Please note that the framework currently supports only AWS Lambda functions. To use the framework, you must first create a Lambda layer of DuckDB that can be used within a Lambda function. Additionally, you must create a Lambda Executor function that can execute the actual DuckDB SQL. Once you've completed these setup steps, you can leverage the power of serverless functions through the SDK written in Python to perform analytics on a Data Lake.
 
 While Apache Spark can perform similar (and more advanced) functions, the cost of running Spark clusters can be prohibitively expensive. As a result, a much more affordable alternative is to use a cluster of serverless functions, such as Lambda functions, to perform the same actions as Spark, without the need to turn them off manually.
 
 ## Installation
 To install the Python SDK from PyPI execute the command below. Nonetheless, it's recommended that you first review the [setup](/README.md#setup) section in order to properly utilize the package.
 
 ```bash
 pip install duckingit
 ```
 
 ## Setup
-Please ensure that you have both Docker and Terraform installed before setting up the infrastructure.
+Before setting up the infrastructure, please make sure that you have installed both Docker and Terraform.
 
-The SDK acts as a gateway to the serverless function cluster, so the entire infrastructure must be set up before executing any commands on the DuckDB instances.
+To interact with the DuckDB instances, the entire infrastructure must be set up first because the SDK functions as an entryway to the serverless function cluster. DuckDB is packaged as a layer to be pre-installed in AWS Lambda, similar to other packages. Docker must be installed to create the layer.
 
-AWS Lambda employs layers to handle pre-installed packages, and DuckDB is no exception. To make the installed binaries work on AWS Lambda, Docker must be installed because the layer is built on the same architecture that runs on AWS Lambda.
-
-The first step is to create the DuckDB layer. Running the following command will produce a duckdb-layer.zip file in the image/release/ folder:
+Running the command below will generate a duckdb-layer.zip file in the image/release/ folder:
 ```bash
 make release-image
 ```
 
-To proceed with setting up the infrastructure on AWS, you need to have Terraform installed. Follow these commands:
+To set up the infrastructure on AWS, follow the commands below:
 ```bash
-make tf-init
-make tf-apply
+make release-infra
 ```
 
-After waiting for a minute or two, the process should be complete. You can now check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
+After waiting for a minute or two, the infrastructure should be set up, and you can check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
 
 Once you have verified the above components, the infrastructure should be set up and fully operational.
 
 ## Usage
-... Coming up
+The framework's developer API draws inspiration from Spark's API, but it uses Python's naming conventions because the framework is implemented in Python.
+
+```python
+from duckingit import DuckSession
+
+query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
+
+# Creates an entrypoint to use serverless DuckDB instances
+session = DuckSession()
+
+# Updates the Lambda function with 128 MB memory size and 30 timeout
+# as well as initializing the Lambda function to avoid cold start
+session.conf.memory_size(128).timeout(30).warm_up().update()
+
+# Execute the command
+session.execute(query=query)
+```
+
+... To be continued
 
 ## Contribution
-... Coming up
+Thank you for taking an interest in my project on GitHub. I am always looking for new contributors to help me improve and evolve my codebase. If you're interested in contributing, feel free to fork the repository and submit a pull request with your changes.
+
+I welcome all kinds of contributions, from bug fixes to feature additions and documentation improvements. If you're not sure where to start, take a look at the issues tab or reach out to us for guidance.
+
+Let's collaborate and make our project better together!
 
 
 ___________________________________
 Ducking it ~ Killing it
```

### Comparing `duckingit-0.0.2/duckingit/_session.py` & `duckingit-0.0.3/duckingit/_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 
 import duckdb
 
-from ._controller import Controller, LocalController
-from ._planner import Planner
-from ._parser import QueryParser
-from ._provider import AWS
+from duckingit._controller import Controller, LocalController
+from duckingit._planner import Plan, Step
+from duckingit._parser import Query
+from duckingit.integrations import AWS
+from duckingit._analyze import scan_bucket
+from duckingit._config import DuckConfig
 
 
 class DuckSession:
     """Entrypoint to a session of serverless DuckDB instances
 
     The main objective of this class is to handle the session and serve as the primary
     entrypoint to a cluster of serverless functions that utilize DuckDB. Its core
@@ -19,15 +21,14 @@
     Attributes:
         conn, duckdb.DuckDBPyConnection: The initialized DuckDB connection
         metadata, dict: Metadata on temporary tables created using the DuckSession
 
     Methods:
         execute: Execute a DuckDB SQL query concurrently using X number of invokations
 
-
     Usage:
         >>> session = DuckSession()
         >>> resp = session.execute(query="SELECT * FROM scan_parquet(['s3::/<BUCKET_NAME>/*'])")
         >>> resp.show()
     """
 
     _CACHE_PREFIX = ".cache/duckingit"
@@ -53,42 +54,45 @@
                 Defaults to 'auto'
             enable_cache, bool: Caches client-side, ie. caches are stored in memory on
                 the machine running the DuckSession. Defaults to True
             **kwargs
         """
         self._function_name = function_name
         self._invokations_default = invokations_default
-        self.enable_cache = enable_cache
+        self._enable_cache = enable_cache
         self._kwargs = kwargs
 
         self._conn = duckdb.connect(**duckdb_config)
         self._load_httpfs()
         self._set_credentials()
 
         self._controller = self._set_controller()
-        self._planner = self._set_planner()
 
+        self._conf: DuckConfig | None = None
         self._metadata: dict[str, str] = dict()
 
     @property
     def metadata(self) -> dict[str, str]:
         return self._metadata
 
     @property
     def conn(self) -> duckdb.DuckDBPyConnection:
         return self._conn
 
-    def _set_planner(self) -> Planner:
-        return Planner(conn=self._conn)
+    @property
+    def conf(self) -> DuckConfig:
+        if self._conf is None:
+            self._conf = DuckConfig(function_name=self._function_name)
+        return self._conf
 
     def _set_controller(self) -> Controller:
         return LocalController(
             conn=self._conn,
             provider=AWS(function_name=self._function_name),
-            enable_cache=self.enable_cache,
+            enable_cache=self._enable_cache,
         )
 
     def _load_httpfs(self) -> None:
         self._conn.execute("INSTALL httpfs; LOAD httpfs;")
 
     def _set_credentials(self) -> None:
         # https://duckdb.org/docs/sql/configuration.html
@@ -97,54 +101,49 @@
             f"""
             SET s3_region='{os.getenv("AWS_DEFAULT_REGION", None)}';
             SET s3_access_key_id='{os.getenv("AWS_ACCESS_KEY_ID", None)}';
             SET s3_secret_access_key='{os.getenv("AWS_SECRET_ACCESS_KEY", None)}';
             """
         )
 
-    def _create_execution_plan(self, query: str, invokations: int | str) -> list[str]:
-        list_of_queries = self._planner.generate_plan(
-            query=query, invokations=invokations
-        )
-
-        return list_of_queries
-
-    def _create_prefix(self, query: str, write_to: str | None) -> str:
-        query_hashed = QueryParser.hash_query(query=query)
-        bucket_name = QueryParser.find_bucket(query=query)
+    def _scan_bucket(self, query: Query) -> list[str]:
+        return scan_bucket(query.source, conn=self.conn)
 
+    def _create_prefix(self, query: Query, write_to: str | None) -> str:
         if write_to is not None:
             if write_to[-1] != "/":
                 return write_to
             return write_to[:-1]
-        return f"{bucket_name}/{self._CACHE_PREFIX}/{query_hashed}"
+        return f"{query.bucket}/{self._CACHE_PREFIX}/{query.hashed}"
 
     def execute(
         self, query: str, *, invokations: int | None = None, write_to: str | None = None
     ) -> duckdb.DuckDBPyRelation:
         """Execute the query against a number of serverless functions
 
         Args:
             query, str: DuckDB SQL query to run
             invokations, int | None: The number of invokations of the Lambda function
                 Defaults to 'auto' (See initialization of the session class)
             write_to, str | None: The prefix to write to, e.g. 's3://BUCKET_NAME/data'
                 Defaults to .cache/duckingit/ prefix
         """
+        query_parsed: Query = Query.parse(query)
+        query_parsed.list_of_prefixes = self._scan_bucket(query=query_parsed)
+
         number_of_invokations = (
             invokations if invokations is not None else self._invokations_default
         )
-        prefix = self._create_prefix(query=query, write_to=write_to)
-
-        execution_plan = self._create_execution_plan(
-            query=query, invokations=number_of_invokations
+        execution_plan = Plan.create_from_query(
+            query=query_parsed, invokations=number_of_invokations
         )
 
+        prefix = self._create_prefix(query=query_parsed, write_to=write_to)
         duckdb_obj, table_name = self._controller.execute(
-            queries=execution_plan, prefix=prefix
+            execution_plan=execution_plan, prefix=prefix
         )
 
         # Update metadata
         if table_name != "":
-            self._metadata[table_name] = query
+            self._metadata[table_name] = query_parsed.sql
 
         return duckdb_obj
```

### Comparing `duckingit-0.0.2/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,79 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# DuckingIt
+![logo](logo.png)
+
 A framework to leverage the endless capabilities of serverless computing powered by DuckDB.
 
 Please note that the framework currently supports only AWS Lambda functions. To use the framework, you must first create a Lambda layer of DuckDB that can be used within a Lambda function. Additionally, you must create a Lambda Executor function that can execute the actual DuckDB SQL. Once you've completed these setup steps, you can leverage the power of serverless functions through the SDK written in Python to perform analytics on a Data Lake.
 
 While Apache Spark can perform similar (and more advanced) functions, the cost of running Spark clusters can be prohibitively expensive. As a result, a much more affordable alternative is to use a cluster of serverless functions, such as Lambda functions, to perform the same actions as Spark, without the need to turn them off manually.
 
 ## Installation
 To install the Python SDK from PyPI execute the command below. Nonetheless, it's recommended that you first review the [setup](/README.md#setup) section in order to properly utilize the package.
 
 ```bash
 pip install duckingit
 ```
 
 ## Setup
-Please ensure that you have both Docker and Terraform installed before setting up the infrastructure.
-
-The SDK acts as a gateway to the serverless function cluster, so the entire infrastructure must be set up before executing any commands on the DuckDB instances.
+Before setting up the infrastructure, please make sure that you have installed both Docker and Terraform.
 
-AWS Lambda employs layers to handle pre-installed packages, and DuckDB is no exception. To make the installed binaries work on AWS Lambda, Docker must be installed because the layer is built on the same architecture that runs on AWS Lambda.
+To interact with the DuckDB instances, the entire infrastructure must be set up first because the SDK functions as an entryway to the serverless function cluster. DuckDB is packaged as a layer to be pre-installed in AWS Lambda, similar to other packages. Docker must be installed to create the layer.
 
-The first step is to create the DuckDB layer. Running the following command will produce a duckdb-layer.zip file in the image/release/ folder:
+Running the command below will generate a duckdb-layer.zip file in the image/release/ folder:
 ```bash
 make release-image
 ```
 
-To proceed with setting up the infrastructure on AWS, you need to have Terraform installed. Follow these commands:
+To set up the infrastructure on AWS, follow the commands below:
 ```bash
-make tf-init
-make tf-apply
+make release-infra
 ```
 
-After waiting for a minute or two, the process should be complete. You can now check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
+After waiting for a minute or two, the infrastructure should be set up, and you can check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
 
 Once you have verified the above components, the infrastructure should be set up and fully operational.
 
 ## Usage
-... Coming up
+The framework's developer API draws inspiration from Spark's API, but it uses Python's naming conventions because the framework is implemented in Python.
+
+```python
+from duckingit import DuckSession
+
+query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
+
+# Creates an entrypoint to use serverless DuckDB instances
+session = DuckSession()
+
+# Updates the Lambda function with 128 MB memory size and 30 timeout
+# as well as initializing the Lambda function to avoid cold start
+session.conf.memory_size(128).timeout(30).warm_up().update()
+
+# Execute the command
+session.execute(query=query)
+```
+
+... To be continued
 
 ## Contribution
-... Coming up
+Thank you for taking an interest in my project on GitHub. I am always looking for new contributors to help me improve and evolve my codebase. If you're interested in contributing, feel free to fork the repository and submit a pull request with your changes.
+
+I welcome all kinds of contributions, from bug fixes to feature additions and documentation improvements. If you're not sure where to start, take a look at the issues tab or reach out to us for guidance.
+
+Let's collaborate and make our project better together!
 
 
 ___________________________________
 Ducking it ~ Killing it
```

### Comparing `duckingit-0.0.2/pyproject.toml` & `duckingit-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
```

