# Comparing `tmp/dagster_cloud-1.2.6.tar.gz` & `tmp/dagster_cloud-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.2.6.tar", last modified: Thu Apr  6 00:35:08 2023, max compression
+gzip compressed data, was "dagster_cloud-1.2.7.tar", last modified: Thu Apr 13 15:16:38 2023, max compression
```

## Comparing `dagster_cloud-1.2.6.tar` & `dagster_cloud-1.2.7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.418906 dagster_cloud-1.2.6/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-06 00:35:08.418906 dagster_cloud-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.442899 dagster_cloud-1.2.6/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.454899 dagster_cloud-1.2.6/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.458900 dagster_cloud-1.2.6/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42939 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.462900 dagster_cloud-1.2.6/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16985 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.530900 dagster_cloud-1.2.6/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.534900 dagster_cloud-1.2.6/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.542900 dagster_cloud-1.2.6/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.610900 dagster_cloud-1.2.6/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14189 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.634901 dagster_cloud-1.2.6/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.650901 dagster_cloud-1.2.6/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18148 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.682901 dagster_cloud-1.2.6/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.706901 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.774901 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.858902 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.862902 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.926902 dagster_cloud-1.2.6/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.934903 dagster_cloud-1.2.6/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.938902 dagster_cloud-1.2.6/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.002903 dagster_cloud-1.2.6/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.018903 dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26776 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.090904 dagster_cloud-1.2.6/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19167 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.102904 dagster_cloud-1.2.6/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     6313 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.162904 dagster_cloud-1.2.6/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.166904 dagster_cloud-1.2.6/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.166904 dagster_cloud-1.2.6/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.182904 dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     3422 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.250905 dagster_cloud-1.2.6/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.326905 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22063 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    19038 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.338905 dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11403 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:08.410906 dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    70432 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:35:07.442899 dagster_cloud-1.2.6/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-06 00:35:06.000000 dagster_cloud-1.2.6/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-06 00:35:07.000000 dagster_cloud-1.2.6/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:35:06.000000 dagster_cloud-1.2.6/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-06 00:35:06.000000 dagster_cloud-1.2.6/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-06 00:35:06.000000 dagster_cloud-1.2.6/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 00:35:08.418906 dagster_cloud-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-04-05 23:52:09.000000 dagster_cloud-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.085919 dagster_cloud-1.2.7/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42939 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.093919 dagster_cloud-1.2.7/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16985 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.093919 dagster_cloud-1.2.7/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14189 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18148 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.105919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.105919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.109919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.109919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.113919 dagster_cloud-1.2.7/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.113919 dagster_cloud-1.2.7/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.117919 dagster_cloud-1.2.7/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.117919 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.121919 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26776 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.125919 dagster_cloud-1.2.7/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19167 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.129919 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.129919 dagster_cloud-1.2.7/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.133919 dagster_cloud-1.2.7/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.133919 dagster_cloud-1.2.7/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.137919 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.137919 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.161919 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22459 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    19970 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.165919 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11403 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.173919 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    70432 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/setup.py
```

### Comparing `dagster_cloud-1.2.6/PKG-INFO` & `dagster_cloud-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.2.6
+Version: 1.2.7
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.2.6/README.md` & `dagster_cloud-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/agent/cli/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tempfile import TemporaryDirectory
 from typing import Optional
 
 import yaml
 from dagster._core.errors import DagsterHomeNotSetError
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.log import default_date_format_string, default_format_string
+from dagster._utils.merger import deep_merge_dicts
 from dagster._utils.yaml_utils import load_yaml_from_globs
 from dagster_cloud_cli import ui
 from typer import Argument, Option, Typer
 
 from dagster_cloud.agent.dagster_cloud_agent import DagsterCloudAgent
 from dagster_cloud.instance import DagsterCloudAgentInstance
 
@@ -73,67 +74,60 @@
             run_local_agent(agent_logging_config_path)
         finally:
             os.environ.clear()
             if old_env is not None:
                 os.environ.update(old_env)
 
 
-DAGSTER_YAML_TEMPLATE = """
-instance_class:
-  module: dagster_cloud.instance
-  class: DagsterCloudAgentInstance
-
-dagster_cloud_api:
-  agent_token: {token}
-  deployment: {deployment}
-  {agent_label_entry}
-
-user_code_launcher:
-  module: {user_code_launcher_module}
-  class: {user_code_launcher_class}
-  {user_code_launcher_config_entry}
-"""
-
-
 def run_local_agent_in_temp_environment(
     agent_token: str,
     deployment: str,
     agent_label: Optional[str],
-    user_code_launcher_module: str,
-    user_code_launcher_class: str,
+    instance_config: Optional[str],
+    user_code_launcher_module: Optional[str],
+    user_code_launcher_class: Optional[str],
     user_code_launcher_config: Optional[str],
 ):
-    with TemporaryDirectory() as d:
-        config_entry = ""
-        if user_code_launcher_config:
-            try:
-                unindented_config_entry: str = yaml.dump(
-                    {"config": json.loads(user_code_launcher_config)}
-                )
-                config_entry = unindented_config_entry.replace("\n", "\n  ")
-            except json.JSONDecodeError as e:
-                raise ui.error(f"Invalid User Code Launcher config JSON:\n{e}")
+    config = {
+        "instance_class": {
+            "module": "dagster_cloud.instance",
+            "class": "DagsterCloudAgentInstance",
+        },
+        "dagster_cloud_api": {},
+        "user_code_launcher": {
+            "module": "dagster_cloud.workspace.user_code_launcher",
+            "class": "ProcessUserCodeLauncher",
+        },
+    }
+    if instance_config:
+        parsed = json.loads(instance_config)
+        config = deep_merge_dicts(config, parsed)
+
+    if agent_token:
+        config["dagster_cloud_api"]["agent_token"] = agent_token
+    if deployment:
+        config["dagster_cloud_api"]["deployment"] = deployment
+    if agent_label:
+        config["dagster_cloud_api"]["agent_label"] = agent_label
+    if user_code_launcher_module:
+        config["user_code_launcher"]["module"] = user_code_launcher_module
+    if user_code_launcher_class:
+        config["user_code_launcher"]["class"] = user_code_launcher_class
+    if user_code_launcher_config:
+        try:
+            config["user_code_launcher"]["config"] = json.loads(user_code_launcher_config)
+        except json.JSONDecodeError as e:
+            raise ui.error(f"Invalid User Code Launcher config JSON:\n{e}")
 
+    with TemporaryDirectory() as d:
         with open(os.path.join(d, "dagster.yaml"), "w", encoding="utf8") as f:
-            f.write(
-                DAGSTER_YAML_TEMPLATE.format(
-                    token=agent_token,
-                    deployment=deployment,
-                    agent_label_entry=f"agent_label: {agent_label}" if agent_label else "",
-                    user_code_launcher_module=user_code_launcher_module,
-                    user_code_launcher_class=user_code_launcher_class,
-                    user_code_launcher_config_entry=config_entry,
-                )
-            )
+            f.write(yaml.dump(config))
         run_local_agent_in_environment(Path(d), None)
 
 
-PROCESS_USER_CODE_LAUNCHER = "dagster_cloud.workspace.user_code_launcher.ProcessUserCodeLauncher"
-
-
 @app.command(
     help=(
         "Runs the Dagster Cloud agent. The agent can either be run ephemerally by specifying an"
         " agent token and deployment name as CLI options, or the agent can pull its config from a"
         " dagster.yaml file. To use a dagster.yaml file, either pass a directory containing the"
         " file as a CLI argument or set the DAGSTER_HOME environment variable."
     ),
@@ -147,22 +141,29 @@
     deployment: str = Option(
         None, "--deployment", "-d", help="Deployment, if running ephemerally."
     ),
     agent_label: str = Option(
         None, "--agent-label", "-l", help="Optional agent label, if running ephemerally."
     ),
     user_code_launcher: str = Option(
-        PROCESS_USER_CODE_LAUNCHER,
+        None,
         "--user-code-launcher",
         help="User Code Launcher to use. Defaults to the local Process User Code Launcher.",
+        hidden=True,
+    ),
+    instance_config: str = Option(
+        None,
+        "--config",
+        help="Dagster instance config, in JSON format.",
     ),
     user_code_launcher_config: str = Option(
         None,
         "--user-code-launcher-config",
         help="Config to supply the User Code Launcher, in JSON format.",
+        hidden=True,
     ),
     agent_logging_config_path: Optional[Path] = Option(
         None,
         "--agent-logging-config-path",
         help=(
             "Yaml file with logging config for the agent process that can be passed into"
             " logging.dictConfig"
@@ -170,29 +171,38 @@
         exists=True,
     ),
 ):
     if (
         agent_token
         or deployment
         or agent_label
+        or instance_config
         or user_code_launcher_config
-        or user_code_launcher != PROCESS_USER_CODE_LAUNCHER
+        or user_code_launcher
     ):
-        if not agent_token or not deployment:
+        if not instance_config and (not agent_token or not deployment):
             raise ui.error("To run ephemerally, must supply both an agent token and a deployment.")
         if dagster_home:
             raise ui.error("Cannot supply both a dagster home directory and ephemeral parameters.")
 
-        user_code_launcher_module = ""
-        user_code_launcher_class = user_code_launcher
-        if "." in user_code_launcher:
-            user_code_launcher_module, user_code_launcher_class = user_code_launcher.rsplit(".", 1)
+        if user_code_launcher:
+            user_code_launcher_module = ""
+            user_code_launcher_class = user_code_launcher
+            if "." in user_code_launcher:
+                user_code_launcher_module, user_code_launcher_class = user_code_launcher.rsplit(
+                    ".", 1
+                )
+        else:
+            user_code_launcher_module = None
+            user_code_launcher_class = None
+
         run_local_agent_in_temp_environment(
             agent_token,
             deployment,
             agent_label,
+            instance_config,
             user_code_launcher_module,
             user_code_launcher_class,
             user_code_launcher_config,
         )
     else:
         run_local_agent_in_environment(dagster_home, agent_logging_config_path)
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.2.7/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/agent/queries.py` & `dagster_cloud-1.2.7/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.2.7/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/auth/constants.py` & `dagster_cloud-1.2.7/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.2.7/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.2.7/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.2.7/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/client.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/schedules/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ALL_STORED_JOB_STATE_QUERY = """
-    query jobStates($repositoryOriginId: String, $repositorySelectorId: String, $jobType: InstigationType) {
+    query jobStates($repositoryOriginId: String, $repositorySelectorId: String, $jobType: InstigationType, $statuses: [String!]) {
         schedules {
-            jobStates(repositoryOriginId: $repositoryOriginId, repositorySelectorId: $repositorySelectorId, jobType: $jobType)
+            jobStates(repositoryOriginId: $repositoryOriginId, repositorySelectorId: $repositorySelectorId, jobType: $jobType, statuses: $statuses)
         }
     }
 """
 
 
 ADD_JOB_STATE_MUTATION = """
     mutation addJobStateMutation($serializedJobState: String!) {
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.2.7/dagster_cloud/storage/schedules/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.scheduler.instigation import (
     InstigatorState,
+    InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.schedules.base import ScheduleStorage
 from dagster._serdes import (
     ConfigurableClass,
@@ -70,21 +71,25 @@
         raise Exception("Not allowed to wipe from user cloud")
 
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional[InstigatorType] = None,
+        instigator_statuses: Optional[Set[InstigatorStatus]] = None,
     ) -> Iterable[InstigatorState]:
         res = self._execute_query(
             ALL_STORED_JOB_STATE_QUERY,
             variables={
                 "repositoryOriginId": repository_origin_id,
                 "repositorySelectorId": repository_selector_id,
                 "jobType": instigator_type.value if instigator_type else None,
+                "statuses": [status.value for status in instigator_statuses]
+                if instigator_statuses
+                else None,
             },
         )
 
         return [
             deserialize_value(state, InstigatorState)
             for state in res["data"]["schedules"]["jobStates"]
         ]
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/util/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dagster import Array, Field, Noneable, Permissive, Shape, StringSource
+from dagster import Array, BoolSource, Field, Noneable, Permissive, Shape, StringSource
 
 # Shared between user code launcher config and container context
 SHARED_ECS_CONFIG = {
     "server_resources": Field(
         Permissive(
             {
                 "cpu": Field(
@@ -11,14 +11,19 @@
                     description="The CPU override to use for the launched task.",
                 ),
                 "memory": Field(
                     str,
                     is_required=False,
                     description="The memory override to use for the launched task.",
                 ),
+                "ephemeral_storage": Field(
+                    int,
+                    is_required=False,
+                    description="The ephemeral storage, in GiB, to use for the launched task.",
+                ),
             }
         )
     ),
     "run_resources": Field(
         Permissive(
             {
                 "cpu": Field(
@@ -27,14 +32,19 @@
                     description="The CPU override to use for the launched task.",
                 ),
                 "memory": Field(
                     str,
                     is_required=False,
                     description="The memory override to use for the launched task.",
                 ),
+                "ephemeral_storage": Field(
+                    int,
+                    is_required=False,
+                    description="The ephemeral storage, in GiB, to use for the launched task.",
+                ),
             }
         )
     ),
     "runtime_platform": Field(
         Shape(
             {
                 "cpuArchitecture": Field(StringSource, is_required=False),
@@ -44,14 +54,46 @@
         is_required=False,
         description=(
             "The operating system that the task definition is running on. See"
             " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_task_definition"
             " for the available options."
         ),
     ),
+    "volumes": Field(
+        Array(
+            Permissive(
+                {
+                    "name": Field(StringSource, is_required=False),
+                }
+            )
+        ),
+        is_required=False,
+        description=(
+            "List of data volume definitions for the task. See"
+            " https://docs.aws.amazon.com/AmazonECS/latest/developerguide/efs-volumes.html"
+            " for the full list of available options."
+        ),
+    ),
+    "mount_points": Field(
+        Array(
+            Shape(
+                {
+                    "sourceVolume": Field(StringSource, is_required=False),
+                    "containerPath": Field(StringSource, is_required=False),
+                    "readOnly": Field(BoolSource, is_required=False),
+                }
+            )
+        ),
+        is_required=False,
+        description=(
+            "Mount points for data volumes in the main container of the task."
+            " See https://docs.aws.amazon.com/AmazonECS/latest/developerguide/efs-volumes.html"
+            " for more information."
+        ),
+    ),
 }
 
 
 ECS_CONTAINER_CONTEXT_CONFIG = {
     "secrets": Field(
         Noneable(Array(Shape({"name": StringSource, "valueFrom": StringSource}))),
         is_required=False,
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,18 @@
         task_role_arn=None,
         env=None,
         secrets=None,
         sidecars=None,
         logger=None,
         cpu=None,
         memory=None,
+        ephemeral_storage=None,
         runtime_platform=None,
+        mount_points=None,
+        volumes=None,
     ):
         container_name = container_name or family
 
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         env = env or {}
         environment = [{"name": key, "value": value} for key, value in env.items()]
@@ -139,15 +142,18 @@
             environment=environment,
             execution_role_arn=execution_role_arn,
             task_role_arn=task_role_arn,
             sidecars=sidecars,
             requires_compatibilities=[self.launch_type],
             cpu=cpu,
             memory=memory,
+            ephemeral_storage=ephemeral_storage,
             runtime_platform=runtime_platform,
+            mount_points=mount_points,
+            volumes=volumes,
         )
 
         try:
             existing_task_definition = self.ecs.describe_task_definition(taskDefinition=family)[
                 "taskDefinition"
             ]
         except ClientError:
@@ -193,16 +199,19 @@
         tags=None,
         register_service_discovery=True,
         secrets=None,
         sidecars=None,
         logger=None,
         cpu=None,
         memory=None,
+        ephemeral_storage=None,
         allow_ecs_exec=False,
         runtime_platform=None,
+        mount_points=None,
+        volumes=None,
     ):
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         service_name = name
         family = family or name
 
         logger.info(f"Checking if task definition {family} for {name} can be re-used...")
@@ -216,15 +225,18 @@
             command=command,
             env=env or {},
             secrets=secrets,
             sidecars=sidecars,
             logger=logger,
             cpu=cpu,
             memory=memory,
+            ephemeral_storage=ephemeral_storage,
             runtime_platform=runtime_platform,
+            mount_points=mount_points,
+            volumes=volumes,
         )
 
         service_registry_arn = None
         # Configure service discovery
         if register_service_discovery:
             logger.info(f"Creating service registry for {service_name}...")
             service_registry_arn = self._create_service_registry(
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Collection, Dict, List, Mapping, Optional
+from typing import Any, Collection, Dict, List, Mapping, Optional, Sequence
 
 import boto3
 from dagster import (
     Array,
     Enum,
     EnumValue,
     Field,
@@ -53,17 +53,19 @@
         inst_data: Optional[ConfigurableClassData] = None,
         secrets=None,
         secrets_tag=None,
         env_vars=None,
         ecs_timeout=None,
         ecs_grace_period=None,
         launch_type: Optional[str] = None,
-        server_resources: Optional[Mapping[str, str]] = None,
-        run_resources: Optional[Mapping[str, str]] = None,
+        server_resources: Optional[Mapping[str, Any]] = None,
+        run_resources: Optional[Mapping[str, Any]] = None,
         runtime_platform: Optional[Mapping[str, Any]] = None,
+        mount_points: Optional[Sequence[Mapping[str, Any]]] = None,
+        volumes: Optional[Sequence[Mapping[str, Any]]] = None,
         **kwargs,
     ):
         self.ecs = boto3.client("ecs")
         self.logs = boto3.client("logs")
         self.service_discovery = boto3.client("servicediscovery")
         self.secrets_manager = boto3.client("secretsmanager")
 
@@ -103,14 +105,17 @@
         self.launch_type = check.opt_str_param(launch_type, "launch_type", default="FARGATE")
 
         self.server_resources = check.opt_mapping_param(server_resources, "server_resources")
         self.run_resources = check.opt_mapping_param(run_resources, "run_resources")
 
         self.runtime_platform = check.opt_mapping_param(runtime_platform, "runtime_platform")
 
+        self.mount_points = check.opt_sequence_param(mount_points, "mount_points")
+        self.volumes = check.opt_sequence_param(volumes, "volumes")
+
         self.client = Client(
             cluster_name=self.cluster,
             subnet_ids=self.subnets,
             security_group_ids=security_group_ids,
             service_discovery_namespace_id=self.service_discovery_namespace_id,
             log_group=self.log_group,
             timeout=self._ecs_timeout,
@@ -221,14 +226,19 @@
 
     def _get_service_cpu_override(self, container_context: EcsContainerContext) -> Optional[str]:
         return container_context.server_resources.get("cpu")
 
     def _get_service_memory_override(self, container_context: EcsContainerContext) -> Optional[str]:
         return container_context.server_resources.get("memory")
 
+    def _get_service_ephemeral_storage_override(
+        self, container_context: EcsContainerContext
+    ) -> Optional[int]:
+        return container_context.server_resources.get("ephemeral_storage")
+
     def _get_enable_ecs_exec(self) -> bool:
         return False
 
     def _get_additional_grpc_server_env(self) -> Dict[str, str]:
         return {}
 
     def _start_new_server_spinup(
@@ -254,14 +264,16 @@
             env_vars=self.env_vars
             + [f"{k}={v}" for k, v in (metadata.cloud_context_env or {}).items()],
             server_resources=self.server_resources,
             run_resources=self.run_resources,
             task_role_arn=self.task_role_arn,
             execution_role_arn=self.execution_role_arn,
             runtime_platform=self.runtime_platform,
+            mount_points=self.mount_points,
+            volumes=self.volumes,
         ).merge(EcsContainerContext.create_from_config(metadata.container_context))
 
         environment = merge_dicts(
             container_context.get_environment_dict(),
             additional_env,
             self._get_additional_grpc_server_env(),
         )
@@ -292,16 +304,19 @@
             },
             task_role_arn=container_context.task_role_arn,
             secrets=container_context.get_secrets_dict(self.secrets_manager),
             sidecars=self._get_grpc_server_sidecars(),
             logger=self._logger,
             cpu=self._get_service_cpu_override(container_context),
             memory=self._get_service_memory_override(container_context),
+            ephemeral_storage=self._get_service_ephemeral_storage_override(container_context),
             allow_ecs_exec=self._get_enable_ecs_exec(),
             runtime_platform=container_context.runtime_platform,
+            mount_points=container_context.mount_points,
+            volumes=container_context.volumes,
         )
         self._logger.info(
             "Created a new service at hostname {} for {}:{}, waiting for server to be ready..."
             .format(service.hostname, deployment_name, location_name)
         )
 
         endpoint = ServerEndpoint(
@@ -425,15 +440,17 @@
         return dict(
             task_definition={
                 "log_group": self.log_group,
                 "execution_role_arn": self.execution_role_arn,
                 "requires_compatibilities": [self.launch_type],
                 **({"task_role_arn": self.task_role_arn} if self.task_role_arn else {}),
                 **({"sidecars": sidecars} if sidecars else {}),
-                **({"runtime_platform": self.task_role_arn} if self.runtime_platform else {}),
+                **({"runtime_platform": self.runtime_platform} if self.runtime_platform else {}),
+                **({"mount_points": self.mount_points} if self.mount_points else {}),
+                **({"volumes": self.volumes} if self.volumes else {}),
             },
             secrets=self.secrets,
             secrets_tag=self.secrets_tag,
             env_vars=self.env_vars,
             use_current_ecs_task_config=False,
             run_task_kwargs={
                 "cluster": self.cluster,
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.2.7/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.2.6
+Version: 1.2.7
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.2.6/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.2.7/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.6/setup.py` & `dagster_cloud-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.6",
-        "dagster-cloud-cli==1.2.6",
+        "dagster==1.2.7",
+        "dagster-cloud-cli==1.2.7",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.18.6",
+            "dagster_k8s==0.18.7",
         ],
-        "docker": ["docker", "dagster_docker==0.18.6"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.18.6"],
-        "ecs": ["dagster_aws==0.18.6", "boto3"],
+        "docker": ["docker", "dagster_docker==0.18.7"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.18.7"],
+        "ecs": ["dagster_aws==0.18.7", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

