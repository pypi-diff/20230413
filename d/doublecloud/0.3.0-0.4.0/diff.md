# Comparing `tmp/doublecloud-0.3.0.tar.gz` & `tmp/doublecloud-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doublecloud-0.3.0.tar", last modified: Thu Apr 13 15:25:50 2023, max compression
+gzip compressed data, was "doublecloud-0.4.0.tar", last modified: Thu Apr 13 15:37:09 2023, max compression
```

## Comparing `doublecloud-0.3.0.tar` & `doublecloud-0.4.0.tar`

### file list

```diff
@@ -1,159 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 15:25:20.000000 doublecloud-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:25:50.402902 doublecloud-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-13 15:25:20.000000 doublecloud-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_auth_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_auth_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_operation_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_retry_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/_wrappers/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_wrappers/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/_wrappers/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/_wrappers/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/clickhouse/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.398902 doublecloud-0.3.0/doublecloud/kafka/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/topic_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.398902 doublecloud-0.3.0/doublecloud/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.398902 doublecloud-0.3.0/doublecloud/network/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_connection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/network_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/network/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.398902 doublecloud-0.3.0/doublecloud/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.398902 doublecloud-0.3.0/doublecloud/transfer/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/transfer_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/doublecloud/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/maintenance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/paging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/v1/paging_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/doublecloud/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.402902 doublecloud-0.3.0/doublecloud/visualization/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/v1/workbook_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/v1/workbook_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-04-13 15:25:20.000000 doublecloud-0.3.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:25:50.394902 doublecloud-0.3.0/doublecloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:25:50.000000 doublecloud-0.3.0/doublecloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-13 15:25:20.000000 doublecloud-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:25:50.402902 doublecloud-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-13 15:25:45.000000 doublecloud-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.285694 doublecloud-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 15:36:30.000000 doublecloud-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:37:09.285694 doublecloud-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-13 15:36:30.000000 doublecloud-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.269694 doublecloud-0.4.0/doublecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_auth_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_auth_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_operation_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/_wrappers/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_wrappers/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/_wrappers/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/_wrappers/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/clickhouse/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.277694 doublecloud-0.4.0/doublecloud/kafka/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.277694 doublecloud-0.4.0/doublecloud/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.277694 doublecloud-0.4.0/doublecloud/network/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/network_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/network/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.277694 doublecloud-0.4.0/doublecloud/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.281694 doublecloud-0.4.0/doublecloud/transfer/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.281694 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.285694 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.285694 doublecloud-0.4.0/doublecloud/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/maintenance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/maintenance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/paging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/paging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/v1/paging_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.285694 doublecloud-0.4.0/doublecloud/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.285694 doublecloud-0.4.0/doublecloud/visualization/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-04-13 15:36:30.000000 doublecloud-0.4.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:37:09.273694 doublecloud-0.4.0/doublecloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:37:09.000000 doublecloud-0.4.0/doublecloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-13 15:36:30.000000 doublecloud-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:37:09.285694 doublecloud-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 15:37:02.000000 doublecloud-0.4.0/setup.py
```

### Comparing `doublecloud-0.3.0/LICENSE` & `doublecloud-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/PKG-INFO` & `doublecloud-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.3.0/README.md` & `doublecloud-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_auth_fabric.py` & `doublecloud-0.4.0/doublecloud/_auth_fabric.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_auth_plugin.py` & `doublecloud-0.4.0/doublecloud/_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_backoff.py` & `doublecloud-0.4.0/doublecloud/_backoff.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_channels.py` & `doublecloud-0.4.0/doublecloud/_channels.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_operation_waiter.py` & `doublecloud-0.4.0/doublecloud/_operation_waiter.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_retry_interceptor.py` & `doublecloud-0.4.0/doublecloud/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/_sdk.py` & `doublecloud-0.4.0/doublecloud/_sdk.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_service_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_service_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/config_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/operation_service_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/version_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/version_service_pb2.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/cluster_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/cluster_service_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/config_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/operation_service_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/topic_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/topic_service_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/user_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/user_service_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/user_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/version_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/version_service_pb2.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/kafka/v1/version_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/kafka/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_connection_pb2.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_connection_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_connection_service_pb2.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_connection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_pb2.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_service_pb2.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/network_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/network/v1/network_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/operation_service_pb2.py` & `doublecloud-0.4.0/doublecloud/network/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/network/v1/operation_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/network/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/common_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/common_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_service_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/operation_service_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/transfer_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/transfer_service_pb2.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/transfer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/v1/cluster_pb2.py` & `doublecloud-0.4.0/doublecloud/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/v1/maintenance_pb2.py` & `doublecloud-0.4.0/doublecloud/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/v1/operation_pb2.py` & `doublecloud-0.4.0/doublecloud/v1/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/v1/paging_pb2.py` & `doublecloud-0.4.0/doublecloud/v1/paging_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/visualization/v1/workbook_pb2.py` & `doublecloud-0.4.0/doublecloud/visualization/v1/workbook_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/visualization/v1/workbook_service_pb2.py` & `doublecloud-0.4.0/doublecloud/visualization/v1/workbook_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py` & `doublecloud-0.4.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/doublecloud.egg-info/PKG-INFO` & `doublecloud-0.4.0/doublecloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.3.0/doublecloud.egg-info/SOURCES.txt` & `doublecloud-0.4.0/doublecloud.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,119 +20,170 @@
 doublecloud.egg-info/top_level.txt
 doublecloud/_wrappers/__init__.py
 doublecloud/_wrappers/clickhouse/__init__.py
 doublecloud/_wrappers/kafka/__init__.py
 doublecloud/clickhouse/__init__.py
 doublecloud/clickhouse/v1/__init__.py
 doublecloud/clickhouse/v1/backup_pb2.py
+doublecloud/clickhouse/v1/backup_pb2.pyi
 doublecloud/clickhouse/v1/backup_pb2_grpc.py
 doublecloud/clickhouse/v1/backup_service_pb2.py
+doublecloud/clickhouse/v1/backup_service_pb2.pyi
 doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
 doublecloud/clickhouse/v1/cluster_pb2.py
+doublecloud/clickhouse/v1/cluster_pb2.pyi
 doublecloud/clickhouse/v1/cluster_pb2_grpc.py
 doublecloud/clickhouse/v1/cluster_service_pb2.py
+doublecloud/clickhouse/v1/cluster_service_pb2.pyi
 doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
 doublecloud/clickhouse/v1/config_pb2.py
+doublecloud/clickhouse/v1/config_pb2.pyi
 doublecloud/clickhouse/v1/config_pb2_grpc.py
 doublecloud/clickhouse/v1/operation_service_pb2.py
+doublecloud/clickhouse/v1/operation_service_pb2.pyi
 doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
 doublecloud/clickhouse/v1/version_pb2.py
+doublecloud/clickhouse/v1/version_pb2.pyi
 doublecloud/clickhouse/v1/version_pb2_grpc.py
 doublecloud/clickhouse/v1/version_service_pb2.py
+doublecloud/clickhouse/v1/version_service_pb2.pyi
 doublecloud/clickhouse/v1/version_service_pb2_grpc.py
 doublecloud/kafka/__init__.py
 doublecloud/kafka/v1/__init__.py
 doublecloud/kafka/v1/cluster_pb2.py
+doublecloud/kafka/v1/cluster_pb2.pyi
 doublecloud/kafka/v1/cluster_pb2_grpc.py
 doublecloud/kafka/v1/cluster_service_pb2.py
+doublecloud/kafka/v1/cluster_service_pb2.pyi
 doublecloud/kafka/v1/cluster_service_pb2_grpc.py
 doublecloud/kafka/v1/config_pb2.py
+doublecloud/kafka/v1/config_pb2.pyi
 doublecloud/kafka/v1/config_pb2_grpc.py
 doublecloud/kafka/v1/operation_service_pb2.py
+doublecloud/kafka/v1/operation_service_pb2.pyi
 doublecloud/kafka/v1/operation_service_pb2_grpc.py
 doublecloud/kafka/v1/topic_pb2.py
+doublecloud/kafka/v1/topic_pb2.pyi
 doublecloud/kafka/v1/topic_pb2_grpc.py
 doublecloud/kafka/v1/topic_service_pb2.py
+doublecloud/kafka/v1/topic_service_pb2.pyi
 doublecloud/kafka/v1/topic_service_pb2_grpc.py
 doublecloud/kafka/v1/user_pb2.py
+doublecloud/kafka/v1/user_pb2.pyi
 doublecloud/kafka/v1/user_pb2_grpc.py
 doublecloud/kafka/v1/user_service_pb2.py
+doublecloud/kafka/v1/user_service_pb2.pyi
 doublecloud/kafka/v1/user_service_pb2_grpc.py
 doublecloud/kafka/v1/version_pb2.py
+doublecloud/kafka/v1/version_pb2.pyi
 doublecloud/kafka/v1/version_pb2_grpc.py
 doublecloud/kafka/v1/version_service_pb2.py
+doublecloud/kafka/v1/version_service_pb2.pyi
 doublecloud/kafka/v1/version_service_pb2_grpc.py
 doublecloud/network/__init__.py
 doublecloud/network/v1/__init__.py
 doublecloud/network/v1/network_connection_pb2.py
+doublecloud/network/v1/network_connection_pb2.pyi
 doublecloud/network/v1/network_connection_pb2_grpc.py
 doublecloud/network/v1/network_connection_service_pb2.py
+doublecloud/network/v1/network_connection_service_pb2.pyi
 doublecloud/network/v1/network_connection_service_pb2_grpc.py
 doublecloud/network/v1/network_pb2.py
+doublecloud/network/v1/network_pb2.pyi
 doublecloud/network/v1/network_pb2_grpc.py
 doublecloud/network/v1/network_service_pb2.py
+doublecloud/network/v1/network_service_pb2.pyi
 doublecloud/network/v1/network_service_pb2_grpc.py
 doublecloud/network/v1/operation_service_pb2.py
+doublecloud/network/v1/operation_service_pb2.pyi
 doublecloud/network/v1/operation_service_pb2_grpc.py
 doublecloud/transfer/__init__.py
 doublecloud/transfer/v1/__init__.py
 doublecloud/transfer/v1/endpoint_pb2.py
+doublecloud/transfer/v1/endpoint_pb2.pyi
 doublecloud/transfer/v1/endpoint_pb2_grpc.py
 doublecloud/transfer/v1/endpoint_service_pb2.py
+doublecloud/transfer/v1/endpoint_service_pb2.pyi
 doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
 doublecloud/transfer/v1/operation_service_pb2.py
+doublecloud/transfer/v1/operation_service_pb2.pyi
 doublecloud/transfer/v1/operation_service_pb2_grpc.py
 doublecloud/transfer/v1/transfer_pb2.py
+doublecloud/transfer/v1/transfer_pb2.pyi
 doublecloud/transfer/v1/transfer_pb2_grpc.py
 doublecloud/transfer/v1/transfer_service_pb2.py
+doublecloud/transfer/v1/transfer_service_pb2.pyi
 doublecloud/transfer/v1/transfer_service_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/__init__.py
 doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
+doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
 doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/common_pb2.py
+doublecloud/transfer/v1/endpoint/common_pb2.pyi
 doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/kafka_pb2.py
+doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
 doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/mongo_pb2.py
+doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
 doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/mysql_pb2.py
+doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
 doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/parsers_pb2.py
+doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
 doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/postgres_pb2.py
+doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
 doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/__init__.py
 doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
 doublecloud/v1/__init__.py
 doublecloud/v1/cluster_pb2.py
+doublecloud/v1/cluster_pb2.pyi
 doublecloud/v1/cluster_pb2_grpc.py
 doublecloud/v1/maintenance_pb2.py
+doublecloud/v1/maintenance_pb2.pyi
 doublecloud/v1/maintenance_pb2_grpc.py
 doublecloud/v1/operation_pb2.py
+doublecloud/v1/operation_pb2.pyi
 doublecloud/v1/operation_pb2_grpc.py
 doublecloud/v1/paging_pb2.py
+doublecloud/v1/paging_pb2.pyi
 doublecloud/v1/paging_pb2_grpc.py
 doublecloud/visualization/__init__.py
 doublecloud/visualization/v1/__init__.py
 doublecloud/visualization/v1/workbook_pb2.py
+doublecloud/visualization/v1/workbook_pb2.pyi
 doublecloud/visualization/v1/workbook_pb2_grpc.py
 doublecloud/visualization/v1/workbook_service_pb2.py
+doublecloud/visualization/v1/workbook_service_pb2.pyi
 doublecloud/visualization/v1/workbook_service_pb2_grpc.py
```

### Comparing `doublecloud-0.3.0/pyproject.toml` & `doublecloud-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doublecloud-0.3.0/setup.py` & `doublecloud-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 packages = find_packages(".", include=["doublecloud*"])
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 setup(
     name="doublecloud",
     version=__version__,
     description="The Double.Cloud official SDK",
     url="https://github.com/doublecloud/python-sdk",
     author="DoubleCloud GmbH",
@@ -29,9 +29,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     tests_require=["pytest"],
     setup_requires=["wheel"],
     packages=packages,
+    package_data={"doublecloud": ["*.pyi", "**/*.pyi"]},
     zip_safe=False,
 )
```

