# Comparing `tmp/google-cloud-bigquery-data-exchange-0.5.2.tar.gz` & `tmp/google-cloud-bigquery-data-exchange-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.2.tar", last modified: Mon Mar 27 15:32:26 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.3.tar", last modified: Thu Apr 13 13:55:30 2023, max compression
```

## Comparing `google-cloud-bigquery-data-exchange-0.5.2.tar` & `google-cloud-bigquery-data-exchange-0.5.3.tar`

### file list

```diff
@@ -1,62 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4952 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4004 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.441749 google-cloud-bigquery-data-exchange-0.5.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.441749 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/
--rw-rw-r--   0 root         (0)     1003     2366 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2177 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/
--rw-rw-r--   0 root         (0)     1003      662 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/__init__.py
--rw-rw-r--   0 root         (0)     1003      272 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      103 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/types/
--rw-rw-r--   0 root         (0)     1003      625 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1497 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/types/common.py
--rw-rw-r--   0 root         (0)     1003     4399 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.445750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    86164 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    97979 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    16537 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-03-27 15:30:11.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13308 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30551 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31129 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1851 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26457 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/
--rw-r--r--   0 root         (0)     1003     4952 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2492 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:32:26.000000 google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:32:26.453750 google-cloud-bigquery-data-exchange-0.5.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3034 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   217243 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:26.449750 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/common/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:12.000000 google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/common/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4952 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4004 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.901104 google-cloud-bigquery-data-exchange-0.5.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.901104 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/
+-rw-rw-r--   0 root         (0)     1003     2366 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2177 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4399 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    86164 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    97979 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16537 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13308 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30551 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31129 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.905107 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1851 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26457 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/
+-rw-r--r--   0 root         (0)     1003     4952 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1986 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-13 13:55:30.000000 google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3034 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 13:55:30.909110 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   217243 2023-04-13 13:53:33.000000 google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/LICENSE` & `google-cloud-bigquery-data-exchange-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/MANIFEST.in` & `google-cloud-bigquery-data-exchange-0.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.2
+Version: 0.5.3
 Summary: Google Cloud Bigquery Data Exchange API client library
 Home-page: https://github.com/googleapis/python-bigquery-data-exchange
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/README.rst` & `google-cloud-bigquery-data-exchange-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.2"  # {x-release-please-version}
+__version__ = "0.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-
-from .types.common import Category
-
-__all__ = ("Category",)
+__version__ = "0.5.3"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/common/services/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py` & `google-cloud-bigquery-data-exchange-0.5.3/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.2
+Version: 0.5.3
 Summary: Google Cloud Bigquery Data Exchange API client library
 Home-page: https://github.com/googleapis/python-bigquery-data-exchange
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt` & `google-cloud-bigquery-data-exchange-0.5.3/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,14 @@
 google/cloud/bigquery_data_exchange/__init__.py
 google/cloud/bigquery_data_exchange/gapic_version.py
 google/cloud/bigquery_data_exchange/py.typed
 google/cloud/bigquery_data_exchange_v1beta1/__init__.py
 google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
 google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
 google/cloud/bigquery_data_exchange_v1beta1/py.typed
-google/cloud/bigquery_data_exchange_v1beta1/common/__init__.py
-google/cloud/bigquery_data_exchange_v1beta1/common/gapic_metadata.json
-google/cloud/bigquery_data_exchange_v1beta1/common/gapic_version.py
-google/cloud/bigquery_data_exchange_v1beta1/common/py.typed
-google/cloud/bigquery_data_exchange_v1beta1/common/services/__init__.py
-google/cloud/bigquery_data_exchange_v1beta1/common/types/__init__.py
-google/cloud/bigquery_data_exchange_v1beta1/common/types/common.py
 google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
 google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
@@ -35,9 +28,8 @@
 google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
 google_cloud_bigquery_data_exchange.egg-info/requires.txt
 google_cloud_bigquery_data_exchange.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
-tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
-tests/unit/gapic/common/__init__.py
+tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/setup.py` & `google-cloud-bigquery-data-exchange-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/tests/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.2/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py` & `google-cloud-bigquery-data-exchange-0.5.3/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py`

 * *Files identical despite different names*

