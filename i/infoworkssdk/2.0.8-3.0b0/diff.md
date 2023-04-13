# Comparing `tmp/infoworkssdk-2.0.8.tar.gz` & `tmp/infoworkssdk-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoworkssdk-2.0.8.tar", last modified: Fri Feb 24 12:11:31 2023, max compression
+gzip compressed data, was "infoworkssdk-3.0b0.tar", last modified: Thu Apr 13 12:48:00 2023, max compression
```

## Comparing `infoworkssdk-2.0.8.tar` & `infoworkssdk-3.0b0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.094301 infoworkssdk-2.0.8/
--rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/LICENSE
--rw-r--r--   0 infoworks   (501) staff       (20)     2431 2023-02-24 12:11:31.094102 infoworkssdk-2.0.8/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-2.0.8/README.md
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.071306 infoworkssdk-2.0.8/infoworks/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/__init__.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.072004 infoworkssdk-2.0.8/infoworks/core/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/core/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4085 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/core/iw_authentication.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1080 2023-01-09 10:04:48.000000 infoworkssdk-2.0.8/infoworks/error.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.082015 infoworkssdk-2.0.8/infoworks/sdk/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    58280 2023-02-06 10:31:40.000000 infoworkssdk-2.0.8/infoworks/sdk/admin_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    20014 2023-01-11 15:41:10.000000 infoworkssdk-2.0.8/infoworks/sdk/base_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.082646 infoworkssdk-2.0.8/infoworks/sdk/cicd/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/cicd_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.085826 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1838 2022-12-19 09:37:04.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1866 2023-02-07 06:50:06.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)    23061 2023-02-07 06:57:00.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/utils.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.091984 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    15404 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/cdata_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    16256 2022-12-19 09:37:04.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/csv_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13421 2022-12-08 16:37:10.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/domains.py
--rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/misc.py
--rw-r--r--   0 infoworks   (501) staff       (20)    17600 2022-12-19 09:37:04.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/pipelines.py
--rw-r--r--   0 infoworks   (501) staff       (20)    16822 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13058 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)      963 2022-12-19 09:42:17.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/update_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12716 2022-12-19 09:37:04.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/workflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)    16379 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
--rw-r--r--   0 infoworks   (501) staff       (20)    23786 2023-02-07 07:32:52.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrappersource.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11359 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1536 2023-01-09 10:16:21.000000 infoworkssdk-2.0.8/infoworks/sdk/client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    18315 2023-02-06 10:33:36.000000 infoworkssdk-2.0.8/infoworks/sdk/domain_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.092317 infoworkssdk-2.0.8/infoworks/sdk/ejson/
--rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-2.0.8/infoworks/sdk/ejson/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-2.0.8/infoworks/sdk/generic_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    47623 2023-02-01 11:21:58.000000 infoworkssdk-2.0.8/infoworks/sdk/jobmetrics.py
--rw-r--r--   0 infoworks   (501) staff       (20)    28866 2023-02-06 09:43:04.000000 infoworkssdk-2.0.8/infoworks/sdk/jobs_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-2.0.8/infoworks/sdk/jobs_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1911 2023-01-27 06:24:03.000000 infoworkssdk-2.0.8/infoworks/sdk/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    36758 2023-02-06 09:43:04.000000 infoworkssdk-2.0.8/infoworks/sdk/pipeline_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/pipeline_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)   114375 2023-02-24 06:20:29.000000 infoworkssdk-2.0.8/infoworks/sdk/source_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/source_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    48803 2023-02-23 16:49:51.000000 infoworkssdk-2.0.8/infoworks/sdk/url_builder.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/utils.py
--rw-r--r--   0 infoworks   (501) staff       (20)    44398 2023-01-30 16:01:11.000000 infoworkssdk-2.0.8/infoworks/sdk/workflow_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-2.0.8/infoworks/sdk/workflow_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-02-24 12:11:31.093777 infoworkssdk-2.0.8/infoworkssdk.egg-info/
--rw-r--r--   0 infoworks   (501) staff       (20)     2431 2023-02-24 12:11:31.000000 infoworkssdk-2.0.8/infoworkssdk.egg-info/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     2227 2023-02-24 12:11:31.000000 infoworkssdk-2.0.8/infoworkssdk.egg-info/SOURCES.txt
--rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-02-24 12:11:31.000000 infoworkssdk-2.0.8/infoworkssdk.egg-info/dependency_links.txt
--rw-r--r--   0 infoworks   (501) staff       (20)      170 2023-02-24 12:11:31.000000 infoworkssdk-2.0.8/infoworkssdk.egg-info/requires.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-02-24 12:11:31.000000 infoworkssdk-2.0.8/infoworkssdk.egg-info/top_level.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-02-24 12:11:31.094371 infoworkssdk-2.0.8/setup.cfg
--rw-r--r--   0 infoworks   (501) staff       (20)     1060 2023-02-23 16:28:27.000000 infoworkssdk-2.0.8/setup.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619391 infoworkssdk-3.0b0/
+-rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/LICENSE
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.619240 infoworkssdk-3.0b0/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-3.0b0/README.md
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.599722 infoworkssdk-3.0b0/infoworks/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/__init__.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.600163 infoworkssdk-3.0b0/infoworks/core/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/core/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/core/iw_authentication.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1080 2023-01-09 10:04:48.000000 infoworkssdk-3.0b0/infoworks/error.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610072 infoworkssdk-3.0b0/infoworks/sdk/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    89421 2023-04-08 13:06:20.000000 infoworkssdk-3.0b0/infoworks/sdk/admin_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/base_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610480 infoworkssdk-3.0b0/infoworks/sdk/cicd/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.612923 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2784 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1929 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    28608 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.617829 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12629 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18649 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13421 2022-12-08 16:37:10.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7881 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    16611 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18556 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    10283 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      963 2022-12-19 09:42:17.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/update_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12796 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    21402 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    26631 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11434 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1650 2023-04-04 12:20:53.000000 infoworkssdk-3.0b0/infoworks/sdk/client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    31762 2023-04-10 04:34:31.000000 infoworkssdk-3.0b0/infoworks/sdk/domain_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.618051 infoworkssdk-3.0b0/infoworks/sdk/ejson/
+-rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-3.0b0/infoworks/sdk/generic_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    32432 2023-04-11 04:32:34.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1911 2023-01-27 06:24:03.000000 infoworkssdk-3.0b0/infoworks/sdk/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    36765 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    47562 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_group_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   176960 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/source_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/source_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    60128 2023-04-11 06:45:26.000000 infoworkssdk-3.0b0/infoworks/sdk/url_builder.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/utils.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    65766 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619020 infoworkssdk-3.0b0/infoworkssdk.egg-info/
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     2325 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/requires.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/top_level.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.619438 infoworkssdk-3.0b0/setup.cfg
+-rw-r--r--   0 infoworks   (501) staff       (20)      896 2023-04-13 12:47:53.000000 infoworkssdk-3.0b0/setup.py
```

### Comparing `infoworkssdk-2.0.8/LICENSE` & `infoworkssdk-3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/PKG-INFO` & `infoworkssdk-3.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 2.0.8
-Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.3 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-2.0
+Version: 3.0b0
+Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
-Author: Abhishek
+Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `infoworkssdk-2.0.8/README.md` & `infoworkssdk-3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/error.py` & `infoworkssdk-3.0b0/infoworks/error.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/admin_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,974 +1,1187 @@
-from infoworks.error import AdminError
+import time
+
+from infoworks.error import WorkflowError
 from infoworks.sdk import url_builder
 from infoworks.sdk.base_client import BaseClient
 from infoworks.sdk.local_configurations import Response, ErrorCode
-from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.utils import IWUtils
+from infoworks.sdk.workflow_response import WorkflowResponse
 
 
-class AdminClient(BaseClient):
+class WorkflowClient(BaseClient):
     def __init__(self):
-        super(AdminClient, self).__init__()
-        self._datalineage = {"path": [], "dataflow_objects": [], "master_pipeline_ids": [],
-                             "master_sourcetable_ids": []}
+        super(WorkflowClient, self).__init__()
 
-    def list_users(self, params=None):
+    def get_list_of_workflows(self, domain_id=None, params=None):
         """
-        Function to list the users
+        Gets List of Infoworks Data workflow details for given domain id
+        :param domain_id: Domain id to which the workflows belongs to, if None all workflows in all domains will be fetched
+        :type domain_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :return: response dict
         """
-        if params is None:
-            params = {"limit": 20, "offset": 0}
-        url_to_list_users = url_builder.list_users_url(self.client_config) \
-                            + IWUtils.get_query_params_string_from_dict(params=params)
+        response = None
+        initial_msg = ""
+        try:
+            if domain_id is None:
+                if params is None:
+                    params = {"limit": 20, "offset": 0}
+                url_to_list_workflows = url_builder.get_all_workflows_url(
+                    self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
+                workflows_list = []
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("GET", url_to_list_workflows,
+                                  IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+                if response is not None:
+                    initial_msg = response.get("message", "")
+                    result = response.get("result", {}).get("items", [])
+                    while len(result) > 0:
+                        workflows_list.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", {}).get("items", [])
+                response["result"] = workflows_list
+                response["message"] = initial_msg
+                return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+            else:
+                workflows_list = []
+                response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.create_workflow_url(
+                    self.client_config, domain_id), IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+
+                if response is not None:
+                    initial_msg = response.get("message", "")
+                    result = response.get("result", [])
+                    while len(result) > 0:
+                        workflows_list.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", [])
+                response["result"] = workflows_list
+                response["message"] = initial_msg
+                return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow details.')
+            raise WorkflowError('Error occurred while trying to get workflow details.')
+
+    def create_workflow(self, domain_id=None, workflow_config=None):
+        """
+        Create a new Workflow
+        :param domain_id: Domain id of the workflow
+        :type domain_id:String
+        :param workflow_config: a JSON object containing workflow configurations
+        :type workflow_config: JSON Object
 
-        users_list = []
+        workflow_config_example = {
+        "name": "workflow_name"
+        }
+        :return: response dict
+        """
+        if None in {domain_id} and workflow_config is None:
+            self.logger.error("domain id or workflow_config cannot be None")
+            raise Exception("domain_id id or workflow_config cannot be None")
+        response = None
         try:
-            response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_users,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None:
-                result = response.get("result", [])
-                while len(result) > 0:
-                    users_list.extend(result)
-                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                      ip=self.client_config['ip'],
-                                                                      port=self.client_config['port'],
-                                                                      protocol=self.client_config['protocol'],
-                                                                      )
-                    response = IWUtils.ejson_deserialize(
-                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                            self.client_config['bearer_token'])).content)
-                    result = response.get("result", None)
-                    if result is None:
-                        return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                            error_code=ErrorCode.GENERIC_ERROR,
-                                                            error_desc="Error in listing users",
-                                                            response=response
-                                                            )
-
-                response["result"] = users_list
-
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-        except Exception as e:
-            self.logger.error("Error in listing users")
-            raise AdminError("Error in listing users" + str(e))
-
-    def create_new_user(self, data=None, name=None, email=None, roles=None, password=None):
-        """
-        Function to create new user in Infoworks
-        :param data: JSON Payload with user details
-        :type data: JSON
-        :param name: Name of the user
-        :type name: String
-        :param email: Email Id of the user
-        :type email: String
-        :param roles: Comma seperated list of roles
-        :type roles: List
-        :param password: Password of the user
-        :type password: String
-
-        example_data = {
-            "profile": {
-                "name": "iwx_sdk_user",
-                "email": "iwx_sdk_user@infoworks.io",
-                "needs_password_reset": False
+            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.create_workflow_url(
+                self.client_config, domain_id), IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                                                               workflow_config).content)
+
+            result = response.get('result', {})
+            workflow_id = result.get('id', None)
+
+            if workflow_id is None:
+                self.logger.error('Workflow failed to create.')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Workflow failed to create.', response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Workflow {id} has been created under domain {domain_id}.'.format(id=workflow_id, domain_id=domain_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to create a new workflow.')
+            raise WorkflowError('Error occurred while trying to create a new workflow.')
+
+    def get_workflow_details(self, workflow_id=None, domain_id=None):
+        """
+        Gets Infoworks Data workflow details for given workflow id
+        :param workflow_id: id of the workflow whose details are to be fetched
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :return: response dict
+        """
+        if None in {domain_id, workflow_id}:
+            self.logger.error("domain id or workflow_id cannot be None")
+            raise Exception("domain_id id or workflow_id cannot be None")
+        response = None
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.create_workflow_url(
+                self.client_config, domain_id) + f"/{workflow_id}", IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', {})
+
+            if result.get('id', None) is None:
+                self.logger.error('Failed to find the workflow details')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to find the workflow details',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully got the workflow {id} details.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow details.')
+            raise WorkflowError('Error occurred while trying to get workflow details.')
+
+    def delete_workflow(self, workflow_id=None, domain_id=None):
+        """
+        Deletes Infoworks Data workflow  for given workflow id
+        :param workflow_id: entity id of the workflow to be deleted
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :return: response dict
+        """
+        if None in {domain_id, workflow_id}:
+            self.logger.error("domain id or workflow_id cannot be None")
+            raise Exception("domain_id id or workflow_id cannot be None")
+        response = None
+        try:
+            if workflow_id is None:
+                self.logger.error('Please pass the mandatory workflow id as parameter.')
+                raise WorkflowError('Please pass the mandatory workflow_id as parameter.')
+            if domain_id is None:
+                self.logger.error('Please pass the mandatory domain_id as parameter.')
+                raise WorkflowError('Please pass the mandatory domain_id as parameter.')
+            response = IWUtils.ejson_deserialize(self.call_api("DELETE", url_builder.create_workflow_url(
+                self.client_config, domain_id) + f"/{workflow_id}", IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', {})
+
+            if result.get('id', None) is None:
+                self.logger.error(f'Failed to delete the workflow {workflow_id}')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to delete the workflow {workflow_id}',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully deleted the workflow {id}.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to delete workflow.')
+            raise WorkflowError('Error occurred while trying to delete workflow.')
+
+    def update_workflow(self, workflow_id=None, domain_id=None, workflow_config=None):
+        """
+        Updates Infoworks Data workflow details for given workflow id
+        :param workflow_id: entity id of the workflow to be updated
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :param workflow_config: a JSON object containing workflow configurations
+        :type workflow_config: JSON Object
+
+        workflow_config_example = {
+         "name": "{string}",
+         "description": "{string}",
+         "child_workflow_ids": [
+          "{array[string]...}"
+         ],
+         "domainId": "{string}",
+         "workflow_graph": {
+          "tasks": [
+           {
+            "task_id": "e77850ad5127a2d7dab870ff",
+            "task_type": "ingest_table_group",
+            "location": "-237 52",
+            "title": "ingest",
+            "task_properties": {},
+            "run_properties": {
+             "enable_exponential_backoff_for_retries": true,
+             "num_retries": 5,
+             "retry_delay": 200,
+             "max_retry_delay": 1000,
+             "trigger_rule": "{string}"
             },
-            "roles": ["modeller"],
-            "password": ""
+            "workflow_variables": "{}"
+           }
+          ],
+          "edges": [
+           {
+            "category": "{string}",
+            "from_task": "{string}",
+            "to_task": "{string}"
+           }
+          ]
+         }
         }
+        :return: response dict
+        """
+        if None in {domain_id, workflow_id} and workflow_config is None:
+            self.logger.error("domain id or workflow_id or workflow_config cannot be None")
+            raise Exception("domain_id or workflow_id or workflow_config cannot be None")
+        response = None
+        try:
+            if "childWorkflowIds" not in workflow_config:
+                workflow_config["child_workflow_ids"] = []
+            response = IWUtils.ejson_deserialize(self.call_api("PATCH", url_builder.create_workflow_url(
+                self.client_config, domain_id) + f"/{workflow_id}", IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), workflow_config).content)
+
+            result = response.get('result', {})
+
+            if result.get('id', None) is None:
+                self.logger.error(f'Failed to update the workflow {workflow_id}')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to update the workflow {workflow_id}',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully updated the workflow {id}.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
 
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to update workflow.')
+            raise WorkflowError('Error occurred while trying to update workflow.')
+
+    def trigger_workflow(self, workflow_id=None, domain_id=None, trigger_wf_body=None):
+        """
+        Triggers Infoworks Data workflow for given workflow id
+        :param workflow_id: entity id of the workflow to be triggered
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :param trigger_wf_body: Pass the workflow parameters if any
+        trigger_wf_body = {
+            "workflow_parameters": [
+                {
+                    "key": "name",
+                    "value": "WF_API_TRIGGER"
+                }
+            ]
+        }
         :return: response dict
         """
-        if roles is None:
-            roles = "modeller"
-        if data is None:
-            if None in {name, email, roles, password}:
-                raise Exception(
-                    f"User creation body (data) or all of the name, email, roles, password has to be passed")
+        if None in {domain_id, workflow_id}:
+            self.logger.error("domain id or workflow_id cannot be None")
+            raise Exception("domain_id or workflow_id cannot be None")
+        response = None
+        try:
+            if trigger_wf_body:
+                response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.trigger_workflow_url(
+                    self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token']), data=trigger_wf_body).content)
             else:
-                data = {
-                    "profile": {
-                        "name": name,
-                        "email": email,
-                        "needs_password_reset": False
-                    },
-                    "roles": roles.split(","),
-                    "password": password
+                response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.trigger_workflow_url(
+                    self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+            result = response.get('result', {})
+            run_id = result.get('id', None)
+            if result.get('id', None) is None:
+                self.logger.error(f'Failed to trigger the workflow {workflow_id}')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to trigger the workflow {workflow_id}',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully triggered the workflow {id} with run id {run_id}.'.format(id=workflow_id, run_id=run_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to trigger workflow.')
+            raise WorkflowError('Error occurred while trying to trigger workflow.')
+
+    def restart_or_cancel_multiple_workflows(self, action_type="restart", workflow_list_body=None):
+        """
+        Restart/Cancel Infoworks Data workflow for given workflow id
+        :param action_type: restart/cancel
+        :param workflow_list_body: JSON object containing array of ids(workflow_id,run_id) to restart/cancel
+        :type workflow_list_body: JSON Dict
+        example: {
+                  "ids": [
+                    {
+                      "workflow_id": "e77850ad5127a2d7dab870ff",
+                      "run_id": "e77850ad5127a2d7dab870ff"
+                    }
+                  ]
                 }
+        :return: response dict
+        """
+        if workflow_list_body is None:
+            self.logger.error("workflow_list_body cannot be None")
+            raise Exception("workflow_list_body cannot be None")
+        if action_type.lower() not in ["restart", "cancel"]:
+            self.logger.error("action_type should be restart or cancel")
+            raise Exception("action_type should be restart or cancel")
+        response = None
         try:
-            response = self.call_api("POST",
-                                     url_builder.list_users_url(self.client_config),
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                     data=data)
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
+            if action_type.lower() == "restart":
+                request_url = url_builder.restart_multiple_workflows_url(self.client_config)
             else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    response=parsed_response,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   "Error in creating user ")
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in creating user " + str(e))
-            raise AdminError("Error in creating user " + str(e))
-
-    def update_the_user(self, user_id, data):
-        """
-        Function to update the user
-        :param user_id: Entity identifier of the user
-        :type user_id: String
-        :param data: JSON Payload with user details
-        :type data: JSON dict
+                request_url = url_builder.cancel_multiple_workflows_url(self.client_config)
+            response = IWUtils.ejson_deserialize(self.call_api("POST", request_url, IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), data=workflow_list_body).content)
+
+            result = response.get('result', None)
+            if result is None:
+                self.logger.error(f'Failed to {action_type} the workflows')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to {action_type} the workflows',
+                                                     response=response)
+
+            self.logger.info(
+                f'Successfully {action_type}d the workflows.')
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception(f'Error occurred while {action_type}ing the workflows.' + str(e))
+            raise WorkflowError(f'Error occurred while {action_type}ing the workflows.' + str(e))
+
+    def cancel_multiple_workflow(self, workflow_list_body=None):
+        """
+        Cancels Infoworks Data workflow for given workflow id
+        :param workflow_list_body: JSON object containing array of ids(workflow_id,run_id) to restart
+        :type workflow_list_body: JSON dict
+        example: {
+                  "ids": [
+                    {
+                      "workflow_id": "e77850ad5127a2d7dab870ff",
+                      "run_id": "e77850ad5127a2d7dab870ff"
+                    }
+                  ]
+                }
         :return: response dict
         """
+        response = None
+        if workflow_list_body is None:
+            self.logger.error("workflow_list_body cannot be None")
+            raise Exception("workflow_list_body cannot be None")
         try:
-            response = self.call_api("PATCH",
-                                     url_builder.list_users_url(self.client_config) + f"/{user_id}",
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                     data=data)
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    response=parsed_response,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   "Error in updating user ")
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in updating user " + str(e))
-            raise AdminError("Error in updating user " + str(e))
-
-    def delete_the_user(self, user_id):
-        """
-        Function to delete the user
-        :param user_id: Entity identifier of the user
-        :type user_id: String
+            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.cancel_multiple_workflows_url(
+                self.client_config), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), data=workflow_list_body).content)
+
+            result_msg = response.get("message", None)
+            if result_msg is None and result_msg == "Submitted Cancel Job for Workflow Run":
+                self.logger.error(f'Failed to cancel the workflows')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to cancel the workflows',
+                                                     response=response)
+
+            self.logger.info(
+                'Successfully Submitted Cancel Job for Workflow Run.')
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while cancelled the workflows.' + str(e))
+            raise WorkflowError('Error occurred while cancelled the workflows.' + str(e))
+
+    def get_status_of_workflow(self, workflow_run_id=None, workflow_id=None):
+        """
+        Fetches status of Infoworks Data workflow for given workflow id and run id
+        :param workflow_run_id: run id of the workflow running
+        :type workflow_run_id: String
+        :param workflow_id: entity id of the workflow running
+        :type workflow_id: String
         :return: response dict
         """
+        if None in {workflow_id, workflow_run_id}:
+            self.logger.error("workflow_id or workflow_run_id cannot be None")
+            raise Exception("workflow_id or workflow_run_id cannot be None")
+        response = None
         try:
-            response = self.call_api("DELETE",
-                                     url_builder.list_users_url(self.client_config) + f"/{user_id}",
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                     )
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    response=parsed_response,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   "Error in deleting user ")
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in deleting user " + str(e))
-            raise AdminError("Error in deleting user " + str(e))
-
-    def get_user_details(self, user_id=None, params=None):
-        """
-        Function to get the user details
-        :param user_id: Entity identifier of the user
-        :type user_id: String
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type params: JSON dict
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
+                self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+            if result is None:
+                self.logger.error('Failed to get the status of workflow')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to get the configuration json of workflow',
+                                                     response=response)
+            run_id = result.get('id', None)
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully got status of the workflow {id} with run id {run_id}.'.format(id=workflow_id,
+                                                                                            run_id=run_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=result)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to fetch status of workflow.')
+            raise WorkflowError('Error occurred while trying to fetch status of workflow.')
+
+    def poll_workflow_run_till_completion(self, workflow_run_id=None, workflow_id=None, poll_interval=30):
+        """
+        Polls Infoworks Data workflow for given workflow id and run id
+        :param workflow_run_id: run id of the workflow running
+        :type workflow_run_id: String
+        :param workflow_id: entity id of the workflow running
+        :type workflow_id: String
+        :param poll_interval:interval in seconds between poll(default 30)
+        :type poll_interval : Int
         :return: response dict
         """
-        if params is None:
-            params = {"limit": 20, "offset": 0}
-        if user_id is not None:
-            url_to_list_user_details = url_builder.list_users_url(self.client_config) + f"/{user_id}"
-        else:
-            url_to_list_user_details = url_builder.list_users_url(
+        response = None
+        if None in {workflow_id, workflow_run_id}:
+            self.logger.error("workflow_id or workflow_run_id cannot be None")
+            raise Exception("workflow_id or workflow_run_id cannot be None")
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
+                self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+            result = response.get('result', {})
+            workflow_status = result['workflow_status']["state"]
+            while workflow_status.lower() not in ['success', 'completed', 'failed', 'aborted', 'canceled']:
+                response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
+                    self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+                result = response.get('result', {})
+                workflow_status = result['workflow_status']["state"]
+                if workflow_status.lower() in ['success', 'completed', 'failed', 'aborted', 'canceled']:
+                    break
+                print(f"workflow_status : {workflow_status}.Sleeping for {poll_interval} seconds")
+                time.sleep(poll_interval)
+
+            run_id = result.get('id', None)
+            if result.get('id', None) is None:
+                self.logger.error(f'Failed to poll status of the workflow {workflow_id}')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to poll status of the workflow {workflow_id}',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully polled status of the workflow {id} with run id {run_id}.'.format(id=workflow_id,
+                                                                                               run_id=run_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to poll status of workflow.')
+            raise WorkflowError('Error occurred while trying to poll status of workflow.')
+
+    def get_workflow_configuration_json_export(self, workflow_id=None, domain_id=None):
+        """
+        Get exported config for workflow with workflow_id in domain with domain_id
+        :param workflow_id: id of the workflow whose details is to be fetched
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :return: response dict
+        """
+        response = None
+        if None in {workflow_id, domain_id}:
+            self.logger.error("workflow_id or domain_id cannot be None")
+            raise Exception("workflow_id or domain_id cannot be None")
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.configure_workflow_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to get the configuration json of workflow')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to get the configuration json of workflow',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully got the workflow {id} configuration json.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow configuration json.')
+            raise WorkflowError('Error occurred while trying to get workflow configuration json.')
+
+    def update_workflow_configuration_json_import(self, workflow_id=None, domain_id=None, workflow_config=None):
+        """
+        Import config for workflow with workflow_id in domain with domain_id
+        :param workflow_id: id of the workflow whose details are to be fetched
+        :type workflow_id: String
+        :param domain_id: Domain id to which the workflow belongs to
+        :type domain_id: String
+        :param workflow_config: configuration json of the workflow
+        :type workflow_config: JSON Object
+        :return: response dict
+        """
+        if None in {workflow_id, domain_id} and workflow_config is None:
+            self.logger.error("workflow_id or domain_id or workflow_config cannot be None")
+            raise Exception("workflow_id or domain_id or workflow_config cannot be None")
+        response = None
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.configure_workflow_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), workflow_config).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to update the configuration json of workflow')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to update the configuration json of workflow',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully updated the workflow {id} configuration json.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to update workflow configuration json.')
+            raise WorkflowError('Error occurred while trying to update workflow configuration json.')
+
+    def get_workflow_id(self, workflow_name=None, domain_id=None, domain_name=None):
+        """
+        Function to get workflow id
+        :param workflow_name: Name of the workflow
+        :param domain_id: Entity identifier of the domain
+        :param domain_name: Entity name of the domain
+        :return: Workflow ID
+
+        example response : {"id": "884236e85b9b1a69b2907e4c"}
+        """
+        if None in {workflow_name}:
+            self.logger.error("workflow_name cannot be None")
+            raise Exception("workflow_name cannot be None")
+        if domain_id is None and domain_name is None:
+            raise Exception(f"Either domain name or domain id has to be passed")
+        if domain_name is not None and domain_id is None:
+            # Find the domain_id
+            params = {"filter": {"name": domain_name}}
+            url_to_list_domains = url_builder.create_domain_url(
                 self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
-        users_list = []
+            try:
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("GET", url_to_list_domains,
+                                  IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+                if response is not None:
+                    result = response.get("result", [])
+                    domain_id = result[0]["id"]
+            except Exception as e:
+                self.logger.error("Error in listing domains")
+                raise WorkflowError("Error in listing domains" + str(e))
         try:
+            params = {"filter": {"name": workflow_name}}
+            url_to_get_wf_info = url_builder.create_workflow_url(self.client_config,
+                                                                 domain_id) + IWUtils.get_query_params_string_from_dict(
+                params=params)
             response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_user_details,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None:
-                initial_msg = response.get("message", "")
-                result = response.get("result", [])
-                if user_id is not None:
-                    users_list.extend([result])
-                else:
-                    while len(result) > 0:
-                        users_list.extend(result)
-                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                          ip=self.client_config['ip'],
-                                                                          port=self.client_config['port'],
-                                                                          protocol=self.client_config['protocol'],
-                                                                          )
-                        response = IWUtils.ejson_deserialize(
-                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                                self.client_config['bearer_token'])).content)
-                        result = response.get("result", [])
-                response["result"] = users_list
-                response["message"] = initial_msg
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error("Failed to get user details")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    response="Failed to get user details"
-                                                    )
-
-        except Exception as e:
-            self.logger.error("Error in listing user information")
-            raise AdminError("Error in listing user information" + str(e))
-
-    def add_domains_to_user(self, domain_id, user_id=None, user_email=None):
-        """
-        Function to make domains accessible to the user
-        :param domain_id: Entity identifier for domain
-        :type domain_id: String
-        :param user_id: Entity identifier for user
-        :type user_id: String
-        :param user_email: email_id of the user
-        :type user_email: String
-        :return: response dict
-        """
-        status_flag = "failed"
-        if user_id is None and user_email is not None:
-            self.logger.info('Getting userID from given user email....')
-            url_for_list_users = url_builder.list_users_url(self.client_config)
-            filter_condition = IWUtils.ejson_serialize({"profile.email": user_email})
-            get_userid_url = url_for_list_users + f"?filter={{filter_condition}}".format(
-                filter_condition=filter_condition)
-            if get_userid_url is not None:
-                try:
-                    response = IWUtils.ejson_deserialize(
-                        self.call_api("GET", get_userid_url,
-                                      IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-                    self.logger.info(response)
-                    if response is not None and "result" in response:
-                        result = response.get("result", [])
-                        if len(result) > 0:
-                            user_id = result[0]["id"]
-                except Exception as e:
-                    self.logger.error('Couldnt get result for the user {}'.format(user_email))
-                    self.logger.error(str(e))
-                    raise AdminError('Couldnt get result for the user {}'.format(user_email))
-                finally:
-                    if user_id is None:
-                        self.logger.error('Couldnt get result for the user {}'.format(user_email))
-                        raise AdminError('Couldnt get result for the user {}'.format(user_email))
-        response = ""
-        if user_id is not None:
-            url_for_adding_user_to_domain = url_builder.add_user_to_domain_url(self.client_config, user_id)
-            self.logger.info('url for adding user to domain - ' + url_for_adding_user_to_domain)
-            if url_for_adding_user_to_domain is not None:
-                self.logger.info('Adding user {user} to domain {domain}'.format(user=user_id, domain=domain_id))
-                try:
-                    json_data = {"entity_ids": [str(domain_id)]}
-                    response = IWUtils.ejson_deserialize(
-                        self.call_api("POST",
-                                      url_for_adding_user_to_domain,
-                                      IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                      data=json_data).content)
-                    if response.get('message', None) is not None:
-                        self.logger.info(response.get('message'))
-                        if response.get('message') == "Added Domain(s) to User":
-                            status_flag = "success"
-                    else:
-                        self.logger.error('Error in adding user to domain - {}'.format(response))
-                except Exception as e:
-                    self.logger.error('Response from server while adding user to domain: {}'.format(user_id))
-                    self.logger.error(str(e))
-                    raise AdminError('Response from server while adding user to domain: {}'.format(user_id))
-        if status_flag == "success":
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-        else:
-            return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                response=response)
-
-    def alation_compatible_lineage_for_source(self, src_id, table_id):
-        """
-        Function to get the lineage of source
-        :param src_id: Entity identifier for source
-        :type src_id: String
-        :param table_id: Entity identifier for table
-        :type table_id: String
-        :return: source lineage info
-        """
-        url_to_get_table_details = url_builder.get_table_configuration(self.client_config, src_id, table_id)
-        response = self.call_api("GET", url_to_get_table_details,
-                                 IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                 )
-        parsed_response = IWUtils.ejson_deserialize(
-            response.content)
-        if response.status_code == 200 and "result" in parsed_response:
-            result = parsed_response.get("result", {})
-            target_schema_name = result["configuration"]["target_schema_name"]
-            target_table_name = result["configuration"]["target_table_name"]
-            orig_db_name = result.get("schema_name_at_source", "csv_source_db")
-            orig_table_name = result.get("original_table_name", "")
-
-            path_to_add = [[{"otype": "table",
-                             "key": f"<DS_ID>.{orig_db_name}.{orig_table_name}"}],
-                           [{"otype": "table",
-                             "key": f"<DS_ID>.{target_schema_name}.{target_table_name}"}]]
-            self._datalineage["path"].append(path_to_add[::])
-
-            for column in result["columns"]:
-                orig_name = column["original_name"]
-                col_name = column["name"]
-                path_to_add = [[{"otype": "column",
-                                 "key": f"<DS_ID>.{orig_db_name}.{orig_table_name}.{orig_name}"}],
-                               [{"otype": "column",
-                                 "key": f"<DS_ID>.{target_schema_name}.{target_table_name}.{col_name}"}]]
-                self._datalineage["path"].append(path_to_add[::])
-        output = {"dataflow_objects": self._datalineage["dataflow_objects"], "paths": self._datalineage["path"]}
-        return output
-
-    def alation_compatible_lineage_for_pipeline(self, domain_id, pipeline_id, pipeline_version_id,
-                                                pl_description=""):
-        """
-        Function to get the lineage of pipeline
-        :param domain_id: Entity identifier for domain
-        :type domain_id: String
-        :param pipeline_id: Entity identifier for pipeline
-        :type pipeline_id: String
-        :param pipeline_version_id: Entity identifier for pipeline version
-        :type pipeline_version_id: String
-        :param pl_description: pipeline description
-        :type pl_description: String
-        :return: response dict
-        """
-        url_to_get_pipelineversion_details = url_builder.list_pipeline_versions_url(self.client_config, domain_id,
-                                                                                    pipeline_id) + f"/{pipeline_version_id}"
-        response = self.call_api("GET", url_to_get_pipelineversion_details,
-                                 IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                 )
-        parsed_response = IWUtils.ejson_deserialize(
-            response.content)
-        if response.status_code == 200 and len(parsed_response.get("result", {})) > 0:
-            pipeline_details = parsed_response.get("result", {})
-            # hash_object = hashlib.md5(f"{pipeline_id}_{pipeline_version_id}".encode())
-            # hashcode = hash_object.hexdigest()
-            hashcode = f"{pipeline_id}_{pipeline_version_id}"
-            for node in pipeline_details["model"].get("nodes", []):
-                req_dict = pipeline_details["model"]["nodes"][node]
-                if req_dict['type'].upper() in ["TARGET", "BIGQUERY_TARGET"]:
-                    src_node_details = []
-                    if req_dict['type'].upper() == "TARGET":
-                        target_schema_name = req_dict['properties'].get("target_schema_name", "")
-                        target_table_name = req_dict['properties'].get("target_table_name", "")
-                    else:
-                        target_schema_name = req_dict['properties'].get("dataset_name", "")
-                        target_table_name = req_dict['properties'].get("table_name", "")
-
-                    output_columns = [i['name'] for i in req_dict["output_entities"]]
-                    for column_name in output_columns:
-                        # print(column_name)
-                        if not column_name.upper().startswith("ZIW"):
-                            url_to_get_pipeline_lineage = url_builder.get_pipeline_lineage_url(self.client_config,
-                                                                                               domain_id,
-                                                                                               pipeline_id,
-                                                                                               pipeline_version_id,
-                                                                                               column_name,
-                                                                                               node)
-                            response = self.call_api("GET", url_to_get_pipeline_lineage,
-                                                     IWUtils.get_default_header_for_v3(
-                                                         self.client_config['bearer_token'])
-                                                     )
-                            parsed_response = IWUtils.ejson_deserialize(
-                                response.content)
-                            if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
-                                graph = parsed_response.get("result", [])
-                                temp_output = []
-                                source_node = graph[-1]
-                                if source_node.get("node_type", "").upper() == "SOURCE_TABLE":
-                                    pl_id = source_node.get("pipeline_id", None)
-                                    if pl_id is not None and pl_id not in self._datalineage["master_pipeline_ids"]:
-                                        self._datalineage["master_pipeline_ids"].append(pl_id)
-                                    src_id = source_node.get("source_id", None)
-                                    table_id = source_node.get("table_id", "")
-                                    if src_id is not None and f"{src_id}:{table_id}" not in self._datalineage[
-                                        "master_sourcetable_ids"]:
-                                        self._datalineage["master_sourcetable_ids"].append(f"{src_id}:{table_id}")
-                                    targetdl_table_name = source_node["target_table_name"]
-                                    targetdl_schema_name = source_node["target_schema_name"]
-                                    if f"<DS_ID>.{targetdl_schema_name}.{targetdl_table_name}" not in src_node_details:
-                                        src_node_details.append(f"<DS_ID>.{targetdl_schema_name}.{targetdl_table_name}")
-                                        path_to_add = [[{"otype": "table",
-                                                         "key": f"<DS_ID>.{targetdl_schema_name}.{targetdl_table_name}"}],
-                                                       [{"otype": "dataflow", "key": f"iwx_pipeline/{hashcode}"}],
-                                                       [{"otype": "table",
-                                                         "key": f"<DS_ID>.{target_schema_name}.{target_table_name}"}]]
-                                        self._datalineage["path"].append(path_to_add[::])
-                                    input_port_column = ""
-                                    if source_node.get("input_port_column", {}) is not None:
-                                        input_port_column = source_node.get("input_port_column", {}).get("name", "")
-                                    key = f"<DS_ID>.{targetdl_schema_name}.{targetdl_table_name}.{input_port_column}"
-                                    temp = [{"otype": "column", "key": key}]
-                                    temp_output.append(temp[::])
-                                temp_output.append([{"otype": "dataflow", "key": f"iwx_pipeline/{hashcode}"}])
-                                key = f"<DS_ID>.{target_schema_name}.{target_table_name}.{column_name}"
-                                temp = [{"otype": "column", "key": key}]
-                                temp_output.append(temp[::])
-                                self._datalineage["path"].append(temp_output[::])
-                        else:
-                            # ziw column direct connect to pipeline
-                            path_to_add = [[{"otype": "dataflow", "key": f"iwx_pipeline/{hashcode}"}],
-                                           [{"otype": "column",
-                                             "key": f"<DS_ID>.{target_schema_name}.{target_table_name}.{column_name}"}]]
-                            self._datalineage["path"].append(path_to_add[::])
-            self._datalineage["dataflow_objects"].append(
-                {"external_id": f"iwx_pipeline/{hashcode}", "content": pl_description})
-            output = {"dataflow_objects": self._datalineage["dataflow_objects"], "paths": self._datalineage["path"]}
-            return output
-
-    def alation_compatible_lineage_for_iwx_metadata(self, domain_id, pipeline_id, sourcetable_ids=None):
-        """
-        Function to ger complete lineage info
-        :param sourcetable_ids: Comma seperated src_id:table_id combination
-        :type sourcetable_ids: Comma seperated src_id:table_id combination
-        :param domain_id: Entity identifier for domain
-        :type domain_id: String
-        :param pipeline_id: Entity identifier for pipeline
-        :type pipeline_id: String
-        :return: lineage info
-        """
-        self._datalineage["master_pipeline_ids"].append(pipeline_id)
-        # Check if there are any more master pipeline ids
-        while len(self._datalineage["master_pipeline_ids"]) > 0:
-            parent_pipeline_id = self._datalineage["master_pipeline_ids"].pop()
-            response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_builder.get_pipeline_url(self.client_config, domain_id, parent_pipeline_id),
+                self.call_api("GET", url_to_get_wf_info,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
                               ).content)
             if response is not None and "result" in response:
-                pipeline_version_id = response.get("result").get("active_version_id")
-                pipeline_description = response.get("result").get("description", "")
-                self.alation_compatible_lineage_for_pipeline(domain_id, parent_pipeline_id, pipeline_version_id,
-                                                             pipeline_description)
-        if sourcetable_ids is not None:
-            self._datalineage["master_sourcetable_ids"].extend(sourcetable_ids.split(","))
-        while len(self._datalineage["master_sourcetable_ids"]) > 0:
-            src_table_id = self._datalineage["master_sourcetable_ids"].pop()
-            src_id, table_id = src_table_id.split(":")
-            self.alation_compatible_lineage_for_source(src_id, table_id)
-
-    def get_environment_details(self, environment_id=None, params=None):
-        """
-        Function to get environment details
-        :param environment_id: Entity identifier of the environment
-        :type environment_id: String
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type params: Dict
-        :return: Response Dict
+                result = response.get("result", None)
+                if result is not None:
+                    return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
+                                                         response={"id": result[0].get('id')})
+        except:
+            raise WorkflowError("Unable to get workflow id from name")
+
+    def get_workflow_name(self, domain_id=None, workflow_id=None):
+        """
+        Function to get workflow name from ID
+        :param workflow_id: Id of the workflow
+        :type workflow_id: String
+        :param domain_id: Entity identifier of the domain
+        :type domain_id: String
+        :return: Workflow name
+
+        example response : {"name": "sample_workflow"}
         """
-        if params is None and environment_id is None:
-            params = {"limit": 20, "offset": 0}
-        url_to_list_environments = url_builder.get_environment_details(
-            self.client_config, environment_id) + IWUtils.get_query_params_string_from_dict(params=params)
-        env_details = []
+        if None in {workflow_id, domain_id}:
+            self.logger.error("workflow_id or domain_id cannot be None")
+            raise Exception("workflow_id or domain_id cannot be None")
         try:
+            url_to_get_wf_info = url_builder.create_workflow_url(self.client_config, domain_id) + f"/{workflow_id}"
             response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_environments,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None:
+                self.call_api("GET", url_to_get_wf_info,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
+                              ).content)
+            if response is not None and "result" in response:
                 result = response.get("result", None)
-                if result is None:
-                    self.logger.error("Failed to get environment details for given id")
-                    return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                        error_code=ErrorCode.USER_ERROR,
-                                                        response=response,
-                                                        error_desc="Failed to get environment details"
-                                                        )
-                initial_msg = response.get("message", "")
-                if environment_id is not None:
-                    env_details.extend([result])
-                else:
-                    while len(result) > 0:
-                        env_details.extend(result)
-                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                          ip=self.client_config['ip'],
-                                                                          port=self.client_config['port'],
-                                                                          protocol=self.client_config['protocol'],
-                                                                          )
-                        response = IWUtils.ejson_deserialize(
-                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                                self.client_config['bearer_token'])).content)
-                        result = response.get("result", [])
-                response["result"] = env_details
-                response["message"] = initial_msg
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error("Failed to get environment details")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    error_desc="Failed to get environment details",
-                                                    response=response
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in getting environment details " + str(e))
-            raise AdminError("Error in getting environment details" + str(e))
-
-    def get_storage_details(self, environment_id, storage_id=None, params=None):
-        """
-        Function to get storage details
-        :param environment_id: Entity identifier of the environment
-        :type environment_id: String
-        :param storage_id: Entity identifier of the storage
-        :type storage_id: String
+                if result is not None:
+                    return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
+                                                         response={"name": result.get("name")})
+        except:
+            raise WorkflowError("Unable to get workflow name")
+
+    def get_list_of_workflow_runs(self, domain_id=None, workflow_id=None, params=None, api_body_for_filter={}):
+        """
+        Gets List of Infoworks Data workflow runs details for given domain id and workflow id
+        :param domain_id: Domain id to which the workflows belongs to, if None all workflows in all domains will be fetched
+        :type domain_id: String
+        :param workflow_id: Workflow id,if None all workflow runs in all domains will be fetched
+        :type workflow_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type params: Dict
-        :return: Response Dict
+        :type: JSON dict
+        :param api_body_for_filter: dict of API body
+        :type api_body_for_filter: JSON dict
+        example: {'limit': 10000, 'date_range': {'type': 'last', 'unit': 'day', 'value': 1}, 'offset': 0}
+        :return: response List
         """
-        if params is None and storage_id is None:
-            params = {"limit": 20, "offset": 0}
-        url_to_list_storages = url_builder.get_environment_storage_details(
-            self.client_config, environment_id, storage_id) + IWUtils.get_query_params_string_from_dict(params=params)
-        storage_details = []
+        response = None
+        initial_msg = ""
         try:
-            response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_storages,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None:
-                result = response.get("result", None)
-                if result is None:
-                    self.logger.error("Failed to get environment storage details for given id")
-                    return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                        error_code=ErrorCode.USER_ERROR,
-                                                        response=response,
-                                                        error_desc="Failed to get environment storage details"
-                                                        )
-                initial_msg = response.get("message", "")
-                if storage_id is not None:
-                    storage_details.extend([result])
-                else:
+            if domain_id is None:
+                url_to_list_workflow_runs = url_builder.get_all_workflows_runs_url(
+                    self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
+                if not api_body_for_filter.get("limit", None):
+                    api_body_for_filter["limit"] = 10000
+
+                if not api_body_for_filter.get("date_range", None):
+                    api_body_for_filter["date_range"] = {"type": "last", "unit": "day", "value": 1}
+                api_body_for_filter["offset"] = 0
+                workflow_runs_list = []
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("POST", url_to_list_workflow_runs,
+                                  IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                                  data=api_body_for_filter).content)
+                if response is not None:
+                    initial_msg = response.get("message", "")
+                    result = response.get("result", [])
+                    if len(result) == 0:
+                        self.logger.error('Failed to update the configuration json of workflow')
+                        return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                             error_code=ErrorCode.USER_ERROR,
+                                                             error_desc='Failed to get the workflow run id jobs',
+                                                             response=response)
                     while len(result) > 0:
-                        storage_details.extend(result)
-                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                          ip=self.client_config['ip'],
-                                                                          port=self.client_config['port'],
-                                                                          protocol=self.client_config['protocol'],
-                                                                          )
+                        workflow_runs_list.extend(result)
+                        api_body_for_filter["offset"] = api_body_for_filter.get("limit")
                         response = IWUtils.ejson_deserialize(
-                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                                self.client_config['bearer_token'])).content)
+                            self.call_api("POST", url_to_list_workflow_runs, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token']), data=api_body_for_filter).content)
                         result = response.get("result", [])
-                response["result"] = storage_details
+                response["result"] = workflow_runs_list
                 response["message"] = initial_msg
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+                return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
             else:
-                self.logger.error("Failed to get storage details")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    response="Failed to get storage details"
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in getting storage details " + str(e))
-            raise AdminError("Error in getting storage details" + str(e))
-
-    def get_compute_template_details(self, environment_id, compute_id=None, is_interactive=False, params=None):
-        """
-         Function to get compute template details
-         :param environment_id: Entity identifier of the environment
-         :type environment_id: String
-         :param compute_id: Entity identifier of compute cluster
-         :type compute_id: String
-         :param is_interactive: True/False. If True only the details of interactive clusters is fetched
-         :type is_interactive: Boolean
-         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-         :type params: Dict
-         :return: Response Dict
-         """
-        if params is None and compute_id is None:
-            params = {"limit": 20, "offset": 0}
-        if is_interactive:
-            url_to_list_computes = url_builder.get_environment_interactive_compute_details(
-                self.client_config, environment_id, compute_id) + IWUtils.get_query_params_string_from_dict(
-                params=params)
-        else:
-            url_to_list_computes = url_builder.get_environment_compute_details(
-                self.client_config, environment_id, compute_id) + IWUtils.get_query_params_string_from_dict(
-                params=params)
-        compute_details = []
-        try:
-            response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_computes,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None and "result" in response:
-                result = response.get("result", None)
+                workflow_runs_list = []
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("GET", url_builder.get_all_workflows_runs_url_with_domain_id(
+                        self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                        self.client_config['bearer_token'])).content)
+
+                result = response.get('result', None)
                 if result is None:
-                    self.logger.error("Failed to get environment compute details for given id")
-                    return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                        error_code=ErrorCode.USER_ERROR,
-                                                        response=response,
-                                                        error_desc="Failed to get environment compute details"
-                                                        )
-                initial_msg = response.get("message", "")
-                if compute_id is not None:
-                    compute_details.extend([result])
-                else:
+                    self.logger.error('Failed to get the list of workflow runs')
+                    return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                         error_code=ErrorCode.USER_ERROR,
+                                                         error_desc='Failed to get the workflow run id jobs',
+                                                         response=response)
+                if response is not None:
+                    result = response.get("result", [])
+                    initial_msg = response.get("message", "")
                     while len(result) > 0:
-                        compute_details.extend(result)
+                        workflow_runs_list.extend(result)
                         nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                           ip=self.client_config['ip'],
                                                                           port=self.client_config['port'],
                                                                           protocol=self.client_config['protocol'],
                                                                           )
                         response = IWUtils.ejson_deserialize(
                             self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
                                 self.client_config['bearer_token'])).content)
                         result = response.get("result", [])
-                response["result"] = compute_details
-                response["message"] = initial_msg
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error("Failed to get compute template details")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    error_desc="Failed to get compute template details",
-                                                    response=response
-                                                    )
-        except Exception as e:
-            self.logger.error("Error in getting compute template details " + str(e))
-            raise AdminError("Error in getting compute template details" + str(e))
-
-    def get_environment_id_from_name(self, environment_name):
-        """
-        Function to return environment Id from name
-        :param environment_name: Infoworks Environment Name
-        :type environment_name: String
-        :return: Response Dict
+                    response["result"] = workflow_runs_list
+                    response["message"] = initial_msg
+                return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow details.')
+            raise WorkflowError('Error occurred while trying to get workflow details.')
+
+    def get_list_of_workflow_runs_jobs(self, run_id=None, params=None):
+        """
+         Gets List of Infoworks Data workflow runs jobs details
+        :param run_id: Run id to which the workflows belongs to, if None all workflows
+        :type run_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response dict
         """
-        response = self.get_environment_details(environment_id=None, params={"filter": {"name": environment_name}})
-        if response.get("result", {}).get("status", "") == Response.Status.SUCCESS:
-            result = response.get("result", {}).get("response", {}).get("result", {})
-            if len(result) > 0:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response={"environment_id": result[0]["id"]})
+        if None in {run_id}:
+            self.logger.error("run_id cannot be None")
+            raise Exception("run_id cannot be None")
+        response = None
+        try:
+            workflow_run_jobs_list = []
+            get_all_workflow_run_jobs_url = url_builder.get_all_workflow_run_jobs_url(self.client_config, run_id)
+            if params is None:
+                get_all_workflow_run_jobs_url = get_all_workflow_run_jobs_url + "?fetch_summary=true&recursive_job_search=true"
             else:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response={"environment_id": None}
-                                                    )
-        else:
-            return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                error_code=ErrorCode.USER_ERROR,
-                                                response=response.get("result", {}).get("response", {})
-                                                )
-
-    def get_environment_default_warehouse(self, environment_id):
-        """
-        Function to return default warehouse name
-        :param environment_id: Infoworks Environment Id
-        :type environment_id: String
-        :return: Response Dict
+                get_all_workflow_run_jobs_url = get_all_workflow_run_jobs_url + \
+                                                IWUtils.get_query_params_string_from_dict(params=params) + \
+                                                "&fetch_summary=true&recursive_job_search=true"
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", get_all_workflow_run_jobs_url, IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+            initial_msg = ""
+            if result is None:
+                self.logger.error('Failed to get list of workflow runs jobs')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to get the workflow run id jobs',
+                                                     response=response)
+
+            if response is not None:
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    workflow_run_jobs_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+            response["result"] = workflow_run_jobs_list
+            response["message"] = initial_msg
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get jobs under workflow run.' + str(e))
+            raise WorkflowError('Error occurred while trying to get jobs under workflow run.' + str(e))
+
+    def get_list_of_domain_workflow_schedules(self, domain_id, params=None):
         """
-        response = self.get_environment_details(environment_id=environment_id, params=None)
-        if response.get("result", {}).get("status", "") == Response.Status.SUCCESS:
-            result = response.get("result", {}).get("response", {}).get("result", [])
-            if len(result) > 0:
-                for item in result[0]["data_warehouse_configuration"]["warehouse"]:
-                    if item["is_default_warehouse"]:
-                        return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                            response={"default_warehouse": item["name"]})
-                else:
-                    return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                        response={"default_warehouse":
-                                                                      result[0]["data_warehouse_configuration"][
-                                                                          "warehouse"][0]["name"]})
-            else:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response=result
-                                                    )
-        else:
-            return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                error_code=ErrorCode.USER_ERROR,
-                                                response=response.get("result", {}).get("response", {})
-                                                )
-
-    def get_compute_id_from_name(self, environment_id, compute_name):
-        """
-        Function to return Environment Compute Id from name
-        :param environment_id: Environment identifier
-        :type environment_id: String
-        :param compute_name: Environment Compute Name
-        :type compute_name: String
+        Gets List of Schedules of all Workflows belonging to the Domain
+        :param domain_id: Domain Id to list the schedules configured
+        :type domain_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type params: JSON Dict
         :return: Response Dict
         """
-        response = self.get_compute_template_details(environment_id, compute_id=None, is_interactive=True,
-                                                     params={"filter": {"name": compute_name}})
-        if response.get("result", {}).get("status", "") == Response.Status.SUCCESS:
-            result = response.get("result", {}).get("response", {}).get("result", [])
-            if len(result) > 0:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response={"compute_id": result[0]["id"]})
-            else:
-                response_non_interactive = self.get_compute_template_details(environment_id, compute_id=None,
-                                                                             is_interactive=False,
-                                                                             params={"filter": {"name": compute_name}})
-                result_non_interactive = response_non_interactive.get("result", {}).get("response", {}).get("result",
-                                                                                                            [])
-                if len(result_non_interactive) > 0:
-                    return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                        response={"compute_id": result_non_interactive[0]["id"]})
-                else:
-                    return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                        response={"compute_id": None}
-                                                        )
-        else:
-            return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                error_code=ErrorCode.USER_ERROR,
-                                                response=response.get("result", {}).get("response", {})
-                                                )
-
-    def get_storage_id_from_name(self, environment_id, storage_name):
-        """
-        Function to return Environment Storage Id from name
-        :param environment_id: Environment identifier
-        :type environment_id: String
-        :param storage_name: Environment Storage Name
-        :type storage_name: String
-        :return: Response Dict
+        if domain_id is None:
+            self.logger.error("domain_id cannot be None")
+            raise Exception("domain_id cannot be None")
+
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+
+        domain_schedules = []
+        response = None
+        initial_msg = ''
+        try:
+            domain_schedules_url = url_builder.get_domain_workflow_schedules_url(self.client_config, domain_id) + \
+                                   IWUtils.get_query_params_string_from_dict(params=params)
+
+            response = IWUtils.ejson_deserialize(self.call_api("GET", domain_schedules_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token'])).content)
+            if response:
+                initial_msg = response.get("message", '')
+                result = response.get("result", [])
+
+                while len(result) > 0:
+                    domain_schedules.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+            response["result"] = domain_schedules
+            response["message"] = initial_msg
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get domain schedules .')
+            raise WorkflowError('Error occurred while trying to get domain schedules.')
+
+    def get_workflow_schedule(self, domain_id, workflow_id):
         """
-        response = self.get_storage_details(environment_id=environment_id,
-                                            params={"filter": {"name": storage_name}})
-        if response.get("result", {}).get("status", "") == Response.Status.SUCCESS:
-            result = response.get("result", {}).get("response", {}).get("result", [])
-            if len(result) > 0:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response={"storage_id": result[0]["id"]})
-            else:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
-                                                    response={"storage_id": None}
-                                                    )
-        else:
-            return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                error_code=ErrorCode.USER_ERROR,
-                                                response=response.get("result", {}).get("response", {})
-                                                )
-
-    def get_source_extension(self, extension_id):
-        """
-        Function to get a source extension details
-        :param extension_id: ID of the source extension
-        :type extension_id: String
+        Gets Schedules of particular Workflow belonging to the Domain
+        :param domain_id: Domain ID of which Workflow belongs
+        :type domain_id: String
+        :param workflow_id: Workflow ID to fetch schedule for.
+        :type workflow_id: String
         :return: Response Dict
         """
+        if domain_id is None or workflow_id is None:
+            self.logger.error("domain_id or workflow_id cannot be None")
+            raise Exception("domain_id or workflow_id cannot be None")
+
+        response = None
+
         try:
-            response = self.call_api("GET",
-                                     url_builder.create_source_extension_url(self.client_config) + f"/{extension_id}",
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                     )
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   f"Error getting source extension {extension_id}."),
-                                                    response=parsed_response
-                                                    )
-        except Exception as e:
-            self.logger.error(f"Error getting source extension {extension_id}.")
-            raise AdminError(
-                f"Error getting source extension {extension_id}." + str(e))
-
-    def create_source_extension(self, data):
-        """
-        Function to create a source extension
-        :param data: Source extension details body
-        :type data: Dict
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_schedule_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow schedule.')
+            raise WorkflowError('Error occurred while trying to get workflow schedule.')
+
+    def enable_workflow_schedule(self, domain_id, workflow_id, schedule_config):
+        """
+        Enables Schedule of a particular Workflow belonging to the Domain
+        :param domain_id: Domain ID of which Workflow belongs
+        :type domain_id: String
+        :param workflow_id: Workflow ID to fetch schedule for.
+        :type workflow_id: String
+        :param schedule_config: Schedule Configuration JSON of the Workflow
+        :type schedule_config: JSON
+
+        schedule_config_example = {
+              "start_date": "02/22/2020",
+              "end_date": "02/24/2020",
+              "start_hour": 12,
+              "start_min": 25,
+              "end_hour": 17,
+              "end_min": 30,
+              "repeat_interval_measure": 2,
+              "repeat_interval_unit": "{string}",
+              "ends": true,
+              "is_custom_job": true,
+              "custom_job_details": {
+                "starts_daily_at": "14:00",
+                "ends_daily_at": "15:00",
+                "repeat_interval_unit": "{string}",
+                "repeat_interval_measure": 2
+              },
+              "repeat_on_last_day": "{boolean}",
+              "specified_days": 1
+        }
+
         :return: Response Dict
         """
+        if domain_id is None or workflow_id is None or schedule_config is None:
+            self.logger.error("domain_id or workflow_id or schedule_config cannot be None")
+            raise Exception("domain_id or workflow_id or schedule_config cannot be None")
+        response = None
         try:
-            response = self.call_api("POST",
-                                     url_builder.create_source_extension_url(self.client_config),
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                     data=data)
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   f"Error creating source extension {data['name']}")
-                                                    )
-        except Exception as e:
-            self.logger.error(f"Error creating source extension {data['name']}.Please do it by yourself from UI.")
-            raise AdminError(
-                f"Error creating source extension  {data['name']}.Please do it by yourself from UI." + str(e))
-
-    def update_source_extension(self, extension_id, data=None):
-        """
-        Function to update a source extension
-        :param extension_id: Id of the source extension to update
-        :type extension_id: String
-        :param data: JSON dict of the body to update
-        :type data: JSON dict
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.get_enable_workflow_schedule_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), schedule_config).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to enable schedule of the workflow')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to enable schedule of the workflow',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully enabled schedule for the workflow {id}.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to enable workflow schedule.')
+            raise WorkflowError('Error occurred while trying to enable workflow schedule.')
+
+    def disable_workflow_schedule(self, domain_id, workflow_id):
+        """
+        Disables Schedule of a particular Workflow belonging to the Domain
+        :param domain_id: Domain ID of which Workflow belongs
+        :type domain_id: String
+        :param workflow_id: Workflow ID to fetch schedule for.
+        :type workflow_id: String
         :return: Response Dict
         """
-        if None in {extension_id} and data is None:
-            self.logger.error("Extension id or data cannot be None")
-            raise Exception("Extension id or data cannot be None")
-        try:
-            response = self.call_api("PUT",
-                                     url_builder.create_source_extension_url(self.client_config) + f"/{extension_id}",
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                     , data=data)
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   f"Error updating source extension {extension_id}."),
-                                                    response=parsed_response
-                                                    )
-        except Exception as e:
-            self.logger.error(f"Error updating source extension {extension_id}.")
-            raise AdminError(
-                f"Error updating source extension {extension_id}." + str(e))
-
-    def delete_source_extension(self, extension_id):
-        """
-        Function to delete a source extension
-        :param extension_id: ID of the source extension
-        :type extension_id: String
+        if domain_id is None or workflow_id is None:
+            self.logger.error("domain_id or workflow_id cannot be None")
+            raise Exception("domain_id or workflow_id cannot be None")
+        response = None
+        try:
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.get_disable_workflow_schedule_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to disable schedule of the workflow')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to disable schedule of the workflow',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully disabled schedule for the workflow {id}.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to disable workflow schedule.')
+            raise WorkflowError('Error occurred while trying to disable workflow schedule.')
+
+    def update_workflow_schedule_user(self, domain_id, workflow_id):
+        """
+        Changes Workflow Schedule User of a particular Workflow belonging to the Domain
+        :param domain_id: Domain ID of which Workflow belongs
+        :type domain_id: String
+        :param workflow_id: Workflow ID to fetch schedule for.
+        :type workflow_id: String
         :return: Response Dict
         """
+        if domain_id is None or workflow_id is None:
+            self.logger.error("domain_id or workflow_id cannot be None")
+            raise Exception("domain_id or workflow_id cannot be None")
+        response = None
         try:
-            response = self.call_api("DELETE",
-                                     url_builder.create_source_extension_url(self.client_config) + f"/{extension_id}",
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-                                     )
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   f"Error deleting source extension {extension_id}."),
-                                                    response=parsed_response
-                                                    )
-        except Exception as e:
-            self.logger.error(f"Error deleting source extension {extension_id}.")
-            raise AdminError(
-                f"Error deleting source extension {extension_id}." + str(e))
-
-    def create_data_connection(self, config_body):
-        """
-        Function to create data connection in the domain
-        :param config_body: JSON payload
-        :type config_body: JSON dict
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", url_builder.update_workflow_schedule_user_url(
+                self.client_config, domain_id, workflow_id), IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token'])).content)
+
+            result = response.get('result', None)
+
+            if result is None:
+                self.logger.error('Failed to update workflow schedule user')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to update workflow schedule user',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully updated workflow {id} schedule user.'.format(id=workflow_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to update workflow schedule user.')
+            raise WorkflowError('Error occurred while trying to update workflow schedule user.')
+
+
+
+    def pause_or_resume_multiple_workflows(self, action_type="pause", workflow_list_body=None):
+        """
+        Pause/resume Infoworks Data workflow for given workflow ids
+        :param action_type: pause/resume
+        :param workflow_list_body: JSON object containing array of workflow ids
+        :type workflow_list_body: JSON Dict
+        workflow_list_body_example: {
+        "workflow_ids": ["c265e25b886a1b5e09896885"]
+        }
         :return: response dict
         """
+        if workflow_list_body is None:
+            self.logger.error("workflow_list_body cannot be None")
+            raise Exception("workflow_list_body cannot be None")
+        if action_type.lower() not in ["pause", "resume"]:
+            self.logger.error(f"action_type cannot be {action_type}. Supported resume/pause")
+            raise Exception(f"action_type cannot be {action_type}. Supported resume/pause")
+        response = None
         try:
-            create_data_connection_url = url_builder.create_data_connection(self.client_config)
-            response = self.call_api("POST", create_data_connection_url,
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                     config_body)
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
+            if action_type.lower() == "pause":
+                request_url = url_builder.pause_multiple_workflows_url(self.client_config)
             else:
-                self.logger.error("Failed to create data connection")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   "Failed to create data connection"),
-                                                    job_id=None, response=parsed_response)
-        except Exception as e:
-            raise AdminError(f"Failed to create data connection" + str(e))
-
-    def get_data_connection(self, data_connection_id=None, params=None):
-        """
-        Function to create data connection in the domain
-        :param data_connection_id: id of dataconnection for which config has to be fetched
-        :type data_connection_id: String
+                request_url = url_builder.resume_multiple_workflows_url(self.client_config)
+            response = IWUtils.ejson_deserialize(self.call_api("POST", request_url, IWUtils.get_default_header_for_v3(
+                self.client_config['bearer_token']), data=workflow_list_body).content)
+            result = response.get('result', None)
+            if result is None:
+                self.logger.error(f'Failed to {action_type} the workflows')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to {action_type} the workflows',
+                                                     response=response)
+
+            self.logger.info(
+                f'Successfully {action_type}d the workflows.')
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS,
+                                                 response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception(f'Error occurred while {action_type}d the workflows.' + str(e))
+            raise WorkflowError(f'Error occurred while {action_type}d the workflows.' + str(e))
+
+    def get_global_list_of_workflow_runs(self, params=None):
+        """
+        Gets List of all the Infoworks Data workflows. Need admin access
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :return: response dict
         """
-        if params is None:
-            params = {"limit": 20, "offset": 0}
-
-        if data_connection_id is None:
-            url_to_get_data_connection = url_builder.create_data_connection(
+        response = None
+        initial_msg = ""
+        try:
+            if params is None:
+                params = {"limit": 20, "offset": 0}
+            url_to_list_workflow_runs = url_builder.get_workflow_runs_url(
                 self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
-        else:
-            url_to_get_data_connection = url_builder.create_data_connection(
-                self.client_config) + f"/{data_connection_id}"
-        dataconnection_list = []
+            workflow_run_list = []
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_list_workflow_runs,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                initial_msg = response.get("message", "")
+                result = response.get("result", {}).get("items", [])
+                while len(result) > 0:
+                    workflow_run_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", {}).get("items", [])
+            response["result"] = workflow_run_list
+            response["message"] = initial_msg
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow run details.')
+            raise WorkflowError('Error occurred while trying to get workflow run details.')
+
+    def get_list_of_workflow_tasks(self, params=None):
+        """
+        Gets List of all the Infoworks Data workflow tasks
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response dict
+        """
+        response = None
+        initial_msg = ""
         try:
-            response = IWUtils.ejson_deserialize(self.call_api("GET", url_to_get_data_connection,
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token'])).content)
+            if params is None:
+                params = {"limit": 20, "offset": 0}
+            url_to_list_workflow_run_tasks = url_builder.get_workflow_tasks_url(
+                self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
+            workflow_run_tasks_list = []
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_list_workflow_run_tasks,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
-                result = response.get("result", [])
                 initial_msg = response.get("message", "")
-                if data_connection_id is not None:
-                    dataconnection_list.extend(result)
-                else:
-                    while len(result) > 0:
-                        dataconnection_list.extend(result)
-                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                          ip=self.client_config['ip'],
-                                                                          port=self.client_config['port'],
-                                                                          protocol=self.client_config['protocol'],
-                                                                          )
-                        response = IWUtils.ejson_deserialize(
-                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                                self.client_config['bearer_token'])).content)
-                        result = response.get("result", [])
-                response["result"] = dataconnection_list
-                response["message"] = initial_msg
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error("Failed to get data connection details")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    response="Failed to get data connection details"
-                                                    )
-        except Exception as e:
-            raise AdminError(f"Failed to get data connection details" + str(e))
-
-    def delete_data_connection(self, data_connection_id):
-        """
-        Function to delete data connection in the domain
-        :param data_connection_id: Entity identifier for the data connection
-        :type data_connection_id: String
+                result = response.get("result", {}).get("items", [])
+                while len(result) > 0:
+                    workflow_run_tasks_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", {}).get("items", [])
+            response["result"] = workflow_run_tasks_list
+            response["message"] = initial_msg
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow run task details.')
+            raise WorkflowError('Error occurred while trying to get workflow run task details.')
+
+    def get_workflow_run_details(self, workflow_id=None, run_id=None):
+        """
+        Gets Infoworks Data workflow run details for given workflow id
+        :param workflow_id: id of the workflow whose details are to be fetched
+        :type workflow_id: String
+        :param run_id: Workflow run id
+        :type run_id: String
         :return: response dict
         """
+        if None in {run_id, workflow_id}:
+            self.logger.error("run_id id or workflow_id cannot be None")
+            raise Exception("run_id id or workflow_id cannot be None")
+        response = None
         try:
-            create_data_connection_url = url_builder.create_data_connection(self.client_config).strip(
-                "/") + f"/{data_connection_id}"
-            response = self.call_api("DELETE", create_data_connection_url,
-                                     IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                                     )
-            parsed_response = IWUtils.ejson_deserialize(
-                response.content)
-            if response.status_code == 200:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=parsed_response)
-            else:
-                self.logger.error("Failed to delete data connection")
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.GENERIC_ERROR,
-                                                    error_desc=parsed_response.get("details",
-                                                                                   "Failed to delete data connection"),
-                                                    response=parsed_response)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_run_id_details_url(self.client_config, workflow_id, run_id)
+                                                               , IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            result = response.get('result', {})
+            if result.get('id', None) is None:
+                self.logger.error('Failed to find the workflow run details')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc='Failed to find the workflow run details',
+                                                     response=response)
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully got the workflow run details.')
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
+
         except Exception as e:
-            raise AdminError(f"Failed in deleting data connection" + str(e))
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to get workflow run details.')
+            raise WorkflowError('Error occurred while trying to get workflow run details.')
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/base_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,389 +1,290 @@
 import json
-import logging.config
-import os
-from configparser import ConfigParser
-from pathlib import Path
 import requests
-from google.cloud import kms, storage
-import boto3
-import base64
-from cryptography.fernet import Fernet
-from infoworks.core.iw_authentication import is_token_valid, get_bearer_token, aes_encrypt
-from infoworks.sdk import local_configurations
-from requests.adapters import HTTPAdapter
-from urllib3.util.retry import Retry
+import yaml
+from infoworks.sdk.url_builder import get_source_details_url, list_secrets_url
 from infoworks.sdk.utils import IWUtils
-import urllib3
-urllib3.disable_warnings()
-
-
-class TimeoutHTTPAdapter(HTTPAdapter):
-    def __init__(self, *args, **kwargs):
-        self.timeout = local_configurations.REQUEST_TIMEOUT_IN_SEC
-        if "timeout" in kwargs:
-            self.timeout = kwargs["timeout"]
-            del kwargs["timeout"]
-        super().__init__(*args, **kwargs)
-
-    def send(self, request, **kwargs):
-        timeout = kwargs.get("timeout")
-        if timeout is None:
-            kwargs["timeout"] = self.timeout
-        return super().send(request, **kwargs)
-
-
-def initialise_http_client():
-    retries = Retry(total=local_configurations.MAX_RETRIES, backoff_factor=1,
-                    status_forcelist=[429, 500, 502, 503, 504])
-    http = requests.Session()
-    adapter = TimeoutHTTPAdapter(max_retries=retries)
-    http.mount("https://", adapter)
-    http.mount("http://", adapter)
-    return http
-
+from infoworks.sdk.source_response import SourceResponse
+from infoworks.sdk.local_configurations import Response
+from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+import configparser
+
+class CSVSource:
+    def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
+        self.storage_id = storage_id
+        self.environment_id = environment_id
+        self.source_config_path = source_config_path
+        self.secrets = secrets
+        with open(self.source_config_path, 'r') as file:
+            json_string = file.read()
+            if replace_words != "":
+                for key, value in [item.split("->") for item in replace_words.split(";")]:
+                    json_string = json_string.replace(key, value)
+        self.configuration_obj = IWUtils.ejson_deserialize(json_string)
+
+    def update_mappings_for_configurations(self, mappings):
+        config = configparser.ConfigParser()
+        config.read_dict(mappings)
+        d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
+        for section in config.sections():
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
+                continue
+            print("section:", section)
+            final = d.setval(section.split("$"), dict(config.items(section)))
+            print(f"section replacement:{d.getval(section.split('$'))}")
+        self.configuration_obj = d.data
+
+    def get_secret_id_from_name(self,cicd_client,secret_name):
+        secret_id = None
+        get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"name":"'+secret_name+'"}'
+        response = cicd_client.call_api("GET", get_secret_details_url,
+                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
+        parsed_response = IWUtils.ejson_deserialize(response.content)
+        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+            result = parsed_response.get("result", [])
+
+            if len(result) > 0:
+                secret_id = result[0]["id"]
+                cicd_client.logger.info("Found secret id {} ".format(secret_id))
+                return secret_id
+            else:
+                cicd_client.logger.info("Secret id is {} ".format(None))
+                return None
 
-class BaseClient(object):
-    def __init__(self):
-        # print("Inside BaseClient")
-        self.client_config = {
-            'protocol': None,
-            'ip': None,
-            'port': None,
-            'refresh_token': None,
-            'bearer_token': None,
-            'default_environment_id': None,
-            'default_storage_id': None,
-            'default_compute_id': None
+    def create_csv_source(self, src_client_obj):
+        data = self.configuration_obj["configuration"]["source_configs"]
+        create_csv_source_payload = {
+            "name": data["name"],
+            "type": data["type"],
+            "sub_type": data["sub_type"],
+            "data_lake_path": data["data_lake_path"],
+            "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
+            "environment_id": self.environment_id,
+            "storage_id": self.storage_id,
+            "is_source_ingested": True
         }
-        self.secrets_config = {"custom_secrets_read": False}
-        self.mappings = {}
-        self.http = initialise_http_client()
-        log_path = Path(local_configurations.LOG_LOCATION)
-        if os.path.isdir(log_path.parent.absolute()):
-            logging.basicConfig(filename=local_configurations.LOG_LOCATION, filemode='w',
-                                format='%(asctime)s - %(module)s - %(pathname)s - %(lineno)d - %(levelname)s - %(message)s',
-                                level=logging.DEBUG, datefmt='%Y-%m-%d %H:%M:%S')
-        else:
-            logging.basicConfig(
-                format='%(asctime)s - %(module)s - %(pathname)s - %(lineno)d - %(levelname)s - %(message)s',
-                level=logging.DEBUG, datefmt='%Y-%m-%d %H:%M:%S')
-        self.logger = logging.getLogger('infoworks_sdk_logs')
-
-    def initialize_client(self, protocol=None, ip=None, port=None, ):
-        """
-        initialize the client
-        :param protocol: protocol to be used for server call
-        :type protocol: String
-        :param ip: Client IP
-        :type ip: String
-        :param port: Client Port
-        :type port: String
-        """
-
-        if all(v is not None for v in [protocol, ip, port]):
-            self.client_config['protocol'] = protocol
-            self.client_config['ip'] = ip
-            self.client_config['port'] = port
+        if data.get("target_database_name",""):
+            create_csv_source_payload["target_database_name"] = data.get("target_database_name","")
+        if data.get("staging_schema_name",""):
+            create_csv_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
+        src_create_response = src_client_obj.create_source(source_config=create_csv_source_payload)
+        if src_create_response["result"]["status"].upper() == "SUCCESS":
+            source_id_created = src_create_response["result"]["source_id"]
+            print("Source created successfully")
+            return src_create_response
         else:
-            logging.error(ValueError("Pass valid values"))
-            raise ValueError("Pass valid values")
-
-    def initialize_client_with_defaults(self, protocol, ip, port, refresh_token, default_environment_id=None,
-                                        default_storage_id=None, default_compute_id=None):
-        """
-        initializes the client and a user with given configuration
-        :param protocol: protocol to be used for server call
-        :type protocol: String
-        :param ip: ip address of the server
-        :type ip: String
-        :param port: port on which the rest service resides
-        :type port: String
-        :param refresh_token: refresh_token of the user
-        :type refresh_token: String
-        :param default_compute_id: Pass the default compute id to be used for all the artifacts to be created
-        :param default_storage_id: Pass the default storage id to be used for all the artifacts to be created
-        :param default_environment_id: Pass the default environment id to be used for all the artifacts to be created
-        """
-        self.client_config['refresh_token'] = refresh_token
-        self.client_config['bearer_token'] = get_bearer_token(protocol, ip, port, refresh_token)
-        self.initialize_client(protocol, ip, port)
-        self.client_config[
-            'default_environment_id'] = default_environment_id if default_environment_id is not None else None
-        self.client_config['default_storage_id'] = default_storage_id if default_storage_id is not None else None
-        self.client_config['default_compute_id'] = default_compute_id if default_compute_id is not None else None
-
-    def get_configurations(self):
-        """
-        returns client configurations
-        :return: configuration dictionary
-        """
-        return self.client_config
-
-    def regenerate_bearer_token_if_needed(self, headers):
-        if not is_token_valid(self.client_config, self.http):
-            self.client_config['bearer_token'] = get_bearer_token(protocol=self.client_config["protocol"],
-                                                                  ip=self.client_config["ip"],
-                                                                  port=self.client_config["port"],
-                                                                  refresh_token=self.client_config["refresh_token"])
-            headers = IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
-        return headers
-
-    def call_api(self, method, url, headers=None, data=None):
-        # headers = self.regenerate_bearer_token_if_needed(headers)
-        if method.upper() == "GET":
-            self.logger.info(f"Calling {url}")
-            response = self.http.get(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
-                                     verify=False, data=data)
-            if response.status_code == 406:
-                headers = self.regenerate_bearer_token_if_needed(headers)
-                return self.http.get(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
-                                     verify=False, data=data)
-            else:
-                return response
-        elif method.upper() == "POST":
-            self.logger.info(f"Calling {url}")
-            response = self.http.post(url, headers=headers, json=data,
-                                      timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
-                headers = self.regenerate_bearer_token_if_needed(headers)
-                return self.http.post(url, headers=headers, json=data,
-                                      timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            else:
-                return response
-        elif method.upper() == "PUT":
-            self.logger.info(f"Calling {url}")
-            response = self.http.put(url, headers=headers, json=data,
-                                     timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
-                headers = self.regenerate_bearer_token_if_needed(headers)
-                return self.http.put(url, headers=headers, json=data,
-                                     timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
+            src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
+            src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
+            filter_condition = IWUtils.ejson_serialize({"name": data['name']})
+            source_detail_url = get_source_details_url(
+                src_client_obj.client_config) + f"?filter={{filter_condition}}".format(
+                filter_condition=filter_condition)
+            response = requests.get(source_detail_url,
+                                    headers={'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
+                                             'Content-Type': 'application/json'}, verify=False)
+            if response.status_code == "406":
+                headers = src_client_obj.regenerate_bearer_token_if_needed(
+                    {'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
+                     'Content-Type': 'application/json'})
+                response = requests.get(source_detail_url, headers=headers, verify=False)
+            response = IWUtils.ejson_deserialize(response.content)
+            if not response.get('result', None):
+                src_client_obj.logger.error("Failed to make an api call to get source details")
+                print("Failed to make an api call to get source details")
+                src_client_obj.logger.info(response)
+                print(response)
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   source_id=None,response=response)
             else:
-                return response
-        elif method.upper() == "PATCH":
-            self.logger.info(f"Calling {url}")
-            response = self.http.patch(url, headers=headers, json=data,
-                                       timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
-            if response.status_code == 406:
-                headers = self.regenerate_bearer_token_if_needed(headers)
-                return self.http.put(url, headers=headers, json=data,
-                                     timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC, verify=False)
+                src_client_obj.logger.info(
+                    f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
+                print(f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=response['result'][0]['id'],response=response)
+
+    def configure_csv_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
+                             secret_type="",config_ini_path=None,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        data = self.configuration_obj["configuration"]["source_configs"]["connection"]
+        src_name = str(self.configuration_obj["configuration"]["source_configs"]["name"])
+        storage_type = data["storage"]["storage_type"]
+        cloud_type = data["storage"].get("cloud_type", None)
+        if storage_type == "cloud" and cloud_type == "s3":
+            access_id = data["storage"].get("access_id", "")
+            secret_key = data["storage"].get("secret_key", "")
+            if "source_secrets" in mappings:
+                access_id = mappings.get("source_secrets").get("access_id", access_id)
+                secret_key = mappings.get("source_secrets").get("secret_key", secret_key)
+            source_configure_payload = {
+                "source_base_path_relative": data.get("source_base_path_relative",""),
+                "source_base_path": data.get("source_base_path",""),
+                "storage": {
+                    "storage_type": data["storage"]["storage_type"],
+                    "cloud_type": data["storage"]["cloud_type"],
+                    "access_id": access_id,
+                    "secret_key": secret_key,
+                    "account_type": data["storage"]["account_type"],
+                    "access_type": data["storage"]["access_type"]
+                }
+            }
+        elif storage_type == "cloud" and cloud_type == "wasb":
+            source_configure_payload = {}
+            pass
+        elif storage_type == "cloud" and "project_id" in data["storage"]:
+            project_id = data["storage"]["project_id"]
+            server_path = data["storage"]["server_path"]
+            if "gcp_details" in mappings:
+                project_id = mappings["gcp_details"].get("project_id", project_id)
+                server_path = mappings["gcp_details"].get("service_json_path", server_path)
+            if "gcp_project_id_mappings" in mappings:
+                project_id = mappings["gcp_project_id_mappings"].get(data["storage"]["project_id"], project_id)
+            if "service_json_mappings" in mappings:
+                server_path = mappings["service_json_mappings"].get(data["storage"]["server_path"].split("/")[-1],
+                                                                    server_path)
+
+            source_configure_payload = {
+                "source_base_path_relative": data.get("source_base_path_relative",""),
+                "source_base_path": data.get("source_base_path",""),
+                "storage": {
+                    "cloud_type": "gs",
+                    "storage_type": data["storage"]["storage_type"],
+                    "project_id": project_id,
+                    "access_type": data["storage"]["access_type"],
+                    "server_path": server_path,
+                    "upload_option": data["storage"]["upload_option"],
+                    "file_details": []
+                }
+            }
+        elif storage_type == "remote":
+            # SFTP Source
+            data = self.configuration_obj["configuration"]["source_configs"]["connection"]
+            source_configure_payload = data
+            source_configure_payload["source_base_path"]=""
+            if data.get("storage", {}).get("password", {}).get("password_type","") == "secret_store":
+                # for SFTP password auth
+                secret_name = data["storage"]["password"]["secret_name"]
+                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+                if secret_name:
+                    data["storage"]["password"]["secret_id"] = secret_id
+                    data["storage"]["password"].pop('secret_name', None)
+            elif data.get("storage", {}).get("access_key_name", {}).get("password_type","") == "secret_store":
+                # for adls gen2 storage account access key auth
+                secret_name = data["storage"]["access_key_name"]["secret_name"]
+                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+                if secret_name:
+                    data["storage"]["access_key_name"]["secret_id"] = secret_id
+                    data["storage"]["access_key_name"].pop('secret_name', None)
+            elif data.get("storage", {}).get("service_credential", {}).get("password_type","") == "secret_store":
+                # for adls gen2 service credential auth
+                secret_name = data["storage"]["service_credential"]["secret_name"]
+                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+                if secret_name:
+                    data["storage"]["service_credential"]["secret_id"] = secret_id
+                    data["storage"]["service_credential"].pop('secret_name', None)
+            elif data.get("storage", {}).get("account_key", {}).get("password_type","") == "secret_store":
+                #for blob storage account key auth
+                secret_name = data["storage"]["account_key"]["secret_name"]
+                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+                if secret_name:
+                    data["storage"]["account_key"]["secret_id"] = secret_id
+                    data["storage"]["account_key"].pop('secret_name', None)
             else:
-                return response
-        elif method.upper() == "DELETE":
-            self.logger.info(f"Calling {url}")
-            response = self.http.delete(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
-                                        verify=False)
-            if response.status_code == 406:
-                headers = self.regenerate_bearer_token_if_needed(headers)
-                return self.http.delete(url, headers=headers, timeout=local_configurations.REQUEST_TIMEOUT_IN_SEC,
-                                        verify=False)
-            else:
-                return response
-
-    def get_mappings_from_config_file(self, ini_config_file_path):
-        config = ConfigParser()
-        config.optionxform = str
-        config.read(ini_config_file_path)
-        if "environment" in config:
-            default_environment_id = config.get("environment", "environment_id")
-            default_storage_id = config.get("environment", "storage_id")
-            default_interactive_id = config.get("environment", "interactive_id")
-            self.client_config["default_environment_id"] = default_environment_id
-            self.client_config["default_storage_id"] = default_storage_id
-            self.client_config["default_compute_id"] = default_interactive_id
-        if "environment_mappings" in config:
-            environment_mappings = dict(config.items("environment_mappings"))
-            self.mappings["environment_mappings"] = environment_mappings
-        if "storage_mappings" in config:
-            storage_mappings = dict(config.items("storage_mappings"))
-            self.mappings["storage_mappings"] = storage_mappings
-        if "compute_mappings" in config:
-            compute_mappings = dict(config.items("compute_mappings"))
-            self.mappings["compute_mappings"] = compute_mappings
-        if "gcp_details" in config:
-            gcp_details = dict(config.items("gcp_details"))
-            self.mappings["gcp_details"] = gcp_details
-        if "gcp_project_id_mappings" in config:
-            gcp_project_id_mappings = dict(config.items("gcp_project_id_mappings"))
-            self.mappings["gcp_project_id_mappings"] = gcp_project_id_mappings
-        if "service_json_mappings" in config:
-            service_json_mappings = dict(config.items("service_json_mappings"))
-            self.mappings["service_json_mappings"] = service_json_mappings
-        if "table_group_compute_mappings" in config:
-            table_group_compute_mappings = dict(config.items("table_group_compute_mappings"))
-            self.mappings["table_group_compute_mappings"] = table_group_compute_mappings
-        if "kms" in config:
-            kms = dict(config.items("kms"))
-            self.mappings["kms"] = kms
-        for section in config.sections():
-            self.mappings[section] = dict(config.items(section))
+                pass
+        else:
+            source_configure_payload = {}
 
-    def _topological_sort_grouping(self, g):
-        # copy the graph
-        _g = g.copy()
-        res = []
-        # while _g is not empty
-        while _g:
-            zero_indegree = [v for v, d in _g.in_degree() if d == 0]
-            res.append(zero_indegree)
-            _g.remove_nodes_from(zero_indegree)
-        return res
+        response = src_client_obj.configure_source_connection(source_id, connection_object=source_configure_payload)
+        return response
 
-    def get_all_secrets(self, secret_type, ini_config_file_path=None, keys=None):
-        # Read all secrets from file and load inmemory
-        # Encrypt using infoworks encoding
-        if secret_type == "gcp_kms" and ini_config_file_path is not None:
-            config = ConfigParser()
-            config.optionxform = str
-            config.read(ini_config_file_path)
-            # Cloud KMS CryptoKey Encrypter
-            service_json_path = config.get("gcp_kms", "service_json_path")
-            # Reading Config Parameters
-            projectId = config.get("gcp_kms", "projectId")
-            locationId = config.get("gcp_kms", "locationId")
-            keyRingId = config.get("gcp_kms", "keyRingId")
-            keyId = config.get("gcp_kms", "keyId")
-            bucketName = config.get("gcp_kms", "bucketName")
-            blobName = config.get("gcp_kms", "encrypted_key_filename")
-            # Reading Encrypted Password File from Cloud Storage
-            storageClient = storage.Client.from_service_account_json(service_json_path)
-            bucket = storageClient.get_bucket(bucketName)
-            blobFile = bucket.get_blob(blobName)
-            cipherText = blobFile.download_as_string()
-            kmsClient = kms.KeyManagementServiceClient.from_service_account_json(service_json_path)
-            keyName = kmsClient.crypto_key_path(projectId, locationId, keyRingId, keyId)
-            # Decrypt Password
-            try:
-                decryptPassword = kmsClient.decrypt(request={'name': keyName, 'ciphertext': cipherText})
-                plainText = str(decryptPassword.plaintext, 'utf-8')
-                plainTextStr = plainText.strip()
-                passwordsDictPlain = json.loads(plainTextStr)
-                passwordsDictEncrypted = {}
-                for key in passwordsDictPlain:
-                    passwordsDictEncrypted[key] = aes_encrypt(passwordsDictPlain[key])
-                self.secrets_config = passwordsDictEncrypted
-            except Exception as e:
-                print(str(e))
-                return ""
-        elif secret_type == "aws_kms" and ini_config_file_path is not None:
-            config = ConfigParser()
-            config.optionxform = str
-            config.read(ini_config_file_path)
-            # Read the encrypted file into memory
-            encrypted_filename = config.get("aws_kms", "encrypted_filename")
-            available_keys = dict(config.items("aws_kms")).keys()
-            if "access_id" in available_keys and "secret_key" in available_keys:
-                ACCESS_KEY = config.get("aws_kms", "access_id")
-                SECRET_KEY = config.get("aws_kms", "secret_key")
-            else:
-                ACCESS_KEY, SECRET_KEY = None, None
-            # Read
-            NUM_BYTES_FOR_LEN = 4
-            try:
-                with open(encrypted_filename, 'rb') as file:
-                    file_contents = file.read()
-            except IOError as e:
-                self.logger.error(str(e))
-                return False
-            data_key_encrypted_len = int.from_bytes(file_contents[:NUM_BYTES_FOR_LEN],
-                                                    byteorder='big') + NUM_BYTES_FOR_LEN
-            data_key_encrypted = file_contents[NUM_BYTES_FOR_LEN:data_key_encrypted_len]
-            # Decrypt the data key before using it
-            if ACCESS_KEY is not None and SECRET_KEY is not None:
-                kms_client = boto3.client('kms', aws_access_key_id=ACCESS_KEY, aws_secret_access_key=SECRET_KEY)
+    def import_source_configuration(self, src_client_obj, source_id,
+                                    mappings, export_configuration_file=None, export_config_lookup=True,
+                                    read_passwords_from_secrets=False,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        src_name = self.configuration_obj["configuration"]["source_configs"]["name"]
+        table_group_compute_mappings = mappings.get("table_group_compute_mappings", {})
+        source_import_payload = {"configuration": self.configuration_obj["configuration"]}
+        modified_table_configs = self.configuration_obj["configuration"]["table_configs"]
+        index = 0
+        for table_config in self.configuration_obj["configuration"]["table_configs"]:
+            modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+            if not table_config["configuration"].get("meta_crawl_performed", False):
+                modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
             else:
-                kms_client = boto3.client('kms')
-            try:
-                response = kms_client.decrypt(CiphertextBlob=data_key_encrypted)
-                data_key_plaintext = base64.b64encode((response['Plaintext']))
-            except Exception as e:
-                self.logger.error(str(e))
-                return False
-
-            if data_key_plaintext is None:
-                return False
-            # Decrypt the rest of the file
-            f = Fernet(data_key_plaintext)
-            file_contents_decrypted = f.decrypt(file_contents[data_key_encrypted_len:])
-            passwordsDictPlain = json.loads(file_contents_decrypted)
-            passwordsDictEncrypted = {}
-            for key in passwordsDictPlain:
-                passwordsDictEncrypted[key] = aes_encrypt(passwordsDictPlain[key])
-            self.secrets_config = passwordsDictEncrypted
-            return True
-        elif secret_type == "aws_secrets":
-            ACCESS_KEY, SECRET_KEY = None, None
-            region = 'us-west-2'
-            if ini_config_file_path is not None:
-                config = ConfigParser()
-                config.optionxform = str
-                config.read(ini_config_file_path)
-                available_keys = dict(config.items("aws_secrets")).keys()
-                if "access_id" in available_keys and "secret_key" in available_keys:
-                    ACCESS_KEY = config.get("aws_secrets", "access_id")
-                    SECRET_KEY = config.get("aws_secrets", "secret_key")
-                else:
-                    ACCESS_KEY, SECRET_KEY = None, None
-                if "region" in available_keys:
-                    region = config.get("aws_secrets", "region")
-            if keys:
-                output_values = []
-                for key in keys.split(","):
-                    secrets_client = boto3.client("secretsmanager", region_name=region)
-                    kwargs = {'SecretId': key}
+                if not table_config["configuration"]["meta_crawl_performed"]:
+                    modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
+                index = index + 1
+        source_import_payload["configuration"]["table_configs"] = modified_table_configs
+        iw_mappings = source_import_payload["configuration"]["iw_mappings"]
+        for item in iw_mappings:
+            if item.get("entity_type", "") == "environment_compute_template":
+                item["recommendation"]["compute_name"] = table_group_compute_mappings.get(
+                    item["recommendation"]["compute_name"], item["recommendation"]["compute_name"])
+        source_import_payload["configuration"]["iw_mappings"] = iw_mappings
+        if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
+            for table in source_import_payload.get("configuration")["table_configs"]:
+                # Check if there are any export configurations and passwords to replace
+                if table.get("configuration", {}).get("export_configuration", None) is not None:
+                    export_configs = table.get("configuration", {}).get("export_configuration")
+                    target_type = export_configs.get("target_type", "").upper()
+                    table_name = table["configuration"]["name"].upper()
+                    override_keys = []
                     try:
-                        value = secrets_client.get_secret_value(**kwargs)["SecretString"]
-                        self.secrets_config[key] = value
-                        output_values.append(value)
+                        if export_configuration_file is not None:
+                            with open(export_configuration_file) as file:
+                                information = yaml.load(file, Loader=yaml.FullLoader)
+                            if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
+                                info_key = src_name + "_" + table_name
+                                override_keys = information["src_export_details"].get(src_name + "_" + table_name,
+                                                                                      {}).keys()
+                            else:
+                                info_key = src_name
+                                override_keys = information["src_export_details"].get(src_name, {}).keys()
+                            for key in override_keys:
+                                table["configuration"]["export_configuration"]["connection"][key] = \
+                                    information["src_export_details"][info_key][key]
                     except Exception as e:
-                        self.logger.error(str(e))
-                return output_values
-            else:
-                # Get all the secrets
-                if ACCESS_KEY is not None and SECRET_KEY is not None:
-                    secrets_client = boto3.client("secretsmanager", aws_access_key_id=ACCESS_KEY,
-                                                  aws_secret_access_key=SECRET_KEY, region=region)
-                else:
-                    secrets_client = boto3.client("secretsmanager",region=region)
-                temp = secrets_client.list_secrets()["SecretList"]
-                all_secrets = [i["Name"] for i in temp]
-                for key in all_secrets:
-                    kwargs = {'SecretId': key}
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration file {export_configuration_file} due to {str(e)}")
+
                     try:
-                        value = secrets_client.get_secret_value(**kwargs)["SecretString"]
-                        self.secrets_config[key] = value
+                        if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
+                            # Read the password from KMS
+                            encrypted_key_name1 = f"export-configuration-{src_name}-{table['configuration']['name']}"
+                            encrypted_key_name2 = f"export-configuration-{src_name}"
+                            passwd = self.secrets.get(encrypted_key_name1, "")
+                            if passwd == "":
+                                passwd = self.secrets.get(encrypted_key_name2, "")
+                            table["configuration"]["export_configuration"]["connection"]["password"] = passwd
+                        elif target_type.upper() == "BIGQUERY":
+                            if "server_path" not in override_keys:
+                                server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
+                                if "gcp_details" in mappings:
+                                    server_path = mappings["gcp_details"].get("service_json_path")
+                                if "service_json_mappings" in mappings:
+                                    server_path = mappings["service_json_mappings"].get(
+                                        server_path.split("/")[-1],
+                                        server_path)
+                                table["configuration"]["export_configuration"]["connection"][
+                                    "server_path"] = server_path if server_path != "" else table["configuration"][
+                                    "export_configuration"].get("connection", {}).get(
+                                    "server_path", "")
+                            table["configuration"]["export_configuration"]["connection"][
+                                "upload_option"] = "serverLocation"
                     except Exception as e:
-                        self.logger.error(str(e))
-        elif secret_type == "azure_keyvault" and ini_config_file_path is not None:
-            from azure.keyvault.secrets import SecretClient
-            from azure.identity import ClientSecretCredential
-            config = ConfigParser()
-            config.optionxform = str
-            config.read(ini_config_file_path)
-            # Read the encrypted file into memory
-            available_keys = dict(config.items("azure_keyvault")).keys()
-            if all(x in ['keyVaultName', 'tenant_id', 'client_id', 'client_secret'] for x in available_keys):
-                keyVaultName = config.get("azure_keyvault", "keyVaultName")
-                KVUri = f"https://{keyVaultName}.vault.azure.net"
-                tenant_id = config.get("azure_keyvault", "tenant_id")
-                client_id = config.get("azure_keyvault", "client_id")
-                client_secret = config.get("azure_keyvault", "client_secret")
-                credential = ClientSecretCredential(tenant_id, client_id, client_secret)
-                client = SecretClient(vault_url=KVUri, credential=credential)
-                output_values=[]
-                if keys:
-                    for key in keys.split(","):
-                        retrieved_secret = client.get_secret(key)
-                        self.secrets_config[key] = aes_encrypt(retrieved_secret.value)
-                        output_values.append(aes_encrypt(retrieved_secret.value))
-                else:
-                    secret_properties = client.list_properties_of_secrets()
-                    all_secrets = [i.name for i in secret_properties]
-                    for key in all_secrets:
-                        retrieved_secret = client.get_secret(key)
-                        self.secrets_config[key] = aes_encrypt(retrieved_secret.value)
-                        output_values.append(retrieved_secret.value)
-                return output_values
-
-        self.secrets_config["custom_secrets_read"] = True
+                        src_client_obj.logger.error(
+                            f"Failed to lookup the export configuration password from secrets due to {str(e)}")
+        response = src_client_obj.configure_tables_and_tablegroups(source_id,
+                                                                   configuration_obj=source_import_payload.get(
+                                                                       "configuration"))
+        return response
+        # if response["result"]["status"].upper() != "SUCCESS":
+        #     src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
+        #                                 .format(source_id, self.source_config_path))
+        #     src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
+        #                                 .format(self.source_config_path))
+        #     return "FAILED"
+        # else:
+        #     src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
+        #     return "SUCCESS"
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/cicd_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_source_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import traceback
 
 from infoworks.sdk.base_client import BaseClient
 from infoworks.sdk.cicd.download_configurations.utils import Utils
 
 
 class DownloadSource(BaseClient):
     def __init__(self):
@@ -31,8 +32,9 @@
                                                                      config_file_dump_path)
                 if filename is not None:
                     f.write(filename)
                     f.write("\n")
             except Exception as e:
                 self.logger.error(f"Unable to export configurations for source {source_id} due to {str(e)}")
                 print(f"Unable to export configurations for source {source_id} due to {str(e)}")
+                print(traceback.format_exc())
         f.close()
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/download_configurations/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 import copy
 import os
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import get_parent_entity_url, list_domains_url, configure_pipeline_url, \
     configure_workflow_url, \
     configure_source_url, get_environment_details, get_environment_storage_details, get_environment_compute_details, \
     get_environment_interactive_compute_details, get_source_configurations_url, get_pipeline_url, \
-    get_data_connection, source_info, list_users_url
+    get_data_connection, source_info, list_users_url, list_secrets_url, get_pipeline_group_base_url,list_pipelines_url
 from infoworks.sdk.cicd.cicd_response import CICDResponse
 import json
 
 
 class Utils:
     def __init__(self, serviceaccountemail):
         self.serviceaccountemail = serviceaccountemail
 
+    def get_secret_name_from_id(self,cicd_client,secret_id):
+        secret_name = None
+        get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"_id":"'+secret_id+'"}'
+        response = cicd_client.call_api("GET", get_secret_details_url,
+                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
+        parsed_response = IWUtils.ejson_deserialize(response.content)
+        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+            result = parsed_response.get("result", [])
+
+            if len(result) > 0:
+                secret_name = result[0]["name"]
+                cicd_client.logger.info("Found secret name {} ".format(secret_name))
+                return secret_name
+            else:
+                cicd_client.logger.info("Secret Name is {} ".format(None))
+                return None
+
     def get_domain_id(self, cicd_client, json_obj):
         parent_entity_url = get_parent_entity_url(cicd_client.client_config)
         response = cicd_client.call_api("GET", parent_entity_url,
                                         IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']),
                                         data=json_obj)
         parsed_response = IWUtils.ejson_deserialize(response.content)
         if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
@@ -133,14 +150,16 @@
         environment_id, environment_compute_template_id, environment_storage_id = None, None, None
         if entity_type == "pipeline":
             url_to_config = configure_pipeline_url(cicd_client.client_config, domain_id, entity_id)
         elif entity_type == "workflow":
             url_to_config = configure_workflow_url(cicd_client.client_config, domain_id, entity_id)
         elif entity_type == "source":
             url_to_config = configure_source_url(cicd_client.client_config, entity_id)
+        elif entity_type == "pipeline_group":
+            url_to_config = get_pipeline_group_base_url(cicd_client.client_config, domain_id) + f"{entity_id}"
         else:
             return None
         cicd_client.logger.info(
             "URL to get configurations of entity {} of type {} is {}".format(entity_id, entity_type, url_to_config))
         response = cicd_client.call_api("GET", url_to_config, IWUtils.get_default_header_for_v3(
             cicd_client.client_config[
                 'bearer_token']))
@@ -150,15 +169,14 @@
             status = "SUCCESS"
         else:
             status = "FAILED"
         response_to_return["get_configuration_entity_response"] = CICDResponse.parse_result(status=status,
                                                                                             entity_id=entity_id,
                                                                                             response=parsed_response)
         configuration_obj = parsed_response.get('result', {})
-        # print(configuration_obj)
         if len(configuration_obj) > 0:
             if entity_type == "source":
                 get_src_details_url = source_info(cicd_client.client_config, entity_id)
                 response = cicd_client.call_api("GET", get_src_details_url,
                                                 IWUtils.get_default_header_for_v3(
                                                     cicd_client.client_config['bearer_token']))
                 parsed_response = IWUtils.ejson_deserialize(response.content)
@@ -172,15 +190,51 @@
                                                                                               response=parsed_response)
                 if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
                     result = parsed_response.get("result", [])
                     if len(result) > 0:
                         data_lake_path = result["data_lake_path"]
                         configuration_obj["configuration"]["source_configs"]["data_lake_path"] = data_lake_path
                         configuration_obj["filter_tables_properties"] = result.get("filter_tables_properties", {})
-
+                        source_connection_objects = configuration_obj["configuration"]["source_configs"]["connection"]
+                        if source_connection_objects.get("storage",None) is not None:
+                            # for File based sources
+                            if source_connection_objects.get("storage",{}).get("password",{}).get("password_type","")=="secret_store":
+                                # for SFTP password auth
+                                secret_id = source_connection_objects["storage"]["password"]["secret_id"]
+                                secret_name = self.get_secret_name_from_id(cicd_client,secret_id)
+                                if secret_name:
+                                    source_connection_objects["storage"]["password"]["secret_name"] = secret_name
+                            elif source_connection_objects.get("storage",{}).get("access_key_name",{}).get("password_type","")=="secret_store":
+                                # for adls gen2 storage account access key auth
+                                secret_id = source_connection_objects["storage"]["access_key_name"]["secret_id"]
+                                secret_name = self.get_secret_name_from_id(cicd_client,secret_id)
+                                if secret_name:
+                                    source_connection_objects["storage"]["access_key_name"]["secret_name"] = secret_name
+                            elif source_connection_objects.get("storage",{}).get("service_credential",{}).get("password_type","")=="secret_store":
+                                # for adls gen2 service credential auth
+                                secret_id = source_connection_objects["storage"]["service_credential"]["secret_id"]
+                                secret_name = self.get_secret_name_from_id(cicd_client,secret_id)
+                                if secret_name:
+                                    source_connection_objects["storage"]["service_credential"]["secret_name"] = secret_name
+                            elif source_connection_objects.get("storage",{}).get("account_key",{}).get("password_type","")=="secret_store":
+                                # for blob storage account key auth
+                                secret_id = source_connection_objects["storage"]["account_key"]["secret_id"]
+                                secret_name = self.get_secret_name_from_id(cicd_client,secret_id)
+                                if secret_name:
+                                    source_connection_objects["storage"]["account_key"]["secret_name"] = secret_name
+                            else:
+                                pass
+                        else:
+                            #for RDBMS sources
+                            if source_connection_objects.get("password",{}).get("password_type","")=="secret_store":
+                                # for SFTP password auth
+                                secret_id = source_connection_objects["password"]["secret_id"]["$oid"]
+                                secret_name = self.get_secret_name_from_id(cicd_client,secret_id)
+                                if secret_name:
+                                    source_connection_objects["password"]["secret_name"] = secret_name
                 # Check if any table has export configurations. Works for postgres/snowflake/synapse
                 # Did not test for cosmos,delimited
                 for table_config in configuration_obj["configuration"]["table_configs"]:
                     if len(table_config["configuration"].get("export_configuration", [])) > 0:
                         if table_config["configuration"]["export_configuration"].get("target_type", "") in ["SNOWFLAKE",
                                                                                                             "POSTGRES",
                                                                                                             "AZURE_SQL_DW"]:
@@ -210,14 +264,15 @@
                 else:
                     status = "FAILED"
                     print("Get Source Configurations failed " + json.dumps(response))
                 response_to_return["get_source_configurations_response"] = CICDResponse.parse_result(status=status,
                                                                                                      entity_id=entity_id,
                                                                                                      response=parsed_response)
             else:
+                entity_name=configuration_obj["configuration"]["entity"]["entity_name"] if entity_type!="pipeline_group" else configuration_obj["name"]
                 if entity_type == "pipeline":
                     environment_id, environment_compute_template_id, environment_storage_id = self.get_env_details(
                         cicd_client, entity_id,
                         entity_type,
                         domain_id)
                     if any([environment_id, environment_compute_template_id, environment_storage_id]):
                         status = "SUCCESS"
@@ -257,14 +312,26 @@
                                 if len(result) > 0:
                                     result["properties"] = self.get_dataconnection_properties(result["sub_type"],
                                                                                               result["properties"])
                                 for key in ['name', 'type', 'sub_type', 'properties']:
                                     dataconnection_obj[key] = result[key]
                                 configuration_obj["dataconnection_configurations"].append(
                                     copy.deepcopy(dataconnection_obj))
+                elif entity_type == "pipeline_group":
+                    list_pipelines_under_domain_url = list_pipelines_url(cicd_client.client_config,domain_id=domain_id)
+                    pipeline_name_lookup={}
+                    pipelines_under_domain_response = cicd_client.call_api("GET", list_pipelines_under_domain_url, IWUtils.get_default_header_for_v3(
+            cicd_client.client_config[
+                'bearer_token']))
+                    pipelines_under_domain_parsed_response = IWUtils.ejson_deserialize(pipelines_under_domain_response.content)
+                    for pipeline in pipelines_under_domain_parsed_response["result"]:
+                        pipeline_name_lookup[pipeline["id"]]=pipeline["name"]
+                    for index,pipeline in enumerate(configuration_obj["pipelines"]):
+                        pipeline["name"]=pipeline_name_lookup.get(pipeline["pipeline_id"],None)
+                    environment_id = configuration_obj["environment_id"]
                 domains_url_base = list_domains_url(cicd_client.client_config)
                 filter_condition = IWUtils.ejson_serialize({"_id": domain_id})
                 domains_url = domains_url_base + f"?filter={{filter_condition}}".format(
                     filter_condition=filter_condition)
                 response = cicd_client.call_api("GET", domains_url,
                                                 IWUtils.get_default_header_for_v3(
                                                     cicd_client.client_config['bearer_token']))
@@ -281,18 +348,18 @@
                 if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
                     result = parsed_response.get("result", [])
                     existing_domain_name = result[0]["name"]
                     if entity_type == "workflow":
                         environment_ids = result[0]["environment_ids"]
                 if existing_domain_name:
                     filename = existing_domain_name + "#{}_".format(entity_type) + \
-                               configuration_obj["configuration"]["entity"][
-                                   "entity_name"] + ".json"
+                               entity_name + ".json"
                     target_file_path = os.path.join(target_file_path, entity_type, filename)
 
+
             if entity_type == "workflow":
                 storage_name, compute_name = None, None
                 environment_names = []
                 if len(environment_ids) > 0:
                     for environment_id in environment_ids:
                         env_name, storage_name, compute_name = self.get_env_entities_names(cicd_client, environment_id,
                                                                                            None, None)
@@ -309,28 +376,29 @@
                     environment_compute_template_id,
                     environment_storage_id)
 
                 configuration_obj["environment_configurations"] = {"environment_name": env_name,
                                                                    "environment_compute_template_name": compute_name,
                                                                    "environment_storage_name": storage_name}
 
-            filter_condition = IWUtils.ejson_serialize(
-                {"$or": [{"_id": configuration_obj["configuration"]["export"]["exported_by"]},
-                         {"profile.name": configuration_obj["configuration"]["export"]["exported_by"]}]})
-            url_to_list_users_base = list_users_url(cicd_client.client_config)
-            url_to_list_users = url_to_list_users_base + f"?filter={{filter_condition}}".format(
-                filter_condition=filter_condition)
-            response = cicd_client.call_api("GET", url_to_list_users,
-                                            IWUtils.get_default_header_for_v3(
-                                                cicd_client.client_config['bearer_token']))
-            parsed_response = IWUtils.ejson_deserialize(response.content)
-            configuration_obj["user_email"] = self.serviceaccountemail
-            if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
-                result = parsed_response.get("result", [])
-                configuration_obj["user_email"] = result[0]["profile"].get("email", "admin@infoworks.io")
+            if entity_type!="pipeline_group":
+                filter_condition = IWUtils.ejson_serialize(
+                    {"$or": [{"_id": configuration_obj["configuration"]["export"]["exported_by"]},
+                             {"profile.name": configuration_obj["configuration"]["export"]["exported_by"]}]})
+                url_to_list_users_base = list_users_url(cicd_client.client_config)
+                url_to_list_users = url_to_list_users_base + f"?filter={{filter_condition}}".format(
+                    filter_condition=filter_condition)
+                response = cicd_client.call_api("GET", url_to_list_users,
+                                                IWUtils.get_default_header_for_v3(
+                                                    cicd_client.client_config['bearer_token']))
+                parsed_response = IWUtils.ejson_deserialize(response.content)
+                configuration_obj["user_email"] = self.serviceaccountemail
+                if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+                    result = parsed_response.get("result", [])
+                    configuration_obj["user_email"] = result[0]["profile"].get("email", "admin@infoworks.io")
             try:
                 if filename is not None and target_file_path is not None:
                     cicd_client.logger.info("{} {}".format(filename, target_file_path))
                     print(f"Exporting configurations file to {target_file_path}")
                     with open(target_file_path, 'w') as file_ptr:
                         contents_to_write = IWUtils.ejson_serialize(configuration_obj)
                         if replace_words != "":
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/cdata_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,29 +72,14 @@
         if override_config_file is not None:
             with open(override_config_file) as file:
                 information = yaml.load(file, Loader=yaml.FullLoader)
             if information["source_details"].get(src_name, None) is not None:
                 override_keys = information["source_details"].get(src_name).keys()
                 for key in override_keys:
                     connection_object[key] = information["source_details"][src_name][key]
-        if read_passwords_from_secrets and self.secrets["custom_secrets_read"] is True:
-            encrypted_key_name = f"{env_tag}-" + src_name
-            decrypt_value = self.secrets.get(encrypted_key_name, "")
-            if IWUtils.is_json(decrypt_value):
-                decrypt_value_dict = json.loads(decrypt_value)
-                for key in decrypt_value_dict.keys():
-                    connection_object[key] = decrypt_value_dict[key]
-        elif read_passwords_from_secrets and self.secrets["custom_secrets_read"] is False:
-            encrypted_key_name = f"{env_tag}-" + src_name
-            decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name)
-            if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                decrypt_value_dict = json.loads(decrypt_value[0])
-                for key in decrypt_value_dict.keys():
-                    connection_object[key] = decrypt_value_dict[key]
-
         response = src_client_obj.configure_source_connection(source_id, connection_object=connection_object)
         if response["result"]["status"].upper() != "SUCCESS":
             src_client_obj.logger.info(f"Failed to configure the source {source_id} connection")
             src_client_obj.logger.info(response["result"])
             return "FAILED"
         else:
             src_client_obj.logger.info(response["result"])
@@ -176,36 +161,16 @@
                                                                                   {}).keys()
                         else:
                             info_key = src_name
                             override_keys = information["src_export_details"].get(src_name, {}).keys()
                         for key in override_keys:
                             table["configuration"]["export_configuration"]["connection"][key] = \
                                 information["src_export_details"][info_key][key]
-                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
-                        if self.secrets["custom_secrets_read"] is True:
-                            encrypted_key_name1 = f"{env_tag}-export-configuration-{src_name}-{table['configuration']['name']}"
-                            encrypted_key_name2 = f"{env_tag}-export-configuration-{src_name}"
-                            decrypt_value = self.secrets.get(encrypted_key_name1, "")
-                            if decrypt_value == "" or decrypt_value is None:
-                                decrypt_value = self.secrets.get(encrypted_key_name2, "")
-                            decrypt_value_dict = json.loads(decrypt_value)
-                            for key in decrypt_value_dict.keys():
-                                table["configuration"]["export_configuration"]["connection"][key] = \
-                                    decrypt_value_dict[key]
-                        else:
-                            encrypted_key_name1 = f"{env_tag}-export-configuration-{src_name}-{table['configuration']['name']}"
-                            encrypted_key_name2 = f"{env_tag}-export-configuration-{src_name}"
-                            decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name1)
-                            if len(decrypt_value) == 0:
-                                decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name2)
-                            if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                                decrypt_value_dict = json.loads(decrypt_value[0])
-                                for key in decrypt_value_dict.keys():
-                                    table["configuration"]["export_configuration"]["connection"][key] = \
-                                            decrypt_value_dict[key]
+                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"]:
+                        pass
                     elif target_type.upper() == "BIGQUERY":
                         if "server_path" not in override_keys:
                             server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
                                 "server_path", "")
                             if "gcp_details" in mappings:
                                 server_path = mappings["gcp_details"].get("service_json_path")
                             if "service_json_mappings" in mappings:
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/csv_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,94 @@
+import copy
 import json
+
 import requests
 import yaml
-from infoworks.sdk.url_builder import get_source_details_url
+
+from infoworks.sdk.url_builder import get_source_details_url,list_secrets_url
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.local_configurations import Response
-from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
 import configparser
+from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+
+class RDBMSSource:
+    def __init__(self):
+        self.configuration_obj = None
+        self.source_config_path = None
+        self.environment_id = None
+        self.storage_id = None
+        self.secrets = None
 
-class CSVSource:
-    def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
+    def set_variables(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
         self.storage_id = storage_id
         self.environment_id = environment_id
         self.source_config_path = source_config_path
-        self.secrets = secrets
         with open(self.source_config_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
+        self.secrets = secrets
+
+    def get_secret_id_from_name(self,cicd_client,secret_name):
+        secret_id = None
+        get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"name":"'+secret_name+'"}'
+        response = cicd_client.call_api("GET", get_secret_details_url,
+                                        IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
+        parsed_response = IWUtils.ejson_deserialize(response.content)
+        if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
+            result = parsed_response.get("result", [])
+
+            if len(result) > 0:
+                secret_id = result[0]["id"]
+                cicd_client.logger.info("Found secret id {} ".format(secret_id))
+                return secret_id
+            else:
+                cicd_client.logger.info("Secret id is {} ".format(None))
+                return None
 
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
             if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
             final = d.setval(section.split("$"), dict(config.items(section)))
             print(f"section replacement:{d.getval(section.split('$'))}")
         self.configuration_obj = d.data
 
-    def create_csv_source(self, src_client_obj):
+    def create_rdbms_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
-        create_csv_source_payload = {
+        create_rdbms_source_payload = {
             "name": data["name"],
-            "type": data["type"],
+            "type": "rdbms",
             "sub_type": data["sub_type"],
             "data_lake_path": data["data_lake_path"],
             "data_lake_schema": data["data_lake_schema"] if "data_lake_schema" in data else "",
             "environment_id": self.environment_id,
             "storage_id": self.storage_id,
             "is_source_ingested": True
         }
         if data.get("target_database_name",""):
-            create_csv_source_payload["target_database_name"] = data.get("target_database_name","")
-        src_create_response = src_client_obj.create_source(source_config=create_csv_source_payload)
+            create_rdbms_source_payload["target_database_name"] = data.get("target_database_name","")
+        if data.get("staging_schema_name",""):
+            create_rdbms_source_payload["staging_schema_name"] = data.get("staging_schema_name", "")
+        src_create_response = src_client_obj.create_source(source_config=create_rdbms_source_payload)
         if src_create_response["result"]["status"].upper() == "SUCCESS":
-            source_id_created = src_create_response["result"]["source_id"]
-            print("Source created successfully")
             return src_create_response
         else:
             src_client_obj.logger.info('Cant create source {} '.format(data["name"]))
+            print('Cant create source {} '.format(data["name"]))
+            print(src_create_response)
             src_client_obj.logger.info(f"Getting the existing SourceId with name {data['name']} if exists")
+            print(f"Getting the existing SourceId with name {data['name']} if exists")
             filter_condition = IWUtils.ejson_serialize({"name": data['name']})
             source_detail_url = get_source_details_url(
                 src_client_obj.client_config) + f"?filter={{filter_condition}}".format(
                 filter_condition=filter_condition)
             response = requests.get(source_detail_url,
                                     headers={'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
                                              'Content-Type': 'application/json'}, verify=False)
@@ -66,187 +96,191 @@
                 headers = src_client_obj.regenerate_bearer_token_if_needed(
                     {'Authorization': 'Bearer ' + src_client_obj.client_config['bearer_token'],
                      'Content-Type': 'application/json'})
                 response = requests.get(source_detail_url, headers=headers, verify=False)
             response = IWUtils.ejson_deserialize(response.content)
             if not response.get('result', None):
                 src_client_obj.logger.error("Failed to make an api call to get source details")
-                print("Failed to make an api call to get source details")
                 src_client_obj.logger.info(response)
+                print("Failed to make an api call to get source details")
                 print(response)
-                return SourceResponse.parse_result(status=Response.Status.FAILED,
-                                                   source_id=None,response=response)
+                return SourceResponse.parse_result(status=Response.Status.FAILED, source_id=None,response=response)
             else:
                 src_client_obj.logger.info(
                     f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 print(f"Source Id with the same Source name {data['name']} : {response['result'][0]['id']}")
                 return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=response['result'][0]['id'],response=response)
 
-    def configure_csv_source(self, src_client_obj, source_id, mappings, read_passwords_from_secrets=False, env_tag="",
-                             secret_type="",config_ini_path=None):
-        data = self.configuration_obj["configuration"]["source_configs"]["connection"]
-        src_name = str(self.configuration_obj["configuration"]["source_configs"]["name"])
-        storage_type = data["storage"]["storage_type"]
-        cloud_type = data["storage"].get("cloud_type", None)
-        if storage_type == "cloud" and cloud_type == "s3":
-            access_id = data["storage"].get("access_id", "")
-            secret_key = data["storage"].get("secret_key", "")
-            if "source_secrets" in mappings:
-                access_id = mappings.get("source_secrets").get("access_id", access_id)
-                secret_key = mappings.get("source_secrets").get("secret_key", secret_key)
-            if read_passwords_from_secrets and self.secrets["custom_secrets_read"] is True:
-                encrypted_key_name = f"{env_tag}-" + src_name
-                decrypt_value = self.secrets.get(encrypted_key_name, "")
-                if IWUtils.is_json(decrypt_value):
-                    decrypt_value_dict = json.loads(decrypt_value)
-                    access_id = decrypt_value_dict["access_id"]
-                    secret_key = decrypt_value_dict["secret_key"]
-            elif read_passwords_from_secrets and self.secrets["custom_secrets_read"] is False:
-                encrypted_key_name = f"{env_tag}-" + src_name
-                decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name,ini_config_file_path=config_ini_path)
-                if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                    decrypt_value_dict = json.loads(decrypt_value[0])
-                    access_id = decrypt_value_dict["access_id"]
-                    secret_key = decrypt_value_dict["secret_key"]
-
-            source_configure_payload = {
-                "source_base_path_relative": data.get("source_base_path_relative",""),
-                "source_base_path": data.get("source_base_path",""),
-                "storage": {
-                    "storage_type": data["storage"]["storage_type"],
-                    "cloud_type": data["storage"]["cloud_type"],
-                    "access_id": access_id,
-                    "secret_key": secret_key,
-                    "account_type": data["storage"]["account_type"],
-                    "access_type": data["storage"]["access_type"]
-                }
-            }
-        elif storage_type == "cloud" and cloud_type == "wasb":
-            source_configure_payload = {}
-            pass
-        elif storage_type == "cloud" and "project_id" in data["storage"]:
-            project_id = data["storage"]["project_id"]
-            server_path = data["storage"]["server_path"]
-            if "gcp_details" in mappings:
-                project_id = mappings["gcp_details"].get("project_id", project_id)
-                server_path = mappings["gcp_details"].get("service_json_path", server_path)
-            if "gcp_project_id_mappings" in mappings:
-                project_id = mappings["gcp_project_id_mappings"].get(data["storage"]["project_id"], project_id)
-            if "service_json_mappings" in mappings:
-                server_path = mappings["service_json_mappings"].get(data["storage"]["server_path"].split("/")[-1],
-                                                                    server_path)
-
-            source_configure_payload = {
-                "source_base_path_relative": data.get("source_base_path_relative",""),
-                "source_base_path": data.get("source_base_path",""),
-                "storage": {
-                    "cloud_type": "gs",
-                    "storage_type": data["storage"]["storage_type"],
-                    "project_id": project_id,
-                    "access_type": data["storage"]["access_type"],
-                    "server_path": server_path,
-                    "upload_option": data["storage"]["upload_option"],
-                    "file_details": []
-                }
-            }
-        elif storage_type == "remote":
-            # SFTP Source
-            data = self.configuration_obj["configuration"]["source_configs"]["connection"]
-            source_configure_payload = data
-            source_configure_payload["source_base_path"]=""
+    def configure_rdbms_source_connection(self, src_client_obj, source_id, override_config_file=None,
+                                          read_passwords_from_secrets=False, env_tag="", secret_type="",config_ini_path=None,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        source_configs = self.configuration_obj["configuration"]["source_configs"]
+        src_name = str(source_configs["name"])
+        connection_object = source_configs["connection"]
+        if connection_object.get('connection_mode','')!='':
+            connection_object['connection_mode'] = connection_object['connection_mode'].lower()
+        else:
+            connection_object['connection_mode'] = 'jdbc'
+        if override_config_file is not None:
+            with open(override_config_file) as file:
+                information = yaml.load(file, Loader=yaml.FullLoader)
+            if information["source_details"].get(src_name, None) is not None:
+                override_keys = information["source_details"].get(src_name).keys()
+                for key in override_keys:
+                    connection_object[key] = information["source_details"][src_name][key]
+        if connection_object.get("password", {}).get("password_type","") == "secret_store":
+                # for RDBMS passwords in keyvault
+                secret_name = connection_object["password"]["secret_name"]
+                secret_id = self.get_secret_id_from_name(src_client_obj, secret_name)
+                if secret_name:
+                    connection_object["password"]["secret_id"] = secret_id
+                    connection_object["password"].pop('secret_name', None)
+        # if read_passwords_from_secrets and self.secrets["custom_secrets_read"] is True:
+        #     encrypted_key_name = f"{env_tag}-" + src_name
+        #     decrypt_value = self.secrets.get(encrypted_key_name, "")
+        #     if IWUtils.is_json(decrypt_value):
+        #         decrypt_value_dict = json.loads(decrypt_value)
+        #         for key in decrypt_value_dict.keys():
+        #             connection_object[key] = decrypt_value_dict[key]
+        # elif read_passwords_from_secrets and self.secrets["custom_secrets_read"] is False:
+        #     encrypted_key_name = f"{env_tag}-" + src_name
+        #     decrypt_value = src_client_obj.get_all_secrets(secret_type,keys=encrypted_key_name,ini_config_file_path=config_ini_path)
+        #     if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
+        #         decrypt_value_dict = json.loads(decrypt_value[0])
+        #         for key in decrypt_value_dict.keys():
+        #             connection_object[key] = decrypt_value_dict[key]
+        response = src_client_obj.configure_source_connection(source_id, connection_object=connection_object)
+        if response["result"]["status"].upper() != "SUCCESS":
+            src_client_obj.logger.info(f"Failed to configure the source {source_id} connection")
+            print(f"Failed to configure the source {source_id} connection")
+            src_client_obj.logger.info(response)
+            print(response)
+            return SourceResponse.parse_result(status=Response.Status.FAILED, source_id=source_id,response=response)
         else:
-            source_configure_payload = {}
+            src_client_obj.logger.info(response)
+            print(response)
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,response=response)
+
+    def test_source_connection(self, src_client_obj, source_id,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        response = src_client_obj.source_test_connection_job_poll(source_id, poll_timeout=300,
+                                                                  polling_frequency=15, retries=1)
+        return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,response=response)
 
-        response = src_client_obj.configure_source_connection(source_id, connection_object=source_configure_payload)
-        return response
+    def browse_source_tables(self, src_client_obj, source_id,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        filter_tables_properties = self.configuration_obj["filter_tables_properties"]
+        response = src_client_obj.browse_source_tables(source_id, filter_tables_properties=filter_tables_properties,
+                                                       poll_timeout=300, polling_frequency=15, retries=1)
+        return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,response=response)
 
-    def import_source_configuration(self, src_client_obj, source_id,
-                                    mappings, export_configuration_file=None, export_config_lookup=True,
-                                    read_passwords_from_secrets=False):
-        src_name = self.configuration_obj["configuration"]["source_configs"]["name"]
+    def add_tables_to_source(self, src_client_obj, source_id,dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        tables_already_added_in_source = src_client_obj.list_tables_in_source(source_id)["result"]["response"]
+        tables_list = []
+        tables = self.configuration_obj["configuration"]["table_configs"]
+        if len(tables_already_added_in_source) > 0:
+            for table in tables:
+                if table["configuration"]["schema_name_at_source"] + "." + table["configuration"][
+                    "name"] not in tables_already_added_in_source:
+                    temp = {"table_name": table["configuration"]["name"],
+                            "schema_name": table["configuration"]["schema_name_at_source"],
+                            "table_type": table["entity_type"].upper(),
+                            "target_table_name": table["configuration"]["configuration"]["target_table_name"],
+                            "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
+                    if table["configuration"].get("catalog_name","")!="":
+                        temp["catalog_name"]=table["configuration"]["catalog_name"]
+                    tables_list.append(copy.deepcopy(temp))
+                    src_client_obj.logger.info(
+                        f"Adding table {temp['table_name']} to source {source_id} config payload")
+        else:
+            for table in tables:
+                temp = {"table_name": table["configuration"]["name"],
+                        "schema_name": table["configuration"]["schema_name_at_source"],
+                        "table_type": table["entity_type"].upper(),
+                        "target_table_name": table["configuration"]["configuration"]["target_table_name"],
+                        "target_schema_name": table["configuration"]["configuration"]["target_schema_name"]}
+                if table["configuration"].get("catalog_name", "") != "":
+                    temp["catalog_name"] = table["configuration"]["catalog_name"]
+                tables_list.append(copy.deepcopy(temp))
+                src_client_obj.logger.info(f"Adding table {temp['table_name']} to source {source_id} config payload")
+        response = src_client_obj.add_tables_to_source(source_id, tables_list)
+        return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
+                                           response=response)
+
+    def configure_tables_and_tablegroups(self, src_client_obj, source_id, export_configuration_file=None,
+                                         export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
+                                         env_tag="", secret_type="",dont_skip_step=True):
+        if not dont_skip_step:
+            return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
+        if mappings is None:
+            mappings = {}
+        iw_mappings = self.configuration_obj["configuration"]["iw_mappings"]
         table_group_compute_mappings = mappings.get("table_group_compute_mappings", {})
-        source_import_payload = {"configuration": self.configuration_obj["configuration"]}
-        modified_table_configs = self.configuration_obj["configuration"]["table_configs"]
-        index = 0
-        for table_config in self.configuration_obj["configuration"]["table_configs"]:
-            modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
-            if not table_config["configuration"].get("meta_crawl_performed", False):
-                modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
-                index = index + 1
-            else:
-                if not table_config["configuration"]["meta_crawl_performed"]:
-                    modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
-                index = index + 1
-        source_import_payload["configuration"]["table_configs"] = modified_table_configs
-        iw_mappings = source_import_payload["configuration"]["iw_mappings"]
+        source_configs = self.configuration_obj["configuration"]["source_configs"]
+        src_name = str(source_configs["name"])
         for item in iw_mappings:
             if item.get("entity_type", "") == "environment_compute_template":
                 item["recommendation"]["compute_name"] = table_group_compute_mappings.get(
                     item["recommendation"]["compute_name"], item["recommendation"]["compute_name"])
-        source_import_payload["configuration"]["iw_mappings"] = iw_mappings
+        self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
+        # Update the service account json file mappings if any
         if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
-            for table in source_import_payload.get("configuration")["table_configs"]:
+            for table in self.configuration_obj["configuration"]["table_configs"]:
                 # Check if there are any export configurations and passwords to replace
                 if table.get("configuration", {}).get("export_configuration", None) is not None:
                     export_configs = table.get("configuration", {}).get("export_configuration")
                     target_type = export_configs.get("target_type", "").upper()
                     table_name = table["configuration"]["name"].upper()
                     override_keys = []
-                    try:
-                        if export_configuration_file is not None:
-                            with open(export_configuration_file) as file:
-                                information = yaml.load(file, Loader=yaml.FullLoader)
-                            if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
-                                info_key = src_name + "_" + table_name
-                                override_keys = information["src_export_details"].get(src_name + "_" + table_name,
-                                                                                      {}).keys()
-                            else:
-                                info_key = src_name
-                                override_keys = information["src_export_details"].get(src_name, {}).keys()
-                            for key in override_keys:
-                                table["configuration"]["export_configuration"]["connection"][key] = \
-                                    information["src_export_details"][info_key][key]
-                    except Exception as e:
-                        src_client_obj.logger.error(
-                            f"Failed to lookup the export configuration file {export_configuration_file} due to {str(e)}")
-
-                    try:
-                        if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
-                            # Read the password from KMS
-                            encrypted_key_name1 = f"export-configuration-{src_name}-{table['configuration']['name']}"
-                            encrypted_key_name2 = f"export-configuration-{src_name}"
-                            passwd = self.secrets.get(encrypted_key_name1, "")
-                            if passwd == "":
-                                passwd = self.secrets.get(encrypted_key_name2, "")
-                            table["configuration"]["export_configuration"]["connection"]["password"] = passwd
-                        elif target_type.upper() == "BIGQUERY":
-                            if "server_path" not in override_keys:
-                                server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
-                                    "server_path", "")
-                                if "gcp_details" in mappings:
-                                    server_path = mappings["gcp_details"].get("service_json_path")
-                                if "service_json_mappings" in mappings:
-                                    server_path = mappings["service_json_mappings"].get(
-                                        server_path.split("/")[-1],
-                                        server_path)
-                                table["configuration"]["export_configuration"]["connection"][
-                                    "server_path"] = server_path if server_path != "" else table["configuration"][
-                                    "export_configuration"].get("connection", {}).get(
-                                    "server_path", "")
+                    if export_configuration_file is not None:
+                        with open(export_configuration_file) as file:
+                            information = yaml.load(file, Loader=yaml.FullLoader)
+                        if information["src_export_details"].get(src_name + "_" + table_name, None) is not None:
+                            info_key = src_name + "_" + table_name
+                            override_keys = information["src_export_details"].get(src_name + "_" + table_name,
+                                                                                  {}).keys()
+                        else:
+                            info_key = src_name
+                            override_keys = information["src_export_details"].get(src_name, {}).keys()
+                        for key in override_keys:
+                            table["configuration"]["export_configuration"]["connection"][key] = \
+                                information["src_export_details"][info_key][key]
+                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"]:
+                        pass
+
+                    elif target_type.upper() == "BIGQUERY":
+                        if "server_path" not in override_keys:
+                            server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
+                                "server_path", "")
+                            if "gcp_details" in mappings:
+                                server_path = mappings["gcp_details"].get("service_json_path")
+                            if "service_json_mappings" in mappings:
+                                server_path = mappings["service_json_mappings"].get(
+                                    server_path.split("/")[-1],
+                                    server_path)
                             table["configuration"]["export_configuration"]["connection"][
-                                "upload_option"] = "serverLocation"
-                    except Exception as e:
-                        src_client_obj.logger.error(
-                            f"Failed to lookup the export configuration password from secrets due to {str(e)}")
-        response = src_client_obj.configure_tables_and_tablegroups(source_id,
-                                                                   configuration_obj=source_import_payload.get(
-                                                                       "configuration"))
-        return response
-        # if response["result"]["status"].upper() != "SUCCESS":
-        #     src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
-        #                                 .format(source_id, self.source_config_path))
-        #     src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
-        #                                 .format(self.source_config_path))
-        #     return "FAILED"
-        # else:
-        #     src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
-        #     return "SUCCESS"
+                                "server_path"] = server_path if server_path != "" else table["configuration"][
+                                "export_configuration"].get("connection", {}).get(
+                                "server_path", "")
+                        table["configuration"]["export_configuration"]["connection"][
+                            "upload_option"] = "serverLocation"
+
+        response = src_client_obj.configure_tables_and_tablegroups(source_id, configuration_obj=self.configuration_obj[
+            "configuration"])
+        if response["result"]["status"].upper() != "SUCCESS":
+            src_client_obj.logger.error("Failed to import the source {} (source config path : {})"
+                                        .format(source_id, self.source_config_path))
+            src_client_obj.logger.error(response.get("message", "") + "(source config path : {})"
+                                        .format(self.source_config_path))
+            return SourceResponse.parse_result(status="FAILED", source_id=source_id,
+                                               response=response)
+
+        else:
+            src_client_obj.logger.info(f"Successfully imported source configurations to {source_id}")
+            return SourceResponse.parse_result(status=response["result"]["status"].upper(), source_id=source_id,
+                                               response=response)
+
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/domains.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/misc.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/pipelines.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,19 @@
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
             if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
-            final = d.setval(section.split("$"), dict(config.items(section)))
-            print(f"section replacement:{d.getval(section.split('$'))}")
+            try:
+                final = d.setval(section.split("$"), dict(config.items(section)))
+                print(f"section replacement:{d.getval(section.split('$'))}")
+            except KeyError as e:
+                pass
         self.configuration_obj = d.data
 
     def create(self, pipeline_client_obj, domain_id, domain_name):
         pipeline_name = self.configuration_obj["configuration"]["entity"]["entity_name"]
         sources_in_pipelines = []
         for item in self.configuration_obj["configuration"]["iw_mappings"]:
             if item["entity_type"] == "table" and "source_name" in item["recommendation"]:
@@ -205,29 +208,16 @@
                         if "service_json_mappings" in mappings:
                             server_path = mappings["service_json_mappings"].get(
                                 server_path.split("/")[-1],
                                 server_path)
                         item["properties"]["server_path"] = server_path
                     if "upload_option" in item["properties"]:
                         item["properties"]["upload_option"] = "serverLocation"
-                elif item.get("sub_type").upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
-                    if self.secrets["custom_secrets_read"] is True:
-                        encrypted_key_name = f"{env_tag}-dataconnection-{item['name']}"
-                        decrypt_value = self.secrets.get(encrypted_key_name, "")
-                        if IWUtils.is_json(decrypt_value):
-                            decrypt_value_dict = json.loads(decrypt_value)
-                            for key in decrypt_value_dict.keys():
-                                item["properties"][key] = decrypt_value_dict[key]
-                    else:
-                        encrypted_key_name = f"{env_tag}-dataconnection-{item['name']}"
-                        decrypt_value = pipeline_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name)
-                        if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                            decrypt_value_dict = json.loads(decrypt_value[0])
-                            for key in decrypt_value_dict.keys():
-                                item["properties"][key] = decrypt_value_dict[key]
+                elif item.get("sub_type").upper() in ["SNOWFLAKE", "POSTGRES"]:
+                    pass
                 data = IWUtils.ejson_serialize(item)
                 response = requests.post(create_data_connection_url,
                                          headers={'Authorization': 'Bearer ' + pipeline_client_obj.client_config[
                                              "bearer_token"],
                                                   'Content-Type': 'application/json'}, data=data, verify=False)
                 if response.status_code == 406:
                     pipeline_client_obj.client_config['bearer_token'] = get_bearer_token(
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/salesforce_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py`

 * *Files 21% similar despite different names*

```diff
@@ -76,29 +76,14 @@
         if override_config_file is not None:
             with open(override_config_file) as file:
                 information = yaml.load(file, Loader=yaml.FullLoader)
             if information["source_details"].get(src_name, None) is not None:
                 override_keys = information["source_details"].get(src_name).keys()
                 for key in override_keys:
                     connection_object[key] = information["source_details"][src_name][key]
-        if read_passwords_from_secrets and self.secrets["custom_secrets_read"] is True:
-            encrypted_key_name = f"{env_tag}-" + src_name
-            decrypt_value = self.secrets.get(encrypted_key_name, "")
-            if IWUtils.is_json(decrypt_value):
-                decrypt_value_dict = json.loads(decrypt_value)
-                for key in decrypt_value_dict.keys():
-                    connection_object[key] = decrypt_value_dict[key]
-        elif read_passwords_from_secrets and self.secrets["custom_secrets_read"] is False:
-            encrypted_key_name = f"{env_tag}-" + src_name
-            decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name)
-            if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                decrypt_value_dict = json.loads(decrypt_value[0])
-                for key in decrypt_value_dict.keys():
-                    connection_object[key] = decrypt_value_dict[key]
-
         response = src_client_obj.configure_source_connection(source_id, connection_object=connection_object)
         if response["result"]["status"].upper() != "SUCCESS":
             src_client_obj.logger.info(f"Failed to configure the source {source_id} connection")
             src_client_obj.logger.info(response["result"])
             return "FAILED"
         else:
             src_client_obj.logger.info(response["result"])
@@ -146,36 +131,16 @@
                                                                                   {}).keys()
                         else:
                             info_key = src_name
                             override_keys = information["src_export_details"].get(src_name, {}).keys()
                         for key in override_keys:
                             table["configuration"]["export_configuration"]["connection"][key] = \
                                 information["src_export_details"][info_key][key]
-                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"] and read_passwords_from_secrets:
-                        if self.secrets["custom_secrets_read"] is True:
-                            encrypted_key_name1 = f"{env_tag}-export-configuration-{src_name}-{table['configuration']['name']}"
-                            encrypted_key_name2 = f"{env_tag}-export-configuration-{src_name}"
-                            decrypt_value = self.secrets.get(encrypted_key_name1, "")
-                            if decrypt_value == "" or decrypt_value is None:
-                                decrypt_value = self.secrets.get(encrypted_key_name2, "")
-                            decrypt_value_dict = json.loads(decrypt_value)
-                            for key in decrypt_value_dict.keys():
-                                table["configuration"]["export_configuration"]["connection"][key] = \
-                                    decrypt_value_dict[key]
-                        else:
-                            encrypted_key_name1 = f"{env_tag}-export-configuration-{src_name}-{table['configuration']['name']}"
-                            encrypted_key_name2 = f"{env_tag}-export-configuration-{src_name}"
-                            decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name1)
-                            if len(decrypt_value) == 0:
-                                decrypt_value = src_client_obj.get_all_secrets(secret_type, keys=encrypted_key_name2)
-                            if len(decrypt_value) > 0 and IWUtils.is_json(decrypt_value[0]):
-                                decrypt_value_dict = json.loads(decrypt_value[0])
-                                for key in decrypt_value_dict.keys():
-                                    table["configuration"]["export_configuration"]["connection"][key] = \
-                                            decrypt_value_dict[key]
+                    if target_type.upper() in ["SNOWFLAKE", "POSTGRES"]:
+                        pass
                     elif target_type.upper() == "BIGQUERY":
                         if "server_path" not in override_keys:
                             server_path = table["configuration"]["export_configuration"].get("connection", {}).get(
                                 "server_path", "")
                             if "gcp_details" in mappings:
                                 server_path = mappings["gcp_details"].get("service_json_path")
                             if "service_json_mappings" in mappings:
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/update_configurations.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/update_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/workflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,19 @@
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
             if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
-            final = d.setval(section.split("$"), dict(config.items(section)))
-            print(f"section replacement:{d.getval(section.split('$'))}")
+            try:
+                final = d.setval(section.split("$"), dict(config.items(section)))
+                print(f"section replacement:{d.getval(section.split('$'))}")
+            except KeyError as e:
+                pass
         self.configuration_obj = d.data
 
     def create(self, wf_client_obj, domain_id, domain_name):
         sources_in_wfs = []
         workflow_name = self.configuration_obj["configuration"]["entity"]["entity_name"]
         for item in self.configuration_obj["configuration"]["iw_mappings"]:
             if item["entity_type"] == "table_group" and "source_name" in item["recommendation"]:
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import traceback
 
 from infoworks.sdk import url_builder
 from infoworks.sdk.base_client import BaseClient
 from infoworks.sdk.cicd.upload_configurations.pipelines import Pipeline
+from infoworks.sdk.cicd.upload_configurations.pipeline_group import PipelineGroup
 from pathlib import Path
 from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.local_configurations import Response
 import os.path
 import queue
 import threading
@@ -165,21 +166,87 @@
                                                                              params={"filter": {"name": compute_name}})
                         if len(result["result"]["response"]) != 0:
                             compute_id = result["result"]["response"][0]["id"]
             if env_id is None:
                 print("No env id and no mapping found")
                 raise Exception("No env id and no mapping found")
             pl_obj = Pipeline(configuration_file_path, env_id, storage_id, compute_id, replace_words, self.secrets_config)
+            pl_obj.update_mappings_for_configurations(self.mappings)
             pipeline_id, domain_id = pl_obj.create(self, domain_id, domain_name)
             if pipeline_id is not None:
                 status = pl_obj.configure(self, pipeline_id, domain_id, override_configuration_file, self.mappings, read_passwords_from_secrets,env_tag=env_tag, secret_type=secret_type)
         except Exception as e:
             self.logger.error(str(e))
             print(str(e))
-            traceback.print_stack()
+            self.logger.error(traceback.format_exc())
+            print(traceback.format_exc())
+
+    def cicd_create_configure_pipeline_group(self, configuration_file_path, domain_id=None, domain_name=None,
+                                       override_configuration_file=None,
+                                       replace_words="", read_passwords_from_secrets=False, env_tag="", secret_type=""):
+        """
+        Function to create and configure pipeline group using the pipeline group configuration JSON file
+        Pass either domain_id or domain_name.If both are not passed the name of the domain should be first part of the file name
+        :param configuration_file_path: Path of the file with pipeline configurations to be imported
+        :param domain_id: Domain id to which the pipeline belongs to
+        :param domain_name: Domain name to which the pipeline belongs to
+        :param override_configuration_file: Path of the file with override keys for dataconnection properties
+        :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
+        :param read_passwords_from_secrets: True/False. If True all the pipeline related passwords are read from encrypted file name passed
+        """
+        try:
+            if domain_id is None and domain_name is None:
+                domain_name = Path(configuration_file_path).name.split("#")[0]
+            env_id = self.client_config.get("default_environment_id", None)
+            storage_id = self.client_config.get("default_storage_id", None)
+            compute_id = self.client_config.get("default_compute_id", None)
+            with open(configuration_file_path, 'r') as file:
+                json_string = file.read()
+            configuration_obj = IWUtils.ejson_deserialize(json_string)
+            environment_configurations = configuration_obj["environment_configurations"]
+            if env_id is None and "environment_mappings" in self.mappings:
+                env_name = self.mappings["environment_mappings"].get(environment_configurations["environment_name"],
+                                                                     environment_configurations["environment_name"])
+                if env_name is not None:
+                    result = self.__wrapper_get_environment_details(params={"filter": {"name": env_name}})
+                    env_id = result["result"]["response"][0]["id"] if len(result["result"]["response"]) > 0 else None
+            if storage_id is None and "storage_mappings" in self.mappings:
+                storage_name = self.mappings["storage_mappings"].get(
+                    environment_configurations["environment_storage_name"],
+                    environment_configurations["environment_storage_name"])
+                if storage_name is not None:
+                    result = self.__wrapper_get_storage_details(environment_id=env_id,
+                                                                params={"filter": {"name": storage_name}})
+                    storage_id = result["result"]["response"][0]["id"] if len(result["result"]["response"]) > 0 else None
+            if compute_id is None and "compute_mappings" in self.mappings:
+                compute_name = self.mappings["compute_mappings"].get(
+                    environment_configurations["environment_compute_template_name"],
+                    environment_configurations["environment_compute_template_name"])
+                if compute_name is not None:
+                    result = self.__wrapper_get_compute_template_details(environment_id=env_id,
+                                                                         params={"filter": {"name": compute_name}})
+                    if len(result["result"]["response"]) != 0:
+                        compute_id = result["result"]["response"][0]["id"]
+                    else:
+                        result = self.__wrapper_get_compute_template_details(environment_id=env_id, is_interactive=True,
+                                                                             params={"filter": {"name": compute_name}})
+                        if len(result["result"]["response"]) != 0:
+                            compute_id = result["result"]["response"][0]["id"]
+            if env_id is None:
+                print("No env id and no mapping found")
+                raise Exception("No env id and no mapping found")
+            pl_grp_obj = PipelineGroup(configuration_file_path, env_id, storage_id, compute_id, replace_words, self.secrets_config)
+            pl_grp_obj.update_mappings_for_configurations(self.mappings)
+            pipeline_group_id, domain_id = pl_grp_obj.create(self, domain_id, domain_name)
+        except Exception as e:
+            self.logger.error(str(e))
+            print(str(e))
+            self.logger.error(traceback.format_exc())
+            print(traceback.format_exc())
+
 
     def __execute(self, thread_number, q):
         while True:
             try:
                 print('%s: Looking for the next task ' % thread_number)
                 task = q.get()
                 print(f'\nThread Number {thread_number} processed {task}')
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrappersource.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
         :param read_passwords_from_secrets: True/False. If True all the source related passwords are read from encrypted file name passed
         """
         response_to_return ={}
         try:
             env_id = self.client_config.get("default_environment_id", None)
             storage_id = self.client_config.get("default_storage_id", None)
+            compute_id = self.client_config.get("default_compute_id", None)
             with open(configuration_file_path, 'r') as file:
                 json_string = file.read()
             configuration_obj = IWUtils.ejson_deserialize(json_string)
             environment_configurations = configuration_obj["environment_configurations"]
             if env_id is None and "environment_mappings" in self.mappings:
                 env_name = self.mappings["environment_mappings"].get(environment_configurations["environment_name"],
                                                                      environment_configurations["environment_name"])
@@ -111,14 +112,20 @@
                     environment_configurations["environment_storage_name"],
                     environment_configurations["environment_storage_name"])
                 if storage_name is not None:
                     result = self.__wrapper_get_storage_details(environment_id=env_id,
                                                                 params={"filter": {"name": storage_name}})
                     storage_id = result["result"]["response"][0]["id"] if len(result["result"]["response"]) > 0 else None
                     response_to_return["get_storage_entity_response"] = result
+            if compute_id is None and "compute_mappings" in self.mappings:
+                iw_mappings = configuration_obj["configuration"]["iw_mappings"]
+                compute_mappings_from_config = dict(self.mappings.get("compute_mappings"))
+                for mapping in iw_mappings:
+                    if mapping["entity_type"]=="environment_compute_template":
+                        mapping["recommendation"]["compute_name"]=compute_mappings_from_config.get(mapping["recommendation"]["compute_name"],mapping["recommendation"]["compute_name"])
             if env_id is None or storage_id is None:
                 print("No env id or storage id found")
                 raise Exception("No env id or storage id found")
 
             source_type = configuration_obj["configuration"]["source_configs"]["type"]
             source_sub_type = configuration_obj["configuration"]["source_configs"]["sub_type"]
             if source_type == "file" and source_sub_type == "structured":
@@ -126,23 +133,23 @@
                 source_obj.update_mappings_for_configurations(self.mappings)
                 create_source_response = source_obj.create_csv_source(self)
                 source_id=create_source_response["result"]["source_id"]
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     source_connection_configurations_response = source_obj.configure_csv_source(self, source_id, self.mappings,
                                                     read_passwords_from_secrets=read_passwords_from_secrets,
-                                                    env_tag=env_tag, secret_type=secret_type,config_ini_path=config_ini_path)
-                    if source_connection_configurations_response["result"]["status"].upper() == "SUCCESS":
+                                                    env_tag=env_tag, secret_type=secret_type,config_ini_path=config_ini_path,dont_skip_step=configuration_obj["steps_to_run"]["configure_rdbms_source_connection"])
+                    if source_connection_configurations_response["result"]["status"].upper() in ["SUCCESS","SKIPPED"]:
                         print("Successfully configured the connection details")
                         self.logger.info("Successfully configured the connection details")
                         # Proceed to configure tables and table groups
                         source_import_configuration_response = source_obj.import_source_configuration(self, source_id, self.mappings,
                                                                         override_configuration_file, export_lookup,
                                                                         read_passwords_from_secrets)
-                        if source_import_configuration_response["result"]["status"].upper() == "SUCCESS":
+                        if source_import_configuration_response["result"]["status"].upper() in ["SUCCESS","SKIPPED"]:
                             self.logger.info("Configured source successfully")
                             print("Configured Source successfully!")
                         else:
                             self.logger.info("Failed to configure source")
                             print("Failed to configure source")
                             print(source_import_configuration_response)
                             self.logger.error("Failed to configure source")
@@ -161,67 +168,85 @@
                 else:
                     print("Failed to create source")
                     self.logger.error("Failed to create source")
                     raise Exception("Failed to create source")
                 response_to_return["create_source_response"] = create_source_response
             elif source_type == "rdbms" and source_sub_type!="snowflake":
                 source_obj = RDBMSSource()
-                source_obj.update_mappings_for_configurations(self.mappings)
                 source_obj.set_variables(env_id, storage_id, configuration_file_path, self.secrets_config,
                                          replace_words)
+                source_obj.update_mappings_for_configurations(self.mappings)
                 source_creation_response = source_obj.create_rdbms_source(self)
                 source_id = source_creation_response["result"]["source_id"]
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     source_connection_configurations_response = source_obj.configure_rdbms_source_connection(self, source_id, override_configuration_file,
                                                                     read_passwords_from_secrets=read_passwords_from_secrets,
                                                                     env_tag=env_tag,
-                                                                    secret_type=secret_type,config_ini_path=config_ini_path)
-                    if source_connection_configurations_response["result"]["status"].upper() == "SUCCESS":
+                                                                    secret_type=secret_type,config_ini_path=config_ini_path,dont_skip_step=configuration_obj["steps_to_run"]["configure_rdbms_source_connection"])
+                    if source_connection_configurations_response["result"]["status"].upper() in ["SUCCESS","SKIPPED"]:
                         print("Successfully configured the connection details")
                         self.logger.info("Successfully configured the connection details")
-                        source_test_connection_response = source_obj.test_source_connection(self, source_id)
-                        if source_test_connection_response["result"]["status"].upper() == "SUCCESS":
-                            source_browse_source_tables_response = source_obj.browse_source_tables(self, source_id)
-                            if source_browse_source_tables_response["result"]["status"].upper() == "SUCCESS":
-                                status = source_obj.add_tables_to_source(self, source_id)
-                                if status == "SUCCESS":
+                        source_test_connection_response = source_obj.test_source_connection(self, source_id,dont_skip_step=configuration_obj["steps_to_run"]["test_source_connection"])
+                        if source_test_connection_response["result"]["status"].upper() in ["SUCCESS","SKIPPED"]:
+                            source_browse_source_tables_response = source_obj.browse_source_tables(self, source_id,configuration_obj["steps_to_run"]["browse_source_tables"])
+                            if source_browse_source_tables_response["result"]["status"].upper() in ["SUCCESS","SKIPPED"]:
+                                add_tables_to_source_response = source_obj.add_tables_to_source(self, source_id,configuration_obj["steps_to_run"]["add_tables_to_source"])
+                                status = add_tables_to_source_response["result"]["status"]
+                                if status == "SUCCESS" or add_tables_to_source_response["result"].get("response",{}).get("result",{}).get("response",{}).get("iw_code","")=="IW10003":
                                     self.logger.info("Added tables to source successfully")
                                     print("Added tables to source successfully")
                                 else:
                                     print("Failed to add tables to source")
+                                    print(add_tables_to_source_response)
                                     self.logger.error("Failed to add tables to source")
+                                    self.logger.error(add_tables_to_source_response)
                                     raise Exception("Failed to add tables to source")
-                                status = source_obj.configure_tables_and_tablegroups(self, source_id,
+                                configure_tables_and_tablegroups_response = source_obj.configure_tables_and_tablegroups(self, source_id,
                                                                                      override_configuration_file,
                                                                                      export_lookup, self.mappings,
                                                                                      read_passwords_from_secrets,
                                                                                      env_tag=env_tag,
-                                                                                     secret_type=secret_type)
+                                                                                     secret_type=secret_type,dont_skip_step=configuration_obj["steps_to_run"]["configure_tables_and_tablegroups"])
+                                status = configure_tables_and_tablegroups_response["result"]["status"]
                                 if status == "SUCCESS":
                                     self.logger.info("Configured source successfully")
+                                    print(configure_tables_and_tablegroups_response)
+                                    self.logger.info(configure_tables_and_tablegroups_response)
                                     print("Configured source successfully")
                                 else:
                                     self.logger.error("Failed to configure source")
                                     print("Failed to configure source")
+                                    print(configure_tables_and_tablegroups_response)
+                                    self.logger.error(configure_tables_and_tablegroups_response)
                                     raise Exception("Failed to configure source")
+                            else:
+                                self.logger.error("Failed while browsing tables")
+                                self.logger.error(source_browse_source_tables_response)
+                                print("Failed while browsing tables")
+                                print(source_browse_source_tables_response)
+                                self.logger.error(source_browse_source_tables_response)
+                                raise Exception("Failed while browsing tables")
                         else:
                             print(source_test_connection_response)
+                            self.logger.error(source_test_connection_response)
                             raise Exception("Failed to launch test connection job")
                     else:
                         print(source_connection_configurations_response)
+                        self.logger.error(source_connection_configurations_response)
                         raise Exception("Failed to configure source connection details")
                 else:
                     print(source_creation_response)
+                    self.logger.error(source_creation_response)
                     raise Exception("Failed to create source")
             elif source_type == "crm" and source_sub_type == "salesforce":
                 source_obj = SalesforceSource()
-                source_obj.update_mappings_for_configurations(self.mappings)
                 source_obj.set_variables(env_id, storage_id, configuration_file_path, self.secrets_config,
                                          replace_words)
+                source_obj.update_mappings_for_configurations(self.mappings)
                 source_id = source_obj.create_salesforce_source(self)
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     if source_obj.configure_salesforce_source_connection(self, source_id, override_configuration_file,
                                                                     read_passwords_from_secrets=read_passwords_from_secrets,
                                                                     env_tag=env_tag,
                                                                     secret_type=secret_type) == "SUCCESS":
@@ -282,15 +307,16 @@
                     else:
                         self.logger.error("Failed to configure the source connection")
                         print("Failed to configure the source connection")
                         raise Exception("Failed to configure the source connection")
             return response_to_return
         except Exception as e:
             self.logger.error(str(e))
-            traceback.print_exc()
+            self.logger.error(traceback.format_exc())
+            print(traceback.format_exc())
             print(str(e))
             return response_to_return
 
     def __execute(self, thread_number, q):
         while True:
             try:
                 print('%s: Looking for the next task ' % thread_number)
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,22 @@
         :param domain_name: Domain name to which the pipeline belongs to
         :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
         """
         try:
             if domain_id is None and domain_name is None:
                 domain_name = Path(configuration_file_path).name.split("#")[0]
             wf_obj = Workflow(configuration_file_path, replace_words)
+            wf_obj.update_mappings_for_configurations(self.mappings)
             wf_id, domain_id = wf_obj.create(self, domain_id, domain_name)
             if wf_id is not None:
                 status = wf_obj.configure(self, wf_id, domain_id)
         except Exception as e:
             self.logger.error(str(e))
             print(str(e))
-            traceback.print_stack()
+            print(traceback.format_exc())
 
     def __execute(self, thread_number, q):
         while True:
             try:
                 print('%s: Looking for the next task ' % thread_number)
                 task = q.get()
                 print(f'\nThread Number {thread_number} processed {task}')
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/client.py` & `infoworkssdk-3.0b0/infoworks/sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from infoworks.sdk.source_client import SourceClient
 from infoworks.sdk.pipeline_client import PipelineClient
 from infoworks.sdk.workflow_client import WorkflowClient
 from infoworks.sdk.domain_client import DomainClient
 from infoworks.sdk.jobmetrics import JobMetricsClient
 from infoworks.sdk.admin_client import AdminClient
 from infoworks.sdk.jobs_client import JobsClient
+from infoworks.sdk.pipeline_group_client import PipelineGroupClient
 
 
 class InfoworksClientSDK(SourceClient, PipelineClient, WorkflowClient, DomainClient, AdminClient, JobMetricsClient,
                          DownloadSource, DownloadPipeline, DownloadWorkflow, DownloadEntityWithLineage,
-                         DownloadAllEntitiesFromDomain, WrapperSource, WrapperPipeline, WrapperWorkflow, JobsClient):
+                         DownloadAllEntitiesFromDomain, WrapperSource, WrapperPipeline, WrapperWorkflow, JobsClient,
+                         PipelineGroupClient):
     def __init__(self):
         super().__init__()
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/ejson/__init__.py` & `infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/generic_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/generic_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/jobmetrics.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,47 +89,56 @@
                                                                       )
                     response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
                     result = response.get("result", [])
                 return combinedJobMetric
         except Exception as e:
             raise AdminError("Unable to get ingestion job metrics info")
 
-    def get_source_file_paths(self, source_id, table_id, job_id):
+    def get_export_metrics(self, job_id, source_id):
+        """
+        Function to get export metrics for the source job
+        :param job_id: Entity identifier of the job
+        :param source_id: Entity identifier of the source
+        :return: List of job metrics
+        """
         try:
-            source_files = []
-            url_to_get_src_filepaths = url_builder.get_source_file_paths_url(self.client_config, source_id, table_id,
-                                                                             job_id) + "?limit=50&offset=0"
+            combinexportMetric = []
+            url_to_get_export_job_metrics = url_builder.get_export_metrics_source_url(self.client_config, source_id,
+                                                                                      job_id) + "?limit=50&offset=0"
             response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_get_src_filepaths,
+                self.call_api("GET", url_to_get_export_job_metrics,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
                               ).content)
             if response is not None and "result" in response:
                 result = response.get("result", [])
                 while len(result) > 0:
-                    source_files.extend(result)
+                    combinexportMetric.extend(result)
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
                     result = response.get("result", [])
-                return source_files
+                return combinexportMetric
         except Exception as e:
-            print(e)
-            raise AdminError("Unable to get source file pat metrics info")
+            raise AdminError("Unable to get export job metrics info")
 
-    def get_export_metrics(self, job_id):
+    def get_ingestion_metrics_with_job_id(self, job_id):
+        """
+        Function to get ingestion metrics for the job
+        :param job_id: Entity identifier of the job
+        :return: List of job metrics
+        """
         try:
             combinedJobMetric = []
-            url_to_get_export_metrics = url_builder.get_export_metrics_url(self.client_config,
-                                                                           job_id) + "?limit=50&offset=0"
-
+            url_to_get_job_ingestion_metrics = url_builder.get_ingestion_metrics_admin_url(self.client_config,
+                                                                                           job_id) + "?limit=50&offset=0"
             response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_get_export_metrics,
+                self.call_api("GET", url_to_get_job_ingestion_metrics,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
                               ).content)
             if response is not None and "result" in response:
                 result = response.get("result", [])
                 while len(result) > 0:
                     combinedJobMetric.extend(result)
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
@@ -137,22 +146,106 @@
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
                     result = response.get("result", [])
                 return combinedJobMetric
         except Exception as e:
-            print(e)
+            raise AdminError("Unable to get ingestion job metrics info")
+
+    def get_export_metrics_with_job_id(self, job_id):
+        """
+        Function to get ingestion metrics for the job
+        :param job_id: Entity identifier of the job
+        :return: List of job metrics
+        """
+        try:
+            exportMetric = []
+            url_to_get_job_ingestion_metrics = url_builder.get_export_metrics_url(self.client_config,
+                                                                                  job_id) + "?limit=50&offset=0"
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_job_ingestion_metrics,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
+                              ).content)
+            if response is not None and "result" in response:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    exportMetric.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
+                    result = response.get("result", [])
+                return exportMetric
+        except Exception as e:
             raise AdminError("Unable to get export job metrics info")
 
+    def get_metrics_prodops(self, config_body):
+        """
+        Function to Fetch the metrics for a given time period
+        :param config_body: JSON dict
+        config_body = {'limit': 10000, 'date_range': {'type': 'last', 'unit': 'day', 'value': 1}, 'offset': 0}
+        :return: List of job metrics
+        """
+        try:
+            if config_body is None:
+                raise Exception("config_body cannot be None")
+            metrics = []
+            url_to_get_metrics = url_builder.get_metrics_prodops_url(self.client_config) + "?limit=50&offset=0"
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_metrics,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
+                              ).content)
+            if response is not None and "result" in response:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    metrics.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
+                    result = response.get("result", [])
+                return metrics
+        except Exception as e:
+            raise AdminError("Unable to get job metrics info")
+
+    def get_source_file_paths(self, source_id, table_id, job_id):
+        try:
+            source_files = []
+            url_to_get_src_filepaths = url_builder.get_source_file_paths_url(self.client_config, source_id, table_id,
+                                                                             job_id) + "?limit=50&offset=0"
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_src_filepaths,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
+                              ).content)
+            if response is not None and "result" in response:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    source_files.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(self.callurl(nextUrl).content)
+                    result = response.get("result", [])
+                return source_files
+        except Exception as e:
+            print(e)
+            raise AdminError("Unable to get source file pat metrics info")
+
     def get_pipeline_build_metrics(self, job_id):
         try:
             combinedJobMetric = []
             url_to_get_pipeline_build_metrics = url_builder.get_pipeline_build_metrics_url(self.client_config,
-                                                                                   job_id) + "?limit=50&offset=0"
+                                                                                           job_id) + "?limit=50&offset=0"
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_get_pipeline_build_metrics,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])
                               ).content)
             if response is not None and "result" in response:
                 result = response.get("result", [])
                 while len(result) > 0:
@@ -721,23 +814,28 @@
             pipeline_jobs_list = self.get_pipeline_jobs(date_string)
             with ThreadPoolExecutor(max_workers=10) as executor:
                 executor.map(self.get_pipeline_build_metrics_results, pipeline_jobs_list,
                              [workflow_id, workflow_run_id] * len(pipeline_jobs_list))
                 executor.shutdown(wait=True)
 
             result = []
-            header = ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time', 'job_end_time', 'job_status', 'source_name', 'source_file_names', 'source_schema_name', 'source_database_name', 'table_group_name', 'iwx_table_name', 'starting_watermark_value', 'ending_watermark_value', 'target_schema_name', 'target_table_name', 'pre_target_count', 'fetch_records_count', 'target_records_count', 'job_link']
-            ui_port = 443 if self.client_config["port"]=='443' else 3000
+            header = ['workflow_id', 'workflow_run_id', 'job_id', 'entity_type', 'job_type', 'job_start_time',
+                      'job_end_time', 'job_status', 'source_name', 'source_file_names', 'source_schema_name',
+                      'source_database_name', 'table_group_name', 'iwx_table_name', 'starting_watermark_value',
+                      'ending_watermark_value', 'target_schema_name', 'target_table_name', 'pre_target_count',
+                      'fetch_records_count', 'target_records_count', 'job_link']
+            ui_port = 443 if self.client_config["port"] == '443' else 3000
             if len(self.job_metrics_final) > 0:
                 for item in self.job_metrics_final:
                     dict_temp = {}
                     for i in header:
                         dict_temp[i] = item.get(i)
-                        if i=="job_link" and dict_temp.get("job_id",None)!=None:
-                            dict_temp[i]=f"{self.client_config['protocol']}://{self.client_config['ip']}:{ui_port}/job/logs?jobId={dict_temp.get('job_id','')}"
+                        if i == "job_link" and dict_temp.get("job_id", None) != None:
+                            dict_temp[
+                                i] = f"{self.client_config['protocol']}://{self.client_config['ip']}:{ui_port}/job/logs?jobId={dict_temp.get('job_id', '')}"
                     result.append(copy.deepcopy(dict_temp))
                 return result
             else:
                 print("Job list empty!!!")
         except Exception as e:
             print("Something went wrong")
             print(str(e))
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/jobs_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,16 @@
             raise Exception("job_id cannot be None")
         if params is None:
             params = {"limit": 20, "offset": 0}
 
         url_to_list_jobs = url_builder.get_jobs_url(self.client_config)
         if job_id is not None:
             url_to_list_jobs = url_to_list_jobs + f"/{job_id}"
-        url_to_list_jobs = url_to_list_jobs + IWUtils.get_query_params_string_from_dict(params=params)
+        else:
+            url_to_list_jobs = url_to_list_jobs + IWUtils.get_query_params_string_from_dict(params=params)
         job_details = []
 
         try:
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_jobs,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             initial_msg = ""
@@ -62,31 +63,28 @@
             response["result"] = job_details
             response["message"] = initial_msg
             return GenericResponse.parse_result(job_id=job_id, status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting job details")
             raise JobsError("Error in getting job details" + str(e))
 
-    def resubmit_failed_tables_for_ingestion(self, job_id=None, params=None):
+    def resubmit_failed_tables_for_ingestion(self, job_id=None, role="admin"):
         """
         Resubmit the failed tables for Ingestion
         :param job_id: job id to resubmit the failed tables for ingestion
         :type job_id: String
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type: JSON dict
+        :param role: Can be either admin/prodops
         :return: response dict
         """
         if None in {job_id}:
             self.logger.error("job_id cannot be None")
             raise Exception("job_id cannot be None")
-        if params is None:
-            params = {"limit": 20, "offset": 0}
         url_to_resubmit_job_for_failed_tables = url_builder.get_jobs_url(self.client_config) + f"/{job_id}/resubmit"
-        url_to_resubmit_job_for_failed_tables = url_to_resubmit_job_for_failed_tables + IWUtils.get_query_params_string_from_dict(
-            params=params)
+        if role.lower() == "prodops":
+            url_to_resubmit_job_for_failed_tables.reaplce("admin", "prodops")
         response = None
         try:
             response = IWUtils.ejson_deserialize(
                 self.call_api("POST", url_to_resubmit_job_for_failed_tables,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
 
             result = response.get('result', [])
@@ -163,37 +161,57 @@
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :return: response dict
         """
         if None in {job_id}:
             self.logger.error("job_id cannot be None")
             raise Exception("job_id cannot be None")
-        try:
-            if params is None:
-                params = {"limit": 20, "offset": 0}
-            url_to_get_cluster_job_details = url_builder.get_jobs_url(self.client_config) + f"/{job_id}/runs"
-            if run_id:
-                url_to_get_cluster_job_details = url_to_get_cluster_job_details + f"/{run_id}"
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+
+        url_to_get_cluster_job_details = url_builder.get_jobs_url(self.client_config) + f"/{job_id}/runs"
+        if run_id:
+            url_to_get_cluster_job_details = url_to_get_cluster_job_details + f"/{run_id}"
+        else:
             url_to_get_cluster_job_details = url_to_get_cluster_job_details + IWUtils.get_query_params_string_from_dict(
                 params=params)
-            response = None
-            response = IWUtils.ejson_deserialize(self.call_api("GET", url_to_get_cluster_job_details,
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token']),
-                                                               ).content)
-            result = response.get('result', None)
-            if result is None:
-                self.logger.error(f"Failed to get the cluster job details for {job_id}.")
-                return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f"Failed to get the cluster job details for {job_id}.",
-                                                    job_id=job_id, response=response)
-            else:
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        job_details = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_cluster_job_details,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            initial_msg = ""
+            if response is not None:
+                initial_msg = response.get("message", "")
+                result = response.get("result", None)
+                if result is None:
+                    self.logger.error('Failed to get job details')
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                        error_desc='Failed to get cluster job details',
+                                                        response=response)
+                if run_id is not None:
+                    job_details.extend([result])
+                else:
+                    while len(result) > 0:
+                        job_details.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", [])
+            response["result"] = job_details
+            response["message"] = initial_msg
+            return GenericResponse.parse_result(job_id=job_id, status=Response.Status.SUCCESS, response=response)
         except Exception as e:
-            raise JobsError(f"Failed to get the cluster job details for {job_id}." + str(e))
+            self.logger.error("Error in getting cluster job details")
+            raise JobsError("Error in getting cluster job details" + str(e))
 
     def get_admin_job_details(self, params=None):
         """
         Function to get the admin job details
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :return: response list of dict
@@ -287,55 +305,55 @@
             response["message"] = initial_msg
             response["result"] = job_details
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting job details")
             raise JobsError("Error in getting job details" + str(e))
 
-    def get_crawl_job_summary(self, job_id=None, source_id=None, params=None):
+    def get_source_job_summary_or_logs(self, job_id=None, source_id=None, type="summary", num_of_lines=1000):
         """
         Function to get job summary for given job_id
         :param source_id: source_id for the job
         :type source_id: String
         :param job_id: job_id for the job
         :type job_id: String
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :param type: can be either summary/logs
         :return: response dict
         """
         if None in {job_id, source_id}:
             self.logger.error("job_id or source_id cannot be None")
             raise Exception("job_id or source_id cannot be None")
         try:
-            if params is None:
-                params = {"limit": 20, "offset": 0}
-            url_to_get_cluster_job_details = url_builder.get_source_details_url(
-                self.client_config) + f"/{source_id}/jobs/{job_id}/summary"
-            url_to_get_cluster_job_details = url_to_get_cluster_job_details + IWUtils.get_query_params_string_from_dict(
-                params=params)
-            response = None
+            if type.lower() == "summary":
+                url_to_get_cluster_job_details = url_builder.get_source_details_url(
+                    self.client_config) + f"/{source_id}/jobs/{job_id}/summary"
+            else:
+                url_to_get_cluster_job_details = url_builder.get_source_details_url(
+                    self.client_config) + f"/{source_id}/jobs/{job_id}/logs?num_of_lines={num_of_lines}"
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_to_get_cluster_job_details,
                                                                IWUtils.get_default_header_for_v3(
                                                                    self.client_config['bearer_token']),
                                                                ).content)
             result = response.get('result', None)
             if result is None:
-                self.logger.error(f"Failed to get the crawl job summary for job_id {job_id}.")
+                self.logger.error(f"Failed to get the crawl job summary/log for job_id {job_id}.")
                 return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f"Failed to get the crawl job summary for job_id {job_id}.",
+                                                    error_desc=f"Failed to get the crawl job summary/log for job_id {job_id}.",
                                                     response=response, job_id=job_id)
             else:
                 return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
-            raise JobsError(f"Failed to get the crawl job summary for job_id {job_id}." + str(e))
+            raise JobsError(f"Failed to get the crawl job summary/log for job_id {job_id}." + str(e))
 
     def get_interactive_jobs_list(self, source_id=None, job_id=None, params=None):
         """
         Function to get all interactive jobs
         :param source_id: source_id for the interactive jobs
         :type source_id: String
+        :param job_id: Entity identifier of the job
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
         :type: JSON dict
         :return: response list of dict
         """
         if None in {source_id}:
             self.logger.error("source_id cannot be None")
             raise Exception("source_id cannot be None")
@@ -426,15 +444,15 @@
             response["message"] = initial_msg
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in getting job details")
             raise JobsError("Error in getting job details" + str(e))
 
     def submit_pipeline_job(self, domain_id=None, pipeline_id=None, version_id=None, job_type=None,
-                            updated_pipeline_parameters=[], params=None):
+                            updated_pipeline_parameters=[]):
         """
         Function to initiate a pipeline job for given pipeline id
         :param domain_id: domain_id for the pipeline
         :type domain_id: String
         :param pipeline_id: Id of the pipeline
         :type pipeline_id: String
         :param version_id: version_id of the pipeline
@@ -445,21 +463,16 @@
         :type job_type: String
         :return: response dict
         """
         if None in {domain_id, pipeline_id}:
             self.logger.error("domain_id or pipeline_id cannot be None")
             raise Exception("domain_id or pipeline_id cannot be None")
         try:
-            if params is None:
-                params = {"limit": 20, "offset": 0}
             url_to_initiate_pipeline_job = url_builder.get_pipeline_jobs_url(self.client_config, domain_id=domain_id,
                                                                              pipeline_id=pipeline_id)
-            url_to_initiate_pipeline_job = url_to_initiate_pipeline_job + IWUtils.get_query_params_string_from_dict(
-                params=params)
-            response = None
             api_payload = {}
             if version_id:
                 api_payload["version_id"] = version_id
             if job_type:
                 api_payload["job_type"] = job_type
             if updated_pipeline_parameters:
                 api_payload["updated_pipeline_parameters"] = updated_pipeline_parameters
@@ -467,43 +480,97 @@
                                                                IWUtils.get_default_header_for_v3(
                                                                    self.client_config['bearer_token']), data=api_payload
                                                                ).content)
             result = response.get('result', None)
             if result is None:
                 self.logger.error(f"Failed to initiate {job_type} job for pipeline {pipeline_id}.")
                 return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f"Failed to initiate {job_type} job for pipeline {pipeline_id}.",response=response)
+                                                    error_desc=f"Failed to initiate {job_type} job for pipeline {pipeline_id}.",
+                                                    response=response)
             else:
                 return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             raise JobsError(f"Failed to initiate {job_type} job for pipeline {pipeline_id}." + str(e))
 
-    def cancel_job(self, job_id=None, params=None):
+    def cancel_job(self, job_id=None, role="admin"):
         """
-        Function to cancel an Infoworks Job
+        Function to cancel an Infoworks Job by prodops user
         :param job_id: job_id in Infoworks
         :type job_id: String
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type: JSON dict
+        :param role: can be either admin/prodops
         :return: response dict
         """
         if None in {job_id}:
             self.logger.error("job_id cannot be None")
             raise Exception("job_id cannot be None")
         try:
-            if params is None:
-                params = {"limit": 20, "offset": 0}
             url_to_cancel_job = url_builder.get_cancel_job_url(self.client_config, job_id=job_id)
-            url_to_cancel_job = url_to_cancel_job + IWUtils.get_query_params_string_from_dict(params=params)
-            response = None
+            if role.lower() == "admin":
+                url_to_cancel_job.replace("prodops", "admin")
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_to_cancel_job,
                                                                IWUtils.get_default_header_for_v3(
                                                                    self.client_config['bearer_token'])
                                                                ).content)
             result = response.get("message", "")
             if result != 'Requested Job Cancellation':
                 self.logger.error(f"Failed to cancel job {job_id}.")
                 return GenericResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f"Failed to cancel job {job_id}.",response=response)
+                                                    error_desc=f"Failed to cancel job {job_id}.", response=response)
             return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             raise JobsError(f"Failed to cancel job for job_id {job_id}." + str(e))
+
+    def get_job_details_by_prodops_user(self, job_id=None, params=None):
+        """
+        Function to get the job details by prodops user
+        :param job_id: entity identifier for job
+        :type: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response list of dict
+        """
+        if None in {job_id}:
+            self.logger.error("job_id cannot be None")
+            raise Exception("job_id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+
+        url_to_list_jobs = url_builder.get_jobs_prodops_url(self.client_config)
+        if job_id is not None:
+            url_to_list_jobs = url_to_list_jobs + f"/{job_id}"
+        else:
+            url_to_list_jobs = url_to_list_jobs + IWUtils.get_query_params_string_from_dict(params=params)
+        job_details = []
+
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_list_jobs,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            initial_msg = ""
+            if response is not None:
+                initial_msg = response.get("message", "")
+                result = response.get("result", None)
+                if result is None:
+                    self.logger.error('Failed to get job details')
+                    return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                        error_desc='Failed to get job details',
+                                                        response=response)
+                if job_id is not None:
+                    job_details.extend([result])
+                else:
+                    while len(result) > 0:
+                        job_details.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", [])
+            response["result"] = job_details
+            response["message"] = initial_msg
+            return GenericResponse.parse_result(job_id=job_id, status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in getting job details")
+            raise JobsError("Error in getting job details" + str(e))
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/local_configurations.py` & `infoworkssdk-3.0b0/infoworks/sdk/local_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/pipeline_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from infoworks.sdk.utils import IWUtils
 
 
 class PipelineClient(BaseClient):
     def __init__(self):
         super(PipelineClient, self).__init__()
 
-    def poll_job(self, pipeline_id=None, job_id=None, poll_timeout=local_configurations.POLLING_TIMEOUT,
-                 polling_frequency=local_configurations.POLLING_FREQUENCY_IN_SEC,
-                 retries=local_configurations.NUM_POLLING_RETRIES):
+    def poll_pipeline_job(self, pipeline_id=None, job_id=None, poll_timeout=local_configurations.POLLING_TIMEOUT,
+                          polling_frequency=local_configurations.POLLING_FREQUENCY_IN_SEC,
+                          retries=local_configurations.NUM_POLLING_RETRIES):
         """
         Function to poll the pipeline job
         :param pipeline_id: ID of the pipeline
         :type pipeline_id: String
         :param job_id: job_id of the pipeline
         :type job_id: String
         :param poll_timeout: Polling timeout(default is 1200 seconds).If -1 then till the job completes polling will be done.
@@ -44,31 +44,30 @@
                 job_monitor_url = url_builder.get_job_status_url(self.client_config, job_id)
                 response = IWUtils.ejson_deserialize(self.call_api("GET", job_monitor_url,
                                                                    IWUtils.get_default_header_for_v3(
                                                                        self.client_config['bearer_token'])).content)
                 result = response.get('result', {})
                 if len(result) != 0:
                     job_status = result["status"]
+                    print(f"pipeline_status : {job_status}.Sleeping for {polling_frequency} seconds")
                     self.logger.info(
                         "Job poll status : " + result["status"] + "Job completion percentage: " + str(result.get(
                             "percentage", 0)))
-                    if job_status in ["completed", "failed", "aborted"]:
-                        if job_status == "completed":
-                            return PipelineResponse.parse_result(status=Response.Status.SUCCESS,
-                                                                 pipeline_id=pipeline_id,
-                                                                 job_id=job_id)
-                        else:
-                            return PipelineResponse.parse_result(status=job_status, pipeline_id=pipeline_id,
-                                                                 job_id=job_id)
+                    if job_status in ["completed", "failed", "aborted", "canceled"]:
+                        return PipelineResponse.parse_result(status=Response.Status.SUCCESS,
+                                                             response=response,
+                                                             pipeline_id=pipeline_id,
+                                                             job_id=job_id)
                 else:
                     self.logger.error(f"Error occurred during job {job_id} status poll")
                     if failed_count >= retries - 1:
                         return PipelineResponse.parse_result(status=Response.Status.FAILED,
                                                              error_code=ErrorCode.GENERIC_ERROR,
-                                                             error_desc=f"Error occurred during job {job_id} status poll",response=response, job_id=job_id,
+                                                             error_desc=f"Error occurred during job {job_id} status poll",
+                                                             response=response, job_id=job_id,
                                                              pipeline_id=pipeline_id)
                     failed_count = failed_count + 1
             except Exception as e:
                 self.logger.exception("Error occurred during job status poll")
                 self.logger.info(str(e))
                 if failed_count >= retries - 1:
                     # traceback.print_stack()
@@ -553,15 +552,15 @@
         if len(result) != 0 and "id" in result:
             job_id = result["id"]
             if not poll:
                 self.logger.info(f"Pipeline build job has been submitted for {pipeline_id} with {job_id}")
                 return PipelineResponse.parse_result(status=Response.Status.SUCCESS, job_id=job_id,
                                                      pipeline_id=pipeline_id, response=response)
             else:
-                return self.poll_job(pipeline_id=pipeline_id, job_id=job_id)
+                return self.poll_pipeline_job(pipeline_id=pipeline_id, job_id=job_id)
         else:
             self.logger.error(response)
             raise PipelineError(f"Failed to submit pipeline build job for {pipeline_id} ")
 
     def get_pipeline_id(self, pipeline_name, domain_id=None, domain_name=None):
         """
         Function to get pipeline id
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/pipeline_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/source_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import traceback
-
 from infoworks.error import SourceError
 from infoworks.sdk import url_builder, local_configurations
 from infoworks.sdk.base_client import BaseClient
+from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.local_configurations import Response, ErrorCode, SourceMappings
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.utils import IWUtils
 
 
 class SourceClient(BaseClient):
 
@@ -49,18 +49,19 @@
                 job_monitor_url = url_builder.get_job_status_url(self.client_config, job_id)
                 response = IWUtils.ejson_deserialize(self.call_api("GET", job_monitor_url,
                                                                    IWUtils.get_default_header_for_v3(
                                                                        self.client_config['bearer_token'])).content)
                 result = response.get('result', {})
                 if len(result) != 0:
                     job_status = result["status"]
+                    print(f"source_job_status : {job_status}.Sleeping for {polling_frequency} seconds")
                     self.logger.info(
                         "Job poll status : " + result["status"] + "Job completion percentage: " + str(result.get(
                             "percentage", 0)))
-                    if job_status in ["completed", "failed", "aborted"]:
+                    if job_status.lower() in ["completed", "failed", "aborted", "canceled"]:
                         return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id,
                                                            job_id=job_id, response=response)
                 else:
                     self.logger.error(f"Error occurred during job {job_id} status poll")
                     if failed_count >= retries - 1:
                         return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                            error_code=ErrorCode.GENERIC_ERROR,
@@ -68,15 +69,15 @@
                                                            response=response, job_id=job_id,
                                                            source_id=source_id)
                     failed_count = failed_count + 1
             except Exception as e:
                 self.logger.exception("Error occurred during job status poll")
                 self.logger.info(str(e))
                 if failed_count >= retries - 1:
-                    # traceback.print_stack()
+                    print(traceback.print_stack())
                     print(response)
                     raise SourceError(response.get("message", "Error occurred during job status poll"))
                 failed_count = failed_count + 1
             time.sleep(polling_frequency)
 
         return SourceResponse.parse_result(status=Response.Status.FAILED,
                                            error_code=ErrorCode.POLL_TIMEOUT,
@@ -310,14 +311,20 @@
             if filter_tables_properties is not None:
                 filter_condition = f"?is_filter_enabled=true&tables_filter={filter_tables_properties['tables_filter']}&catalogs_filter={filter_tables_properties['catalogs_filter']}&schemas_filter={filter_tables_properties['schemas_filter']}"
                 url_for_browse_source = url_for_browse_source + filter_condition
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_for_browse_source,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             result = response.get('result', {})
+            if result.get("message","")=="Interactive Cluster is not running. Please bring up cluster and retry":
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.GENERIC_ERROR,
+                                                   error_desc=f"Interactive Cluster is not running. Please bring up cluster and retry",
+                                                   response=response, job_id=None,
+                                                   source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to create browse table job for {source_id} " + str(e))
         if len(result) == 0 and "id" not in result:
             self.logger.error(f"Failed to create browse table job")
             return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                error_code=ErrorCode.GENERIC_ERROR,
                                                error_desc=f"Failed to create browse table job",
@@ -345,15 +352,15 @@
                                       IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
                     result = response.get('result', {})
                     if len(result) == 0:
                         self.logger.error(f"Failed to poll interactive job {job_id}")
                         job_status = None
                     else:
                         job_status = result["status"]
-                    self.logger.info("Browse source job poll status : " + job_status)
+                    self.logger.info(f"Browse source job poll status : {job_status}" )
                     if job_status in ["completed", "failed", "aborted"]:
                         break
                     if job_status is None:
                         self.logger.info(f"Error occurred during job {job_id} status poll")
                         if failed_count >= retries - 1:
                             return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                                error_code=ErrorCode.GENERIC_ERROR,
@@ -421,15 +428,15 @@
                 self.logger.info(f"Added the below table Ids to the source {source_id}")
                 self.logger.info(result["added_tables"])
                 self.logger.info(response["message"])
                 self.logger.info(f"Triggered metacrawl job for tables. Infoworks JobID {result['job_created']}")
                 job_id = result['job_created']
                 if not poll:
                     self.logger.info(f"Tables added to source {source_id} and metacrawl job was submitted {job_id}")
-                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS)
                 else:
                     return self.poll_job(source_id=source_id, job_id=job_id, poll_timeout=poll_timeout,
                                          polling_frequency=polling_frequency,
                                          retries=retries)
             else:
                 self.logger.error(f"Failed to add the tables to the source {source_id}")
                 self.logger.debug(response)
@@ -581,15 +588,15 @@
                                                    error_code=ErrorCode.GENERIC_ERROR,
                                                    error_desc="Failed to create table groups",
                                                    response=response, job_id=None,
                                                    source_id=source_id)
         except Exception as e:
             raise SourceError(f"Failed to update table group" + str(e))
 
-    def get_list_of_table_groups(self, source_id=None, params=None, tg_id=None):
+    def get_table_group_details(self, source_id=None, params=None, tg_id=None):
         """
         Function to list the table groups under source
         :param source_id: entity identifier for source
         :type source_id: String
         :param tg_id: id of table group config to fetch
         :type tg_id: String
         :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
@@ -671,20 +678,22 @@
         except Exception as e:
             self.logger.error("Error in deleting the table group")
             raise SourceError("Error in deleting table group" + str(e))
 
     def submit_source_job(self, source_id=None, body=None, poll=False, poll_timeout=300, polling_frequency=15,
                           retries=3):
         """
-        Function to trigger the jobs related to source
+        Initiates jobs for source and its artifacts.
+        The job types that can be submitted are export_data, streaming_start, segmentation_load, truncate_reload, cdc_merge, truncate_table, source_test_connection, source_fetch_metadata, table_fetch_metadata.
         :param source_id: source entity id
         :type source_id: String
         :param body: JSON body containing type of job to trigger
         :type body: JSON dict
 
+
         metadata_job_body_example = {
                 "job_type": "source_fetch_metadata",
                 "overwrite": true
             }
 
         ingest_table_body_example = {
             "job_type": "cdc_merge" or "truncate_reload",
@@ -786,15 +795,14 @@
         url_to_list_sources = url_builder.list_sources_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
         source_list = []
         try:
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_sources,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            initial_msg = ""
             if response is not None:
                 initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 while len(result) > 0:
                     source_list.extend(result)
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
@@ -802,17 +810,17 @@
                                                                       protocol=self.client_config['protocol'],
                                                                       )
                     response = IWUtils.ejson_deserialize(
                         self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
                             self.client_config['bearer_token'])).content)
                     result = response.get("result", [])
             else:
-                self.logger.error("Failed to submit get list of sources")
+                self.logger.error("Failed to get list of sources")
                 return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
-                                                   error_desc="Failed to submit get list of sources", response=response)
+                                                   error_desc="Failed to get list of sources", response=response)
             response["result"] = source_list
             response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
 
         except Exception as e:
             self.logger.error("Error in listing sources")
             raise SourceError("Error in listing sources " + str(e))
@@ -1116,14 +1124,15 @@
         tables_list = []
         try:
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_tables,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             if response is not None:
                 result = response.get("result", [])
+                initial_msg = response.get("message", "")
                 while len(result) > 0:
                     tables_list.extend(result)
                     nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
                                                                       ip=self.client_config['ip'],
                                                                       port=self.client_config['port'],
                                                                       protocol=self.client_config['protocol'],
                                                                       )
@@ -1135,15 +1144,15 @@
                         return SourceResponse.parse_result(status=Response.Status.FAILED,
                                                            error_code=ErrorCode.GENERIC_ERROR,
                                                            error_desc="Error in listing tables under the source",
                                                            response=response
                                                            )
 
                 response["result"] = tables_list
-
+                response["message"] = initial_msg
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error("Error in listing tables under source")
             raise SourceError("Error in listing tables under source" + str(e))
 
     def get_table_columns_details(self, source_id=None, table_name=None, schema_name=None, database_name=None):
         """
@@ -1562,17 +1571,15 @@
         url_to_list_sources = url_builder.list_sources_url(
             self.client_config) + IWUtils.get_query_params_string_from_dict(params=params)
         try:
 
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_to_list_sources,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            initial_msg = ""
             if response is not None:
-                initial_msg = response.get("message", "")
                 result = response.get("result", [])
                 if len(result) > 0:
                     return SourceResponse.parse_result(status=Response.Status.SUCCESS, response={"id": result[0]["id"]})
                 else:
                     raise Exception("Could not get the source details")
         except Exception as e:
             self.logger.error("Error in listing sources")
@@ -1690,30 +1697,30 @@
         else:
             self.logger.error(f"Failed to create source {src_name}", src_create_response)
             raise Exception(f"Failed to create source  {src_name}", src_create_response)
 
     def configure_table_ingestion_properties(self, source_id=None, table_id=None, natural_keys=None,
                                              sync_type="full-load",
                                              update_strategy=None,
-                                             watermark_column=None, partition_key=None, derived_partition=False,
+                                             watermark_columns=None, partition_key=None, derived_partition=False,
                                              derive_partition_format=None, split_by_key=None, storage_format=None):
         """
         Function to configure the ingestion configs of table
         :param source_id: Entity identifier for source
         :type source_id: String
         :param table_id: table entity id
         :type table_id: String
         :param natural_keys: natural keys List
         :type natural_keys: List
         :param sync_type: full-load/incremental
         :type sync_type: String
         :param update_strategy: append/merge
         :type update_strategy: String
-        :param watermark_column: Watermark column to be used during incremental ingestion
-        :type watermark_column: String
+        :param watermark_columns: Watermark columns to be used during incremental ingestion
+        :type watermark_columns: Array
         :param partition_key: Partition by Column
         :type partition_key: String
         :param derived_partition: True/False. If True pass the derive_partition_format
         :type derived_partition: Boolean
         :param derive_partition_format: Derived partition format. Choose one from ['dd', 'MM', 'yyyy', 'yyyyMM', 'MMdd', 'yyyyMMdd']
         :type derive_partition_format: String
         :param split_by_key: Split by Column
@@ -1733,23 +1740,23 @@
                 self.logger.error("Table id for this method cannot be None")
             if source_id is None:
                 self.logger.error("Source id for this method cannot be None")
             if natural_keys != []:
                 table_config_body['natural_keys'] = natural_keys
             if sync_type in ['full-load', 'incremental']:
                 table_config_body["sync_type"] = "full-load"
-                if update_strategy in ["append", "merge"] and watermark_column is not None:
+                if update_strategy in ["append", "merge"] and watermark_columns is not None:
                     if update_strategy == "append":
                         table_config_body["sync_type"] = "incremental"
                         table_config_body["update_strategy"] = "append"
-                        table_config_body["watermark_column"] = watermark_column
-                    elif update_strategy == "merge" and watermark_column is not None:
+                        table_config_body["watermark_columns"] = watermark_columns
+                    elif update_strategy == "merge" and watermark_columns is not None:
                         table_config_body["sync_type"] = "incremental"
                         table_config_body["update_strategy"] = "merge"
-                        table_config_body["watermark_column"] = watermark_column
+                        table_config_body["watermark_columns"] = watermark_columns
             if partition_key:
                 if not derived_partition:
                     table_config_body["partition_keys"] = [{
                         "partition_column": partition_key,
                         "is_derived_partition": False}]
                 else:
                     allowed_values_for_date_partition = ['dd', 'MM', 'yyyy', 'yyyyMM', 'MMdd', 'yyyyMMdd']
@@ -1949,19 +1956,167 @@
                     result = response.get("result", [])
             else:
                 self.logger.error("Failed to get list of tables")
                 return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                    error_desc="Failed to submit get list of tables", response=response)
             response["result"] = tables_list
             response["message"] = initial_msg
-            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
         except Exception as e:
             self.logger.error(f"Failed to get the tables under {source_id} " + str(e))
             raise SourceError(f"Failed to get the tables under {source_id} " + str(e))
 
+    def get_source_metadata(self, source_id=None):
+        """
+        Function to get source metadata (like tags,description etc)
+        :param source_id: Entity identifier for table
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id}:
+            self.logger.error("source id cannot be None")
+            raise Exception("source id cannot be None")
+        try:
+            source_configurations_url = url_builder.get_source_details_url(self.client_config)
+            source_configurations_url = source_configurations_url + f"/{source_id}/metadata"
+            response = IWUtils.ejson_deserialize(self.call_api("GET", source_configurations_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the table metadata for {source_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the table metadata for {source_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the table metadata for {source_id} " + str(e))
+
+    def update_source_metadata(self, source_id, tags_to_add: str = None, tags_to_remove: str = None,
+                               description: str = None, is_favorite=False, data=None):
+        """
+        Function to update source metadata (like tags,description etc)
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param tags_to_add: Pass comma seperated tags to add. Optional field
+        :param tags_to_remove: Pass comma seperated tags to remove. Optional field
+        :param description: Pass the description of the tag
+        :param is_favorite: Boolean. True/False
+        :param data : Json body to update source metadata. You can pass only this param if the body of API is known. Else pass other individual params
+        :type data: JSON dict
+        :return: response dict
+        """
+        if None in {source_id}:
+            self.logger.error("source id cannot be None")
+            raise Exception("source id cannot be None")
+        try:
+            if data is None:
+                data = {
+                    "tags_to_add": [] if tags_to_add is None else tags_to_add.split(","),
+                    "tags_to_remove": [] if tags_to_remove is None else tags_to_remove.split(","),
+                    "is_favorite": is_favorite,
+                    "description": "" if description is None else description
+                }
+            source_configurations_url = url_builder.get_source_details_url(self.client_config)
+            source_configurations_url = source_configurations_url + f"/{source_id}/metadata"
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", source_configurations_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), data=data
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to update the source metadata for {source_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the source metadata for {source_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to update the source metadata for {source_id} " + str(e))
+
+    def get_table_metadata(self, source_id=None, table_id=None):
+        """
+        Function to get table metadata (like tags,description etc)
+        :param table_id: Entity identifier for table
+        :type table_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, table_id}:
+            self.logger.error("source id or table_id cannot be None")
+            raise Exception("source id or table_id cannot be None")
+        try:
+            table_configurations_url = url_builder.get_table_configuration(self.client_config, source_id, table_id)
+            table_configurations_url = table_configurations_url + "/metadata"
+            response = IWUtils.ejson_deserialize(self.call_api("GET", table_configurations_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the table metadata for {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the table metadata for {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the table metadata for {table_id} " + str(e))
+
+    def update_table_metadata(self, source_id, table_id, tags_to_add: str = None, tags_to_remove: str = None,
+                              description: str = None, is_favorite=False, data=None):
+        """
+        Function to update table metadata (like tags,description etc)
+        :param table_id: Entity identifier for table
+        :type table_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param tags_to_add: Pass comma seperated tags to add. Optional field
+        :param tags_to_remove: Pass comma seperated tags to remove. Optional field
+        :param description: Pass the description of the tag
+        :param is_favorite: Boolean. True/False
+        :param data : Json body to update source metadata. You can pass only this param if the body of API is known. Else pass other individual params
+        :type data: JSON dict
+        :return: response dict
+        """
+        if None in {source_id, table_id}:
+            self.logger.error("source id or table_id cannot be None")
+            raise Exception("source id or table_id cannot be None")
+        try:
+            if data is None:
+                data = {
+                    "tags_to_add": [] if tags_to_add is None else tags_to_add.split(","),
+                    "tags_to_remove": [] if tags_to_remove is None else tags_to_remove.split(","),
+                    "is_favorite": is_favorite,
+                    "description": "" if description is None else description
+                }
+            table_configurations_url = url_builder.get_table_configuration(self.client_config, source_id, table_id)
+            table_configurations_url = table_configurations_url + "/metadata"
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", table_configurations_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), data=data
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the table metadata for {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the table metadata for {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the table metadata for {table_id} " + str(e))
+
     def create_query_as_table(self, source_id, tables_to_add_body: list):
         """
         Function to create query as table under source
         :param source_id: Entity identifier for source
         :type source_id: String
         :param tables_to_add_body: Pass the body required to create query as a table
         :type: array of dict
@@ -1982,7 +2137,870 @@
                     return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
                                                        error_desc="Could not create query as table",
                                                        response=response)
             return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
         except Exception as e:
             self.logger.error(f"Unable to create query as a table under {source_id} " + str(e))
             raise SourceError(f"Unable to create query as a table under {source_id} " + str(e))
+
+    def get_table_schema(self, source_id=None, table_id=None):
+        """
+        Function to get table schema
+        :param table_id: Entity identifier for table
+        :type table_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, table_id}:
+            self.logger.error("source id or table_id cannot be None")
+            raise Exception("source id or table_id cannot be None")
+        try:
+            table_schema_url = url_builder.source_table_schema_url(self.client_config, source_id, table_id)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", table_schema_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the table schema for {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the table schema for {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the table schema for {table_id} " + str(e))
+
+    def update_table_schema(self, source_id=None, table_id=None, config_body=None):
+        """
+        Function to update the table schema
+        :param table_id: Entity identifier for table
+        :type table_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param config_body: JSON body
+        config_body_example: {
+            "type" : "column",
+            "columns": [
+                    {
+                        "is_deleted": false,
+                        "name": "STATE_ID",
+                        "original_name": "STATE_ID",
+                        "target_sql_type": 12,
+                        "target_scale": 0,
+                        "col_size": 11,
+                        "target_precision": 10
+                    }
+            ]
+        }
+        :return: response dict
+        """
+        if None in {source_id, table_id} or config_body is None:
+            self.logger.error("source id or table_id or config_body cannot be None")
+            raise Exception("source id or table_id or config_body cannot be None")
+        try:
+            table_schema_url = url_builder.source_table_schema_url(self.client_config, source_id, table_id)
+            response = IWUtils.ejson_deserialize(self.call_api("PATCH", table_schema_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), data=config_body
+                                                               ).content)
+            result = response.get('result', {})
+            if "id" not in result:
+                self.logger.error(f"Failed to update the table schema for {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to update the table schema for {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to update the table schema for {table_id} " + str(e))
+
+    def get_file_mappings_for_json_source(self, source_id=None, file_mapping_id=None, file_mapping_name=None,
+                                          params=None):
+        """
+        Function to get file mappings
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param file_mapping_id: Entity identifier of the file mapping
+        :param file_mapping_name: Name of the file mapping for which details are to be fetched
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :return: response dict
+        """
+        if None in {source_id}:
+            self.logger.error("source id cannot be None")
+            raise Exception("source id cannot be None")
+
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+
+        try:
+            if file_mapping_id is None:
+                if file_mapping_name is not None:
+                    params = {"filter": {"name": file_mapping_name}}
+                file_mappings_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                      source_id) + IWUtils.get_query_params_string_from_dict(
+                    params=params)
+                file_mappings_list = []
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("GET", file_mappings_url,
+                                  IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+                if response is not None:
+                    initial_msg = response.get("message", "")
+                    result = response.get("result", [])
+                    while len(result) > 0:
+                        file_mappings_list.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", [])
+                else:
+                    self.logger.error("Failed to get list of file mappings")
+                    return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                       error_desc="Failed to get list of file mappings",
+                                                       response=response)
+                response["result"] = file_mappings_list
+                response["message"] = initial_msg
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+            else:
+                file_mappings_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                      source_id) + f"/{file_mapping_id}"
+                response = IWUtils.ejson_deserialize(self.call_api("GET", file_mappings_url,
+                                                                   IWUtils.get_default_header_for_v3(
+                                                                       self.client_config['bearer_token']),
+                                                                   ).content)
+                result = response.get('result', False)
+                if not result:
+                    self.logger.error(f"Failed to get file mappings")
+                    return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                       error_desc=f"Failed to get file mappings",
+                                                       response=response, job_id=None, source_id=source_id)
+                else:
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                       source_id=source_id)
+        except Exception as e:
+            self.logger.error("Error in getting file mappings")
+            raise SourceError("Error in getting file mappings " + str(e))
+
+    def modify_file_mappings_for_json_source(self, source_id=None, config_body=None, action_type="create",
+                                             file_mappings_id=None):
+        """
+        Function to create file mappings
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param file_mappings_id: Entity identifier of the file mapping. Pass this incase you want to update the file mapping
+        :param action_type: create/update
+        :param config_body: JSON dict with necessary keys
+        config_body_example =
+            {       "name" :"xyz",
+                "source_relative_path": "/test",
+                "record_scope": "file",
+                "include_subdirectories": true,
+                "character_encoding": "UTF-8",
+                "include_filename_regex": ".*",
+                "exclude_filename_regex": ""
+            }
+        :return: response dict
+        """
+        if None in {source_id} or config_body is None:
+            self.logger.error("source id or config_body cannot be None")
+            raise Exception("source id or config_body cannot be None")
+        try:
+            if action_type.lower() == "create":
+                request_type = "POST"
+                file_mappings_url = url_builder.get_file_mappings_for_json_source_url(self.client_config, source_id)
+            else:
+                request_type = "PATCH"
+                file_mappings_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                      source_id) + f"/{file_mappings_id}"
+
+            response = IWUtils.ejson_deserialize(self.call_api(request_type, file_mappings_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               data=config_body).content)
+            result = response.get('result', {})
+            message = response.get('message', "")
+            created_file_mapping_id = result.get('id', None)
+            if created_file_mapping_id is not None:
+                adv_config_id = str(created_file_mapping_id)
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+            elif message == "Updated File mappings":
+                self.logger.info('File Mappings has been updated')
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+            else:
+                self.logger.error(f'Failed to {action_type} file mappings')
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f'Failed to {action_type} file mappings',
+                                                   response=response)
+        except Exception as e:
+            raise SourceError(f"Failed to {action_type} the file mappings for {source_id} " + str(e))
+
+    def delete_file_mappings_for_json_source(self, source_id=None, file_mapping_id=None):
+        """
+        Function to get table schema
+        :param file_mapping_id: Entity identifier of the file mapping
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, file_mapping_id}:
+            self.logger.error("source id or file_mapping_id cannot be None")
+            raise Exception("source id or file_mapping_id cannot be None")
+        try:
+            file_mappings_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                  source_id) + f"/{file_mapping_id}"
+            response = IWUtils.ejson_deserialize(self.call_api("DELETE", file_mappings_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get("result", None)
+            if result is None:
+                self.logger.error(f"Failed to delete the file mappings for {file_mapping_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to delete the file mappings for {file_mapping_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to delete the file mappings for {file_mapping_id} " + str(e))
+
+    def crawl_schema_for_file_mapping_json_source(self, source_id=None, file_mapping_id=None):
+        """
+        Function to get table schema
+        :param file_mapping_id: Entity identifier for file mapping
+        :type file_mapping_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, file_mapping_id}:
+            self.logger.error("source id or file_mapping_id cannot be None")
+            raise Exception("source id or file_mapping_id cannot be None")
+        try:
+            crawl_schema_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                 source_id) + f"/{file_mapping_id}/crawl-schema"
+            response = IWUtils.ejson_deserialize(self.call_api("GET", crawl_schema_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the crawl schema for file mapping {file_mapping_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the crawl schema for file mapping {file_mapping_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the crawl schema for file mapping {file_mapping_id} " + str(e))
+
+    def get_table_schema_from_file_mapping_json_source(self, source_id=None, file_mapping_id=None):
+        """
+        Function to get table schema
+        :param file_mapping_id: Entity identifier for file mapping
+        :type file_mapping_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, file_mapping_id}:
+            self.logger.error("source id or file_mapping_id cannot be None")
+            raise Exception("source id or file_mapping_id cannot be None")
+        try:
+            table_schema_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                 source_id) + f"/{file_mapping_id}/table-schema"
+            response = IWUtils.ejson_deserialize(self.call_api("GET", table_schema_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the table schema from file mapping {file_mapping_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the table schema from file mapping {file_mapping_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the table schema from file mapping {file_mapping_id} " + str(e))
+
+    def create_json_source_table(self, source_id=None, file_mapping_id=None):
+        """
+        Function to create Infoworks JSON Source Table
+        :param file_mapping_id: Entity identifier for file mapping
+        :type file_mapping_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        response = None
+        if None in {source_id, file_mapping_id}:
+            self.logger.error("source id or file_mapping_id cannot be None")
+            raise Exception("source id or file_mapping_id cannot be None")
+        try:
+            table_create_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                 source_id) + f"/{file_mapping_id}/tables"
+            response = IWUtils.ejson_deserialize(
+                self.call_api("POST", table_create_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                              "").content)
+
+            result = response.get('result', {})
+            table_id = result.get('id', None)
+            if table_id is None:
+                self.logger.error('Table creation failed')
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_desc='Table creation failed',
+                                                   response=response)
+
+            table_id = str(table_id)
+            self.logger.info('Table {id} has been created.'.format(id=table_id))
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, source_id=source_id, response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(response))
+            self.logger.exception('Error occurred while trying to create a json table.')
+            raise SourceError(response.get("message", "Error occurred while trying to create a json table."))
+
+    def get_json_source_table(self, source_id=None, file_mapping_id=None, table_id=None, params=None):
+        """
+        Function to get json source table details
+        :param file_mapping_id: Entity identifier for file mapping
+        :type file_mapping_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param table_id: Entity identifier for table
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :return: response dict
+        """
+        if None in {source_id, file_mapping_id}:
+            self.logger.error("source id or file_mapping_id cannot be None")
+            raise Exception("source id or file_mapping_id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        try:
+            if table_id is None:
+                get_json_src_tbls_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                          source_id) + IWUtils.get_query_params_string_from_dict(
+                    params=params)
+                tables_list = []
+                response = IWUtils.ejson_deserialize(
+                    self.call_api("GET", get_json_src_tbls_url,
+                                  IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+                if response is not None:
+                    initial_msg = response.get("message", "")
+                    result = response.get("result", [])
+                    while len(result) > 0:
+                        tables_list.extend(result)
+                        nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                          ip=self.client_config['ip'],
+                                                                          port=self.client_config['port'],
+                                                                          protocol=self.client_config['protocol'],
+                                                                          )
+                        response = IWUtils.ejson_deserialize(
+                            self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                                self.client_config['bearer_token'])).content)
+                        result = response.get("result", [])
+                else:
+                    self.logger.error("Failed to get list of json source tables")
+                    return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                       error_desc="Failed to get list of json source tables",
+                                                       response=response)
+                response["result"] = tables_list
+                response["message"] = initial_msg
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+
+            else:
+                get_json_src_tbl_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                         source_id) + f"/{file_mapping_id}/tables/{table_id}"
+                response = IWUtils.ejson_deserialize(self.call_api("GET", get_json_src_tbl_url,
+                                                                   IWUtils.get_default_header_for_v3(
+                                                                       self.client_config['bearer_token']),
+                                                                   ).content)
+                result = response.get('result', False)
+                if not result:
+                    self.logger.error(f"Failed to get the table details for {table_id}")
+                    return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                       error_desc=f"Failed to get the table details for {table_id}",
+                                                       response=response, job_id=None, source_id=source_id)
+                else:
+                    return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                       source_id=source_id)
+        except Exception as e:
+            self.logger.error(f"Failed to get the table details for {table_id} " + str(e))
+            raise SourceError(f"Failed to get the table details for {table_id} " + str(e))
+
+    def delete_json_source_table(self, source_id=None, file_mapping_id=None, table_id=None):
+        """
+        Function to delete json source table
+        :param file_mapping_id: Entity identifier for file mapping
+        :type file_mapping_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param table_id: Entity identifier for table
+        :return: response dict
+        """
+        if None in {source_id, file_mapping_id, table_id}:
+            self.logger.error("source id or file_mapping_id or table_id cannot be None")
+            raise Exception("source id or file_mapping_id or table_id cannot be None")
+        try:
+            get_json_src_tbl_url = url_builder.get_file_mappings_for_json_source_url(self.client_config,
+                                                                                     source_id) + f"/{file_mapping_id}/tables/{table_id}"
+            response = IWUtils.ejson_deserialize(self.call_api("DELETE", get_json_src_tbl_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            message = response.get('message', "")
+            if message != "Table Deleted Successfully":
+                self.logger.error(f"Failed to delete the json source table {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to delete the json source table {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to delete the json source table {table_id} " + str(e))
+
+    def get_source_audit_logs(self, source_id=None, params=None):
+        """
+        Function to get audit logs of source
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response dict
+        """
+        audit_logs = []
+        if None in {source_id}:
+            self.logger.error("source id cannot be None")
+            raise Exception("source id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        try:
+            src_audit_logs_url = url_builder.get_source_audit_logs_url(self.client_config, source_id)
+            src_audit_logs_url = src_audit_logs_url + IWUtils.get_query_params_string_from_dict(params=params)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", src_audit_logs_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            initial_msg = response.get("message", "")
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    audit_logs.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+            else:
+                self.logger.error("Failed to get audit logs of source")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc="Failed to get audit logs of source", response=response)
+            response["result"] = audit_logs
+            response["message"] = initial_msg
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
+        except Exception as e:
+            self.logger.error(f"Failed to get the audit logs of {source_id} " + str(e))
+            raise SourceError(f"Failed to get the audit logs of {source_id} " + str(e))
+
+    def get_table_audit_logs(self, source_id=None, table_id=None, params=None):
+        """
+        Function to get audit logs of source
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param table_id: Entity identifier of table
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response dict
+        """
+        audit_logs = []
+        if None in {source_id, table_id}:
+            self.logger.error("source id or table_id cannot be None")
+            raise Exception("source id or table_id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        try:
+            tbl_audit_logs_url = url_builder.get_table_audit_logs_url(self.client_config, source_id, table_id)
+            tbl_audit_logs_url = tbl_audit_logs_url + IWUtils.get_query_params_string_from_dict(params=params)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", tbl_audit_logs_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            initial_msg = response.get("message", "")
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    audit_logs.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+            else:
+                self.logger.error("Failed to get audit logs of table")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc="Failed to get audit logs of table", response=response)
+            response["result"] = audit_logs
+            response["message"] = initial_msg
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
+        except Exception as e:
+            self.logger.error(f"Failed to get the audit logs of table {table_id} " + str(e))
+            raise SourceError(f"Failed to get the audit logs of table {table_id} " + str(e))
+
+    def get_tablegroup_audit_logs(self, source_id=None, table_group_id=None, params=None):
+        """
+        Function to get audit logs of source
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param table_group_id: Entity identifier of table group
+        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+        :type: JSON dict
+        :return: response dict
+        """
+        audit_logs = []
+        if None in {source_id, table_group_id}:
+            self.logger.error("source id or table_group_id cannot be None")
+            raise Exception("source id or table_group_id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        try:
+            tblgrp_audit_logs_url = url_builder.get_table_group_audit_logs_url(self.client_config, source_id,
+                                                                               table_group_id)
+            tblgrp_audit_logs_url = tblgrp_audit_logs_url + IWUtils.get_query_params_string_from_dict(params=params)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", tblgrp_audit_logs_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            initial_msg = response.get("message", "")
+            if response is not None:
+                result = response.get("result", [])
+                while len(result) > 0:
+                    audit_logs.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", [])
+            else:
+                self.logger.error("Failed to get audit logs of table group")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc="Failed to get audit logs of table group",
+                                                   response=response)
+            response["result"] = audit_logs
+            response["message"] = initial_msg
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response, source_id=source_id)
+        except Exception as e:
+            self.logger.error(f"Failed to get the audit logs of table group {table_group_id} " + str(e))
+            raise SourceError(f"Failed to get the audit logs of table group {table_group_id} " + str(e))
+
+    def get_list_of_advanced_config_of_table(self, source_id, table_id, params=None):
+        """
+            Function to get list of Advance Config of the table
+            :param source_id: Entity identifier of the source
+            :param table_id: Entity identifier of the table
+            :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
+            :type: JSON dict
+            :return: response dict
+        """
+        if None in {source_id, table_id}:
+            raise Exception(f"source_id, table_id cannot be None")
+        if params is None:
+            params = {"limit": 20, "offset": 0}
+        url_to_get_table_adv_config = url_builder.table_advanced_base_url(self.client_config, source_id,
+                                                                          table_id) + IWUtils.get_query_params_string_from_dict(
+            params=params)
+        adv_config_list = []
+        try:
+            response = IWUtils.ejson_deserialize(
+                self.call_api("GET", url_to_get_table_adv_config,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
+            if response is not None:
+                result = response.get("result", [])
+                initial_msg = response.get("message", "")
+                while len(result) > 0:
+                    adv_config_list.extend(result)
+                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
+                                                                      ip=self.client_config['ip'],
+                                                                      port=self.client_config['port'],
+                                                                      protocol=self.client_config['protocol'],
+                                                                      )
+                    response = IWUtils.ejson_deserialize(
+                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
+                            self.client_config['bearer_token'])).content)
+                    result = response.get("result", None)
+                    if result is None:
+                        return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                           error_code=ErrorCode.GENERIC_ERROR,
+                                                           error_desc="Error in listing adv config of table",
+                                                           response=response
+                                                           )
+
+                response["result"] = adv_config_list
+                response["message"] = initial_msg
+            return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+        except Exception as e:
+            self.logger.error("Error in listing adv config of table")
+            raise SourceError("Error in listing adv config of table" + str(e))
+
+    def modify_advanced_config_of_table(self, source_id, table_id, adv_config_body,
+                                        action_type="update", key=None):
+        """
+        Function to add/update the adv config for the pipeline group
+        :param source_id: Entity identifier of the source
+        :param table_id: Entity identifier of the table
+        :param action_type: values can be either create/update. default update
+        :type action_type: String
+        :param adv_config_body: JSON dict
+        adv_config_body_example = {
+            "key" : "",
+            "value": "",
+            "description": "",
+            "is_active": True
+            }
+        :param key: In case of update, name of the adv config to update
+        :return: response dict
+        """
+        if None in {source_id, table_id} or adv_config_body is None:
+            raise Exception(f"source_id, table_id and adv_config_body cannot be None")
+        try:
+            if action_type.lower() == "create":
+                request_type = "POST"
+                request_url = url_builder.table_advanced_base_url(self.client_config, source_id,
+                                                                  table_id)
+            else:
+                request_type = "PUT"
+                request_url = url_builder.table_advanced_base_url(self.client_config, source_id,
+                                                                  table_id) + f"{key}"
+            response = IWUtils.ejson_deserialize(
+                self.call_api(request_type, request_url,
+                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
+                              adv_config_body).content)
+            result = response.get('result', {})
+            message = response.get('message', "")
+            adv_config_id = result.get('id', None)
+            if adv_config_id is not None:
+                adv_config_id = str(adv_config_id)
+                self.logger.info(
+                    'Advanced Config has been created {id}.'.format(id=adv_config_id))
+                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=adv_config_id,
+                                                    response=response)
+            elif message == "Successfully updated Advance configuration":
+                self.logger.info('Advanced Config has been updated')
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response)
+            else:
+                self.logger.error(f'Failed to {action_type} advanced config for pipeline group.')
+                return SourceResponse.parse_result(status=Response.Status.FAILED,
+                                                   error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f'Failed to {action_type} advanced config for table',
+                                                   response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(e))
+            self.logger.exception('Error occurred while trying to add/update adv config for table')
+            raise SourceError('Error occurred while trying to add/update adv config for table')
+
+    def get_or_delete_advance_config_of_table(self, source_id, table_id, key,
+                                              action_type="get"):
+        """
+        Gets/Deletes advance configuration of pipeline group
+        :param source_id: Entity identifier of the source
+        :param table_id: Entity identifier of the table
+        :param key: name of the advanced configuration
+        :param action_type: values can be get/delete
+        :return: response dict
+        """
+        try:
+            if None in {source_id, table_id, key}:
+                raise Exception(f"source_id, table_id, key cannot be None")
+            request_type = "GET" if action_type.lower() == "get" else "DELETE"
+            response = IWUtils.ejson_deserialize(
+                self.call_api(request_type, url_builder.table_advanced_base_url(
+                    self.client_config, source_id, table_id) + f"{key}", IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+            result = response.get('result', {})
+            message = response.get("message", "")
+            if action_type.lower() == "delete" and message == "Successfully removed Advance configuration":
+                self.logger.info(
+                    'Successfully deleted the advanced config')
+                return GenericResponse.parse_result(status=Response.Status.SUCCESS,
+                                                    response=response)
+
+            if result.get('entity_id', None) is None:
+                self.logger.error('Failed to find the advance config details')
+                return GenericResponse.parse_result(status=Response.Status.FAILED,
+                                                    error_code=ErrorCode.USER_ERROR,
+                                                    error_desc='Failed to find the advance config details',
+                                                    response=response)
+
+            self.logger.info(
+                'Successfully got the advanced config details.')
+            return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=result.get('entity_id', ''),
+                                                response=response)
+
+        except Exception as e:
+            self.logger.error('Response from server: ' + str(e))
+            self.logger.exception('Error occurred while trying to get/delete adv config details.')
+            raise SourceError('Error occurred while trying to get/delete adv config details.')
+
+    def update_table_configurations(self, source_id=None, table_id=None, config_body=None):
+        """
+        Function to update the table configurations including columns and ingestion configurations
+        :param table_id: Entity identifier for table
+        :type table_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :param config_body: JSON body
+        config_body_example: {
+            "id": "9376bf97a286e35efe86d321",
+            "name": "dim_state",
+            "original_table_name": "dim_state",
+            "data_lake_path": "/iw/sources/customer_360_sql_server_schema/9376bf97a286e35efe86d321",
+            "meta_crawl_performed": true,
+            "columns": [
+                {
+                    "sql_type": 4,
+                    "is_deleted": false,
+                    "name": "STATE_ID",
+                    "original_name": "STATE_ID",
+                    "target_sql_type": 12,
+                    "is_audit_column": false,
+                    "col_size": 11,
+                    "precision": 10,
+                    "target_precision": 10,
+                    "scale": 0
+                },
+                {
+                    "sql_type": 93,
+                    "is_deleted": false,
+                    "name": "ziw_target_timestamp",
+                    "original_name": "ziw_target_timestamp",
+                    "target_sql_type": 93,
+                    "is_audit_column": true,
+                    "target_scale": "6",
+                    "precision": 0,
+                    "target_precision": "0",
+                    "scale": 6,
+                    "format": "yyyy-MM-dd HH:mm:ss"
+                },
+                {
+                    "sql_type": 16,
+                    "is_deleted": false,
+                    "name": "ziw_is_deleted",
+                    "original_name": "ziw_is_deleted",
+                    "target_sql_type": 16,
+                    "is_audit_column": true,
+                    "target_scale": "0",
+                    "precision": 0,
+                    "target_precision": "0",
+                    "scale": 0
+                }
+            ],
+            "configuration": {
+                "exclude_legacy_audit_columns": true,
+                "sync_type": "full-load",
+                "write_supported_engines": [
+                    "SNOWFLAKE",
+                    "SPARK"
+                ],
+                "read_supported_engines": [
+                    "SNOWFLAKE",
+                    "SPARK"
+                ],
+                "target_table_name": "DIM_STATE",
+                "storage_format": "delta",
+                "target_schema_name": "CUSTOMER_360",
+                "is_table_case_sensitive": false,
+                "is_schema_case_sensitive": false,
+                "target_database_name": "CUSTOMER_360",
+                "is_database_case_sensitive": false,
+                "is_scd2_table": false,
+                "is_archive_enabled": false,
+                "natural_keys": [],
+                "generate_history_view": false,
+                "segmented_load_columns": [],
+                "segmentation_status": "disabled"
+            },
+            "source": "1f9dd7b2bc9f656a4743f458",
+            "last_ingested_cdc_value": null,
+            "is_jtds_driver": false,
+            "schema_name_at_source": "dbo",
+            "catalog_name": "customer_360",
+            "catalog_is_database": true,
+            "has_catalog": true
+        }
+        :return: response dict
+        """
+        if None in {source_id, table_id} or config_body is None:
+            self.logger.error("source id or table_id or config_body cannot be None")
+            raise Exception("source id or table_id or config_body cannot be None")
+        try:
+            table_config_url = url_builder.get_table_configuration(self.client_config, source_id, table_id)
+            response = IWUtils.ejson_deserialize(self.call_api("PUT", table_config_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']), data=config_body
+                                                               ).content)
+            result = response.get('result', {})
+            if "id" not in result:
+                self.logger.error(f"Failed to update the table configurations for {table_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to update the table configurations for {table_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to update the table configurations for {table_id} " + str(e))
+
+    def get_source_job_details(self, source_id=None, job_id=None):
+        """
+        Function to get the source job details
+        :param job_id: Entity identifier for the job
+        :type job_id: String
+        :param source_id: Entity identifier for source
+        :type source_id: String
+        :return: response dict
+        """
+        if None in {source_id, job_id}:
+            self.logger.error("source id or job_id cannot be None")
+            raise Exception("source id or job_id cannot be None")
+        try:
+            source_job_url = url_builder.get_source_job_url(self.client_config, source_id, job_id)
+            response = IWUtils.ejson_deserialize(self.call_api("GET", source_job_url,
+                                                               IWUtils.get_default_header_for_v3(
+                                                                   self.client_config['bearer_token']),
+                                                               ).content)
+            result = response.get('result', False)
+            if not result:
+                self.logger.error(f"Failed to get the job details for {job_id}")
+                return SourceResponse.parse_result(status=Response.Status.FAILED, error_code=ErrorCode.USER_ERROR,
+                                                   error_desc=f"Failed to get the job details for {job_id}",
+                                                   response=response, job_id=None, source_id=source_id)
+            else:
+                return SourceResponse.parse_result(status=Response.Status.SUCCESS, response=response,
+                                                   source_id=source_id)
+        except Exception as e:
+            raise SourceError(f"Failed to get the job details for {job_id} " + str(e))
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/source_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/url_builder.py` & `infoworkssdk-3.0b0/infoworks/sdk/url_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1079,14 +1079,35 @@
         protocol=config['protocol'],
         job_id=job_id,
         source_id=source_id
     )
     return request
 
 
+def get_ingestion_metrics_admin_url(config, job_id):
+    request = '{protocol}://{ip}:{port}/v3/admin/jobs/{job_id}/reports/ingestion-metrics'.format(
+        ip=config['ip'],
+        port=config['port'],
+        protocol=config['protocol'],
+        job_id=job_id,
+    )
+    return request
+
+
+def get_export_metrics_source_url(config, source_id, job_id):
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/jobs/{job_id}/reports/export-metrics'.format(
+        ip=config['ip'],
+        port=config['port'],
+        protocol=config['protocol'],
+        job_id=job_id,
+        source_id=source_id
+    )
+    return request
+
+
 def get_source_file_paths_url(config, source_id, table_id, job_id):
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/jobs/{job_id}/reports/sourceFilesPath'.format(
         ip=config['ip'],
         port=config['port'],
         protocol=config['protocol'],
         table_id=table_id,
         job_id=job_id,
@@ -1261,16 +1282,334 @@
     request = '{protocol}://{ip}:{port}/v3/prodops/jobs/{job_id}/cancel'.format(
         job_id=job_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
 
 
+def list_service_authentication_url(config):
+    """
+    returns URL to list service authentication using v3 api
+    :param config: client configurations
+    :type config: dict
+    :return: url to list service authentication
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/manage-secrets/service-auth'.format(ip=config['ip'],
+                                                                                     port=config['port'],
+                                                                                     protocol=config['protocol'])
+    return request
+
+
+def list_secret_stores_url(config):
+    """
+    returns URL to list secret stores using v3 api
+    :param config: client configurations
+    :type config: dict
+    :return: url to list secret stores
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/manage-secrets/secret-store'.format(ip=config['ip'],
+                                                                                     port=config['port'],
+                                                                                     protocol=config['protocol'])
+    return request
+
+
 def get_query_as_table_url(config, source_id):
     """
         returns URL to create query as table
     """
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/query_tables'.format(
         source_id=source_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
+
+
+def get_pipeline_group_jobs_base_url(config, domain_id, pipeline_group_id):
+    """
+        returns URL to get list of pipeline group jobs
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipeline-groups/{pipeline_group_id}/jobs'.format(
+        domain_id=domain_id,
+        pipeline_group_id=pipeline_group_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_pipeline_group_base_url(config, domain_id):
+    """
+        returns URL to get details of pipeline group
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipeline-groups/'.format(
+        domain_id=domain_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_accessible_pipeline_groups_url(config, domain_id):
+    """
+    returns URL to get accessible pipeline group
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-pipeline-groups'.format(
+        domain_id=domain_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def advance_config_under_pipeline_groups_base_url(config, domain_id, pipeline_group_id):
+    """
+    returns base URL to get the advance config under pipeline group.
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipeline-groups/{pipeline_group_id}/configurations/advance/'.format(
+        domain_id=domain_id, pipeline_group_id=pipeline_group_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_domain_workflow_schedules_url(config, domain_id):
+    """
+    Returns URL to get Schedules of Workflows belonging to the Domain.
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/schedules'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], domain_id=domain_id
+    )
+    return request
+
+
+def get_workflow_schedule_url(config, domain_id, workflow_id):
+    """
+    Returns URL to get Schedules of particular Workflow belonging to the Domain.
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/workflows/{workflow_id}/schedules'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], domain_id=domain_id, workflow_id=workflow_id
+    )
+    return request
+
+
+def get_enable_workflow_schedule_url(config, domain_id, workflow_id):
+    """
+    Returns URL to Enable Workflow Schedule.
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/workflows/{workflow_id}/schedules/enable'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], domain_id=domain_id, workflow_id=workflow_id
+    )
+    return request
+
+
+def get_disable_workflow_schedule_url(config, domain_id, workflow_id):
+    """
+    Returns URL to Disable Workflow Schedule.
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/workflows/{workflow_id}/schedules/disable'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], domain_id=domain_id, workflow_id=workflow_id
+    )
+    return request
+
+
+def update_workflow_schedule_user_url(config, domain_id, workflow_id):
+    """
+    Return URL to Change Workflow Schedule User
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/workflows/{workflow_id}/schedules/user'.format(
+        protocol=config['protocol'], ip=config['ip'], port=config['port'], domain_id=domain_id, workflow_id=workflow_id
+    )
+    return request
+
+
+def pause_multiple_workflows_url(config):
+    """
+    returns url to pause multiple workflows
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/workflows/pause'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def resume_multiple_workflows_url(config):
+    """
+    returns url to resume workflow
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/workflows/resume'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_workflow_runs_url(config):
+    """
+    returns url to get workflow runs
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/workflows/runs'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_workflow_tasks_url(config):
+    """
+    returns url to get workflow tasks
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/workflows/tasks'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_workflow_run_id_details_url(config, workflow_id, run_id):
+    """
+    returns url to get workflow run id details
+    """
+    request = '{protocol}://{ip}:{port}/v3/admin/workflows/{workflow_id}/runs/{run_id}'.format(
+        workflow_id=workflow_id, run_id=run_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def source_table_schema_url(config, source_id, table_id):
+    """
+    returns url to get table schema details
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/configurations/schema'.format(
+        source_id=source_id,
+        table_id=table_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_file_mappings_for_json_source_url(config, source_id):
+    """
+    returns url to get table schema details
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/file-mappings'.format(
+        source_id=source_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_source_audit_logs_url(config, source_id):
+    """
+    returns url to get source audit logs
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/audit-logs'.format(
+        source_id=source_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_table_audit_logs_url(config, source_id, table_id):
+    """
+    returns url to get table audit logs
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}//tables/table_id/audit-logs'.format(
+        source_id=source_id,
+        table_id=table_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_table_group_audit_logs_url(config, source_id, table_group_id):
+    """
+    returns url to get table group audit logs
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/table-groups/table_group_id/audit-logs'.format(
+        source_id=source_id,
+        table_group_id=table_group_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def accessible_pipeline_extensions_url(config, domain_id):
+    """
+    returns url to get all the Pipeline Extensions associated with this Domain
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-pipeline-extensions'.format(
+        domain_id=domain_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def advanced_config_domain_url(config, domain_id):
+    """
+    returns url to work with adv config of the domain
+    """
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-pipeline-extensions'.format(
+        domain_id=domain_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def table_advanced_base_url(config, source_id, table_id):
+    """
+    returns url to work with table level advanced configuration
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/configurations/advance'.format(
+        source_id=source_id,
+        table_id=table_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def table_segmentation_base_url(config, source_id, table_id):
+    """
+        returns url to work with table segmentation
+    """
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/segmentation'.format(
+        source_id=source_id,
+        table_id=table_id,
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_source_job_url(config, source_id, job_id):
+    request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/jobs/{job_id}'.format(
+        ip=config['ip'],
+        port=config['port'],
+        protocol=config['protocol'],
+        job_id=job_id,
+        source_id=source_id
+    )
+    return request
+
+
+def get_jobs_prodops_url(config):
+    """
+    returns URL to get jobs details
+    :param config: client configurations
+    :type config: dict
+    :return: URL to get jobs details
+    """
+    request = '{protocol}://{ip}:{port}/v3/prodops/jobs'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
+
+
+def get_metrics_prodops_url(config):
+    request = '{protocol}://{ip}:{port}/v3/prodops/metrics'.format(
+        ip=config['ip'],
+        port=config['port'],
+        protocol=config['protocol'],
+    )
+
+
+def list_secrets_url(config):
+    """
+        returns url to get secret details in Infoworks
+        """
+    request = '{protocol}://{ip}:{port}/v3/admin/manage-secrets/secrets'.format(
+        ip=config['ip'], port=config['port'],
+        protocol=config['protocol'])
+    return request
```

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworks/sdk/workflow_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-2.0.8/infoworkssdk.egg-info/PKG-INFO` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 2.0.8
-Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.3 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-2.0
+Version: 3.0b0
+Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
-Author: Abhishek
+Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `infoworkssdk-2.0.8/infoworkssdk.egg-info/SOURCES.txt` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 infoworks/sdk/domain_client.py
 infoworks/sdk/generic_response.py
 infoworks/sdk/jobmetrics.py
 infoworks/sdk/jobs_client.py
 infoworks/sdk/jobs_response.py
 infoworks/sdk/local_configurations.py
 infoworks/sdk/pipeline_client.py
+infoworks/sdk/pipeline_group_client.py
 infoworks/sdk/pipeline_response.py
 infoworks/sdk/source_client.py
 infoworks/sdk/source_response.py
 infoworks/sdk/url_builder.py
 infoworks/sdk/utils.py
 infoworks/sdk/workflow_client.py
 infoworks/sdk/workflow_response.py
@@ -34,14 +35,15 @@
 infoworks/sdk/cicd/download_configurations/lineage.py
 infoworks/sdk/cicd/download_configurations/utils.py
 infoworks/sdk/cicd/upload_configurations/__init__.py
 infoworks/sdk/cicd/upload_configurations/cdata_source.py
 infoworks/sdk/cicd/upload_configurations/csv_source.py
 infoworks/sdk/cicd/upload_configurations/domains.py
 infoworks/sdk/cicd/upload_configurations/misc.py
+infoworks/sdk/cicd/upload_configurations/pipeline_group.py
 infoworks/sdk/cicd/upload_configurations/pipelines.py
 infoworks/sdk/cicd/upload_configurations/rdbms_source.py
 infoworks/sdk/cicd/upload_configurations/salesforce_source.py
 infoworks/sdk/cicd/upload_configurations/update_configurations.py
 infoworks/sdk/cicd/upload_configurations/workflow.py
 infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
 infoworks/sdk/cicd/upload_configurations/wrappersource.py
```

### Comparing `infoworkssdk-2.0.8/setup.py` & `infoworkssdk-3.0b0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="infoworkssdk",
-    version="2.0.8",
-    author="Abhishek",
+    version="3.0-beta",
+    author="Infoworks CE Team",
     author_email="abhishek.raviprasad@infoworks.io",
-    description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.3 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-2.0",
+    description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Infoworks/InfoworksPythonSDK",
     packages=setuptools.find_packages(),
     install_requires=[
-        'requests', 'bson', 'pycryptodomex>=3.13.0', 'cryptography==37.0.2', 'urllib3', 'pandas', 'networkx',
-        'pyyaml', 'google-cloud-kms',
-        'google-cloud-storage', 'boto3', 'azure-identity', 'azure-keyvault-secrets'
-    ],
+        'requests', 'bson', 'urllib3', 'pandas', 'networkx'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

