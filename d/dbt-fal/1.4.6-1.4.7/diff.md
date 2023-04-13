# Comparing `tmp/dbt-fal-1.4.6.tar.gz` & `tmp/dbt-fal-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fal-1.4.6.tar", max compression
+gzip compressed data, was "dbt-fal-1.4.7.tar", max compression
```

## Comparing `dbt-fal-1.4.6.tar` & `dbt-fal-1.4.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3009 2023-04-06 09:21:59.516688 dbt-fal-1.4.6/README.md
--rw-r--r--   0        0        0     1590 2023-04-06 09:22:19.005017 dbt-fal-1.4.6/pyproject.toml
--rw-r--r--   0        0        0      303 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-04-06 09:22:19.561027 dbt-fal-1.4.6/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     6047 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     4091 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-04-06 09:22:19.561027 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4691 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8200 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8685 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     2781 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10763 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6367 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     3069 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1083 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      910 2023-04-06 09:21:59.520688 dbt-fal-1.4.6/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     4847 2023-04-06 09:22:20.473145 dbt-fal-1.4.6/setup.py
--rw-r--r--   0        0        0     4580 2023-04-06 09:22:20.473587 dbt-fal-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-04-13 09:04:59.757103 dbt-fal-1.4.7/README.md
+-rw-r--r--   0        0        0     1590 2023-04-13 09:05:09.969715 dbt-fal-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-13 09:05:10.585752 dbt-fal-1.4.7/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     6047 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     4091 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-13 09:05:10.585752 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4691 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8200 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8685 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     2781 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10763 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6367 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     3069 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-04-13 09:04:59.761103 dbt-fal-1.4.7/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1083 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      910 2023-04-13 09:04:59.765103 dbt-fal-1.4.7/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     4847 2023-04-13 09:05:11.604185 dbt-fal-1.4.7/setup.py
+-rw-r--r--   0        0        0     4580 2023-04-13 09:05:11.604734 dbt-fal-1.4.7/PKG-INFO
```

### Comparing `dbt-fal-1.4.6/README.md` & `dbt-fal-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/pyproject.toml` & `dbt-fal-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-fal"
-version = "1.4.6"
+version = "1.4.7"
 description = "Simplest way to run dbt python models."
 readme = "README.md"
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/adapter"
 repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
     { include = "dbt", from = "src" }
@@ -40,15 +40,15 @@
 
 # teleport
 s3fs = { version = ">=2022.8.2", optional = true }
 
 # fal cloud
 dill = ">=0.3.5.1"
 packaging = "<22"
-fal-serverless = "^0.6.24"
+fal-serverless = "^0.6.28"
 importlib-metadata = "^6.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.extras]
 postgres = []
```

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal/impl.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal/wrappers.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal/wrappers.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/adapter.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/adapter_support.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/connections.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/impl.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/athena.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/athena.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/bigquery.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/bigquery.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/duckdb.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/postgres.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/snowflake.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/support/trino.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/support/trino.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/telemetry/telemetry.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_adapter_support.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/__init__.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/environments.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/environments.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/adapters/fal_experimental/utils/yaml_helper.py` & `dbt-fal-1.4.7/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/fal/adapters/python/connections.py` & `dbt-fal-1.4.7/src/dbt/fal/adapters/python/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/fal/adapters/python/impl.py` & `dbt-fal-1.4.7/src/dbt/fal/adapters/python/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/fal/adapters/teleport/impl.py` & `dbt-fal-1.4.7/src/dbt/fal/adapters/teleport/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/fal/adapters/teleport/info.py` & `dbt-fal-1.4.7/src/dbt/fal/adapters/teleport/info.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/include/fal/macros/materializations/table.sql` & `dbt-fal-1.4.7/src/dbt/include/fal/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/include/fal/macros/teleport_snowflake.sql` & `dbt-fal-1.4.7/src/dbt/include/fal/macros/teleport_snowflake.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/src/dbt/include/fal_experimental/macros/materializations/table.sql` & `dbt-fal-1.4.7/src/dbt/include/fal_experimental/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.4.6/setup.py` & `dbt-fal-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'dbt.include.fal': ['macros/*', 'macros/materializations/*'],
  'dbt.include.fal_experimental': ['macros/materializations/*']}
 
 install_requires = \
 ['backports.functools_lru_cache>=1.6.4,<2.0.0',
  'dbt-core>=1.4.0,<1.5',
  'dill>=0.3.5.1',
- 'fal-serverless>=0.6.24,<0.7.0',
+ 'fal-serverless>=0.6.28,<0.7.0',
  'importlib-metadata>=6.0.0,<7.0.0',
  'packaging<22',
  'pandas>=1.3.4,<2.0.0',
  'posthog>=1.4.5,<2.0.0',
  'sqlalchemy>=1.4.41,<2.0.0']
 
 extras_require = \
@@ -38,15 +38,15 @@
  'redshift': ['sqlalchemy-redshift>=0.8.9,<0.9.0'],
  'snowflake': ['snowflake-connector-python[pandas]>=2.8.0,<2.8.2'],
  'teleport': ['s3fs>=2022.8.2'],
  'trino': ['trino[sqlalchemy]>=0.321.0,<0.322.0']}
 
 setup_kwargs = {
     'name': 'dbt-fal',
-    'version': '1.4.6',
+    'version': '1.4.7',
     'description': 'Simplest way to run dbt python models.',
     'long_description': '<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/adapter/" target="_blank" /> -->\n\n# Welcome to dbt-fal 👋\n\ndbt-fal adapter is the ✨easiest✨ way to run your [dbt Python models](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/python-models).\n\nStarting with dbt v1.3, you can now build your dbt models in Python. This leads to some cool use cases that was once difficult to build with SQL alone. Some examples are:\n\n- Using Python stats libraries to calculate stats\n- Building forecasts\n- Building other predictive models such as classification and clustering\n\nThis is fantastic! BUT, there is still one issue though! The developer experience with Snowflake and Bigquery is not great, and there is no Python support for Redshift and Postgres.\n\ndbt-fal provides the best environment to run your Python models that works with all other data warehouses! With dbt-fal, you can:\n\n- Build and test your models locally\n- Isolate each model to run in its own environment with its own dependencies\n- [Coming Soon] Run your Python models in the ☁️ cloud ☁️ with elasticly scaling Python environments.\n- [Coming Soon] Even add GPUs to your models for some heavier workloads such as training ML models.\n\n## Getting Started\n\n### 1. Install dbt-fal\n`pip install dbt-fal[bigquery, snowflake]` *Add your current warehouse here*\n\n### 2. Update your `profiles.yml` and add the fal adapter\n\n```yaml\njaffle_shop:\n  target: dev_with_fal\n  outputs:\n    dev_with_fal:\n      type: fal\n      db_profile: dev_bigquery # This points to your main adapter\n    dev_bigquery:\n      type: bigquery\n      ...\n```\n\nDon\'t forget to point to your main adapter with the `db_profile` attribute. This is how the fal adapter knows how to connect to your data warehouse.\n\n### 3. `dbt run`!\nThat is it! It is really that simple 😊\n\n### 4. [🚨 Cool Feature Alert 🚨] Environment management with dbt-fal\nIf you want some help with environment management (vs sticking to the default env that the dbt process runs in), you can create a fal_project.yml in the same folder as your dbt project and have “named environments”:\n\nIn your dbt project folder:\n```bash\n$ touch fal_project.yml\n\n# Paste the config below\nenvironments:\n  - name: ml\n    type: venv\n    requirements:\n      - prophet\n```\n\nand then in your dbt model:\n\n```bash\n$ vi models/orders_forecast.py\n\ndef model(dbt, fal):\n    dbt.config(fal_environment="ml") # Add this line\n\n    df: pd.DataFrame = dbt.ref("orders_daily")\n```\n\nThe `dbt.config(fal_environment=“ml”)` will give you an isolated clean env to run things in, so you dont pollute your package space.\n\n### 5. [Coming Soon™️] Move your compute to the Cloud!\nLet us know if you are interested in this. We are looking for beta users.\n\n# Have feedback or need help?\n\n- Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)\n- Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fal-ai/fal/blob/-/projects/adapter',
```

### Comparing `dbt-fal-1.4.6/PKG-INFO` & `dbt-fal-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fal
-Version: 1.4.6
+Version: 1.4.7
 Summary: Simplest way to run dbt python models.
 Home-page: https://github.com/fal-ai/fal/blob/-/projects/adapter
 Keywords: dbt,pandas,fal,runtime
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: teleport
 Provides-Extra: trino
 Requires-Dist: backports.functools_lru_cache (>=1.6.4,<2.0.0)
 Requires-Dist: dbt-core (>=1.4.0,<1.5)
 Requires-Dist: dill (>=0.3.5.1)
-Requires-Dist: fal-serverless (>=0.6.24,<0.7.0)
+Requires-Dist: fal-serverless (>=0.6.28,<0.7.0)
 Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0); extra == "bigquery"
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
 Requires-Dist: packaging (<22)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: posthog (>=1.4.5,<2.0.0)
 Requires-Dist: s3fs (>=2022.8.2); extra == "teleport"
 Requires-Dist: snowflake-connector-python[pandas] (>=2.8.0,<2.8.2); extra == "snowflake"
```

