# Comparing `tmp/commonsharedclasses-0.0.8.tar.gz` & `tmp/commonsharedclasses-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonsharedclasses-0.0.8.tar", last modified: Mon Dec 19 06:41:00 2022, max compression
+gzip compressed data, was "commonsharedclasses-0.0.9.tar", last modified: Mon Dec 19 07:12:53 2022, max compression
```

## Comparing `commonsharedclasses-0.0.8.tar` & `commonsharedclasses-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 06:41:00.302726 commonsharedclasses-0.0.8/
--rw-rw-rw-   0        0        0      272 2022-12-19 06:41:00.302726 commonsharedclasses-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-19 06:41:00.271540 commonsharedclasses-0.0.8/commonsharedclasses/
--rw-rw-rw-   0        0        0     3534 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/CosmosLogConfiguration.py
--rw-rw-rw-   0        0        0     3263 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/DynamicCosmosRetrieve.py
--rw-rw-rw-   0        0        0      865 2022-12-15 14:25:41.000000 commonsharedclasses-0.0.8/commonsharedclasses/__init__.py
--rw-rw-rw-   0        0        0      883 2022-09-29 12:08:35.000000 commonsharedclasses-0.0.8/commonsharedclasses/blob_service_connection.py
--rw-rw-rw-   0        0        0     1274 2022-09-29 12:08:33.000000 commonsharedclasses-0.0.8/commonsharedclasses/cosmos_connection.py
--rw-rw-rw-   0        0        0     2551 2022-12-18 23:56:00.000000 commonsharedclasses-0.0.8/commonsharedclasses/cosmos_utility.py
--rw-rw-rw-   0        0        0     4012 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/databricks_sql.py
--rw-rw-rw-   0        0        0     2559 2022-09-29 12:08:31.000000 commonsharedclasses-0.0.8/commonsharedclasses/fetch_details.py
--rw-rw-rw-   0        0        0     9677 2022-09-29 12:08:54.000000 commonsharedclasses-0.0.8/commonsharedclasses/service_principal_access_provider.py
--rw-rw-rw-   0        0        0     1633 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/service_principal_authorization_provider.py
--rw-rw-rw-   0        0        0      402 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/singleton.py
--rw-rw-rw-   0        0        0      486 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/singleton_blob_service_client.py
--rw-rw-rw-   0        0        0      483 2022-09-29 12:09:40.000000 commonsharedclasses-0.0.8/commonsharedclasses/singleton_cluster_thrift_connection.py
--rw-rw-rw-   0        0        0      555 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.8/commonsharedclasses/singleton_cosmos_client.py
--rw-rw-rw-   0        0        0     3922 2022-12-14 17:42:49.000000 commonsharedclasses-0.0.8/commonsharedclasses/sql_query_provider.py
--rw-rw-rw-   0        0        0     5811 2022-12-13 08:35:20.000000 commonsharedclasses-0.0.8/commonsharedclasses/tenant_lakehouse_query.py
-drwxrwxrwx   0        0        0        0 2022-12-19 06:41:00.302726 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/
--rw-rw-rw-   0        0        0      272 2022-12-19 06:40:59.000000 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      957 2022-12-19 06:40:59.000000 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 06:40:59.000000 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-09-27 11:56:13.000000 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2022-12-19 06:40:59.000000 commonsharedclasses-0.0.8/commonsharedclasses.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-19 06:41:00.302726 commonsharedclasses-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      309 2022-12-19 06:40:24.000000 commonsharedclasses-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-19 07:12:53.382542 commonsharedclasses-0.0.9/
+-rw-rw-rw-   0        0        0      272 2022-12-19 07:12:53.383455 commonsharedclasses-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-19 07:12:53.348266 commonsharedclasses-0.0.9/commonsharedclasses/
+-rw-rw-rw-   0        0        0     3534 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/CosmosLogConfiguration.py
+-rw-rw-rw-   0        0        0     3263 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/DynamicCosmosRetrieve.py
+-rw-rw-rw-   0        0        0      865 2022-12-15 14:25:41.000000 commonsharedclasses-0.0.9/commonsharedclasses/__init__.py
+-rw-rw-rw-   0        0        0      883 2022-09-29 12:08:35.000000 commonsharedclasses-0.0.9/commonsharedclasses/blob_service_connection.py
+-rw-rw-rw-   0        0        0     1274 2022-09-29 12:08:33.000000 commonsharedclasses-0.0.9/commonsharedclasses/cosmos_connection.py
+-rw-rw-rw-   0        0        0     2551 2022-12-18 23:56:00.000000 commonsharedclasses-0.0.9/commonsharedclasses/cosmos_utility.py
+-rw-rw-rw-   0        0        0     4012 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/databricks_sql.py
+-rw-rw-rw-   0        0        0     2559 2022-09-29 12:08:31.000000 commonsharedclasses-0.0.9/commonsharedclasses/fetch_details.py
+-rw-rw-rw-   0        0        0     9677 2022-09-29 12:08:54.000000 commonsharedclasses-0.0.9/commonsharedclasses/service_principal_access_provider.py
+-rw-rw-rw-   0        0        0     1633 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/service_principal_authorization_provider.py
+-rw-rw-rw-   0        0        0      402 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/singleton.py
+-rw-rw-rw-   0        0        0      486 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/singleton_blob_service_client.py
+-rw-rw-rw-   0        0        0      483 2022-09-29 12:09:40.000000 commonsharedclasses-0.0.9/commonsharedclasses/singleton_cluster_thrift_connection.py
+-rw-rw-rw-   0        0        0      555 2022-09-26 11:39:38.000000 commonsharedclasses-0.0.9/commonsharedclasses/singleton_cosmos_client.py
+-rw-rw-rw-   0        0        0     3922 2022-12-14 17:42:49.000000 commonsharedclasses-0.0.9/commonsharedclasses/sql_query_provider.py
+-rw-rw-rw-   0        0        0     5811 2022-12-13 08:35:20.000000 commonsharedclasses-0.0.9/commonsharedclasses/tenant_lakehouse_query.py
+drwxrwxrwx   0        0        0        0 2022-12-19 07:12:53.381456 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/
+-rw-rw-rw-   0        0        0      272 2022-12-19 07:12:52.000000 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2022-12-19 07:12:52.000000 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-19 07:12:52.000000 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-09-27 11:56:13.000000 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2022-12-19 07:12:52.000000 commonsharedclasses-0.0.9/commonsharedclasses.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-19 07:12:53.384468 commonsharedclasses-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      309 2022-12-19 07:12:20.000000 commonsharedclasses-0.0.9/setup.py
```

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/CosmosLogConfiguration.py` & `commonsharedclasses-0.0.9/commonsharedclasses/CosmosLogConfiguration.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/DynamicCosmosRetrieve.py` & `commonsharedclasses-0.0.9/commonsharedclasses/DynamicCosmosRetrieve.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/__init__.py` & `commonsharedclasses-0.0.9/commonsharedclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/blob_service_connection.py` & `commonsharedclasses-0.0.9/commonsharedclasses/blob_service_connection.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/cosmos_connection.py` & `commonsharedclasses-0.0.9/commonsharedclasses/cosmos_connection.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/cosmos_utility.py` & `commonsharedclasses-0.0.9/commonsharedclasses/cosmos_utility.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/databricks_sql.py` & `commonsharedclasses-0.0.9/commonsharedclasses/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/fetch_details.py` & `commonsharedclasses-0.0.9/commonsharedclasses/fetch_details.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/service_principal_access_provider.py` & `commonsharedclasses-0.0.9/commonsharedclasses/service_principal_access_provider.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/service_principal_authorization_provider.py` & `commonsharedclasses-0.0.9/commonsharedclasses/service_principal_authorization_provider.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/singleton_cosmos_client.py` & `commonsharedclasses-0.0.9/commonsharedclasses/singleton_cosmos_client.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/sql_query_provider.py` & `commonsharedclasses-0.0.9/commonsharedclasses/sql_query_provider.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses/tenant_lakehouse_query.py` & `commonsharedclasses-0.0.9/commonsharedclasses/tenant_lakehouse_query.py`

 * *Files identical despite different names*

### Comparing `commonsharedclasses-0.0.8/commonsharedclasses.egg-info/SOURCES.txt` & `commonsharedclasses-0.0.9/commonsharedclasses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

