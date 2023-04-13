# Comparing `tmp/dagster-graphql-1.2.6.tar.gz` & `tmp/dagster-graphql-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.2.6.tar", last modified: Thu Apr  6 00:26:29 2023, max compression
+gzip compressed data, was "dagster-graphql-1.2.7.tar", last modified: Thu Apr 13 15:11:35 2023, max compression
```

## Comparing `dagster-graphql-1.2.6.tar` & `dagster-graphql-1.2.7.tar`

### file list

```diff
@@ -1,117 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.443597 dagster-graphql-1.2.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-06 00:26:29.443597 dagster-graphql-1.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.207596 dagster-graphql-1.2.6/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.215596 dagster-graphql-1.2.6/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21641 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.287596 dagster-graphql-1.2.6/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.291596 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11579 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8860 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7594 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12620 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15390 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     7794 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10363 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.371597 dagster-graphql-1.2.6/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    12887 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18079 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16228 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    11017 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     4681 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    22897 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.371597 dagster-graphql-1.2.6/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20899 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17666 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.383597 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11072 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39733 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.387597 dagster-graphql-1.2.6/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    24881 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    35011 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4051 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.387597 dagster-graphql-1.2.6/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7971 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.443597 dagster-graphql-1.2.6/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/test/preset_query.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 00:26:29.211596 dagster-graphql-1.2.6/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-06 00:26:28.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4137 2023-04-06 00:26:29.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 00:26:28.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-06 00:26:28.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-06 00:26:28.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-06 00:26:28.000000 dagster-graphql-1.2.6/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-06 00:26:29.443597 dagster-graphql-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-05 23:51:52.000000 dagster-graphql-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.337411 dagster-graphql-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:11:35.337411 dagster-graphql-1.2.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.261411 dagster-graphql-1.2.7/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.265411 dagster-graphql-1.2.7/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21649 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.277411 dagster-graphql-1.2.7/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.281411 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11579 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12620 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15390 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10803 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.309411 dagster-graphql-1.2.7/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40174 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    14998 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18079 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16228 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    22897 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.313411 dagster-graphql-1.2.7/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20899 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17864 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.325411 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11072 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39733 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.333412 dagster-graphql-1.2.7/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    24881 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36131 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4051 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.333412 dagster-graphql-1.2.7/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29755 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.333412 dagster-graphql-1.2.7/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:11:35.261411 dagster-graphql-1.2.7/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-13 15:11:35.000000 dagster-graphql-1.2.7/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-13 15:11:35.337411 dagster-graphql-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-13 15:03:06.000000 dagster-graphql-1.2.7/setup.py
```

### Comparing `dagster-graphql-1.2.6/LICENSE` & `dagster-graphql-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/PKG-INFO` & `dagster-graphql-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.2.6
+Version: 1.2.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/cli.py` & `dagster-graphql-1.2.7/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/client/client.py` & `dagster-graphql-1.2.7/dagster_graphql/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Any, Dict, Iterable, List, Mapping, Optional
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence
 
 import dagster._check as check
 import requests.exceptions
 from dagster import DagsterRunStatus
 from dagster._annotations import public
 from dagster._core.definitions.utils import validate_tags
 from dagster._utils.backcompat import experimental_class_warning
@@ -116,18 +116,18 @@
 
     def _core_submit_execution(
         self,
         pipeline_name: str,
         repository_location_name: Optional[str] = None,
         repository_name: Optional[str] = None,
         run_config: Optional[Mapping[str, Any]] = None,
-        mode: Optional[str] = None,
+        mode: str = "default",
         preset: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
-        solid_selection: Optional[List[str]] = None,
+        solid_selection: Optional[Sequence[str]] = None,
         is_using_job_op_graph_apis: Optional[bool] = False,
     ):
         check.opt_str_param(repository_location_name, "repository_location_name")
         check.opt_str_param(repository_name, "repository_name")
         check.str_param(pipeline_name, "pipeline_name")
         check.opt_str_param(mode, "mode")
         check.opt_str_param(preset, "preset")
@@ -216,18 +216,18 @@
 
     def submit_pipeline_execution(
         self,
         pipeline_name: str,
         repository_location_name: Optional[str] = None,
         repository_name: Optional[str] = None,
         run_config: Optional[Any] = None,
-        mode: Optional[str] = None,
+        mode: str = "default",
         preset: Optional[str] = None,
         tags: Optional[Dict[str, Any]] = None,
-        solid_selection: Optional[List[str]] = None,
+        solid_selection: Optional[Sequence[str]] = None,
     ) -> str:
         """Submits a Pipeline with attached configuration for execution.
 
         Args:
             pipeline_name (str): The pipeline's name
             repository_location_name (Optional[str], optional): The name of the repository location where
                 the pipeline is located. If omitted, the client will try to infer the repository location
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.2.7/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/client/query.py` & `dagster-graphql-1.2.7/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/client/utils.py` & `dagster-graphql-1.2.7/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/events.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/external.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_schedules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.definitions.selector import (
     PipelineSelector,
     RepositorySelector,
     ScheduleSelector,
 )
-from dagster._core.scheduler.instigation import InstigatorState
+from dagster._core.scheduler.instigation import InstigatorState, InstigatorStatus
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven import get_current_datetime_in_utc, get_timestamp_from_utc_datetime
 
 from dagster_graphql.schema.util import ResolveInfo
 
 from .loader import RepositoryScopedBatchLoader
 from .utils import (
@@ -95,38 +95,49 @@
         raise UserFacingGraphQLError(GrapheneSchedulerNotDefinedError())
 
     return GrapheneScheduler(scheduler_class=instance.scheduler.__class__.__name__)
 
 
 @capture_error
 def get_schedules_or_error(
-    graphene_info: ResolveInfo, repository_selector: RepositorySelector
+    graphene_info: ResolveInfo,
+    repository_selector: RepositorySelector,
+    instigator_statuses: Optional[Set[InstigatorStatus]] = None,
 ) -> "GrapheneSchedules":
     from ..schema.schedules import GrapheneSchedule, GrapheneSchedules
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
 
     location = graphene_info.context.get_code_location(repository_selector.location_name)
     repository = location.get_repository(repository_selector.repository_name)
     batch_loader = RepositoryScopedBatchLoader(graphene_info.context.instance, repository)
     external_schedules = repository.get_external_schedules()
-    schedule_states_by_name = {
-        state.name: state
-        for state in graphene_info.context.instance.all_instigator_state(
-            repository_origin_id=repository.get_external_origin_id(),
-            repository_selector_id=repository_selector.selector_id,
-            instigator_type=InstigatorType.SCHEDULE,
-        )
-    }
+    schedule_states = graphene_info.context.instance.all_instigator_state(
+        repository_origin_id=repository.get_external_origin_id(),
+        repository_selector_id=repository_selector.selector_id,
+        instigator_type=InstigatorType.SCHEDULE,
+        instigator_statuses=instigator_statuses,
+    )
+
+    schedule_states_by_name = {state.name: state for state in schedule_states}
+    if instigator_statuses:
+        filtered = [
+            external_schedule
+            for external_schedule in external_schedules
+            if external_schedule.get_current_instigator_state(
+                schedule_states_by_name.get(external_schedule.name)
+            ).status
+            in instigator_statuses
+        ]
+    else:
+        filtered = external_schedules
 
     results = [
-        GrapheneSchedule(
-            external_schedule, schedule_states_by_name.get(external_schedule.name), batch_loader
-        )
-        for external_schedule in external_schedules
+        GrapheneSchedule(schedule, schedule_states_by_name.get(schedule.name), batch_loader)
+        for schedule in filtered
     ]
 
     return GrapheneSchedules(results=results)
 
 
 def get_schedules_for_pipeline(
     graphene_info: ResolveInfo, pipeline_selector: PipelineSelector
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_sensors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.definitions.selector import PipelineSelector, RepositorySelector, SensorSelector
-from dagster._core.scheduler.instigation import InstigatorState, SensorInstigatorData
+from dagster._core.scheduler.instigation import (
+    InstigatorState,
+    InstigatorStatus,
+    SensorInstigatorData,
+)
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven import get_current_datetime_in_utc, get_timestamp_from_utc_datetime
 
 from dagster_graphql.schema.util import ResolveInfo
 
 from .loader import RepositoryScopedBatchLoader
 from .utils import (
@@ -24,36 +28,48 @@
         GrapheneInstigationStates,
     )
     from ..schema.sensors import GrapheneSensor, GrapheneSensors, GrapheneStopSensorMutationResult
 
 
 @capture_error
 def get_sensors_or_error(
-    graphene_info: ResolveInfo, repository_selector: RepositorySelector
+    graphene_info: ResolveInfo,
+    repository_selector: RepositorySelector,
+    instigator_statuses: Optional[Set[InstigatorStatus]] = None,
 ) -> "GrapheneSensors":
     from ..schema.sensors import GrapheneSensor, GrapheneSensors
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
 
     location = graphene_info.context.get_code_location(repository_selector.location_name)
     repository = location.get_repository(repository_selector.repository_name)
     batch_loader = RepositoryScopedBatchLoader(graphene_info.context.instance, repository)
     sensors = repository.get_external_sensors()
-    sensor_states_by_name = {
-        state.name: state
-        for state in graphene_info.context.instance.all_instigator_state(
-            repository_origin_id=repository.get_external_origin_id(),
-            repository_selector_id=repository_selector.selector_id,
-            instigator_type=InstigatorType.SENSOR,
-        )
-    }
+    sensor_states = graphene_info.context.instance.all_instigator_state(
+        repository_origin_id=repository.get_external_origin_id(),
+        repository_selector_id=repository_selector.selector_id,
+        instigator_type=InstigatorType.SENSOR,
+        instigator_statuses=instigator_statuses,
+    )
+
+    sensor_states_by_name = {state.name: state for state in sensor_states}
+    if instigator_statuses:
+        filtered = [
+            sensor
+            for sensor in sensors
+            if sensor.get_current_instigator_state(sensor_states_by_name.get(sensor.name)).status
+            in instigator_statuses
+        ]
+    else:
+        filtered = sensors
+
     return GrapheneSensors(
         results=[
             GrapheneSensor(sensor, sensor_states_by_name.get(sensor.name), batch_loader)
-            for sensor in sensors
+            for sensor in filtered
         ]
     )
 
 
 @capture_error
 def get_sensor_or_error(graphene_info: ResolveInfo, selector: SensorSelector) -> "GrapheneSensor":
     from ..schema.errors import GrapheneSensorNotFoundError
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.2.7/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dagster import (
     AssetKey,
     _check as check,
 )
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.data_version import (
     NULL_DATA_VERSION,
+    StaleCauseCategory,
     StaleStatus,
 )
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.event_api import EventRecordsFilter
 from dagster._core.events import DagsterEventType
@@ -80,18 +81,22 @@
 )
 from .util import ResolveInfo, non_null_list
 
 if TYPE_CHECKING:
     from .external import GrapheneRepository
 
 GrapheneAssetStaleStatus = graphene.Enum.from_enum(StaleStatus, name="StaleStatus")
+GrapheneAssetStaleCauseCategory = graphene.Enum.from_enum(
+    StaleCauseCategory, name="StaleCauseCategory"
+)
 
 
 class GrapheneAssetStaleCause(graphene.ObjectType):
     key = graphene.NonNull(GrapheneAssetKey)
+    category = graphene.NonNull(GrapheneAssetStaleCauseCategory)
     reason = graphene.NonNull(graphene.String)
     dependency = graphene.Field(GrapheneAssetKey)
 
     class Meta:
         name = "StaleCause"
 
 
@@ -574,14 +579,15 @@
         return self.stale_status_loader.get_status(self._external_asset_node.asset_key)
 
     def resolve_staleCauses(self, graphene_info: ResolveInfo) -> Sequence[GrapheneAssetStaleCause]:
         causes = self.stale_status_loader.get_stale_root_causes(self._external_asset_node.asset_key)
         return [
             GrapheneAssetStaleCause(
                 GrapheneAssetKey(path=cause.key.path),
+                cause.category,
                 cause.reason,
                 GrapheneAssetKey(path=cause.dependency.path) if cause.dependency else None,
             )
             for cause in causes
         ]
 
     def resolve_currentDataVersion(self, graphene_info: ResolveInfo) -> Optional[str]:
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/backfill.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from typing import TYPE_CHECKING, Optional, Sequence
 
 import dagster._check as check
 import graphene
-from dagster._core.execution.backfill import BackfillPartitionsStatus, PartitionBackfill
+from dagster._core.definitions.time_window_partitions import (
+    TimeWindowPartitionsSubset,
+)
+from dagster._core.execution.backfill import (
+    BackfillPartitionsStatus,
+    BulkActionStatus,
+    PartitionBackfill,
+)
 from dagster._core.host_representation.external import ExternalPartitionSet
 from dagster._core.storage.pipeline_run import RunPartitionData, RunRecord, RunsFilter
 from dagster._core.storage.tags import BACKFILL_ID_TAG
 from dagster._core.workspace.permissions import Permissions
 
 from ..implementation.fetch_partition_sets import (
     partition_status_counts_from_run_partition_data,
@@ -25,19 +32,20 @@
     create_execution_params_error_types,
 )
 from .pipelines.config import GrapheneRunConfigValidationInvalid
 from .util import ResolveInfo, non_null_list
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.partition_sets import (
-        GrapheneAssetPartitionsStatusCounts,
         GraphenePartitionStatusCounts,
     )
 
-    from ..schema.partition_sets import GraphenePartitionSet
+    from ..schema.partition_sets import (
+        GraphenePartitionSet,
+    )
     from .pipelines.pipeline import GrapheneRun
 
 pipeline_execution_error_types = (
     GrapheneInvalidStepError,
     GrapheneInvalidOutputError,
     GrapheneRunConfigValidationInvalid,
     GraphenePipelineNotFoundError,
@@ -97,14 +105,27 @@
     FAILED = "FAILED"
     CANCELED = "CANCELED"
 
     class Meta:
         name = "BulkActionStatus"
 
 
+class GrapheneAssetBackfillData(graphene.ObjectType):
+    class Meta:
+        name = "AssetBackfillData"
+
+    assetPartitionsStatusCounts = non_null_list(
+        "dagster_graphql.schema.partition_sets.GrapheneAssetPartitionsStatusCounts"
+    )
+    rootAssetTargetedRanges = graphene.List(
+        graphene.NonNull("dagster_graphql.schema.partition_sets.GraphenePartitionKeyRange")
+    )
+    rootAssetTargetedPartitions = graphene.List(graphene.NonNull(graphene.String))
+
+
 class GraphenePartitionBackfill(graphene.ObjectType):
     class Meta:
         name = "PartitionBackfill"
 
     backfillId = graphene.NonNull(graphene.String)
     status = graphene.NonNull(GrapheneBulkActionStatus)
     partitionNames = graphene.List(graphene.NonNull(graphene.String))
@@ -112,14 +133,15 @@
     numPartitions = graphene.Field(graphene.Int)
     numCancelable = graphene.NonNull(graphene.Int)
     fromFailure = graphene.NonNull(graphene.Boolean)
     reexecutionSteps = graphene.List(graphene.NonNull(graphene.String))
     assetSelection = graphene.List(graphene.NonNull(GrapheneAssetKey))
     partitionSetName = graphene.Field(graphene.String)
     timestamp = graphene.NonNull(graphene.Float)
+    endTimestamp = graphene.Field(graphene.Float)
     partitionSet = graphene.Field("dagster_graphql.schema.partition_sets.GraphenePartitionSet")
     runs = graphene.Field(
         non_null_list("dagster_graphql.schema.pipelines.pipeline.GrapheneRun"),
         limit=graphene.Int(),
     )
     unfinishedRuns = graphene.Field(
         non_null_list("dagster_graphql.schema.pipelines.pipeline.GrapheneRun"),
@@ -128,17 +150,16 @@
     error = graphene.Field(GraphenePythonError)
     partitionStatuses = graphene.NonNull(
         "dagster_graphql.schema.partition_sets.GraphenePartitionStatuses"
     )
     partitionStatusCounts = non_null_list(
         "dagster_graphql.schema.partition_sets.GraphenePartitionStatusCounts"
     )
-    assetPartitionsStatusCounts = non_null_list(
-        "dagster_graphql.schema.partition_sets.GrapheneAssetPartitionsStatusCounts"
-    )
+    isAssetBackfill = graphene.NonNull(graphene.Boolean)
+    assetBackfillData = graphene.Field(GrapheneAssetBackfillData)
 
     hasCancelPermission = graphene.NonNull(graphene.Boolean)
     hasResumePermission = graphene.NonNull(graphene.Boolean)
 
     def __init__(self, backfill_job: PartitionBackfill):
         self._backfill_job = check.inst_param(backfill_job, "backfill_job", PartitionBackfill)
 
@@ -209,14 +230,24 @@
 
     def resolve_runs(self, graphene_info: ResolveInfo) -> "Sequence[GrapheneRun]":
         from .pipelines.pipeline import GrapheneRun
 
         records = self._get_records(graphene_info)
         return [GrapheneRun(record) for record in records]
 
+    def resolve_endTimestamp(self, graphene_info: ResolveInfo) -> Optional[float]:
+        if self._backfill_job.status == BulkActionStatus.REQUESTED:
+            # if it's still in progress then there is no end time
+            return None
+        records = self._get_records(graphene_info)
+        max_end_time = 0
+        for record in records:
+            max_end_time = max(record.end_time or 0, max_end_time)
+        return max_end_time
+
     def resolve_isValidSerialization(self, _graphene_info: ResolveInfo) -> bool:
         return self._backfill_job.is_valid_serialization(_graphene_info.context)
 
     def resolve_partitionNames(self, _graphene_info: ResolveInfo) -> Optional[Sequence[str]]:
         return self._backfill_job.get_partition_names(_graphene_info.context)
 
     def resolve_numPartitions(self, _graphene_info: ResolveInfo) -> Optional[int]:
@@ -256,19 +287,21 @@
     ) -> Sequence["GraphenePartitionStatusCounts"]:
         partition_run_data = self._get_partition_run_data(graphene_info)
         return partition_status_counts_from_run_partition_data(
             partition_run_data,
             check.not_none(self._backfill_job.get_partition_names(graphene_info.context)),
         )
 
-    def resolve_assetPartitionsStatusCounts(
-        self, graphene_info: ResolveInfo
-    ) -> Sequence["GrapheneAssetPartitionsStatusCounts"]:
+    def resolve_isAssetBackfill(self, _graphene_info: ResolveInfo) -> bool:
+        return self._backfill_job.is_asset_backfill
+
+    def resolve_assetBackfillData(self, graphene_info: ResolveInfo) -> GrapheneAssetBackfillData:
         from dagster_graphql.schema.partition_sets import (
             GrapheneAssetPartitionsStatusCounts,
+            GraphenePartitionKeyRange,
         )
 
         status_counts_by_asset = (
             self._backfill_job.get_partitions_status_counts_and_totals_by_asset(
                 graphene_info.context
             )
         )
@@ -283,15 +316,36 @@
                     numPartitionsTargeted=partitions_counts[1],
                     numPartitionsRequested=counts_by_status[BackfillPartitionsStatus.REQUESTED],
                     numPartitionsCompleted=counts_by_status[BackfillPartitionsStatus.COMPLETED],
                     numPartitionsFailed=counts_by_status[BackfillPartitionsStatus.FAILED],
                 )
             )
 
-        return asset_partition_status_counts
+        root_partitions_subset = self._backfill_job.get_target_root_partitions_subset(
+            graphene_info.context
+        )
+
+        if not root_partitions_subset:
+            root_targeted_ranges = None
+            root_targeted_partitions = None
+        elif isinstance(root_partitions_subset, TimeWindowPartitionsSubset):
+            root_targeted_ranges = [
+                GraphenePartitionKeyRange(start, end)
+                for start, end in root_partitions_subset.get_partition_key_ranges()
+            ]
+            root_targeted_partitions = None
+        else:  # Default partitions subset
+            root_targeted_ranges = None
+            root_targeted_partitions = root_partitions_subset.get_partition_keys()
+
+        return GrapheneAssetBackfillData(
+            assetPartitionsStatusCounts=asset_partition_status_counts,
+            rootAssetTargetedRanges=root_targeted_ranges,
+            rootAssetTargetedPartitions=root_targeted_partitions,
+        )
 
     def resolve_error(self, _graphene_info: ResolveInfo) -> Optional[GraphenePythonError]:
         if self._backfill_job.error:
             return GraphenePythonError(self._backfill_job.error)
         return None
 
     def resolve_hasCancelPermission(self, graphene_info: ResolveInfo) -> bool:
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/errors.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/execution.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/external.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/instance.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/partition_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,22 @@
     assetKey = graphene.NonNull(GrapheneAssetKey)
     numPartitionsTargeted = graphene.NonNull(graphene.Int)
     numPartitionsRequested = graphene.NonNull(graphene.Int)
     numPartitionsCompleted = graphene.NonNull(graphene.Int)
     numPartitionsFailed = graphene.NonNull(graphene.Int)
 
 
+class GraphenePartitionKeyRange(graphene.ObjectType):
+    class Meta:
+        name = "PartitionKeyRange"
+
+    start = graphene.NonNull(graphene.String)
+    end = graphene.NonNull(graphene.String)
+
+
 class GraphenePartitionTagsOrError(graphene.Union):
     class Meta:
         types = (GraphenePartitionTags, GraphenePythonError)
         name = "PartitionTagsOrError"
 
 
 class GraphenePartition(graphene.ObjectType):
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/resources.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     RepositorySelector,
     ResourceSelector,
     ScheduleSelector,
     SensorSelector,
 )
 from dagster._core.execution.backfill import BulkActionStatus
 from dagster._core.nux import get_has_seen_nux
-from dagster._core.scheduler.instigation import InstigatorType
+from dagster._core.scheduler.instigation import InstigatorStatus, InstigatorType
 
 from dagster_graphql.implementation.fetch_env_vars import get_utilized_env_vars_or_error
 from dagster_graphql.implementation.fetch_logs import get_captured_log_metadata
 from dagster_graphql.implementation.fetch_runs import get_assets_latest_info
 from dagster_graphql.schema.env_vars import GrapheneEnvVarWithConsumersListOrError
 
 from ...implementation.external import (
@@ -103,14 +103,15 @@
     GrapheneScheduleSelector,
     GrapheneSensorSelector,
 )
 from ..instance import GrapheneInstance
 from ..instigation import (
     GrapheneInstigationStateOrError,
     GrapheneInstigationStatesOrError,
+    GrapheneInstigationStatus,
     GrapheneInstigationType,
 )
 from ..logs.compute_logs import (
     GrapheneCapturedLogs,
     GrapheneCapturedLogsMetadata,
     from_captured_log_data,
 )
@@ -204,14 +205,15 @@
         schedule_selector=graphene.NonNull(GrapheneScheduleSelector),
         description="Retrieve a schedule by its location name, repository name, and schedule name.",
     )
 
     schedulesOrError = graphene.Field(
         graphene.NonNull(GrapheneSchedulesOrError),
         repositorySelector=graphene.NonNull(GrapheneRepositorySelector),
+        scheduleStatus=graphene.Argument(GrapheneInstigationStatus),
         description="Retrieve all the schedules.",
     )
 
     topLevelResourceDetailsOrError = graphene.Field(
         graphene.NonNull(GrapheneResourceDetailsOrError),
         resourceSelector=graphene.NonNull(GrapheneResourceSelector),
         description=(
@@ -236,14 +238,15 @@
         graphene.NonNull(GrapheneSensorOrError),
         sensorSelector=graphene.NonNull(GrapheneSensorSelector),
         description="Retrieve a sensor by its location name, repository name, and sensor name.",
     )
     sensorsOrError = graphene.Field(
         graphene.NonNull(GrapheneSensorsOrError),
         repositorySelector=graphene.NonNull(GrapheneRepositorySelector),
+        sensorStatus=graphene.Argument(GrapheneInstigationStatus),
         description="Retrieve all the sensors.",
     )
 
     instigationStateOrError = graphene.Field(
         graphene.NonNull(GrapheneInstigationStateOrError),
         instigationSelector=graphene.NonNull(GrapheneInstigationSelector),
         description=(
@@ -525,19 +528,30 @@
         self, graphene_info: ResolveInfo, schedule_selector: GrapheneScheduleSelector
     ):
         return get_schedule_or_error(
             graphene_info, ScheduleSelector.from_graphql_input(schedule_selector)
         )
 
     def resolve_schedulesOrError(
-        self, graphene_info: ResolveInfo, repositorySelector: GrapheneRepositorySelector
+        self,
+        graphene_info: ResolveInfo,
+        repositorySelector: GrapheneRepositorySelector,
+        scheduleStatus: Optional[GrapheneInstigationStatus] = None,
     ):
+        if scheduleStatus == GrapheneInstigationStatus.RUNNING:
+            instigator_statuses = {InstigatorStatus.RUNNING, InstigatorStatus.AUTOMATICALLY_RUNNING}
+        elif scheduleStatus == GrapheneInstigationStatus.STOPPED:
+            instigator_statuses = {InstigatorStatus.STOPPED}
+        else:
+            instigator_statuses = None
+
         return get_schedules_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
+            instigator_statuses,
         )
 
     def resolve_topLevelResourceDetailsOrError(self, graphene_info: ResolveInfo, resourceSelector):
         return get_resource_or_error(
             graphene_info, ResourceSelector.from_graphql_input(resourceSelector)
         )
 
@@ -554,18 +568,30 @@
         )
 
     def resolve_sensorOrError(
         self, graphene_info: ResolveInfo, sensorSelector: GrapheneRepositorySelector
     ):
         return get_sensor_or_error(graphene_info, SensorSelector.from_graphql_input(sensorSelector))
 
-    def resolve_sensorsOrError(self, graphene_info, repositorySelector: GrapheneRepositorySelector):
+    def resolve_sensorsOrError(
+        self,
+        graphene_info,
+        repositorySelector: GrapheneRepositorySelector,
+        sensorStatus: Optional[GrapheneInstigationStatus] = None,
+    ):
+        if sensorStatus == GrapheneInstigationStatus.RUNNING:
+            instigator_statuses = {InstigatorStatus.RUNNING, InstigatorStatus.AUTOMATICALLY_RUNNING}
+        elif sensorStatus == GrapheneInstigationStatus.STOPPED:
+            instigator_statuses = {InstigatorStatus.STOPPED}
+        else:
+            instigator_statuses = None
         return get_sensors_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
+            instigator_statuses,
         )
 
     def resolve_instigationStateOrError(
         self, graphene_info: ResolveInfo, instigationSelector: GrapheneInstigationSelector
     ):
         return get_instigator_state_or_error(
             graphene_info, InstigatorSelector.from_graphql_input(instigationSelector)
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/runs.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/solids.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/table.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/tags.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/schema/util.py` & `dagster-graphql-1.2.7/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.2.6/dagster_graphql/test/utils.py` & `dagster-graphql-1.2.7/dagster_graphql/test/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,60 @@
 import asyncio
 from contextlib import contextmanager
+from typing import Any, Dict, Iterator, Mapping, Optional, Sequence
 
 import dagster._check as check
+from dagster._core.host_representation.external import ExternalRepository
 from dagster._core.instance import DagsterInstance
 from dagster._core.test_utils import wait_for_runs_to_finish
-from dagster._core.workspace.context import WorkspaceProcessContext
+from dagster._core.workspace.context import WorkspaceProcessContext, WorkspaceRequestContext
 from dagster._core.workspace.load_target import PythonFileTarget
+from typing_extensions import Protocol, TypeAlias, TypedDict
 
 from dagster_graphql.schema import create_schema
 
 
-def main_repo_location_name():
+class GqlResult(Protocol):
+    @property
+    def data(self) -> Mapping[str, Any]:
+        ...
+
+    @property
+    def errors(self) -> Optional[Sequence[str]]:
+        ...
+
+
+Selector: TypeAlias = Dict[str, Any]
+
+GqlVariables: TypeAlias = Mapping[str, Any]
+
+
+class GqlTag(TypedDict):
+    key: str
+    value: str
+
+
+class GqlAssetKey(TypedDict):
+    path: Sequence[str]
+
+
+def main_repo_location_name() -> str:
     return "test_location"
 
 
-def main_repo_name():
+def main_repo_name() -> str:
     return "test_repo"
 
 
 SCHEMA = create_schema()
 
 
-def execute_dagster_graphql(context, query, variables=None):
+def execute_dagster_graphql(
+    context: WorkspaceRequestContext, query: str, variables: Optional[GqlVariables] = None
+) -> GqlResult:
     result = SCHEMA.execute(
         query,
         context_value=context,
         variable_values=variables,
     )
 
     if result.errors:
@@ -35,18 +64,18 @@
 
         raise result.errors[0]
 
     return result
 
 
 def execute_dagster_graphql_subscription(
-    context,
-    query,
-    variables=None,
-):
+    context: WorkspaceRequestContext,
+    query: str,
+    variables: Optional[GqlVariables] = None,
+) -> Sequence[GqlResult]:
     results = []
 
     subscription = SCHEMA.subscribe(
         query,
         context_value=context,
         variable_values=variables,
     )
@@ -59,57 +88,63 @@
             break
 
     asyncio.run(_process())
 
     return results
 
 
-def execute_dagster_graphql_and_finish_runs(context, query, variables=None):
+def execute_dagster_graphql_and_finish_runs(
+    context: WorkspaceRequestContext, query: str, variables: Optional[GqlVariables] = None
+) -> GqlResult:
     result = execute_dagster_graphql(context, query, variables)
     wait_for_runs_to_finish(context.instance, timeout=30)
     return result
 
 
 @contextmanager
-def define_out_of_process_context(python_file, fn_name, instance, read_only=False):
+def define_out_of_process_context(
+    python_file: str, fn_name: str, instance: DagsterInstance, read_only: bool = False
+) -> Iterator[WorkspaceRequestContext]:
     check.inst_param(instance, "instance", DagsterInstance)
 
     with define_out_of_process_workspace(
         python_file, fn_name, instance, read_only=read_only
     ) as workspace_process_context:
         yield workspace_process_context.create_request_context()
 
 
-def define_out_of_process_workspace(python_file, fn_name, instance, read_only=False):
+def define_out_of_process_workspace(
+    python_file: str, fn_name: str, instance: DagsterInstance, read_only: bool = False
+) -> WorkspaceProcessContext:
     return WorkspaceProcessContext(
         instance,
         PythonFileTarget(
             python_file=python_file,
             attribute=fn_name,
             working_directory=None,
             location_name=main_repo_location_name(),
         ),
         version="",
         read_only=read_only,
     )
 
 
-def infer_repository(graphql_context):
+def infer_repository(graphql_context: WorkspaceRequestContext) -> ExternalRepository:
     if len(graphql_context.code_locations) == 1:
         # This is to account for having a single in process repository
         code_location = graphql_context.code_locations[0]
         repositories = code_location.get_repositories()
         assert len(repositories) == 1
         return next(iter(repositories.values()))
 
     code_location = graphql_context.get_code_location("test")
     return code_location.get_repository("test_repo")
 
 
-def infer_repository_selector(graphql_context):
+def infer_repository_selector(graphql_context: WorkspaceRequestContext) -> Selector:
     if len(graphql_context.code_locations) == 1:
         # This is to account for having a single in process repository
         code_location = graphql_context.code_locations[0]
         repositories = code_location.get_repositories()
         assert len(repositories) == 1
         repository = next(iter(repositories.values()))
     else:
@@ -119,60 +154,62 @@
     return {
         "repositoryLocationName": code_location.name,
         "repositoryName": repository.name,
     }
 
 
 def infer_job_or_pipeline_selector(
-    graphql_context,
-    pipeline_name,
-    solid_selection=None,
-    asset_selection=None,
-):
+    graphql_context: WorkspaceRequestContext,
+    pipeline_name: str,
+    solid_selection: Optional[Sequence[str]] = None,
+    asset_selection: Optional[Sequence[GqlAssetKey]] = None,
+) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update(
         {
             "pipelineName": pipeline_name,
             "solidSelection": solid_selection,
             "assetSelection": asset_selection,
         }
     )
     return selector
 
 
 def infer_pipeline_selector(
-    graphql_context,
-    pipeline_name,
-    solid_selection=None,
-):
+    graphql_context: WorkspaceRequestContext,
+    pipeline_name: str,
+    solid_selection: Optional[Sequence[str]] = None,
+) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update(
         {
             "pipelineName": pipeline_name,
             "solidSelection": solid_selection,
         }
     )
     return selector
 
 
-def infer_schedule_selector(graphql_context, schedule_name):
+def infer_schedule_selector(
+    graphql_context: WorkspaceRequestContext, schedule_name: str
+) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update({"scheduleName": schedule_name})
     return selector
 
 
-def infer_sensor_selector(graphql_context, sensor_name):
+def infer_sensor_selector(graphql_context: WorkspaceRequestContext, sensor_name: str) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update({"sensorName": sensor_name})
     return selector
 
 
-def infer_instigation_selector(graphql_context, name):
+def infer_instigation_selector(graphql_context: WorkspaceRequestContext, name: str) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update({"name": name})
     return selector
 
 
-def infer_resource_selector(graphql_context, name):
+def infer_resource_selector(graphql_context: WorkspaceRequestContext, name: str) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector = {**selector, **{"resourceName": name}}
     return selector
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.2.7/dagster_graphql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.2.6
+Version: 1.2.7
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.2.6/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.2.7/dagster_graphql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,9 +96,8 @@
 dagster_graphql/schema/roots/pipeline.py
 dagster_graphql/schema/roots/query.py
 dagster_graphql/schema/roots/subscription.py
 dagster_graphql/schema/schedules/__init__.py
 dagster_graphql/schema/schedules/schedules.py
 dagster_graphql/schema/schedules/ticks.py
 dagster_graphql/test/__init__.py
-dagster_graphql/test/preset_query.py
 dagster_graphql/test/utils.py
```

### Comparing `dagster-graphql-1.2.6/setup.py` & `dagster-graphql-1.2.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.2.6",
+        "dagster==1.2.7",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

