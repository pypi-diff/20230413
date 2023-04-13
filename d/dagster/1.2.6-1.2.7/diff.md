# Comparing `tmp/dagster-1.2.6.tar.gz` & `tmp/dagster-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.2.6.tar", last modified: Wed Apr  5 23:52:13 2023, max compression
+gzip compressed data, was "dagster-1.2.7.tar", last modified: Thu Apr 13 15:03:47 2023, max compression
```

## Comparing `dagster-1.2.6.tar` & `dagster-1.2.7.tar`

### file list

```diff
@@ -1,622 +1,622 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.258597 dagster-1.2.6/
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-05 23:51:52.000000 dagster-1.2.6/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-05 23:51:52.000000 dagster-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-05 23:51:52.000000 dagster-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-05 23:52:13.258597 dagster-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-04-05 23:51:52.000000 dagster-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.186596 dagster-1.2.6/dagster/
--rw-r--r--   0 root         (0) root         (0)    24981 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.186596 dagster-1.2.6/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.186596 dagster-1.2.6/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.190596 dagster-1.2.6/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27129 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8207 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    34000 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5141 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.190596 dagster-1.2.6/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28499 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.190596 dagster-1.2.6/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16840 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.190596 dagster-1.2.6/dagster/_config/structured_config/
--rw-r--r--   0 root         (0) root         (0)    39294 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/structured_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/structured_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/structured_config/utils.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.194596 dagster-1.2.6/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.194596 dagster-1.2.6/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.206596 dagster-1.2.6/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7855 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27488 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10380 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)    22609 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_group.py
--rw-r--r--   0 root         (0) root         (0)     3817 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36853 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    41014 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    16079 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    56324 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    23019 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)    15009 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45721 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10877 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    15333 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.210596 dagster-1.2.6/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      682 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39361 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9563 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10261 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17663 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9674 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/pipeline_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14491 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8199 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11709 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    21501 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39915 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    33816 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21562 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     8507 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8001 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    15897 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22927 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)    46388 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    16650 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.210596 dagster-1.2.6/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    33294 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/mode.py
--rw-r--r--   0 root         (0) root         (0)    54997 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    21053 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11938 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     7844 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    16158 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)    18931 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    43072 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    34900 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/pipeline_definition.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)     9054 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/preset.py
--rw-r--r--   0 root         (0) root         (0)    30684 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.210596 dagster-1.2.6/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    23982 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    19566 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    19048 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1166 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8118 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    25150 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    10663 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    35086 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    32936 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    37087 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    12300 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    73361 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15845 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    23017 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.210596 dagster-1.2.6/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    65013 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.214596 dagster-1.2.6/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53159 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    24028 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    13610 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6082 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.214596 dagster-1.2.6/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22487 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    27186 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27386 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    34437 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    43180 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    20099 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/context_creation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     6480 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/execute_job_result.py
--rw-r--r--   0 root         (0) root         (0)     8518 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8734 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.218596 dagster-1.2.6/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23056 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7095 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12509 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16478 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27421 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10256 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    38667 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    60978 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15617 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    16031 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19527 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)    25987 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/results.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4175 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.218596 dagster-1.2.6/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15452 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.218596 dagster-1.2.6/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14347 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.218596 dagster-1.2.6/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33996 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    33186 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    68293 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4341 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)    17336 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     5205 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/pipeline_index.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104096 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11309 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24286 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17104 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    18194 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.222596 dagster-1.2.6/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.226596 dagster-1.2.6/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4019 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12052 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14447 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)    17447 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/snap/pipeline_snapshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.230596 dagster-1.2.6/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.230596 dagster-1.2.6/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.238597 dagster-1.2.6/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.238597 dagster-1.2.6/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16259 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)    11527 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14277 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    77841 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7409 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18916 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)     9985 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26021 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17376 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23190 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)    23993 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/pipeline_run.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16059 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8629 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46758 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19274 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.242596 dagster-1.2.6/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3660 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14835 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15908 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    25557 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    16949 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7393 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35947 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2839 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/utility_solids.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5451 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26703 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9084 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4422 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17377 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5781 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    34426 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.246596 dagster-1.2.6/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.182596 dagster-1.2.6/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11665 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38179 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18538 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22483 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    52578 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26100 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)     1144 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.250597 dagster-1.2.6/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.254597 dagster-1.2.6/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32009 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.254597 dagster-1.2.6/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    33924 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.254597 dagster-1.2.6/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.254597 dagster-1.2.6/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.258597 dagster-1.2.6/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23212 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    20449 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    11070 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.258597 dagster-1.2.6/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    17259 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    22948 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.258597 dagster-1.2.6/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-05 23:51:52.000000 dagster-1.2.6/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 23:52:13.186596 dagster-1.2.6/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24861 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1290 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-05 23:52:13.000000 dagster-1.2.6/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-05 23:52:13.262597 dagster-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6429 2023-04-05 23:51:52.000000 dagster-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-13 15:03:06.000000 dagster-1.2.7/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:06.000000 dagster-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-13 15:03:06.000000 dagster-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-13 15:03:47.032711 dagster-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-04-13 15:03:06.000000 dagster-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/
+-rw-r--r--   0 root         (0) root         (0)    24945 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27129 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8207 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    33891 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5141 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28486 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14686 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18799 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16840 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_config/structured_config/
+-rw-r--r--   0 root         (0) root         (0)    47857 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.976711 dagster-1.2.7/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.976711 dagster-1.2.7/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7829 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28701 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10380 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)    22609 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_group.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36853 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    43705 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    16164 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    57573 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    23019 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45721 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10877 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20631 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    15887 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10261 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17814 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14491 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8349 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11709 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    21501 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    33816 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21562 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10087 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8001 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15897 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44446 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22927 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)    46465 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    16650 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    33294 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/mode.py
+-rw-r--r--   0 root         (0) root         (0)    54997 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    21053 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    20633 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18471 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    44315 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    34900 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/pipeline_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9054 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/preset.py
+-rw-r--r--   0 root         (0) root         (0)    30644 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    23982 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    19566 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    19180 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8118 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    25150 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14761 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    35086 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    32988 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    41375 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    13809 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    73361 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    65032 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.992711 dagster-1.2.7/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41958 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    25196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6082 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.992711 dagster-1.2.7/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22487 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    27186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34437 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    43261 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    20099 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context_creation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_job_result.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8734 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14650 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23056 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7095 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12509 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27421 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10255 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    38667 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    60978 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15617 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    16031 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19527 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)    25987 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/results.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4175 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15452 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14347 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33996 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    33186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    69236 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)    17332 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/pipeline_index.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   103980 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11309 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24286 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17327 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18194 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20631 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.004711 dagster-1.2.7/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4019 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12052 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14447 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)    17447 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/pipeline_snapshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.008711 dagster-1.2.7/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.008711 dagster-1.2.7/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8073 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16259 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)    11527 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    77841 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18916 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9985 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26222 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17376 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23190 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)    23993 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/pipeline_run.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16059 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46758 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15907 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27288 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18680 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7393 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35947 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/utility_solids.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5451 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26703 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9084 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17377 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8371 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    35694 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.964711 dagster-1.2.7/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11665 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38179 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    22252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    52644 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26106 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32009 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    33924 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23212 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    23709 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10483 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    23902 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24855 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-13 15:03:47.032711 dagster-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-04-13 15:03:07.000000 dagster-1.2.7/setup.py
```

### Comparing `dagster-1.2.6/COPYING` & `dagster-1.2.7/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/LICENSE` & `dagster-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/PKG-INFO` & `dagster-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.2.6
+Version: 1.2.7
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.2.6/README.md` & `dagster-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/__init__.py` & `dagster-1.2.7/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-from types import ModuleType
 
 from . import _module_alias_map
 
 # Imports of a key will return the module named by the corresponding value.
 sys.meta_path.insert(
     _module_alias_map.get_meta_path_insertion_index(),
     _module_alias_map.AliasedModuleFinder(
@@ -288,15 +287,15 @@
     reconstructable as reconstructable,
 )
 from dagster._core.definitions.repository_definition import (
     RepositoryData as RepositoryData,
     RepositoryDefinition as RepositoryDefinition,
 )
 from dagster._core.definitions.resource_annotation import (
-    Resource as Resource,
+    ResourceParam as ResourceParam,
 )
 from dagster._core.definitions.resource_definition import (
     ResourceDefinition as ResourceDefinition,
     make_values_resource as make_values_resource,
     resource as resource,
 )
 from dagster._core.definitions.run_config import RunConfig as RunConfig
@@ -575,9 +574,9 @@
         stacklevel = 3 if sys.version_info >= (3, 7) else 4
         rename_warning(value.__name__, name, breaking_version, stacklevel=stacklevel)
         return value
     else:
         raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
 
 
-def __dir__(_self: ModuleType) -> Sequence[str]:
+def __dir__() -> Sequence[str]:
     return [*globals(), *_DEPRECATED.keys(), *_DEPRECATED_RENAMED.keys()]
```

### Comparing `dagster-1.2.6/dagster/_annotations.py` & `dagster-1.2.7/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/get_server_id.py` & `dagster-1.2.7/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/list_repositories.py` & `dagster-1.2.7/dagster/_api/list_repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import TYPE_CHECKING, Optional
 
 import dagster._check as check
 from dagster._core.errors import DagsterUserCodeProcessError
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
-from dagster._grpc.types import ListRepositoriesResponse
 from dagster._serdes import deserialize_value
 from dagster._utils.error import SerializableErrorInfo
 
 if TYPE_CHECKING:
     from dagster._grpc.client import DagsterGrpcClient
+    from dagster._grpc.types import ListRepositoriesResponse
 
 
-def sync_list_repositories_grpc(api_client: "DagsterGrpcClient") -> ListRepositoriesResponse:
+def sync_list_repositories_grpc(api_client: "DagsterGrpcClient") -> "ListRepositoriesResponse":
     from dagster._grpc.client import DagsterGrpcClient
+    from dagster._grpc.types import ListRepositoriesResponse
 
     check.inst_param(api_client, "api_client", DagsterGrpcClient)
     result = deserialize_value(
         api_client.list_repositories(),
         (ListRepositoriesResponse, SerializableErrorInfo),
     )
     if isinstance(result, SerializableErrorInfo):
@@ -30,15 +31,15 @@
 def sync_list_repositories_ephemeral_grpc(
     executable_path: str,
     python_file: Optional[str],
     module_name: Optional[str],
     working_directory: Optional[str],
     attribute: Optional[str],
     package_name: Optional[str],
-) -> ListRepositoriesResponse:
+) -> "ListRepositoriesResponse":
     from dagster._grpc.client import ephemeral_grpc_api_client
 
     check.str_param(executable_path, "executable_path")
     check.opt_str_param(python_file, "python_file")
     check.opt_str_param(module_name, "module_name")
     check.opt_str_param(working_directory, "working_directory")
     check.opt_str_param(attribute, "attribute")
```

### Comparing `dagster-1.2.6/dagster/_api/notebook_data.py` & `dagster-1.2.7/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/snapshot_execution_plan.py` & `dagster-1.2.7/dagster/_api/snapshot_execution_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, FrozenSet, Mapping, Optional, Sequence
+from typing import TYPE_CHECKING, AbstractSet, Any, Mapping, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterUserCodeProcessError
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.host_representation.origin import ExternalPipelineOrigin
 from dagster._core.instance import DagsterInstance
@@ -19,15 +19,15 @@
 
 def sync_get_external_execution_plan_grpc(
     api_client: "DagsterGrpcClient",
     pipeline_origin: ExternalPipelineOrigin,
     run_config: Mapping[str, Any],
     mode: str,
     pipeline_snapshot_id: str,
-    asset_selection: Optional[FrozenSet[AssetKey]] = None,
+    asset_selection: Optional[AbstractSet[AssetKey]] = None,
     solid_selection: Optional[Sequence[str]] = None,
     step_keys_to_execute: Optional[Sequence[str]] = None,
     known_state: Optional[KnownExecutionState] = None,
     instance: Optional[DagsterInstance] = None,
 ) -> ExecutionPlanSnapshot:
     from dagster._grpc.client import DagsterGrpcClient
```

### Comparing `dagster-1.2.6/dagster/_api/snapshot_partition.py` & `dagster-1.2.7/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/snapshot_pipeline.py` & `dagster-1.2.7/dagster/_api/snapshot_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/snapshot_repository.py` & `dagster-1.2.7/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/snapshot_schedule.py` & `dagster-1.2.7/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_api/snapshot_sensor.py` & `dagster-1.2.7/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_check/README.md` & `dagster-1.2.7/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_check/__init__.py` & `dagster-1.2.7/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/__init__.py` & `dagster-1.2.7/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/api.py` & `dagster-1.2.7/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/asset.py` & `dagster-1.2.7/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/config_scaffolder.py` & `dagster-1.2.7/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/debug.py` & `dagster-1.2.7/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/dev.py` & `dagster-1.2.7/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/instance.py` & `dagster-1.2.7/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/job.py` & `dagster-1.2.7/dagster/_cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     get_job_python_origin_from_kwargs,
     get_workspace_from_kwargs,
     job_repository_target_argument,
     job_target_argument,
     python_job_config_argument,
     python_job_target_argument,
 )
-from dagster._core.definitions.pipeline_base import IPipeline
+from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.definitions.utils import validate_tags
 from dagster._core.errors import DagsterBackfillFailedError, DagsterInvariantViolationError
-from dagster._core.execution.api import create_execution_plan
+from dagster._core.execution.api import create_execution_plan, execute_job
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
+from dagster._core.execution.execution_result import ExecutionResult
 from dagster._core.execution.job_backfill import create_backfill_run
-from dagster._core.execution.results import PipelineExecutionResult
 from dagster._core.host_representation import (
     CodeLocation,
     ExternalPipeline,
     ExternalRepository,
     RepositoryHandle,
 )
 from dagster._core.host_representation.external_data import (
@@ -48,15 +48,15 @@
 from dagster._core.instance import DagsterInstance
 from dagster._core.snap import NodeInvocationSnap, PipelineSnapshot
 from dagster._core.storage.pipeline_run import DagsterRun
 from dagster._core.storage.tags import MEMOIZED_RUN_TAG
 from dagster._core.telemetry import log_external_repo_stats, telemetry_wrapper
 from dagster._core.utils import make_new_backfill_id
 from dagster._core.workspace.workspace import IWorkspace
-from dagster._legacy import PipelineDefinition, execute_pipeline
+from dagster._legacy import PipelineDefinition
 from dagster._seven import IS_WINDOWS, JSONDecodeError, json
 from dagster._utils import DEFAULT_WORKSPACE_YAML_FILENAME, PrintFn
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_pipeline_from_origin
 from dagster._utils.indenting_printer import IndentingPrinter
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.merger import merge_dicts
@@ -313,34 +313,32 @@
 def job_execute_command(**kwargs: ClickArgValue):
     with capture_interrupts():
         with get_instance_for_service("``dagster job execute``") as instance:
             execute_execute_command(instance, kwargs)
 
 
 @telemetry_wrapper
-def execute_execute_command(
-    instance: DagsterInstance, kwargs: ClickArgMapping
-) -> PipelineExecutionResult:
+def execute_execute_command(instance: DagsterInstance, kwargs: ClickArgMapping) -> ExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
     config = list(
         check.opt_tuple_param(cast(Tuple[str, ...], kwargs.get("config")), "config", of_type=str)
     )
     preset = cast(Optional[str], kwargs.get("preset"))
-    mode = cast(Optional[str], kwargs.get("mode"))
+    cast(Optional[str], kwargs.get("mode"))
 
     if preset and config:
         raise click.UsageError("Can not use --preset with --config.")
 
     tags = get_tags_from_args(kwargs)
 
     pipeline_origin = get_job_python_origin_from_kwargs(kwargs)
     pipeline = recon_pipeline_from_origin(pipeline_origin)
     solid_selection = get_solid_selection_from_args(kwargs)
-    result = do_execute_command(pipeline, instance, config, mode, tags, solid_selection, preset)
+    result = do_execute_command(pipeline, instance, config, tags, solid_selection)
 
     if not result.success:
         raise click.ClickException(f"Pipeline run {result.run_id} resulted in failure.")
 
     return result
 
 
@@ -394,36 +392,33 @@
     if not isinstance(solid_selection_str, str):
         return None
 
     return [ele.strip() for ele in solid_selection_str.split(",")] if solid_selection_str else None
 
 
 def do_execute_command(
-    pipeline: IPipeline,
+    recon_job: ReconstructableJob,
     instance: DagsterInstance,
     config: Optional[Sequence[str]],
-    mode: Optional[str] = None,
     tags: Optional[Mapping[str, str]] = None,
-    solid_selection: Optional[Sequence[str]] = None,
-    preset: Optional[str] = None,
-) -> PipelineExecutionResult:
-    check.inst_param(pipeline, "pipeline", IPipeline)
+    op_selection: Optional[Sequence[str]] = None,
+) -> ExecutionResult:
+    check.inst_param(recon_job, "recon_job", ReconstructableJob)
     check.inst_param(instance, "instance", DagsterInstance)
     check.opt_sequence_param(config, "config", of_type=str)
 
-    return execute_pipeline(
-        pipeline,
+    with execute_job(
+        recon_job,
         run_config=get_run_config_from_file_list(config),
-        mode=mode,
         tags=tags,
         instance=instance,
         raise_on_error=False,
-        solid_selection=solid_selection,
-        preset=preset,
-    )
+        op_selection=op_selection,
+    ) as result:
+        return result
 
 
 @job_cli.command(
     name="launch",
     help=(
         "Launch a job using the run launcher configured on the Dagster instance.\n\n{instructions}"
         .format(instructions=get_job_instructions("launch"))
```

### Comparing `dagster-1.2.6/dagster/_cli/load_handle.py` & `dagster-1.2.7/dagster/_cli/load_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 
 import dagster._check as check
 from dagster._cli.workspace.cli_target import get_working_directory_from_kwargs
 from dagster._core.definitions.reconstruct import ReconstructableRepository
 
 
 def _cli_load_invariant(condition, msg=None):
-    msg = (
-        msg
-        or "Invalid set of CLI arguments for loading repository/pipeline. See --help for details."
-    )
+    msg = msg or "Invalid set of CLI arguments for loading repository/job. See --help for details."
     if not condition:
         raise UsageError(msg)
 
 
 def recon_repo_for_cli_args(kwargs: Mapping[str, str]):
     """Builds a ReconstructableRepository for CLI arguments, which can be any of the combinations
     for repo loading above.
```

### Comparing `dagster-1.2.6/dagster/_cli/project.py` & `dagster-1.2.7/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/run.py` & `dagster-1.2.7/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/schedule.py` & `dagster-1.2.7/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/sensor.py` & `dagster-1.2.7/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/utils.py` & `dagster-1.2.7/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_cli/workspace/cli_target.py` & `dagster-1.2.7/dagster/_cli/workspace/cli_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 ClickArgValue: TypeAlias = Union[str, Tuple[str]]
 ClickArgMapping: TypeAlias = Mapping[str, ClickArgValue]
 ClickOption: TypeAlias = Callable[[T_Callable], T_Callable]
 
 
 def _raise_cli_usage_error(msg: Optional[str] = None) -> Never:
     raise UsageError(
-        msg
-        or "Invalid set of CLI arguments for loading repository/pipeline. See --help for details."
+        msg or "Invalid set of CLI arguments for loading repository/job. See --help for details."
     )
 
 
 def _check_cli_arguments_none(kwargs: ClickArgMapping, *keys: str) -> None:
     for key in keys:
         if kwargs.get(key):
             _raise_cli_usage_error()
```

### Comparing `dagster-1.2.6/dagster/_config/__init__.py` & `dagster-1.2.7/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/config_schema.py` & `dagster-1.2.7/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/config_type.py` & `dagster-1.2.7/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/errors.py` & `dagster-1.2.7/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/evaluate_value_result.py` & `dagster-1.2.7/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/field.py` & `dagster-1.2.7/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/field_utils.py` & `dagster-1.2.7/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/post_process.py` & `dagster-1.2.7/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/primitive_mapping.py` & `dagster-1.2.7/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/snap.py` & `dagster-1.2.7/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/source.py` & `dagster-1.2.7/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/stack.py` & `dagster-1.2.7/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/structured_config/__init__.py` & `dagster-1.2.7/dagster/_config/structured_config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,35 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from pydantic import ConstrainedFloat, ConstrainedInt, ConstrainedStr
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, get_args
 
 from dagster import Enum as DagsterEnum
 from dagster._annotations import experimental
 from dagster._config.config_type import Array, ConfigFloatInstance, ConfigType, EnumValue, Noneable
 from dagster._config.field_utils import config_dictionary_from_values
 from dagster._config.post_process import resolve_defaults
 from dagster._config.source import BoolSource, IntSource, StringSource
 from dagster._config.structured_config.typing_utils import TypecheckAllowPartialResourceInitParams
 from dagster._config.validate import process_config, validate_config
+from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.definition_config_schema import (
     ConfiguredDefinitionConfigSchema,
     DefinitionConfigSchema,
 )
-from dagster._core.errors import DagsterInvalidConfigError
+from dagster._core.errors import (
+    DagsterInvalidConfigDefinitionError,
+    DagsterInvalidConfigError,
+    DagsterInvalidDefinitionError,
+    DagsterInvalidPythonicConfigDefinitionError,
+)
 from dagster._core.execution.context.init import InitResourceContext
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
 except ImportError:
 
     class cached_property:
@@ -139,14 +145,19 @@
                 continue
             if field:
                 output[field.alias] = value
             else:
                 output[key] = value
         return output
 
+    @classmethod
+    def to_config_schema(cls) -> DefinitionConfigSchema:
+        """Converts the config structure represented by this class into a DefinitionConfigSchema."""
+        return DefinitionConfigSchema(infer_schema_from_config_class(cls))
+
 
 @experimental
 class PermissiveConfig(Config):
     # Pydantic config for this class
     # Cannot use kwargs for base class as this is not support for pydantic<1.8
     class Config:
         extra = "allow"
@@ -390,30 +401,60 @@
 @experimental
 class ConfigurableResourceFactory(
     Generic[TResValue],
     ResourceDefinition,
     Config,
     TypecheckAllowPartialResourceInitParams,
     AllowDelayedDependencies,
+    ABC,
     metaclass=BaseResourceMeta,
 ):
-    """Base class for Dagster resources that utilize structured config.
+    """Base class for creating and managing the lifecycle of Dagster resources that utilize structured config.
+
+    Users should directly inherit from this class when they want the object passed to user-defined
+    code (such as an asset or op) to be different than the object that defines the configuration
+    schema and is passed to the :py:class:`Definitions` object. Cases where this is useful include is
+    when the object passed to user code is:
+
+    * An existing class from a third-party library that the user does not control.
+    * A complex class that requires substantial internal state management or itself requires arguments beyond its config values.
+    * A class with expensive initialization that should not be invoked on code location load, but rather lazily on first use in an op or asset during a run.
+    * A class that you desire to be a plain Python class, rather than a Pydantic class, for whatever reason.
 
     This class is a subclass of both :py:class:`ResourceDefinition` and :py:class:`Config`, and
-    must implement ``create_resource``, which defines the resource value to pass to user code.
+    must implement ``create_resource``, which creates the resource to pass to user code.
+
+    Example definition:
 
-    Example:
     .. code-block:: python
 
-        class DatabseResource(ConfigurableResourceFactory[Database]):
+        class DatabaseResource(ConfigurableResourceFactory[Database]):
             connection_uri: str
 
             def create_resource(self, _init_context) -> Database:
+                # For example Database could be from a third-party library or require expensive setup.
+                # Or you could just prefer to separate the concerns of configuration and runtime representation
                 return Database(self.connection_uri)
 
+    To use a resource created by a factory in a pipeline, you must use the Resource type annotation.
+
+    Example usage:
+
+    .. code-block:: python
+
+        @asset
+        def asset_that_uses_database(database: ResourceParam[Database]):
+            # Database used directly in user code
+            database.query("SELECT * FROM table")
+
+        defs = Definitions(
+            assets=[asset_that_uses_database],
+            resources={"database": DatabaseResource(connection_uri="some_uri")},
+        )
+
     """
 
     def __init__(self, **data: Any):
         resource_pointers, data_without_resources = separate_resource_params(data)
 
         schema = infer_schema_from_config_class(
             self.__class__, fields_to_omit=set(resource_pointers.keys())
@@ -443,14 +484,22 @@
             description=self.__doc__,
         )
         self._resolved_config_dict = resolved_config_dict
         self._schema = schema
 
         self._nested_resources = {k: v for k, v in resource_pointers.items()}
 
+    @abstractmethod
+    def create_resource(self, context: InitResourceContext) -> TResValue:
+        """Returns the object that this resource hands to user code, accessible by ops or assets
+        through the context or resource parameters. This works like the function decorated
+        with @resource when using function-based resources.
+        """
+        raise NotImplementedError()
+
     @property
     def nested_resources(self) -> Mapping[str, ResourceDefinition]:
         return self._nested_resources
 
     @classmethod
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialResource[Self]":
         """Returns a partially initialized copy of the resource, with remaining config fields
@@ -525,38 +574,66 @@
         with_env_vars = with_nested_resources._resolve_and_update_env_vars()  # noqa: SLF001
 
         return with_env_vars._create_object_fn(context)  # noqa: SLF001
 
     def _create_object_fn(self, context: InitResourceContext) -> TResValue:
         return self.create_resource(context)
 
-    def create_resource(self, context: InitResourceContext) -> TResValue:
-        """Returns the object that this resource hands to user code, accessible by ops or assets
-        through the context or resource parameters. This works like the function decorated
-        with @resource when using function-based resources.
+    @classmethod
+    def from_resource_context(cls, context: InitResourceContext) -> TResValue:
+        """Creates a new instance of this resource from a populated InitResourceContext.
+        Useful when creating a resource from a function-based resource, for backwards
+        compatibility purposes.
+
+        Example usage:
+
+        .. code-block:: python
+
+            class MyResource(ConfigurableResource):
+                my_str: str
+
+            @resource(config_schema=MyResource.to_config_schema())
+            def my_resource(context: InitResourceContext) -> MyResource:
+                return MyResource.from_resource_context(context)
+
         """
-        raise NotImplementedError()
+        return cls(**context.resource_config).create_resource(context)
 
 
 @experimental
 class ConfigurableResource(ConfigurableResourceFactory[TResValue]):
     """Base class for Dagster resources that utilize structured config.
 
-    This class is a subclass of both :py:class:`ResourceDefinition` and :py:class:`Config`, and
-    provides a default implementation of the resource_fn that returns the resource itself.
+    This class is a subclass of both :py:class:`ResourceDefinition` and :py:class:`Config`.
+
+    Example definition:
 
-    Example:
     .. code-block:: python
 
         class WriterResource(ConfigurableResource):
             prefix: str
 
             def output(self, text: str) -> None:
                 print(f"{self.prefix}{text}")
 
+        # which can be used in a pipeline like so:
+
+    Example usage:
+
+    .. code-block:: python
+
+        @asset
+        def asset_that_uses_writer(writer: WriterResource):
+            writer.output("text")
+
+        defs = Definitions(
+            assets=[asset_that_uses_writer],
+            resources={"writer": WriterResource(prefix="a_prefix")},
+        )
+
     """
 
     def create_resource(self, context: InitResourceContext) -> TResValue:
         """Returns the object that this resource hands to user code, accessible by ops or assets
         through the context or resource parameters. This works like the function decorated
         with @resource when using function-based resources.
 
@@ -704,22 +781,27 @@
         IOManagerDefinition.__init__(
             self,
             resource_fn=self.initialize_and_run,
             config_schema=self._config_schema,
             description=self.__doc__,
         )
 
-    def _create_object_fn(self, context: InitResourceContext) -> TIOManagerValue:
-        return self.create_io_manager(context)
-
     @abstractmethod
     def create_io_manager(self, context) -> TIOManagerValue:
         """Implement as one would implement a @io_manager decorator function."""
         raise NotImplementedError()
 
+    def _create_object_fn(self, context: InitResourceContext) -> TIOManagerValue:
+        return self.create_io_manager(context)
+
+    def create_resource(self, context: InitResourceContext) -> TIOManagerValue:
+        # I/O manager factories execute a different code path that does not
+        # call create_resource
+        raise NotImplementedError()
+
     @classmethod
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialIOManager[Self]":
         """Returns a partially initialized copy of the IO manager, with remaining config fields
         set at runtime.
         """
         return PartialIOManager(cls, data=kwargs)
 
@@ -779,16 +861,44 @@
                 f"{', '.join([str(t) for t in MAPPING_KEY_TYPE_TO_SCALAR.keys()])}."
             )
         return Map(MAPPING_KEY_TYPE_TO_SCALAR[key_type], config_type)
     else:
         raise NotImplementedError(f"Pydantic shape type {shape_type} not supported.")
 
 
-def _convert_pydantic_field(pydantic_field: ModelField) -> Field:
-    """Transforms a Pydantic field into a corresponding Dagster config field."""
+def _get_inner_field_if_exists(
+    shape_type: PydanticShapeType, field: ModelField
+) -> Optional[ModelField]:
+    """Grabs the inner Pydantic field type for a data structure such as a list or dictionary.
+
+    Returns None for types which have no inner field.
+    """
+    # See https://github.com/pydantic/pydantic/blob/v1.10.3/pydantic/fields.py#L758 for
+    # where sub_fields is set.
+    if shape_type == SHAPE_SINGLETON:
+        return None
+    elif shape_type == SHAPE_LIST:
+        # List has a single subfield, which is the type of the list elements.
+        return check.not_none(field.sub_fields)[0]
+    elif shape_type in MAPPING_TYPES:
+        # Mapping has a single subfield, which is the type of the mapping values.
+        return check.not_none(field.sub_fields)[0]
+    else:
+        raise NotImplementedError(f"Pydantic shape type {shape_type} not supported.")
+
+
+def _convert_pydantic_field(pydantic_field: ModelField, model_cls: Optional[Type] = None) -> Field:
+    """Transforms a Pydantic field into a corresponding Dagster config field.
+
+
+    Args:
+        pydantic_field (ModelField): The Pydantic field to convert.
+        model_cls (Optional[Type]): The Pydantic model class that the field belongs to. This is
+            used for error messages.
+    """
     key_type = (
         _config_type_for_pydantic_field(pydantic_field.key_field)
         if pydantic_field.key_field
         else None
     )
     if pydantic_field.field_info.discriminator:
         return _convert_pydantic_descriminated_union_field(pydantic_field)
@@ -799,38 +909,63 @@
             description=pydantic_field.field_info.description,
         )
         wrapped_config_type = _wrap_config_type(
             shape_type=pydantic_field.shape,
             config_type=inferred_field.config_type,
             key_type=key_type,
         )
-
-        return Field(config=wrapped_config_type, description=inferred_field.description)
+        return Field(
+            config=Noneable(wrapped_config_type)
+            if pydantic_field.allow_none
+            else wrapped_config_type,
+            description=inferred_field.description,
+            is_required=_is_pydantic_field_required(pydantic_field),
+        )
     else:
-        config_type = _config_type_for_pydantic_field(pydantic_field)
+        # For certain data structure types, we need to grab the inner Pydantic field (e.g. List type)
+        inner_field = _get_inner_field_if_exists(pydantic_field.shape, pydantic_field)
+        if inner_field:
+            config_type = _convert_pydantic_field(inner_field, model_cls=model_cls).config_type
+        else:
+            config_type = _config_type_for_pydantic_field(pydantic_field)
+
         wrapped_config_type = _wrap_config_type(
             shape_type=pydantic_field.shape, config_type=config_type, key_type=key_type
         )
-        if pydantic_field.allow_none:
-            wrapped_config_type = Noneable(wrapped_config_type)
         return Field(
-            config=wrapped_config_type,
+            config=Noneable(wrapped_config_type)
+            if pydantic_field.allow_none
+            else wrapped_config_type,
             description=pydantic_field.field_info.description,
             is_required=_is_pydantic_field_required(pydantic_field),
             default_value=pydantic_field.default
             if pydantic_field.default
             else FIELD_NO_DEFAULT_PROVIDED,
         )
 
 
 def _config_type_for_pydantic_field(pydantic_field: ModelField) -> ConfigType:
-    return _config_type_for_type_on_pydantic_field(pydantic_field.type_)
+    """Generates a Dagster ConfigType from a Pydantic field.
+
+    Args:
+        pydantic_field (ModelField): The Pydantic field to convert.
+    """
+    return _config_type_for_type_on_pydantic_field(
+        pydantic_field.type_,
+    )
 
 
-def _config_type_for_type_on_pydantic_field(potential_dagster_type: Any) -> ConfigType:
+def _config_type_for_type_on_pydantic_field(
+    potential_dagster_type: Any,
+) -> ConfigType:
+    """Generates a Dagster ConfigType from a Pydantic field's Python type.
+
+    Args:
+        potential_dagster_type (Any): The Python type of the Pydantic field.
+    """
     # special case pydantic constrained types to their source equivalents
     if safe_is_subclass(potential_dagster_type, ConstrainedStr):
         return StringSource
     # no FloatSource, so we just return float
     elif safe_is_subclass(potential_dagster_type, ConstrainedFloat):
         potential_dagster_type = float
     elif safe_is_subclass(potential_dagster_type, ConstrainedInt):
@@ -971,15 +1106,20 @@
             config_arg_default is inspect.Parameter.empty,
             "Cannot provide a default value when using a Config class",
         )
         return infer_schema_from_config_class(model_cls)
 
     # If were are here config is annotated with a primitive type
     # We do a conversion to a type as if it were a type on a pydantic field
-    inner_config_type = _config_type_for_type_on_pydantic_field(model_cls)
+    try:
+        inner_config_type = _config_type_for_type_on_pydantic_field(model_cls)
+    except (DagsterInvalidDefinitionError, DagsterInvalidConfigDefinitionError):
+        raise DagsterInvalidPythonicConfigDefinitionError(
+            invalid_type=model_cls, config_class=None, field_name=None
+        )
     return Field(
         config=inner_config_type,
         default_value=FIELD_NO_DEFAULT_PROVIDED
         if config_arg_default is inspect.Parameter.empty
         else config_arg_default,
     )
 
@@ -996,15 +1136,33 @@
         safe_is_subclass(model_cls, Config),
         "Config type annotation must inherit from dagster._config.structured_config.Config",
     )
 
     fields = {}
     for pydantic_field in model_cls.__fields__.values():
         if pydantic_field.name not in fields_to_omit:
-            fields[pydantic_field.alias] = _convert_pydantic_field(pydantic_field)
+            if isinstance(pydantic_field.default, Field):
+                raise DagsterInvalidDefinitionError(
+                    "Using 'dagster.Field' is not supported within a Pythonic config or resource"
+                    " definition. 'dagster.Field' should only be used in legacy Dagster config"
+                    " schemas. Did you mean to use 'pydantic.Field' instead?"
+                )
+
+            try:
+                fields[pydantic_field.alias] = _convert_pydantic_field(
+                    pydantic_field,
+                )
+            except DagsterInvalidConfigDefinitionError as e:
+                raise DagsterInvalidPythonicConfigDefinitionError(
+                    config_class=model_cls,
+                    field_name=pydantic_field.name,
+                    invalid_type=e.current_value,
+                    is_resource=model_cls is not None
+                    and safe_is_subclass(model_cls, ConfigurableResourceFactory),
+                )
 
     shape_cls = Permissive if model_cls.__config__.extra == Extra.allow else Shape
 
     docstring = model_cls.__doc__.strip() if model_cls.__doc__ else None
     return Field(config=shape_cls(fields), description=description or docstring)
 
 
@@ -1036,7 +1194,49 @@
 
 
 LateBoundTypesForResourceTypeChecking.set_actual_types_for_type_checking(
     resource_dep_type=ResourceDependency,
     resource_type=ConfigurableResourceFactory,
     partial_resource_type=PartialResource,
 )
+
+
+def validate_resource_annotated_function(fn) -> None:
+    """Validates any parameters on the decorated function that are annotated with
+    :py:class:`dagster.ResourceDefinition`, raising a :py:class:`dagster.DagsterInvalidDefinitionError`
+    if any are not also instances of :py:class:`dagster.ConfigurableResource` (these resources should
+    instead be wrapped in the :py:func:`dagster.Resource` Annotation).
+    """
+    from dagster import DagsterInvalidDefinitionError
+    from dagster._config.structured_config import (
+        ConfigurableResource,
+        ConfigurableResourceFactory,
+        TResValue,
+    )
+    from dagster._config.structured_config.utils import safe_is_subclass
+
+    malformed_params = [
+        param
+        for param in get_function_params(fn)
+        if safe_is_subclass(param.annotation, ResourceDefinition)
+        and not safe_is_subclass(param.annotation, ConfigurableResource)
+    ]
+    if len(malformed_params) > 0:
+        malformed_param = malformed_params[0]
+        output_type = None
+        if safe_is_subclass(malformed_param.annotation, ConfigurableResourceFactory):
+            orig_bases = getattr(malformed_param.annotation, "__orig_bases__", None)
+            output_type = get_args(orig_bases[0])[0] if orig_bases and len(orig_bases) > 0 else None
+            if output_type == TResValue:
+                output_type = None
+
+        output_type_name = getattr(output_type, "__name__", str(output_type))
+        raise DagsterInvalidDefinitionError(
+            """Resource param '{param_name}' is annotated as '{annotation_type}', but '{annotation_type}' outputs {value_message} value to user code such as @ops and @assets. This annotation should instead be {annotation_suggestion}""".format(
+                param_name=malformed_param.name,
+                annotation_type=malformed_param.annotation,
+                value_message=f"a '{output_type}'" if output_type else "an unknown",
+                annotation_suggestion=f"'ResourceParam[{output_type_name}]'"
+                if output_type
+                else "'ResourceParam[Any]' or 'ResourceParam[<output type>]'",
+            )
+        )
```

### Comparing `dagster-1.2.6/dagster/_config/structured_config/typing_utils.py` & `dagster-1.2.7/dagster/_config/structured_config/typing_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TYPE_CHECKING, Any, Generic, Optional, Type, TypeVar, Union, cast
 
 import pydantic
+from pydantic import Field
 from typing_extensions import dataclass_transform, get_origin
 
 from .utils import safe_is_subclass
 
 if TYPE_CHECKING:
     from dagster._config.structured_config import PartialResource
 
@@ -45,15 +46,15 @@
         LateBoundTypesForResourceTypeChecking._ResourceDep = resource_dep_type  # noqa: SLF001
         LateBoundTypesForResourceTypeChecking._Resource = resource_type  # noqa: SLF001
         LateBoundTypesForResourceTypeChecking._PartialResource = (  # noqa: SLF001
             partial_resource_type
         )
 
 
-@dataclass_transform()
+@dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
 class BaseResourceMeta(pydantic.main.ModelMetaclass):
     """Custom metaclass for Resource and PartialResource. This metaclass is responsible for
     transforming the type annotations on the class so that Pydantic constructor-time validation
     does not error when users provide partially configured resources to resource params.
 
     For example, the following code would ordinarily fail Pydantic validation:
```

### Comparing `dagster-1.2.6/dagster/_config/structured_config/utils.py` & `dagster-1.2.7/dagster/_config/structured_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/traversal_context.py` & `dagster-1.2.7/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/type_printer.py` & `dagster-1.2.7/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_config/validate.py` & `dagster-1.2.7/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/assets.py` & `dagster-1.2.7/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/code_pointer.py` & `dagster-1.2.7/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/container_context/config.py` & `dagster-1.2.7/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/debug.py` & `dagster-1.2.7/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/decorator_utils.py` & `dagster-1.2.7/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/__init__.py` & `dagster-1.2.7/dagster/_core/definitions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
     config_mapping as config_mapping,
     failure_hook as failure_hook,
     graph as graph,
     hook_decorator as hook_decorator,
     job as job,
     multi_asset as multi_asset,
     op as op,
-    pipeline as pipeline,
     repository as repository,
     schedule as schedule,
     sensor as sensor,
     success_hook as success_hook,
 )
 from .graph_definition import GraphDefinition as GraphDefinition
 from .job_definition import JobDefinition as JobDefinition
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_graph.py` & `dagster-1.2.7/dagster/_core/definitions/asset_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Union,
     cast,
 )
 
 import toposort
 
 import dagster._check as check
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.errors import DagsterInvalidInvocationError, DagsterInvariantViolationError
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.selector.subset_selector import DependencyGraph, generate_asset_dep_graph
 from dagster._utils.cached_method import cached_method
 
 from .assets import AssetsDefinition
 from .events import AssetKey, AssetKeyPartitionKey
@@ -43,24 +44,26 @@
         self,
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
+        auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
     ):
         self._asset_dep_graph = asset_dep_graph
         self._source_asset_keys = source_asset_keys
         self._partitions_defs_by_key = partitions_defs_by_key
         self._partition_mappings_by_key = partition_mappings_by_key
         self._group_names_by_key = group_names_by_key
         self._freshness_policies_by_key = freshness_policies_by_key
+        self._auto_materialize_policies_by_key = auto_materialize_policies_by_key
         self._required_multi_asset_sets_by_key = required_multi_asset_sets_by_key
         self._code_versions_by_key = code_versions_by_key
         self._is_observable_by_key = is_observable_by_key
 
     @property
     def asset_dep_graph(self) -> DependencyGraph[AssetKey]:
         return self._asset_dep_graph
@@ -80,26 +83,33 @@
 
         return AssetSelection.keys(*self.non_source_asset_keys).roots().resolve(self)
 
     @property
     def freshness_policies_by_key(self) -> Mapping[AssetKey, Optional[FreshnessPolicy]]:
         return self._freshness_policies_by_key
 
+    @property
+    def auto_materialize_policies_by_key(
+        self,
+    ) -> Mapping[AssetKey, Optional[AutoMaterializePolicy]]:
+        return self._auto_materialize_policies_by_key
+
     @staticmethod
     def from_assets(
         all_assets: Iterable[Union[AssetsDefinition, SourceAsset]]
     ) -> "InternalAssetGraph":
         assets_defs: List[AssetsDefinition] = []
         source_assets: List[SourceAsset] = []
         partitions_defs_by_key: Dict[AssetKey, Optional[PartitionsDefinition]] = {}
         partition_mappings_by_key: Dict[
             AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]
         ] = {}
         group_names_by_key: Dict[AssetKey, Optional[str]] = {}
         freshness_policies_by_key: Dict[AssetKey, Optional[FreshnessPolicy]] = {}
+        auto_materialize_policies_by_key: Dict[AssetKey, Optional[AutoMaterializePolicy]] = {}
         required_multi_asset_sets_by_key: Dict[AssetKey, AbstractSet[AssetKey]] = {}
         code_versions_by_key: Dict[AssetKey, Optional[str]] = {}
         is_observable_by_key: Dict[AssetKey, bool] = {}
 
         for asset in all_assets:
             if isinstance(asset, SourceAsset):
                 source_assets.append(asset)
@@ -110,26 +120,28 @@
                 assets_defs.append(asset)
                 partition_mappings_by_key.update(
                     {key: asset.partition_mappings for key in asset.keys}
                 )
                 partitions_defs_by_key.update({key: asset.partitions_def for key in asset.keys})
                 group_names_by_key.update(asset.group_names_by_key)
                 freshness_policies_by_key.update(asset.freshness_policies_by_key)
+                auto_materialize_policies_by_key.update(asset.auto_materialize_policies_by_key)
                 if len(asset.keys) > 1 and not asset.can_subset:
                     for key in asset.keys:
                         required_multi_asset_sets_by_key[key] = asset.keys
                 code_versions_by_key.update(asset.code_versions_by_key)
 
         return InternalAssetGraph(
             asset_dep_graph=generate_asset_dep_graph(assets_defs, source_assets),
             source_asset_keys={source_asset.key for source_asset in source_assets},
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
+            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             assets=assets_defs,
             source_assets=source_assets,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
         )
 
@@ -234,15 +246,16 @@
         if parent_partition_key is None:
             return child_partitions_def.get_partition_keys(
                 dynamic_partitions_store=dynamic_partitions_store
             )
 
         if parent_partitions_def is None:
             raise DagsterInvalidInvocationError(
-                "Parent partition key provided, but parent asset is not partitioned."
+                f"Parent partition key '{parent_partition_key}' provided, but parent asset"
+                f" '{parent_asset_key}' is not partitioned."
             )
 
         partition_mapping = self.get_partition_mapping(child_asset_key, parent_asset_key)
         child_partitions_subset = partition_mapping.get_downstream_partitions_for_partitions(
             parent_partitions_def.empty_subset().with_partition_keys([parent_partition_key]),
             downstream_partitions_def=child_partitions_def,
             dynamic_partitions_store=dynamic_partitions_store,
@@ -371,14 +384,17 @@
 
     @cached_method
     def toposort_asset_keys(self) -> Sequence[AbstractSet[AssetKey]]:
         return [
             {key for key in level} for level in toposort.toposort(self._asset_dep_graph["upstream"])
         ]
 
+    def get_auto_materialize_policy(self, asset_key: AssetKey) -> Optional[AutoMaterializePolicy]:
+        return self.auto_materialize_policies_by_key.get(asset_key)
+
     @cached_method
     def get_downstream_freshness_policies(
         self, *, asset_key: AssetKey
     ) -> AbstractSet[FreshnessPolicy]:
         downstream_policies = set().union(
             *(
                 self.get_downstream_freshness_policies(asset_key=child_key)
@@ -525,27 +541,29 @@
         self,
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
+        auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         assets: Sequence[AssetsDefinition],
         source_assets: Sequence[SourceAsset],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
     ):
         super().__init__(
             asset_dep_graph=asset_dep_graph,
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
+            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
         )
         self._assets = assets
         self._source_assets = source_assets
 
@@ -619,15 +637,18 @@
             if partitions_def is not None and isinstance(
                 partitions_def, TimeWindowPartitionsDefinition
             ):
                 partition_sort_key = partitions_def.time_window_for_partition_key(
                     cast(str, asset_partition.partition_key)
                 ).start.timestamp()
             else:
-                check.failed("Assets with self-dependencies must have time-window partitions")
+                check.failed(
+                    "Assets with self-dependencies must have time-window partitions, but"
+                    f" {asset_key} does not."
+                )
         else:
             partition_sort_key = None
 
         return ToposortedPriorityQueue.QueueItem(
             level,
             partition_sort_key,
             [
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.2.7/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_group.py` & `dagster-1.2.7/dagster/_core/definitions/asset_group.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_in.py` & `dagster-1.2.7/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_layer.py` & `dagster-1.2.7/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_out.py` & `dagster-1.2.7/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.2.7/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,37 +18,101 @@
 )
 
 import pendulum
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
 )
 from dagster._utils.schedules import cron_string_iterator
 
 from .asset_selection import AssetGraph, AssetSelection
 from .decorators.sensor_decorator import sensor
 from .partition import PartitionsDefinition, PartitionsSubset
-from .repository_definition import RepositoryDefinition
 from .run_request import RunRequest
 from .sensor_definition import DefaultSensorStatus, SensorDefinition
 from .utils import check_valid_name
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
 
+def get_implicit_auto_materialize_policy(
+    asset_graph: AssetGraph, asset_key: AssetKey
+) -> Optional[AutoMaterializePolicy]:
+    """For backcompat with pre-auto materialize policy graphs, assume a default scope of 1 day."""
+    auto_materialize_policy = asset_graph.get_auto_materialize_policy(asset_key)
+    if auto_materialize_policy is None:
+        return AutoMaterializePolicy(
+            on_missing=True,
+            on_upstream_data_newer=not bool(
+                asset_graph.get_downstream_freshness_policies(asset_key=asset_key)
+            ),
+            for_freshness=True,
+            time_window_partition_scope_minutes=24 * 60,
+        )
+    return auto_materialize_policy
+
+
+def reconciliation_window_for_time_window_partitions(
+    partitions_def: TimeWindowPartitionsDefinition,
+    time_window_partition_scope: Optional[datetime.timedelta],
+    current_time: datetime.datetime,
+) -> Optional[TimeWindow]:
+    latest_partition_window = partitions_def.get_last_partition_window(current_time=current_time)
+    earliest_partition_window = partitions_def.get_first_partition_window(current_time=current_time)
+    if latest_partition_window is None or earliest_partition_window is None:
+        return None
+
+    allowable_start_time = (
+        max(
+            earliest_partition_window.start,
+            latest_partition_window.start
+            - time_window_partition_scope
+            + datetime.timedelta.resolution,
+        )
+        if time_window_partition_scope is not None
+        else earliest_partition_window.start
+    )
+    return TimeWindow(allowable_start_time, latest_partition_window.end)
+
+
+def can_reconcile_time_window_partition(
+    partitions_def: TimeWindowPartitionsDefinition,
+    partition_key: Optional[str],
+    time_window_partition_scope: Optional[datetime.timedelta],
+    current_time: datetime.datetime,
+) -> bool:
+    if partition_key is None:
+        return False
+    if time_window_partition_scope is None:
+        return True
+    reconciliation_window = reconciliation_window_for_time_window_partitions(
+        partitions_def=partitions_def,
+        time_window_partition_scope=time_window_partition_scope,
+        current_time=current_time,
+    )
+    if reconciliation_window is None:
+        return False
+    key_window = partitions_def.time_window_for_partition_key(partition_key)
+    return (
+        key_window.start >= reconciliation_window.start
+        and key_window.end <= reconciliation_window.end
+    )
+
+
 class AssetReconciliationCursor(NamedTuple):
     """Attributes:
     latest_storage_id: The latest observed storage ID across all assets. Useful for
         finding out what has happened since the last tick.
     materialized_or_requested_root_asset_keys: Every entry is a non-partitioned asset with no
         parents that has been requested by this sensor or has been materialized (even if not by
         this sensor).
@@ -65,35 +129,39 @@
         return asset_key in self.materialized_or_requested_root_asset_keys
 
     def get_never_requested_never_materialized_partitions(
         self,
         asset_key: AssetKey,
         asset_graph,
         dynamic_partitions_store: "DynamicPartitionsStore",
-        evaluation_time: datetime.datetime,
+        current_time: datetime.datetime,
+        time_window_partition_scope: Optional[datetime.timedelta],
     ) -> Iterable[str]:
         partitions_def = asset_graph.get_partitions_def(asset_key)
 
         materialized_or_requested_subset = (
             self.materialized_or_requested_root_partitions_by_asset_key.get(
                 asset_key, partitions_def.empty_subset()
             )
         )
 
         if isinstance(partitions_def, TimeWindowPartitionsDefinition):
-            allowable_time_window = allowable_time_window_for_partitions_def(
-                partitions_def, evaluation_time
+            # for performance, only iterate over keys within the allowable time window
+            reconciliation_window = reconciliation_window_for_time_window_partitions(
+                partitions_def=partitions_def,
+                time_window_partition_scope=time_window_partition_scope,
+                current_time=current_time,
             )
-            if allowable_time_window is None:
+            if reconciliation_window is None:
                 return []
             # for performance, only iterate over keys within the allowable time window
             return [
                 partition_key
                 for partition_key in partitions_def.get_partition_keys_in_time_window(
-                    allowable_time_window
+                    reconciliation_window
                 )
                 if partition_key not in materialized_or_requested_subset
             ]
         else:
             return materialized_or_requested_subset.get_partition_keys_not_in_subset(
                 dynamic_partitions_store=dynamic_partitions_store
             )
@@ -180,17 +248,24 @@
         ) = json.loads(cursor)
         materialized_or_requested_root_partitions_by_asset_key = {}
         for (
             key_str,
             serialized_subset,
         ) in serialized_materialized_or_requested_root_partitions_by_asset_key.items():
             key = AssetKey.from_user_string(key_str)
-            materialized_or_requested_root_partitions_by_asset_key[key] = cast(
-                PartitionsDefinition, asset_graph.get_partitions_def(key)
-            ).deserialize_subset(serialized_subset)
+            if key not in asset_graph.non_source_asset_keys:
+                continue
+
+            partitions_def = asset_graph.get_partitions_def(key)
+            if partitions_def is None:
+                continue
+
+            materialized_or_requested_root_partitions_by_asset_key[
+                key
+            ] = partitions_def.deserialize_subset(serialized_subset)
         return cls(
             latest_storage_id=latest_storage_id,
             materialized_or_requested_root_asset_keys={
                 AssetKey.from_user_string(key_str)
                 for key_str in serialized_materialized_or_requested_root_asset_keys
             },
             materialized_or_requested_root_partitions_by_asset_key=materialized_or_requested_root_partitions_by_asset_key,
@@ -239,35 +314,41 @@
 
     return result
 
 
 def find_parent_materialized_asset_partitions(
     instance_queryer: "CachingInstanceQueryer",
     latest_storage_id: Optional[int],
-    target_asset_selection: AssetSelection,
+    target_asset_keys: AbstractSet[AssetKey],
+    target_asset_keys_and_parents: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
     can_reconcile_fn: Callable[[AssetKeyPartitionKey], bool] = lambda _: True,
 ) -> Tuple[AbstractSet[AssetKeyPartitionKey], Optional[int]]:
     """Finds asset partitions in the given selection whose parents have been materialized since
     latest_storage_id.
 
     Returns:
         - A set of asset partitions.
         - The latest observed storage_id across all relevant assets. Can be used to avoid scanning
             the same events the next time this function is called.
     """
     result_asset_partitions: Set[AssetKeyPartitionKey] = set()
     result_latest_storage_id = latest_storage_id
 
-    target_asset_keys = target_asset_selection.resolve(asset_graph)
-
-    target_parent_asset_keys = target_asset_selection.upstream(depth=1).resolve(asset_graph)
-
-    for asset_key in target_parent_asset_keys:
+    for asset_key in target_asset_keys_and_parents:
         if asset_graph.is_source(asset_key):
+            if asset_graph.is_observable(asset_key) and instance_queryer.new_version_exists(
+                observable_source_asset_key=asset_key, after_cursor=latest_storage_id
+            ):
+                for child in asset_graph.get_children_partitions(
+                    instance_queryer, asset_key, partition_key=None
+                ):
+                    if child.asset_key in target_asset_keys:
+                        result_asset_partitions.add(child)
+
             continue
 
         partitions_def = asset_graph.get_partitions_def(asset_key)
         latest_record = instance_queryer.get_latest_materialization_record(
             asset_key, after_cursor=latest_storage_id
         )
         if latest_record is None:
@@ -341,17 +422,17 @@
 
     return (result_asset_partitions, result_latest_storage_id)
 
 
 def find_never_materialized_or_requested_root_asset_partitions(
     instance_queryer: "CachingInstanceQueryer",
     cursor: AssetReconciliationCursor,
-    target_asset_selection: AssetSelection,
+    target_asset_keys: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
-    evaluation_time: datetime.datetime,
+    current_time: datetime.datetime,
 ) -> Tuple[
     Iterable[AssetKeyPartitionKey], AbstractSet[AssetKey], Mapping[AssetKey, AbstractSet[str]]
 ]:
     """Finds asset partitions that have never been materialized or requested and that have no
     parents.
 
     Returns:
@@ -361,18 +442,25 @@
     - Asset (partition)s that had never been materialized or requested up to the previous cursor but
         are now materialized.
     """
     never_materialized_or_requested = set()
     newly_materialized_root_asset_keys = set()
     newly_materialized_root_partitions_by_asset_key = defaultdict(set)
 
-    for asset_key in (target_asset_selection & AssetSelection.all().sources()).resolve(asset_graph):
+    for asset_key in target_asset_keys & asset_graph.root_asset_keys:
         if asset_graph.is_partitioned(asset_key):
+            auto_materialize_policy = check.not_none(
+                get_implicit_auto_materialize_policy(asset_graph, asset_key)
+            )
             for partition_key in cursor.get_never_requested_never_materialized_partitions(
-                asset_key, asset_graph, instance_queryer, evaluation_time
+                asset_key,
+                asset_graph,
+                instance_queryer,
+                current_time,
+                time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
             ):
                 asset_partition = AssetKeyPartitionKey(asset_key, partition_key)
                 if instance_queryer.get_latest_materialization_record(asset_partition, None):
                     newly_materialized_root_partitions_by_asset_key[asset_key].add(partition_key)
                 else:
                     never_materialized_or_requested.add(asset_partition)
         else:
@@ -386,121 +474,76 @@
     return (
         never_materialized_or_requested,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     )
 
 
-def allowable_time_window_for_partitions_def(
-    partitions_def: TimeWindowPartitionsDefinition,
-    evaluation_time: datetime.datetime,
-) -> Optional[TimeWindow]:
-    """Returns a time window encompassing the partitions that the reconciliation sensor is currently
-    allowed to materialize for this partitions_def.
-    """
-    latest_partition_window = partitions_def.get_last_partition_window(current_time=evaluation_time)
-    if latest_partition_window is None:
-        return None
-
-    earliest_partition_window = partitions_def.get_first_partition_window(
-        current_time=evaluation_time
-    )
-    if earliest_partition_window is None:
-        return None
-
-    start = max(
-        earliest_partition_window.start,
-        # we add datetime.timedelta.resolution because if the latest partition starts at 2023-01-02,
-        # then we don't want 2023-01-01 to be within the allowable time window
-        latest_partition_window.start - datetime.timedelta(days=1) + datetime.timedelta.resolution,
-    )
-
-    return TimeWindow(
-        start=start,
-        end=latest_partition_window.end,
-    )
-
-
-def candidates_unit_within_allowable_time_window(
-    asset_graph: AssetGraph,
-    candidates_unit: Iterable[AssetKeyPartitionKey],
-    evaluation_time: datetime.datetime,
-):
-    """A given time-window partition may only be materialized if its window ends within 1 day of the
-    latest window for that partition.
-    """
-    representative_candidate = next(iter(candidates_unit), None)
-    if not representative_candidate:
-        return True
-
-    partitions_def = asset_graph.get_partitions_def(representative_candidate.asset_key)
-    partition_key = representative_candidate.partition_key
-    if not isinstance(partitions_def, TimeWindowPartitionsDefinition) or not partition_key:
-        return True
-
-    partitions_def = cast(TimeWindowPartitionsDefinition, partitions_def)
-
-    allowable_time_window = allowable_time_window_for_partitions_def(
-        partitions_def, evaluation_time
-    )
-    if allowable_time_window is None:
-        return False
-
-    candidate_partition_window = partitions_def.time_window_for_partition_key(partition_key)
-    return (
-        candidate_partition_window.start >= allowable_time_window.start
-        and candidate_partition_window.end <= allowable_time_window.end
-    )
-
-
 def determine_asset_partitions_to_reconcile(
     instance_queryer: "CachingInstanceQueryer",
     cursor: AssetReconciliationCursor,
-    target_asset_selection: AssetSelection,
+    target_asset_keys: AbstractSet[AssetKey],
+    target_asset_keys_and_parents: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
-    eventual_asset_partitions_to_reconcile_for_freshness: AbstractSet[AssetKeyPartitionKey],
-    evaluation_time: datetime.datetime,
+    current_time: datetime.datetime,
 ) -> Tuple[
     AbstractSet[AssetKeyPartitionKey],
     AbstractSet[AssetKey],
     Mapping[AssetKey, AbstractSet[str]],
     Optional[int],
 ]:
     (
         never_materialized_or_requested_roots,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     ) = find_never_materialized_or_requested_root_asset_partitions(
         instance_queryer=instance_queryer,
         cursor=cursor,
-        target_asset_selection=target_asset_selection,
+        target_asset_keys=target_asset_keys,
         asset_graph=asset_graph,
-        evaluation_time=evaluation_time,
+        current_time=current_time,
     )
 
-    # a quick filter for eliminating some stale candidates
-    def can_reconcile_fn(candidate: AssetKeyPartitionKey) -> bool:
-        if candidate.partition_key is None:
-            return True
-        return candidates_unit_within_allowable_time_window(
-            asset_graph=asset_graph,
-            candidates_unit=[candidate],
-            evaluation_time=evaluation_time,
+    # a filter for eliminating candidates
+    def can_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
+        auto_materialize_policy = get_implicit_auto_materialize_policy(
+            asset_graph=asset_graph, asset_key=candidate.asset_key
         )
+        partitions_def = asset_graph.get_partitions_def(candidate.asset_key)
+
+        # no policy means no reconciliation
+        if auto_materialize_policy is None:
+            return False
+        # the partition is too old to reconcile
+        elif isinstance(
+            partitions_def, TimeWindowPartitionsDefinition
+        ) and not can_reconcile_time_window_partition(
+            partitions_def=partitions_def,
+            partition_key=candidate.partition_key,
+            time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
+            current_time=current_time,
+        ):
+            return False
+        # the policy does not allow for materializing missing partitions and it's missing
+        elif not auto_materialize_policy.on_missing and not instance_queryer.materialization_exists(
+            candidate
+        ):
+            return False
+
+        return True
 
     stale_candidates, latest_storage_id = find_parent_materialized_asset_partitions(
         instance_queryer=instance_queryer,
         latest_storage_id=cursor.latest_storage_id,
-        target_asset_selection=target_asset_selection,
+        target_asset_keys=target_asset_keys,
+        target_asset_keys_and_parents=target_asset_keys_and_parents,
         asset_graph=asset_graph,
-        can_reconcile_fn=can_reconcile_fn,
+        can_reconcile_fn=can_reconcile_candidate,
     )
 
-    target_asset_keys = target_asset_selection.resolve(asset_graph)
-
     backfill_target_asset_graph_subset = get_active_backfill_target_asset_graph_subset(
         asset_graph=asset_graph,
         instance=instance_queryer.instance,
     )
 
     def parents_will_be_reconciled(
         candidate: AssetKeyPartitionKey,
@@ -521,40 +564,49 @@
             for parent in asset_graph.get_parents_partitions(
                 instance_queryer,
                 candidate.asset_key,
                 candidate.partition_key,
             )
         )
 
+    def should_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
+        auto_materialize_policy = get_implicit_auto_materialize_policy(
+            asset_graph=asset_graph, asset_key=candidate.asset_key
+        )
+        if auto_materialize_policy is None:
+            return False
+
+        return (
+            auto_materialize_policy.on_missing
+            and not instance_queryer.materialization_exists(asset_partition=candidate)
+        ) or (
+            auto_materialize_policy.on_upstream_data_newer
+            and not instance_queryer.is_reconciled(
+                asset_partition=candidate, asset_graph=asset_graph
+            )
+        )
+
     def should_reconcile(
         candidates_unit: Iterable[AssetKeyPartitionKey],
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
-        if not candidates_unit_within_allowable_time_window(
-            asset_graph, candidates_unit, evaluation_time
-        ):
-            return False
-
         if any(
-            # do not reconcile assets if the freshness system will update them
-            candidate in eventual_asset_partitions_to_reconcile_for_freshness
+            # do not reconcile assets if they are not reconcilable
+            not can_reconcile_candidate(candidate)
             # do not reconcile assets if an active backfill will update them
             or candidate in backfill_target_asset_graph_subset
             # do not reconcile assets if they are not in the target selection
             or candidate.asset_key not in target_asset_keys
             for candidate in candidates_unit
         ):
             return False
 
         return all(
             parents_will_be_reconciled(candidate, to_reconcile) for candidate in candidates_unit
-        ) and any(
-            not instance_queryer.is_reconciled(asset_partition=candidate, asset_graph=asset_graph)
-            for candidate in candidates_unit
-        )
+        ) and any(should_reconcile_candidate(candidate) for candidate in candidates_unit)
 
     to_reconcile = asset_graph.bfs_filter_asset_partitions(
         instance_queryer,
         should_reconcile,
         set(itertools.chain(never_materialized_or_requested_roots, stale_candidates)),
     )
 
@@ -565,22 +617,22 @@
         latest_storage_id,
     )
 
 
 def get_execution_period_for_policy(
     freshness_policy: FreshnessPolicy,
     effective_data_time: Optional[datetime.datetime],
-    evaluation_time: datetime.datetime,
+    current_time: datetime.datetime,
 ) -> pendulum.Period:
     if effective_data_time is None:
-        return pendulum.Period(start=evaluation_time, end=evaluation_time)
+        return pendulum.Period(start=current_time, end=current_time)
 
     if freshness_policy.cron_schedule:
         tick_iterator = cron_string_iterator(
-            start_timestamp=evaluation_time.timestamp(),
+            start_timestamp=current_time.timestamp(),
             cron_string=freshness_policy.cron_schedule,
             execution_timezone=freshness_policy.cron_schedule_timezone,
         )
 
         while True:
             # find the next tick tick that requires data after the current effective data time
             # (usually, this will be the next tick)
@@ -589,30 +641,30 @@
             if effective_data_time is None or effective_data_time < required_data_time:
                 return pendulum.Period(start=required_data_time, end=tick)
 
     else:
         return pendulum.Period(
             # we don't want to execute this too frequently
             start=effective_data_time + 0.9 * freshness_policy.maximum_lag_delta,
-            end=max(effective_data_time + freshness_policy.maximum_lag_delta, evaluation_time),
+            end=max(effective_data_time + freshness_policy.maximum_lag_delta, current_time),
         )
 
 
 def get_execution_period_for_policies(
     policies: AbstractSet[FreshnessPolicy],
     effective_data_time: Optional[datetime.datetime],
-    evaluation_time: datetime.datetime,
+    current_time: datetime.datetime,
 ) -> Optional[pendulum.Period]:
     """Determines a range of times for which you can kick off an execution of this asset to solve
     the most pressing constraint, alongside a maximum number of additional constraints.
     """
     merged_period = None
     for period in sorted(
         (
-            get_execution_period_for_policy(policy, effective_data_time, evaluation_time)
+            get_execution_period_for_policy(policy, effective_data_time, current_time)
             for policy in policies
         ),
         # sort execution periods by most pressing
         key=lambda period: period.end,
     ):
         if merged_period is None:
             merged_period = period
@@ -626,161 +678,175 @@
 
     return merged_period
 
 
 def determine_asset_partitions_to_reconcile_for_freshness(
     data_time_resolver: "CachingDataTimeResolver",
     asset_graph: AssetGraph,
-    target_asset_selection: AssetSelection,
-    evaluation_time: datetime.datetime,
-) -> Tuple[AbstractSet[AssetKeyPartitionKey], AbstractSet[AssetKeyPartitionKey]]:
+    target_asset_keys: AbstractSet[AssetKey],
+    target_asset_keys_and_parents: AbstractSet[AssetKey],
+    current_time: datetime.datetime,
+) -> AbstractSet[AssetKeyPartitionKey]:
     """Returns a set of AssetKeyPartitionKeys to materialize in order to abide by the given
     FreshnessPolicies, as well as a set of AssetKeyPartitionKeys which will be materialized at
     some point within the plan window.
 
     Attempts to minimize the total number of asset executions.
     """
-    # get the set of asset keys we're allowed to execute
-    target_asset_keys = target_asset_selection.resolve(asset_graph)
-
     # now we have a full set of constraints, we can find solutions for them as we move down
     to_materialize: Set[AssetKeyPartitionKey] = set()
-    eventually_materialize: Set[AssetKeyPartitionKey] = set()
     expected_data_time_by_key: Dict[AssetKey, Optional[datetime.datetime]] = {}
+
     for level in asset_graph.toposort_asset_keys():
         for key in level:
-            if asset_graph.is_source(key) or not asset_graph.get_downstream_freshness_policies(
-                asset_key=key
+            if (
+                key not in target_asset_keys_and_parents
+                or key not in asset_graph.all_asset_keys
+                or not asset_graph.get_downstream_freshness_policies(asset_key=key)
             ):
                 continue
 
             # figure out the current contents of this asset with respect to its constraints
-            current_data_time = data_time_resolver.get_current_data_time(key, evaluation_time)
+            current_data_time = data_time_resolver.get_current_data_time(key, current_time)
 
             # figure out the expected data time of this asset if it were to be executed on this tick
             expected_data_time = min(
                 (
                     cast(datetime.datetime, expected_data_time_by_key[k])
                     for k in asset_graph.get_parents(key)
                     if k in expected_data_time_by_key and expected_data_time_by_key[k] is not None
                 ),
-                default=evaluation_time,
+                default=current_time,
             )
 
             if key in target_asset_keys:
                 # calculate the data times you would expect after all currently-executing runs
                 # were to successfully complete
                 in_progress_data_time = data_time_resolver.get_in_progress_data_time(
-                    key, evaluation_time
+                    key, current_time
                 )
 
                 # calculate the data times you would have expected if the most recent run succeeded
                 failed_data_time = data_time_resolver.get_ignored_failure_data_time(
-                    key, evaluation_time
+                    key, current_time
                 )
 
                 effective_data_time = max(
                     filter(None, (current_data_time, in_progress_data_time, failed_data_time)),
                     default=None,
                 )
 
                 # figure out a time period that you can execute this asset within to solve a maximum
                 # number of constraints
                 execution_period = get_execution_period_for_policies(
                     policies=asset_graph.get_downstream_freshness_policies(asset_key=key),
                     effective_data_time=effective_data_time,
-                    evaluation_time=evaluation_time,
+                    current_time=current_time,
                 )
-                if execution_period:
-                    eventually_materialize.add(AssetKeyPartitionKey(key, None))
-
             else:
                 execution_period = None
 
             # a key may already be in to_materialize by the time we get here if a required
             # neighbor was selected to be updated
             asset_key_partition_key = AssetKeyPartitionKey(key, None)
             if asset_key_partition_key in to_materialize:
                 expected_data_time_by_key[key] = expected_data_time
             elif (
                 execution_period is not None
-                and execution_period.start <= evaluation_time
+                and execution_period.start <= current_time
                 and expected_data_time is not None
                 and expected_data_time >= execution_period.start
             ):
                 to_materialize.add(asset_key_partition_key)
                 expected_data_time_by_key[key] = expected_data_time
                 # all required neighbors will be updated on the same tick
                 for required_key in asset_graph.get_required_multi_asset_keys(key):
                     to_materialize.add(AssetKeyPartitionKey(required_key, None))
             else:
                 # if downstream assets consume this, they should expect data time equal to the
                 # current time for this asset, as it's not going to be updated
                 expected_data_time_by_key[key] = current_data_time
 
-    return to_materialize, eventually_materialize
+    return to_materialize
 
 
 def reconcile(
-    repository_def: RepositoryDefinition,
-    asset_selection: AssetSelection,
+    asset_graph: AssetGraph,
+    target_asset_keys: AbstractSet[AssetKey],
     instance: "DagsterInstance",
     cursor: AssetReconciliationCursor,
     run_tags: Optional[Mapping[str, str]],
 ):
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
     current_time = pendulum.now("UTC")
 
     instance_queryer = CachingInstanceQueryer(instance=instance)
-    asset_graph = repository_def.asset_graph
 
-    # fetch some data in advance to batch together some queries
-    relevant_asset_keys = list(asset_selection.upstream(depth=1).resolve(asset_graph))
-    instance_queryer.prefetch_asset_records(relevant_asset_keys)
+    # if there is a auto materialize policy set in the selection, use that
+    if any(
+        asset_graph.get_auto_materialize_policy(target_key) is not None
+        for target_key in target_asset_keys
+    ):
+        target_asset_keys = {
+            target_key
+            for target_key in target_asset_keys
+            if asset_graph.get_auto_materialize_policy(target_key) is not None
+        }
+
+    target_parent_asset_keys = {
+        parent
+        for target_asset_key in target_asset_keys
+        for parent in asset_graph.get_parents(target_asset_key)
+    }
+    target_asset_keys_and_parents = target_asset_keys | target_parent_asset_keys
+
+    # fetch some data in advance to batch some queries
+    target_asset_keys_and_parents_list = list(target_asset_keys_and_parents)
+    instance_queryer.prefetch_asset_records(target_asset_keys_and_parents_list)
     instance_queryer.prefetch_asset_partition_counts(
-        relevant_asset_keys, after_cursor=cursor.latest_storage_id
+        target_asset_keys_and_parents_list, after_cursor=cursor.latest_storage_id
     )
 
-    (
-        asset_partitions_to_reconcile_for_freshness,
-        eventual_asset_partitions_to_reconcile_for_freshness,
-    ) = determine_asset_partitions_to_reconcile_for_freshness(
-        data_time_resolver=CachingDataTimeResolver(
-            instance_queryer=instance_queryer, asset_graph=asset_graph
-        ),
-        asset_graph=asset_graph,
-        target_asset_selection=asset_selection,
-        evaluation_time=current_time,
+    asset_partitions_to_reconcile_for_freshness = (
+        determine_asset_partitions_to_reconcile_for_freshness(
+            data_time_resolver=CachingDataTimeResolver(
+                instance_queryer=instance_queryer, asset_graph=asset_graph
+            ),
+            asset_graph=asset_graph,
+            target_asset_keys=target_asset_keys,
+            target_asset_keys_and_parents=target_asset_keys_and_parents,
+            current_time=current_time,
+        )
     )
 
     (
         asset_partitions_to_reconcile,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
         latest_storage_id,
     ) = determine_asset_partitions_to_reconcile(
         instance_queryer=instance_queryer,
         asset_graph=asset_graph,
         cursor=cursor,
-        target_asset_selection=asset_selection,
-        eventual_asset_partitions_to_reconcile_for_freshness=eventual_asset_partitions_to_reconcile_for_freshness,
-        evaluation_time=current_time,
+        target_asset_keys=target_asset_keys,
+        target_asset_keys_and_parents=target_asset_keys_and_parents,
+        current_time=current_time,
     )
 
     run_requests = build_run_requests(
         asset_partitions_to_reconcile | asset_partitions_to_reconcile_for_freshness,
         asset_graph,
         run_tags,
     )
 
     return run_requests, cursor.with_updates(
         latest_storage_id=latest_storage_id,
         run_requests=run_requests,
-        asset_graph=repository_def.asset_graph,
+        asset_graph=asset_graph,
         newly_materialized_root_asset_keys=newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key=newly_materialized_root_partitions_by_asset_key,
     )
 
 
 def build_run_requests(
     asset_partitions: Iterable[AssetKeyPartitionKey],
@@ -938,24 +1004,23 @@
         name=name,
         asset_selection=asset_selection,
         minimum_interval_seconds=minimum_interval_seconds,
         description=description,
         default_status=default_status,
     )
     def _sensor(context):
+        asset_graph = context.repository_def.asset_graph
         cursor = (
-            AssetReconciliationCursor.from_serialized(
-                context.cursor, context.repository_def.asset_graph
-            )
+            AssetReconciliationCursor.from_serialized(context.cursor, asset_graph)
             if context.cursor
             else AssetReconciliationCursor.empty()
         )
         run_requests, updated_cursor = reconcile(
-            repository_def=context.repository_def,
-            asset_selection=asset_selection,
+            asset_graph=asset_graph,
+            target_asset_keys=asset_selection.resolve(asset_graph),
             instance=context.instance,
             cursor=cursor,
             run_tags=run_tags,
         )
 
         context.update_cursor(updated_cursor.serialize())
         return run_requests
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_selection.py` & `dagster-1.2.7/dagster/_core/definitions/asset_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,24 +393,28 @@
     ):
         self._child = child
         self.depth = depth
         self.include_self = include_self
 
     def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
         selection = self._child.resolve_inner(asset_graph)
+        if len(selection) == 0:
+            return selection
+
         all_upstream = operator.sub(
             reduce(
                 operator.or_,
                 [
                     {asset_key}
                     | fetch_connected(
                         item=asset_key,
                         graph=asset_graph.asset_dep_graph,
                         direction="upstream",
                         depth=self.depth,
                     )
                     for asset_key in selection
                 ],
+                set(),
             ),
             selection if not self.include_self else set(),
         )
         return {key for key in all_upstream if key not in asset_graph.source_asset_keys}
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/assets.py` & `dagster-1.2.7/dagster/_core/definitions/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.asset_layer import get_dep_node_handles_of_graph_backed_asset
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
 from dagster._core.selector.subset_selector import SelectionTree
 from dagster._utils.backcompat import (
@@ -80,14 +81,15 @@
     _asset_deps: Mapping[AssetKey, AbstractSet[AssetKey]]
     _resource_defs: Mapping[str, ResourceDefinition]
     _group_names_by_key: Mapping[AssetKey, str]
     _selected_asset_keys: AbstractSet[AssetKey]
     _can_subset: bool
     _metadata_by_key: Mapping[AssetKey, ArbitraryMetadataMapping]
     _freshness_policies_by_key: Mapping[AssetKey, FreshnessPolicy]
+    _auto_materialize_policies_by_key: Mapping[AssetKey, AutoMaterializePolicy]
     _code_versions_by_key: Mapping[AssetKey, Optional[str]]
     _descriptions_by_key: Mapping[AssetKey, str]
 
     def __init__(
         self,
         *,
         keys_by_input_name: Mapping[str, AssetKey],
@@ -98,14 +100,15 @@
         asset_deps: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]] = None,
         selected_asset_keys: Optional[AbstractSet[AssetKey]] = None,
         can_subset: bool = False,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
+        auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
         descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         # if adding new fields, make sure to handle them in the with_attributes
         # and from_graph methods
     ):
         from .graph_definition import GraphDefinition
 
         if isinstance(node_def, GraphDefinition):
@@ -217,14 +220,21 @@
         self._freshness_policies_by_key = check.opt_mapping_param(
             freshness_policies_by_key,
             "freshness_policies_by_key",
             key_type=AssetKey,
             value_type=FreshnessPolicy,
         )
 
+        self._auto_materialize_policies_by_key = check.opt_mapping_param(
+            auto_materialize_policies_by_key,
+            "auto_materialize_policies_by_key",
+            key_type=AssetKey,
+            value_type=AutoMaterializePolicy,
+        )
+
         _validate_self_deps(
             input_keys=self._keys_by_input_name.values(),
             output_keys=self._keys_by_output_name.values(),
             partition_mappings=self._partition_mappings,
         )
 
     def __call__(self, *args: object, **kwargs: object) -> object:
@@ -313,15 +323,15 @@
                 outputs, and values are the group name. Cannot be used with the group_name argument.
             descriptions_by_output_name (Optional[Mapping[str, Optional[str]]]): Defines a description to be
                 associated with each of the output asstes for this graph.
             metadata_by_output_name (Optional[Mapping[str, Optional[MetadataUserInput]]]): Defines metadata to
                 be associated with each of the output assets for this node. Keys are names of the
                 outputs, and values are dictionaries of metadata to be associated with the related
                 asset.
-            freshness_policies_by_output_name_ouptut_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
+            freshness_policies_by_output_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
         """
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "AssetsDefinition.from_graph")
         return AssetsDefinition._from_node(
@@ -393,15 +403,15 @@
                 outputs, and values are the group name. Cannot be used with the group_name argument.
             descriptions_by_output_name (Optional[Mapping[str, Optional[str]]]): Defines a description to be
                 associated with each of the output asstes for this graph.
             metadata_by_output_name (Optional[Mapping[str, Optional[MetadataUserInput]]]): Defines metadata to
                 be associated with each of the output assets for this node. Keys are names of the
                 outputs, and values are dictionaries of metadata to be associated with the related
                 asset.
-            freshness_policies_by_output_name_ouptut_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
+            freshness_policies_by_output_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
         """
         return AssetsDefinition._from_node(
             node_def=op_def,
             keys_by_input_name=keys_by_input_name,
@@ -512,29 +522,29 @@
             partition_mappings={
                 keys_by_input_name[input_name]: partition_mapping
                 for input_name, partition_mapping in partition_mappings.items()
             }
             if partition_mappings
             else None,
             metadata_by_key={
-                keys_by_output_name[output_name]: metadata
+                keys_by_output_name_with_prefix[output_name]: metadata
                 for output_name, metadata in metadata_by_output_name.items()
                 if metadata is not None
             }
             if metadata_by_output_name
             else None,
             freshness_policies_by_key={
-                keys_by_output_name[output_name]: freshness_policy
+                keys_by_output_name_with_prefix[output_name]: freshness_policy
                 for output_name, freshness_policy in freshness_policies_by_output_name.items()
                 if freshness_policy is not None
             }
             if freshness_policies_by_output_name
             else None,
             descriptions_by_key={
-                keys_by_output_name[output_name]: description
+                keys_by_output_name_with_prefix[output_name]: description
                 for output_name, description in descriptions_by_output_name.items()
                 if description is not None
             }
             if descriptions_by_output_name
             else None,
             can_subset=can_subset,
         )
@@ -643,14 +653,18 @@
             name: key for name, key in self.node_keys_by_input_name.items() if key in upstream_keys
         }
 
     @property
     def freshness_policies_by_key(self) -> Mapping[AssetKey, FreshnessPolicy]:
         return self._freshness_policies_by_key
 
+    @property
+    def auto_materialize_policies_by_key(self) -> Mapping[AssetKey, AutoMaterializePolicy]:
+        return self._auto_materialize_policies_by_key
+
     @public
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         return self._partitions_def
 
     @property
     def metadata_by_key(self) -> Mapping[AssetKey, ArbitraryMetadataMapping]:
@@ -761,14 +775,19 @@
                 replaced_freshness_policy = self.freshness_policies_by_key.get(key)
 
             if replaced_freshness_policy:
                 replaced_freshness_policies_by_key[
                     output_asset_key_replacements.get(key, key)
                 ] = replaced_freshness_policy
 
+        replaced_auto_materialize_policies_by_key = {
+            output_asset_key_replacements.get(key, key): policy
+            for key, policy in self._auto_materialize_policies_by_key.items()
+        }
+
         replaced_descriptions_by_key = {
             output_asset_key_replacements.get(key, key): description
             for key, description in self._descriptions_by_key.items()
         }
 
         return self.__class__(
             keys_by_input_name={
@@ -806,14 +825,15 @@
                 **group_names_by_key,
             },
             metadata_by_key={
                 output_asset_key_replacements.get(key, key): value
                 for key, value in self.metadata_by_key.items()
             },
             freshness_policies_by_key=replaced_freshness_policies_by_key,
+            auto_materialize_policies_by_key=replaced_auto_materialize_policies_by_key,
             descriptions_by_key=replaced_descriptions_by_key,
         )
 
     def _subset_graph_backed_asset(
         self,
         selected_asset_keys: AbstractSet[AssetKey],
     ):
@@ -918,14 +938,15 @@
                 asset_deps=subsetted_asset_deps,
                 can_subset=self.can_subset,
                 selected_asset_keys=selected_asset_keys & self.keys,
                 resource_defs=self.resource_defs,
                 group_names_by_key=self.group_names_by_key,
                 metadata_by_key=self.metadata_by_key,
                 freshness_policies_by_key=self.freshness_policies_by_key,
+                auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
             )
         else:
             # multi_asset subsetting
             return AssetsDefinition(
                 # keep track of the original mapping
                 keys_by_input_name=self._keys_by_input_name,
                 keys_by_output_name=self._keys_by_output_name,
@@ -935,14 +956,15 @@
                 asset_deps=self._asset_deps,
                 can_subset=self.can_subset,
                 selected_asset_keys=asset_subselection,
                 resource_defs=self.resource_defs,
                 group_names_by_key=self.group_names_by_key,
                 metadata_by_key=self.metadata_by_key,
                 freshness_policies_by_key=self.freshness_policies_by_key,
+                auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
             )
 
     @public
     def to_source_assets(self) -> Sequence[SourceAsset]:
         """Returns a SourceAsset for each asset in this definition.
 
         Each produced SourceAsset will have the same key, metadata, io_manager_key, etc. as the
@@ -1078,14 +1100,15 @@
             asset_deps=self._asset_deps,
             selected_asset_keys=self._selected_asset_keys,
             can_subset=self._can_subset,
             resource_defs=relevant_resource_defs,
             group_names_by_key=self.group_names_by_key,
             metadata_by_key=self.metadata_by_key,
             freshness_policies_by_key=self.freshness_policies_by_key,
+            auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
         )
 
 
 def _infer_keys_by_input_names(
     node_def: Union["GraphDefinition", OpDefinition], keys_by_input_name: Mapping[str, AssetKey]
 ) -> Mapping[str, AssetKey]:
     all_input_names = [input_def.name for input_def in node_def.input_defs]
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/assets_job.py` & `dagster-1.2.7/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.2.7/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/composition.py` & `dagster-1.2.7/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/config.py` & `dagster-1.2.7/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/configurable.py` & `dagster-1.2.7/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/data_time.py` & `dagster-1.2.7/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/data_version.py` & `dagster-1.2.7/dagster/_core/definitions/data_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -218,16 +218,23 @@
 
 class StaleStatus(Enum):
     MISSING = "MISSING"
     STALE = "STALE"
     FRESH = "FRESH"
 
 
+class StaleCauseCategory(Enum):
+    CODE = "CODE"
+    DATA = "DATA"
+    DEPENDENCIES = "DEPENDENCIES"
+
+
 class StaleCause(NamedTuple):
     key: AssetKey
+    category: StaleCauseCategory
     reason: str
     dependency: Optional[AssetKey] = None
     children: Optional[Sequence["StaleCause"]] = None
 
 
 class CachingStaleStatusResolver:
     """Used to resolve data version information. Avoids redundant database
@@ -296,68 +303,75 @@
 
         # only used if no provenance available
         materialization = check.not_none(self._get_latest_materialization_event(key=key))
         materialization_time = materialization.timestamp
 
         if provenance:
             if code_version and code_version != provenance.code_version:
-                yield StaleCause(key, "updated code version")
+                yield StaleCause(key, StaleCauseCategory.CODE, "updated code version")
 
             removed_deps = set(provenance.input_data_versions.keys()) - set(dependency_keys)
             for dep_key in removed_deps:
                 yield StaleCause(
                     key,
+                    StaleCauseCategory.DEPENDENCIES,
                     "removed dependency",
                     dep_key,
                 )
 
         for dep_key in sorted(dependency_keys):
             if self._get_status(key=dep_key) == StaleStatus.STALE:
                 yield StaleCause(
                     key,
+                    StaleCauseCategory.DATA,
                     "stale dependency",
                     dep_key,
                     self._get_stale_causes(key=dep_key),
                 )
             elif provenance:
                 if dep_key not in provenance.input_data_versions:
                     yield StaleCause(
                         key,
+                        StaleCauseCategory.DEPENDENCIES,
                         "new dependency",
                         dep_key,
                     )
                 elif provenance.input_data_versions[dep_key] != self._get_current_data_version(
                     key=dep_key
                 ):
                     yield StaleCause(
                         key,
+                        StaleCauseCategory.DATA,
                         "updated dependency data version",
                         dep_key,
                         [
                             StaleCause(
                                 dep_key,
+                                StaleCauseCategory.DATA,
                                 "updated data version",
                             )
                         ],
                     )
             # if no provenance, then use materialization timestamps instead of versions
             # this should be removable eventually since provenance is on all newer materializations
             else:
                 dep_materialization = self._get_latest_materialization_event(key=dep_key)
                 if dep_materialization is None:
                     # The input must be new if it has no materialization
-                    yield StaleCause(key, "new input", dep_key)
+                    yield StaleCause(key, StaleCauseCategory.DATA, "new input", dep_key)
                 elif dep_materialization.timestamp > materialization_time:
                     yield StaleCause(
                         key,
+                        StaleCauseCategory.DATA,
                         "updated dependency timestamp",
                         dep_key,
                         [
                             StaleCause(
                                 dep_key,
+                                StaleCauseCategory.DATA,
                                 "updated timestamp",
                             )
                         ],
                     )
 
     @cached_method
     def _get_stale_root_causes(self, key: AssetKey) -> Sequence[StaleCause]:
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,14 @@
     failure_hook as failure_hook,
     success_hook as success_hook,
 )
 from .job_decorator import (
     job as job,
 )
 from .op_decorator import op as op
-from .pipeline_decorator import (
-    pipeline as pipeline,
-)
 from .repository_decorator import (
     repository as repository,
 )
 from .schedule_decorator import (
     schedule as schedule,
 )
 from .sensor_decorator import (
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,20 @@
     overload,
 )
 
 import dagster._check as check
 from dagster._builtins import Nothing
 from dagster._config import UserConfigSchema
 from dagster._core.decorator_utils import get_function_params, get_valid_name_permutations
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping, MetadataUserInput
-from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.resource_annotation import (
+    get_resource_args,
+)
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._core.types.dagster_type import DagsterType
 from dagster._utils.backcompat import (
     ExperimentalWarning,
     deprecation_warning,
     experimental_arg_warning,
@@ -68,14 +71,15 @@
     compute_kind: Optional[str] = ...,
     dagster_type: Optional[DagsterType] = ...,
     partitions_def: Optional[PartitionsDefinition[Any]] = ...,
     op_tags: Optional[Mapping[str, Any]] = ...,
     group_name: Optional[str] = ...,
     output_required: bool = ...,
     freshness_policy: Optional[FreshnessPolicy] = ...,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
     retry_policy: Optional[RetryPolicy] = ...,
     code_version: Optional[str] = ...,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     ...
 
 
 def asset(
@@ -95,14 +99,15 @@
     compute_kind: Optional[str] = None,
     dagster_type: Optional[DagsterType] = None,
     partitions_def: Optional[PartitionsDefinition[Any]] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     group_name: Optional[str] = None,
     output_required: bool = True,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     retry_policy: Optional[RetryPolicy] = None,
     code_version: Optional[str] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
     """Create a definition for how to compute an asset.
 
     A software-defined asset is the combination of:
       1. An asset key, e.g. the name of a table.
@@ -156,14 +161,15 @@
             will be initialized during execution, and can be accessed from the
             context within the body of the function.
         output_required (bool): Whether the decorated function will always materialize an asset.
             Defaults to True. If False, the function can return None, which will not be materialized to
             storage and will halt execution of downstream assets.
         freshness_policy (FreshnessPolicy): A constraint telling Dagster how often this asset is intended to be updated
             with respect to its root data.
+        auto_materialize_policy (AutoMaterializePolicy): (Experimental) This currently has no effect.
         retry_policy (Optional[RetryPolicy]): The retry policy for the op that computes the asset.
         code_version (Optional[str]): (Experimental) Version of the code that generates this asset. In
             general, versions should be set only for code that deterministically produces the same
             output when given the same inputs.
 
     Examples:
         .. code-block:: python
@@ -188,14 +194,15 @@
             compute_kind=check.opt_str_param(compute_kind, "compute_kind"),
             dagster_type=dagster_type,
             partitions_def=partitions_def,
             op_tags=op_tags,
             group_name=group_name,
             output_required=output_required,
             freshness_policy=freshness_policy,
+            auto_materialize_policy=auto_materialize_policy,
             retry_policy=retry_policy,
             code_version=code_version,
         )
 
     if compute_fn is not None:
         return create_asset()(compute_fn)
 
@@ -209,14 +216,17 @@
         )
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "asset")
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "asset")
 
+        if auto_materialize_policy is not None:
+            experimental_arg_warning("auto_materialize_policy", "asset")
+
         return create_asset()(fn)
 
     return inner
 
 
 class _Asset:
     def __init__(
@@ -234,14 +244,15 @@
         compute_kind: Optional[str] = None,
         dagster_type: Optional[DagsterType] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         op_tags: Optional[Mapping[str, Any]] = None,
         group_name: Optional[str] = None,
         output_required: bool = True,
         freshness_policy: Optional[FreshnessPolicy] = None,
+        auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
         retry_policy: Optional[RetryPolicy] = None,
         code_version: Optional[str] = None,
     ):
         self.name = name
 
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
@@ -260,17 +271,21 @@
         self.partitions_def = partitions_def
         self.op_tags = op_tags
         self.resource_defs = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
         self.group_name = group_name
         self.output_required = output_required
         self.freshness_policy = freshness_policy
         self.retry_policy = retry_policy
+        self.auto_materialize_policy = auto_materialize_policy
         self.code_version = code_version
 
     def __call__(self, fn: Callable) -> AssetsDefinition:
+        from dagster._config.structured_config import validate_resource_annotated_function
+
+        validate_resource_annotated_function(fn)
         asset_name = self.name or fn.__name__
 
         asset_ins = build_asset_ins(fn, self.ins or {}, self.non_argument_deps)
 
         out_asset_key = AssetKey(list(filter(None, [*(self.key_prefix or []), asset_name])))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=ExperimentalWarning)
@@ -344,14 +359,17 @@
             partitions_def=self.partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             resource_defs=self.resource_defs,
             group_names_by_key={out_asset_key: self.group_name} if self.group_name else None,
             freshness_policies_by_key={out_asset_key: self.freshness_policy}
             if self.freshness_policy
             else None,
+            auto_materialize_policies_by_key={out_asset_key: self.auto_materialize_policy}
+            if self.auto_materialize_policy
+            else None,
         )
 
 
 def multi_asset(
     *,
     outs: Mapping[str, AssetOut],
     name: Optional[str] = None,
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     format_docstring_for_description,
     get_function_params,
     get_valid_name_permutations,
     param_is_var_keyword,
     positional_arg_name_list,
 )
 from dagster._core.definitions.inference import infer_input_props
-from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.resource_annotation import (
+    get_resource_args,
+)
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.types.dagster_type import DagsterTypeKind
 from dagster._utils.backcompat import canonicalize_backcompat_args
 
 from ..input import In, InputDefinition
 from ..output import Out
 from ..policy import RetryPolicy
@@ -69,16 +71,20 @@
         # config will be checked within SolidDefinition
         self.config_schema = config_schema
 
         self.ins = check.opt_nullable_mapping_param(ins, "ins", key_type=str, value_type=In)
         self.out = out
 
     def __call__(self, fn: Callable[..., Any]) -> "OpDefinition":
+        from dagster._config.structured_config import validate_resource_annotated_function
+
         from ..op_definition import OpDefinition
 
+        validate_resource_annotated_function(fn)
+
         if not self.name:
             self.name = fn.__name__
 
         compute_fn = (
             DecoratedOpFunction(decorated_fn=fn)
             if self.decorator_takes_context
             else NoContextDecoratedOpFunction(decorated_fn=fn)
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     Sequence,
     Set,
     Union,
     cast,
 )
 
 import dagster._check as check
-from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.resource_annotation import (
+    get_resource_args,
+)
 from dagster._core.definitions.sensor_definition import get_context_param_name
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     ScheduleExecutionError,
     user_code_error_boundary,
 )
 from dagster._utils import ensure_gen
@@ -95,15 +97,18 @@
             that should execute when this schedule runs.
         default_status (DefaultScheduleStatus): Whether the schedule starts as running or not. The default
             status can be overridden from Dagit or via the GraphQL API.
         required_resource_keys (Optional[Set[str]]): The set of resource keys required by the schedule.
     """
 
     def inner(fn: RawScheduleEvaluationFunction) -> ScheduleDefinition:
+        from dagster._config.structured_config import validate_resource_annotated_function
+
         check.callable_param(fn, "fn")
+        validate_resource_annotated_function(fn)
 
         schedule_name = name or fn.__name__
 
         validated_tags = None
 
         # perform upfront validation of schedule tags
         if tags_fn and tags:
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.2.7/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Mapping, Optional, Union, overload
+from typing import AbstractSet, Mapping, Optional, Union, overload
 
+import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import (
     MetadataUserInput,
 )
 from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.source_asset import SourceAsset, SourceAssetObserveFunction
 from dagster._core.storage.io_manager import IOManagerDefinition
 
 
 @overload
 def observable_source_asset(observe_fn: SourceAssetObserveFunction) -> SourceAsset:
@@ -23,14 +25,15 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[IOManagerDefinition] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
+    required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> "_ObservableSourceAsset":
     ...
 
 
 @experimental
 def observable_source_asset(
@@ -40,14 +43,15 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[IOManagerDefinition] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
+    required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Union[SourceAsset, "_ObservableSourceAsset"]:
     """Create a `SourceAsset` with an associated observation function.
 
     The observation function of a source asset is wrapped inside of an op and can be executed as
     part of a job. Each execution generates an `AssetObservation` event associated with the source
     asset. The source asset observation function should return a metadata dictionary that will be
@@ -67,14 +71,15 @@
         io_manager_def (Optional[IOManagerDefinition]): (Experimental) The definition of the IOManager that will be used to load the contents of
             the source asset when it's used as an input to other assets inside a job.
         description (Optional[str]): The description of the asset.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the source asset.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If not provided,
             the name "default" is used.
+        required_resource_keys (Optional[Set[str]]): Set of resource keys required by the observe op.
         resource_defs (Optional[Mapping[str, ResourceDefinition]]): (Experimental) resource
             definitions that may be required by the :py:class:`dagster.IOManagerDefinition` provided in
             the `io_manager_def` argument.
         observe_fn (Optional[SourceAssetObserveFunction]) Observation function for the source asset.
     """
     if observe_fn is not None:
         return _ObservableSourceAsset()(observe_fn)
@@ -84,14 +89,15 @@
         key_prefix,
         metadata,
         io_manager_key,
         io_manager_def,
         description,
         partitions_def,
         group_name,
+        required_resource_keys,
         resource_defs,
     )
 
 
 class _ObservableSourceAsset:
     def __init__(
         self,
@@ -99,38 +105,52 @@
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         metadata: Optional[MetadataUserInput] = None,
         io_manager_key: Optional[str] = None,
         io_manager_def: Optional[IOManagerDefinition] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
+        required_resource_keys: Optional[AbstractSet[str]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ):
         self.name = name
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
         elif key_prefix is None:
             key_prefix = []
         self.key_prefix = key_prefix
         self.metadata = metadata
         self.io_manager_key = io_manager_key
         self.io_manager_def = io_manager_def
         self.description = description
         self.partitions_def = partitions_def
         self.group_name = group_name
+        self.required_resource_keys = required_resource_keys
         self.resource_defs = resource_defs
 
     def __call__(self, observe_fn: SourceAssetObserveFunction) -> SourceAsset:
         source_asset_name = self.name or observe_fn.__name__
         source_asset_key = AssetKey([*self.key_prefix, source_asset_name])
 
+        arg_resource_keys = {arg.name for arg in get_resource_args(observe_fn)}
+        decorator_resource_keys = set(self.required_resource_keys or [])
+        check.param_invariant(
+            len(decorator_resource_keys) == 0 or len(arg_resource_keys) == 0,
+            (
+                "Cannot specify resource requirements in both @op decorator and as arguments to the"
+                " decorated function"
+            ),
+        )
+        resolved_resource_keys = decorator_resource_keys.union(arg_resource_keys)
+
         return SourceAsset(
             key=source_asset_key,
             metadata=self.metadata,
             io_manager_key=self.io_manager_key,
             io_manager_def=self.io_manager_def,
             description=self.description,
             partitions_def=self.partitions_def,
             group_name=self.group_name,
+            _required_resource_keys=resolved_resource_keys,
             resource_defs=self.resource_defs,
             observe_fn=observe_fn,
         )
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.2.7/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/definitions_class.py` & `dagster-1.2.7/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/dependency.py` & `dagster-1.2.7/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/events.py` & `dagster-1.2.7/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/executor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.2.7/dagster/_core/definitions/external_asset_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
+    List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
 )
 
+from dagster._core.definitions.assets_job import ASSET_BASE_JOB_PREFIX
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.host_representation.external import ExternalRepository
 from dagster._core.host_representation.handle import RepositoryHandle
 from dagster._core.selector.subset_selector import DependencyGraph
 from dagster._core.workspace.workspace import IWorkspace
 
 from .asset_graph import AssetGraph
 from .events import AssetKey
@@ -31,34 +34,41 @@
         self,
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
+        auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         repo_handles_by_key: Mapping[AssetKey, RepositoryHandle],
         job_names_by_key: Mapping[AssetKey, Sequence[str]],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
     ):
         super().__init__(
             asset_dep_graph=asset_dep_graph,
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
+            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
         )
         self._repo_handles_by_key = repo_handles_by_key
         self._materialization_job_names_by_key = job_names_by_key
 
+        self._asset_keys_by_job_name: Mapping[str, List[AssetKey]] = defaultdict(list)
+        for asset_key, job_names in self._materialization_job_names_by_key.items():
+            for job_name in job_names:
+                self._asset_keys_by_job_name[job_name].append(asset_key)
+
     @classmethod
     def from_workspace(cls, context: IWorkspace) -> "ExternalAssetGraph":
         code_locations = (
             location_entry.code_location
             for location_entry in context.get_workspace_snapshot().values()
             if location_entry.code_location
         )
@@ -97,14 +107,15 @@
         source_asset_keys: Set[AssetKey] = set()
         partitions_defs_by_key: Dict[AssetKey, Optional[PartitionsDefinition]] = {}
         partition_mappings_by_key: Dict[AssetKey, Dict[AssetKey, PartitionMapping]] = defaultdict(
             defaultdict
         )
         group_names_by_key = {}
         freshness_policies_by_key = {}
+        auto_materialize_policies_by_key = {}
         asset_keys_by_atomic_execution_unit_id: Dict[str, Set[AssetKey]] = defaultdict(set)
         repo_handles_by_key = {
             node.asset_key: repo_handle
             for repo_handle, node in repo_handle_external_asset_nodes
             if not node.is_source
         }
         job_names_by_key = {
@@ -144,14 +155,15 @@
             partitions_defs_by_key[node.asset_key] = (
                 node.partitions_def_data.get_partitions_definition()
                 if node.partitions_def_data
                 else None
             )
             group_names_by_key[node.asset_key] = node.group_name
             freshness_policies_by_key[node.asset_key] = node.freshness_policy
+            auto_materialize_policies_by_key[node.asset_key] = node.auto_materialize_policy
 
             if node.atomic_execution_unit_id is not None:
                 asset_keys_by_atomic_execution_unit_id[node.atomic_execution_unit_id].add(
                     node.asset_key
                 )
 
         downstream: Dict[AssetKey, Set[AssetKey]] = defaultdict(set)
@@ -168,14 +180,15 @@
         return cls(
             asset_dep_graph={"upstream": upstream, "downstream": downstream},
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
+            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             repo_handles_by_key=repo_handles_by_key,
             job_names_by_key=job_names_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
         )
 
@@ -193,7 +206,23 @@
     def get_materialization_asset_keys_for_job(self, job_name: str) -> Sequence[AssetKey]:
         """Returns asset keys that are targeted for materialization in the given job."""
         return [
             k
             for k in self.non_source_asset_keys
             if job_name in self.get_materialization_job_names(k)
         ]
+
+    def get_asset_keys_for_job(self, job_name: str) -> Sequence[AssetKey]:
+        return self._asset_keys_by_job_name[job_name]
+
+    def get_implicit_job_name_for_assets(self, asset_keys: Iterable[AssetKey]) -> Optional[str]:
+        """Returns the name of the asset base job that contains all the given assets, or None if there is no such
+        job.
+
+        Note: all asset_keys should be in the same repository.
+        """
+        for job_name in sorted(self._asset_keys_by_job_name.keys()):
+            if not job_name.startswith(ASSET_BASE_JOB_PREFIX):
+                continue
+            if all(asset_key in self._asset_keys_by_job_name[job_name] for asset_key in asset_keys):
+                return job_name
+        return None
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/freshness_policy.py` & `dagster-1.2.7/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/graph_definition.py` & `dagster-1.2.7/dagster/_core/definitions/graph_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.config import ConfigMapping
 from dagster._core.definitions.definition_config_schema import IDefinitionConfigSchema
 from dagster._core.definitions.policy import RetryPolicy
 from dagster._core.definitions.resource_definition import ResourceDefinition
-from dagster._core.errors import DagsterInvalidDefinitionError
+from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 from dagster._core.selector.subset_selector import AssetSelectionData
 from dagster._core.types.dagster_type import (
     DagsterType,
     DagsterTypeKind,
     construct_dagster_type_dictionary,
 )
 
@@ -319,18 +319,16 @@
 
     def has_node_named(self, name: str) -> bool:
         check.str_param(name, "name")
         return name in self._node_dict
 
     def node_named(self, name: str) -> Node:
         check.str_param(name, "name")
-        check.invariant(
-            name in self._node_dict,
-            f"{self._name} has no op named {name}.",
-        )
+        if name not in self._node_dict:
+            raise DagsterInvariantViolationError(f"{self._name} has no op named {name}.")
 
         return self._node_dict[name]
 
     def get_node(self, handle: NodeHandle) -> Node:
         check.inst_param(handle, "handle", NodeHandle)
         current = handle
         lineage: List[str] = []
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/hook_definition.py` & `dagster-1.2.7/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/hook_invocation.py` & `dagster-1.2.7/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/inference.py` & `dagster-1.2.7/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/input.py` & `dagster-1.2.7/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/instigation_logger.py` & `dagster-1.2.7/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/job_definition.py` & `dagster-1.2.7/dagster/_core/definitions/job_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,19 @@
             "2.0.0",
             additional_warn_txt="Directly instantiate `RunRequest(partition_key=...)` instead.",
         )
 
         if not (self.partitions_def and self.partitioned_config):
             check.failed("Called run_request_for_partition on a non-partitioned job")
 
-        if isinstance(self.partitions_def, DynamicPartitionsDefinition) and not instance:
+        if (
+            isinstance(self.partitions_def, DynamicPartitionsDefinition)
+            and self.partitions_def.name
+            and not instance
+        ):
             check.failed(
                 "Must provide a dagster instance when calling run_request_for_partition on a "
                 "dynamic partition set"
             )
 
         partition = self.partitions_def.get_partition(
             partition_key, dynamic_partitions_store=instance, current_time=current_time
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.2.7/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/logger_definition.py` & `dagster-1.2.7/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/logger_invocation.py` & `dagster-1.2.7/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/materialize.py` & `dagster-1.2.7/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.2.7/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/metadata/table.py` & `dagster-1.2.7/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/mode.py` & `dagster-1.2.7/dagster/_core/definitions/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.2.7/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/node_container.py` & `dagster-1.2.7/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/node_definition.py` & `dagster-1.2.7/dagster/_core/definitions/node_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Sequence,
     Tuple,
 )
 
 import dagster._check as check
 from dagster._core.definitions.configurable import NamedConfigurableDefinition
 from dagster._core.definitions.policy import RetryPolicy
+from dagster._core.errors import DagsterInvariantViolationError
 
 from .hook_definition import HookDefinition
 from .utils import check_valid_name, validate_tags
 
 if TYPE_CHECKING:
     from dagster._core.types.dagster_type import DagsterType
 
@@ -143,14 +144,16 @@
 
     def has_output(self, name: str) -> bool:
         check.str_param(name, "name")
         return name in self._output_dict
 
     def output_def_named(self, name: str) -> "OutputDefinition":
         check.str_param(name, "name")
+        if name not in self._output_dict:
+            raise DagsterInvariantViolationError(f"{self._name} has no output named {name}.")
         return self._output_dict[name]
 
     @abstractmethod
     def iterate_node_defs(self) -> Iterable["NodeDefinition"]:
         ...
 
     @abstractmethod
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/observe.py` & `dagster-1.2.7/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/op_definition.py` & `dagster-1.2.7/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/op_invocation.py` & `dagster-1.2.7/dagster/_core/definitions/op_invocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import inspect
-from typing import TYPE_CHECKING, Any, Mapping, Optional, TypeVar, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import dagster._check as check
-from dagster._core.definitions.resource_definition import ResourceDefinition
+from dagster._core.decorator_utils import get_function_params
 from dagster._core.errors import (
-    DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
     DagsterTypeCheckDidNotPass,
 )
 
 from .events import (
     AssetMaterialization,
@@ -25,14 +35,66 @@
     from .decorators.op_decorator import DecoratedOpFunction
     from .op_definition import OpDefinition
     from .output import OutputDefinition
 
 T = TypeVar("T")
 
 
+class InputsAndResources(NamedTuple):
+    input_args: Tuple[Any, ...]
+    input_kwargs: Dict[str, Any]
+    resources_by_param_name: Dict[str, Any]
+
+
+def _separate_args_and_kwargs(
+    compute_fn: "DecoratedOpFunction",
+    args: Tuple[Any, ...],
+    kwargs: Dict[str, Any],
+    resource_arg_mapping: Dict[str, Any],
+) -> InputsAndResources:
+    """Given a decorated compute function, a set of args and kwargs, and set of resource param names,
+    separates the set of resource inputs from op/asset inputs returns a tuple of the categorized
+    args and kwargs.
+
+    We use the remaining args and kwargs to cleanly invoke the compute function, and we use the
+    extracted resource inputs to populate the execution context.
+    """
+    resource_inputs_from_args_and_kwargs = {}
+    params = get_function_params(compute_fn.decorated_fn)
+
+    adjusted_args = []
+
+    params_without_context = params[1:] if compute_fn.has_context_arg() else params
+
+    # Get any (non-kw) args that correspond to resource inputs & strip them from the args list
+    for i, arg in enumerate(args):
+        param = params_without_context[i] if i < len(params_without_context) else None
+        if param and param.kind != inspect.Parameter.KEYWORD_ONLY:
+            if param.name in resource_arg_mapping:
+                resource_inputs_from_args_and_kwargs[param.name] = arg
+                continue
+
+        adjusted_args.append(arg)
+
+    # Get any kwargs that correspond to resource inputs & strip them from the kwargs dict
+    for resource_arg in resource_arg_mapping:
+        if resource_arg in kwargs:
+            resource_inputs_from_args_and_kwargs[resource_arg] = kwargs[resource_arg]
+
+    adjusted_kwargs = {
+        k: v for k, v in kwargs.items() if k not in resource_inputs_from_args_and_kwargs
+    }
+
+    return InputsAndResources(
+        input_args=tuple(adjusted_args),
+        input_kwargs=adjusted_kwargs,
+        resources_by_param_name=resource_inputs_from_args_and_kwargs,
+    )
+
+
 def op_invocation_result(
     op_def_or_invocation: Union["OpDefinition", "PendingNodeInvocation[OpDefinition]"],
     context: Optional["UnboundOpExecutionContext"],
     *args,
     **kwargs,
 ) -> Any:
     from dagster._core.definitions.decorators.op_decorator import DecoratedOpFunction
@@ -55,39 +117,41 @@
     compute_fn = cast(DecoratedOpFunction, compute_fn)
 
     from ..execution.plan.compute_generator import invoke_compute_fn
 
     context = context or build_op_context()
 
     resource_arg_mapping = {arg.name: arg.name for arg in compute_fn.get_resource_args()}
-    resource_args_from_kwargs = {}
-    for resource_arg in resource_arg_mapping:
-        if resource_arg in kwargs:
-            resource_args_from_kwargs[resource_arg] = kwargs[resource_arg]
-            del kwargs[resource_arg]
 
-    resources_provided_in_multiple_places = (resource_args_from_kwargs) and (context.resource_keys)
+    # The user is allowed to invoke an op with an arbitrary mix of args and kwargs.
+    # We ensure that these args and kwargs are correctly categorized as inputs, config, or resource objects and then validated.
+    #
+    # Depending on arg/kwarg type, we do various things:
+    # - Any resources passed as parameters are also made available to user-defined code as part of the op execution context
+    # - Provide high-quality error messages (e.g. if something tried to pass a value to an input typed Nothing)
+    # - Default values are applied appropriately
+    # - Inputs are type checked
+    #
+    # We recollect all the varying args/kwargs into a dictionary and invoke the user-defined function with kwargs only.
+    extracted = _separate_args_and_kwargs(compute_fn, args, kwargs, resource_arg_mapping)
+
+    input_args = extracted.input_args
+    input_kwargs = extracted.input_kwargs
+    resources_by_param_name = extracted.resources_by_param_name
+
+    resources_provided_in_multiple_places = resources_by_param_name and context.resource_keys
     if resources_provided_in_multiple_places:
         raise DagsterInvalidInvocationError("Cannot provide resources in both context and kwargs")
 
-    if resource_args_from_kwargs:
-        context = context.replace_resources(resource_args_from_kwargs)
+    if resources_by_param_name:
+        context = context.replace_resources(resources_by_param_name)
+
+    bound_context = context.bind(op_def_or_invocation)
 
-    try:
-        bound_context = context.bind(op_def_or_invocation)
-    except DagsterInvalidDefinitionError as e:
-        if any(isinstance(arg, ResourceDefinition) for arg in args):
-            raise DagsterInvalidInvocationError(
-                str(e)
-                + "\n\nIf directly invoking an op/asset, you may not provide resources as"
-                " positional"
-                " arguments, only as keyword arguments."
-            ) from e
-        raise
-    input_dict = _resolve_inputs(op_def, args, kwargs, bound_context)
+    input_dict = _resolve_inputs(op_def, input_args, input_kwargs, bound_context)
 
     result = invoke_compute_fn(
         fn=compute_fn.decorated_fn,
         context=bound_context,
         kwargs=input_dict,
         context_arg_provided=compute_fn.has_context_arg(),
         config_arg_cls=compute_fn.get_config_arg().annotation
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/output.py` & `dagster-1.2.7/dagster/_core/definitions/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
         ) from e
 
 
 class DynamicOutputDefinition(OutputDefinition):
     """Variant of :py:class:`OutputDefinition <dagster.OutputDefinition>` for an
     output that will dynamically alter the graph at runtime.
 
-    When using in a composition function such as :py:func:`@pipeline <dagster.pipeline>`,
-    dynamic outputs must be used with either
+    When using in a composition function such as :py:func:`@job <dagster.job>`,
+    dynamic outputs must be used with either:
 
     * ``map`` - clone downstream nodes for each separate :py:class:`DynamicOutput`
     * ``collect`` - gather across all :py:class:`DynamicOutput` in to a list
 
     Uses the same constructor as :py:class:`OutputDefinition <dagster.OutputDefinition>`
 
         .. code-block:: python
@@ -227,15 +227,15 @@
             )
             def files_in_directory(context):
                 path = context.op_config["path"]
                 dirname, _, filenames = next(os.walk(path))
                 for file in filenames:
                     yield DynamicOutput(os.path.join(dirname, file), mapping_key=_clean(file))
 
-            @pipeline
+            @job
             def process_directory():
                 files = files_in_directory()
 
                 # use map to invoke an op on each dynamic output
                 file_results = files.map(process_file)
 
                 # use collect to gather the results in to a list
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/partition.py` & `dagster-1.2.7/dagster/_core/definitions/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
 import pendulum
 from dateutil.relativedelta import relativedelta
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, public
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
+from dagster._core.definitions.run_request import (
+    AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest,
+)
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.tags import PARTITION_NAME_TAG, PARTITION_SET_TAG
 from dagster._serdes import whitelist_for_serdes
 from dagster._seven.compat.pendulum import PendulumDateTime, to_timezone
 from dagster._utils.backcompat import deprecation_warning, experimental_arg_warning
 from dagster._utils.cached_method import cached_method
 from dagster._utils.schedules import schedule_execution_time_iterator
@@ -600,15 +604,15 @@
         .. code-block:: python
 
             fruits = DynamicPartitionsDefinition(name="fruits")
 
             @sensor(job=my_job)
             def my_sensor(context):
                 context.instance.add_dynamic_partitions(fruits.name, [partition_key])
-                return my_job.run_request_for_partition(partition_key, instance=context.instance)
+                return RunRequest(partition_key=partition_key)
 
     """
 
     def __new__(
         cls,
         partition_fn: Optional[
             Callable[[Optional[datetime]], Union[Sequence[Partition], Sequence[str]]]
@@ -706,14 +710,24 @@
                 " is older than 1.1.18."
             )
 
         return dynamic_partitions_store.has_dynamic_partition(
             partitions_def_name=self._validated_name(), partition_key=partition_key
         )
 
+    def build_add_request(self, partition_keys: Sequence[str]) -> AddDynamicPartitionsRequest:
+        check.sequence_param(partition_keys, "partition_keys", of_type=str)
+        validated_name = self._validated_name()
+        return AddDynamicPartitionsRequest(validated_name, partition_keys)
+
+    def build_delete_request(self, partition_keys: Sequence[str]) -> DeleteDynamicPartitionsRequest:
+        check.sequence_param(partition_keys, "partition_keys", of_type=str)
+        validated_name = self._validated_name()
+        return DeleteDynamicPartitionsRequest(validated_name, partition_keys)
+
 
 class PartitionedConfig(Generic[T_cov]):
     """Defines a way of configuring a job where the job can be run on one of a discrete set of
     partitions, and each partition corresponds to run configuration for the job.
 
     Setting PartitionedConfig as the config for a job allows you to launch backfills for that job
     and view the run history across partitions.
@@ -763,28 +777,36 @@
     ) -> Mapping[str, Any]:
         """Generates the run config corresponding to a partition key.
 
         Args:
             partition_key (str): the key for a partition that should be used to generate a run config.
         """
         partition = self._key_to_partition(partition_key, current_time, dynamic_partitions_store)
+        return self.get_run_config_for_partition(partition)
+
+    def get_run_config_for_partition(
+        self,
+        partition: Partition,
+    ) -> Mapping[str, Any]:
+        """Generates the run config corresponding to a partition.
+
+        Args:
+            partition: the partition that should be used to generate a run config.
+        """
         return copy.deepcopy(self.run_config_for_partition_fn(partition))
 
-    def get_tags_for_partition_key(
+    def get_tags_for_partition(
         self,
-        partition_key: str,
-        dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
-        current_time: Optional[datetime] = None,
+        partition: Partition,
         job_name: Optional[str] = None,
     ) -> Mapping[str, str]:
         from dagster._core.host_representation.external_data import (
             external_partition_set_name_for_job_name,
         )
 
-        partition = self._key_to_partition(partition_key, current_time, dynamic_partitions_store)
         user_tags = (
             validate_tags(self._tags_for_partition_fn(partition), allow_reserved_tags=False)
             if self._tags_for_partition_fn
             else {}
         )
         system_tags = {
             **self.partitions_def.get_tags_for_partition_key(partition.name),
@@ -794,14 +816,24 @@
                 else {}
             ),
         }
         # `PartitionSetDefinition` has been deleted but we still need to attach this special tag in
         # order for reexecution against partitions to work properly.
         return {**user_tags, **system_tags}
 
+    def get_tags_for_partition_key(
+        self,
+        partition_key: str,
+        dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
+        current_time: Optional[datetime] = None,
+        job_name: Optional[str] = None,
+    ) -> Mapping[str, str]:
+        partition = self._key_to_partition(partition_key, current_time, dynamic_partitions_store)
+        return self.get_tags_for_partition(partition, job_name)
+
     def _key_to_partition(
         self,
         partition_key: str,
         current_time: Optional[datetime],
         dynamic_partitions_store: Optional[DynamicPartitionsStore],
     ) -> Partition[T_cov]:
         matches = [
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/partition_mapping.py` & `dagster-1.2.7/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.2.7/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/pipeline_base.py` & `dagster-1.2.7/dagster/_core/definitions/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/pipeline_definition.py` & `dagster-1.2.7/dagster/_core/definitions/pipeline_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/policy.py` & `dagster-1.2.7/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/preset.py` & `dagster-1.2.7/dagster/_core/definitions/preset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/reconstruct.py` & `dagster-1.2.7/dagster/_core/definitions/reconstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
 ReconstructableJob = ReconstructablePipeline
 
 
 def reconstructable(target: Callable[..., "PipelineDefinition"]) -> ReconstructablePipeline:
     """Create a :py:class:`~dagster._core.definitions.reconstructable.ReconstructablePipeline` from a
     function that returns a :py:class:`~dagster.PipelineDefinition`/:py:class:`~dagster.JobDefinition`,
-    or a function decorated with :py:func:`@pipeline <dagster.pipeline>`/:py:func:`@job <dagster.job>`.
+    or a function decorated with :py:func:`@job <dagster.job>`.
 
     When your pipeline/job must cross process boundaries, e.g., for execution on multiple nodes or
     in different systems (like ``dagstermill``), Dagster must know how to reconstruct the pipeline/job
     on the other side of the process boundary.
 
     Passing a job created with ``~dagster.GraphDefinition.to_job`` to ``reconstructable()``,
     requires you to wrap that job's definition in a module-scoped function, and pass that function
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,20 @@
             base_job = self.get_job(ASSET_BASE_JOB_PREFIX)
             if all(key in base_job.asset_layer.assets_defs_by_key for key in asset_keys):
                 return base_job
         else:
             i = 0
             while self.has_job(f"{ASSET_BASE_JOB_PREFIX}_{i}"):
                 base_job = self.get_job(f"{ASSET_BASE_JOB_PREFIX}_{i}")
-                if all(key in base_job.asset_layer.assets_defs_by_key for key in asset_keys):
+
+                if all(
+                    key in base_job.asset_layer.assets_defs_by_key
+                    or base_job.asset_layer.is_observable_for_asset(key)
+                    for key in asset_keys
+                ):
                     return base_job
 
                 i += 1
 
         return None
 
     def get_maybe_subset_job_def(
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.2.7/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.2.7/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/resource_annotation.py` & `dagster-1.2.7/dagster/_core/definitions/resource_annotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 from dagster._core.definitions.resource_definition import ResourceDefinition
 
 
 def get_resource_args(fn) -> Sequence[Parameter]:
     return [param for param in get_function_params(fn) if _is_resource_annotated(param)]
 
 
+RESOURCE_PARAM_METADATA = "resource_param"
+
+
 def _is_resource_annotated(param: Parameter) -> bool:
     extends_resource_definition = False
     try:
         extends_resource_definition = isinstance(param.annotation, type) and issubclass(
             param.annotation, ResourceDefinition
         )
     except TypeError:
         # Using builtin Python types in python 3.9+ will raise a TypeError when using issubclass
         # even though the isinstance check will succeed (as will inspect.isclass), for example
         # list[dict[str, str]] will raise a TypeError
         pass
 
     return (extends_resource_definition) or (
         hasattr(param.annotation, "__metadata__")
-        and getattr(param.annotation, "__metadata__") == ("resource_output",)
+        and getattr(param.annotation, "__metadata__") == (RESOURCE_PARAM_METADATA,)
     )
 
 
 T = TypeVar("T")
-Resource = Annotated[T, "resource_output"]
+ResourceParam = Annotated[T, RESOURCE_PARAM_METADATA]
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/resource_definition.py` & `dagster-1.2.7/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/resource_invocation.py` & `dagster-1.2.7/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/resource_requirement.py` & `dagster-1.2.7/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/run_config.py` & `dagster-1.2.7/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/run_config_schema.py` & `dagster-1.2.7/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/schedule_definition.py` & `dagster-1.2.7/dagster/_core/definitions/schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,14 +776,15 @@
                         "Must provide repository def to build_schedule_context when yielding"
                         " partitioned run requests"
                     )
 
                 scheduled_target = context.repository_def.get_job(self._target.pipeline_name)
                 resolved_request = run_request.with_resolved_tags_and_config(
                     target_definition=scheduled_target,
+                    dynamic_partitions_requests=[],
                     current_time=context.scheduled_execution_time,
                     dynamic_partitions_store=dynamic_partitions_store,
                 )
             else:
                 resolved_request = run_request
 
             resolved_run_requests.append(
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.2.7/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/selector.py` & `dagster-1.2.7/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/sensor_definition.py` & `dagster-1.2.7/dagster/_core/definitions/sensor_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import logging
+from collections import defaultdict
 from contextlib import ExitStack
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -24,15 +25,17 @@
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.instigation_logger import InstigationLogger
 from dagster._core.definitions.partition import (
     CachingDynamicPartitionsLoader,
 )
-from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.resource_annotation import (
+    get_resource_args,
+)
 from dagster._core.definitions.resource_definition import (
     Resources,
 )
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidSubsetError,
@@ -48,14 +51,16 @@
 )
 from .asset_selection import AssetSelection
 from .graph_definition import GraphDefinition
 from .job_definition import JobDefinition
 from .mode import DEFAULT_MODE_NAME
 from .pipeline_definition import PipelineDefinition
 from .run_request import (
+    AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest,
     PipelineRunReaction,
     RunRequest,
     SensorResult,
     SkipReason,
 )
 from .target import DirectTarget, ExecutableDefinition, RepoRelativeTarget
 from .unresolved_asset_job_definition import UnresolvedAssetJobDefinition
@@ -385,14 +390,64 @@
             "Sensor evaluation function expected context argument, but no context argument "
             "was provided when invoking."
         )
 
     return context or build_sensor_context()
 
 
+def _check_dynamic_partitions_requests(
+    dynamic_partitions_requests: Sequence[
+        Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]
+    ],
+) -> None:
+    req_keys_to_add_by_partitions_def_name = defaultdict(set)
+    req_keys_to_delete_by_partitions_def_name = defaultdict(set)
+
+    for req in dynamic_partitions_requests:
+        duplicate_req_keys_to_delete = req_keys_to_delete_by_partitions_def_name.get(
+            req.partitions_def_name, set()
+        ).intersection(req.partition_keys)
+        duplicate_req_keys_to_add = req_keys_to_add_by_partitions_def_name.get(
+            req.partitions_def_name, set()
+        ).intersection(req.partition_keys)
+        if isinstance(req, AddDynamicPartitionsRequest):
+            if duplicate_req_keys_to_delete:
+                raise DagsterInvariantViolationError(
+                    "Dynamic partition requests cannot contain both add and delete requests for"
+                    " the same partition keys.Invalid request: partitions_def_name"
+                    f" '{req.partitions_def_name}', partition_keys: {duplicate_req_keys_to_delete}"
+                )
+            elif duplicate_req_keys_to_add:
+                raise DagsterInvariantViolationError(
+                    "Cannot request to add duplicate dynamic partition keys: \npartitions_def_name"
+                    f" '{req.partitions_def_name}', partition_keys: {duplicate_req_keys_to_add}"
+                )
+            req_keys_to_add_by_partitions_def_name[req.partitions_def_name].update(
+                req.partition_keys
+            )
+        elif isinstance(req, DeleteDynamicPartitionsRequest):
+            if duplicate_req_keys_to_delete:
+                raise DagsterInvariantViolationError(
+                    "Cannot request to add duplicate dynamic partition keys: \npartitions_def_name"
+                    f" '{req.partitions_def_name}', partition_keys:"
+                    f" {req_keys_to_add_by_partitions_def_name}"
+                )
+            elif duplicate_req_keys_to_add:
+                raise DagsterInvariantViolationError(
+                    "Dynamic partition requests cannot contain both add and delete requests for"
+                    " the same partition keys.Invalid request: partitions_def_name"
+                    f" '{req.partitions_def_name}', partition_keys: {duplicate_req_keys_to_add}"
+                )
+            req_keys_to_delete_by_partitions_def_name[req.partitions_def_name].update(
+                req.partition_keys
+            )
+        else:
+            check.failed(f"Unexpected dynamic partition request type: {req}")
+
+
 class SensorDefinition:
     """Define a sensor that initiates a set of runs based on some external state.
 
     Args:
         evaluation_fn (Callable[[SensorEvaluationContext]]): The core evaluation function for the
             sensor, which is run at an interval to determine whether a run should be launched or
             not. Takes a :py:class:`~dagster.SensorEvaluationContext`.
@@ -438,14 +493,16 @@
         description: Optional[str] = None,
         job: Optional[ExecutableDefinition] = None,
         jobs: Optional[Sequence[ExecutableDefinition]] = None,
         default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
         asset_selection: Optional[AssetSelection] = None,
         required_resource_keys: Optional[Set[str]] = None,
     ):
+        from dagster._config.structured_config import validate_resource_annotated_function
+
         if evaluation_fn is None:
             raise DagsterInvalidDefinitionError("Must provide evaluation_fn to SensorDefinition.")
 
         if (
             sum(
                 [
                     int(job is not None),
@@ -501,14 +558,15 @@
         self._targets = check.opt_list_param(targets, "targets", (DirectTarget, RepoRelativeTarget))
         self._default_status = check.inst_param(
             default_status, "default_status", DefaultSensorStatus
         )
         self._asset_selection = check.opt_inst_param(
             asset_selection, "asset_selection", AssetSelection
         )
+        validate_resource_annotated_function(self._raw_fn)
         resource_arg_names: Set[str] = {arg.name for arg in get_resource_args(self._raw_fn)}
 
         check.param_invariant(
             len(required_resource_keys or []) == 0 or len(resource_arg_names) == 0,
             (
                 "Cannot specify resource requirements in both @sensor decorator and as arguments to"
                 " the decorated function"
@@ -585,14 +643,17 @@
         context = check.inst_param(context, "context", SensorEvaluationContext)
 
         result = list(self._evaluation_fn(context))
 
         skip_message: Optional[str] = None
         run_requests: List[RunRequest] = []
         pipeline_run_reactions: List[PipelineRunReaction] = []
+        dynamic_partitions_requests: Optional[
+            Sequence[Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]]
+        ] = []
         updated_cursor = context.cursor
 
         if not result or result == [None]:
             skip_message = "Sensor function returned an empty result"
         elif len(result) == 1:
             item = result[0]
             check.inst(item, (SkipReason, RunRequest, PipelineRunReaction, SensorResult))
@@ -601,14 +662,19 @@
                 run_requests = list(item.run_requests) if item.run_requests else []
                 skip_message = (
                     item.skip_reason.skip_message
                     if item.skip_reason
                     else (None if run_requests else "Sensor function returned an empty result")
                 )
 
+                _check_dynamic_partitions_requests(
+                    item.dynamic_partitions_requests or [],
+                )
+                dynamic_partitions_requests = item.dynamic_partitions_requests or []
+
                 if item.cursor and context.cursor_updated:
                     raise DagsterInvariantViolationError(
                         "SensorResult.cursor cannot be set if context.update_cursor() was called."
                     )
                 updated_cursor = item.cursor
 
             elif isinstance(item, RunRequest):
@@ -647,24 +713,26 @@
                     check.failed(
                         "Expected a single SkipReason or one or more PipelineRunReaction: "
                         "received both PipelineRunReaction and SkipReason"
                     )
                 else:
                     check.failed("Expected a single SkipReason: received multiple SkipReasons")
 
+        _check_dynamic_partitions_requests(dynamic_partitions_requests)
         resolved_run_requests = self.resolve_run_requests(
-            run_requests, context, self._asset_selection
+            run_requests, context, self._asset_selection, dynamic_partitions_requests
         )
 
         return SensorExecutionData(
             resolved_run_requests,
             skip_message,
             updated_cursor,
             pipeline_run_reactions,
             captured_log_key=context.log_key if context.has_captured_logs() else None,
+            dynamic_partitions_requests=dynamic_partitions_requests,
         )
 
     def has_loadable_targets(self) -> bool:
         for target in self._targets:
             if isinstance(target, DirectTarget):
                 return True
         return False
@@ -682,14 +750,17 @@
         return targets
 
     def resolve_run_requests(
         self,
         run_requests: Sequence[RunRequest],
         context: SensorEvaluationContext,
         asset_selection: Optional[AssetSelection],
+        dynamic_partitions_requests: Sequence[
+            Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]
+        ],
     ) -> Sequence[RunRequest]:
         def _get_repo_job_by_name(context: SensorEvaluationContext, job_name: str) -> JobDefinition:
             if context.repository_def is None:
                 raise DagsterInvariantViolationError(
                     "Must provide repository def to build_sensor_context when yielding partitioned"
                     " run requests"
                 )
@@ -740,14 +811,15 @@
                     context, run_request.job_name if run_request.job_name else target_names[0]
                 )
                 resolved_run_requests.append(
                     run_request.with_resolved_tags_and_config(
                         target_definition=selected_job,
                         current_time=None,
                         dynamic_partitions_store=dynamic_partitions_store,
+                        dynamic_partitions_requests=dynamic_partitions_requests,
                     )
                 )
             else:
                 resolved_run_requests.append(run_request)
 
         return resolved_run_requests
 
@@ -781,42 +853,57 @@
         "_SensorExecutionData",
         [
             ("run_requests", Optional[Sequence[RunRequest]]),
             ("skip_message", Optional[str]),
             ("cursor", Optional[str]),
             ("pipeline_run_reactions", Optional[Sequence[PipelineRunReaction]]),
             ("captured_log_key", Optional[Sequence[str]]),
+            (
+                "dynamic_partitions_requests",
+                Optional[
+                    Sequence[Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]]
+                ],
+            ),
         ],
     )
 ):
     def __new__(
         cls,
         run_requests: Optional[Sequence[RunRequest]] = None,
         skip_message: Optional[str] = None,
         cursor: Optional[str] = None,
         pipeline_run_reactions: Optional[Sequence[PipelineRunReaction]] = None,
         captured_log_key: Optional[Sequence[str]] = None,
+        dynamic_partitions_requests: Optional[
+            Sequence[Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]]
+        ] = None,
     ):
         check.opt_sequence_param(run_requests, "run_requests", RunRequest)
         check.opt_str_param(skip_message, "skip_message")
         check.opt_str_param(cursor, "cursor")
         check.opt_sequence_param(
             pipeline_run_reactions, "pipeline_run_reactions", PipelineRunReaction
         )
         check.opt_list_param(captured_log_key, "captured_log_key", str)
+        check.opt_sequence_param(
+            dynamic_partitions_requests,
+            "dynamic_partitions_requests",
+            (AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest),
+        )
         check.invariant(
             not (run_requests and skip_message), "Found both skip data and run request data"
         )
         return super(SensorExecutionData, cls).__new__(
             cls,
             run_requests=run_requests,
             skip_message=skip_message,
             cursor=cursor,
             pipeline_run_reactions=pipeline_run_reactions,
             captured_log_key=captured_log_key,
+            dynamic_partitions_requests=dynamic_partitions_requests,
         )
 
 
 def wrap_sensor_evaluation(
     sensor_name: str,
     fn: RawSensorEvaluationFunction,
 ) -> SensorEvaluationFunction:
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/source_asset.py` & `dagster-1.2.7/dagster/_core/definitions/source_asset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from __future__ import annotations
 
 import warnings
-from typing import TYPE_CHECKING, Dict, Iterator, Mapping, Optional, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    AbstractSet,
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    Mapping,
+    Optional,
+    cast,
+)
 
-from typing_extensions import Protocol, TypeAlias
+from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, public
-from dagster._core.decorator_utils import has_at_least_one_parameter
+from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.data_version import DATA_VERSION_TAG, DataVersion
 from dagster._core.definitions.events import AssetKey, AssetObservation, CoercibleToAssetKey
 from dagster._core.definitions.metadata import (
     ArbitraryMetadataMapping,
     MetadataMapping,
     normalize_metadata,
 )
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.resource_requirement import (
     ResourceAddable,
     ResourceRequirement,
     SourceAssetIOManagerRequirement,
+    ensure_requirements_satisfied,
     get_resource_key_conflicts,
 )
 from dagster._core.definitions.utils import (
     DEFAULT_GROUP_NAME,
     DEFAULT_IO_MANAGER_KEY,
     validate_group_name,
 )
@@ -33,39 +45,19 @@
 from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._utils.backcompat import ExperimentalWarning, experimental_arg_warning
 from dagster._utils.merger import merge_dicts
 
 if TYPE_CHECKING:
     from dagster._core.execution.context.compute import (
         OpExecutionContext,
-        SourceAssetObserveContext,
     )
 
 
-class SourceAssetObserveFunctionWithContext(Protocol):
-    @property
-    def __name__(self) -> str:
-        ...
-
-    def __call__(self, context: "SourceAssetObserveContext") -> DataVersion:
-        ...
-
-
-class SourceAssetObserveFunctionNoContext(Protocol):
-    @property
-    def __name__(self) -> str:
-        ...
-
-    def __call__(self) -> DataVersion:
-        ...
-
-
-SourceAssetObserveFunction: TypeAlias = Union[
-    SourceAssetObserveFunctionWithContext, SourceAssetObserveFunctionNoContext
-]
+# Going with this catch-all for the time-being to permit pythonic resources
+SourceAssetObserveFunction: TypeAlias = Callable[..., Any]
 
 
 class SourceAsset(ResourceAddable):
     """A SourceAsset represents an asset that will be loaded by (but not updated by) Dagster.
 
     Attributes:
         key (Union[AssetKey, Sequence[str], str]): The key of the asset.
@@ -100,14 +92,20 @@
         io_manager_key: Optional[str] = None,
         io_manager_def: Optional[IOManagerDefinition] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         observe_fn: Optional[SourceAssetObserveFunction] = None,
+        # This is currently private because it is necessary for source asset observation functions,
+        # but we have not yet decided on a final API for associated one or more ops with a source
+        # asset. If we were to make this public, then we would have a canonical public
+        # `required_resource_keys` used for observation that might end up conflicting with a set of
+        # required resource keys for a different operation.
+        _required_resource_keys: Optional[AbstractSet[str]] = None,
         # Add additional fields to with_resources and with_group below
     ):
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "SourceAsset.__new__")
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "SourceAsset.__new__")
@@ -138,14 +136,17 @@
         self.io_manager_key = check.opt_str_param(io_manager_key, "io_manager_key")
         self.partitions_def = check.opt_inst_param(
             partitions_def, "partitions_def", PartitionsDefinition
         )
         self.group_name = validate_group_name(group_name)
         self.description = check.opt_str_param(description, "description")
         self.observe_fn = check.opt_callable_param(observe_fn, "observe_fn")
+        self._required_resource_keys = check.opt_set_param(
+            _required_resource_keys, "_required_resource_keys", of_type=str
+        )
         self._node_def = None
 
     def get_io_manager_key(self) -> str:
         return self.io_manager_key or DEFAULT_IO_MANAGER_KEY
 
     @property
     def io_manager_def(self) -> Optional[IOManagerDefinition]:
@@ -166,20 +167,29 @@
 
     @public
     @property
     def is_observable(self) -> bool:
         return self.node_def is not None
 
     def _get_op_def_compute_fn(self, observe_fn: SourceAssetObserveFunction):
-        from dagster._core.definitions.decorators.op_decorator import DecoratedOpFunction
+        from dagster._core.definitions.decorators.op_decorator import (
+            DecoratedOpFunction,
+            is_context_provided,
+        )
 
-        observe_fn_has_context = has_at_least_one_parameter(observe_fn)
+        observe_fn_has_context = is_context_provided(get_function_params(observe_fn))
 
         def fn(context: OpExecutionContext):
-            data_version = observe_fn(context) if observe_fn_has_context else observe_fn()  # type: ignore
+            resource_kwarg_keys = [param.name for param in get_resource_args(observe_fn)]
+            resource_kwargs = {key: getattr(context.resources, key) for key in resource_kwarg_keys}
+            data_version = (
+                observe_fn(context, **resource_kwargs)
+                if observe_fn_has_context
+                else observe_fn(**resource_kwargs)
+            )
 
             check.inst(
                 data_version,
                 DataVersion,
                 "Source asset observation function must return a DataVersion",
             )
             tags = {DATA_VERSION_TAG: data_version.value}
@@ -189,24 +199,29 @@
                     tags=tags,
                 )
             )
 
         return DecoratedOpFunction(fn)
 
     @property
+    def required_resource_keys(self) -> AbstractSet[str]:
+        return {requirement.key for requirement in self.get_resource_requirements()}
+
+    @property
     def node_def(self) -> Optional[OpDefinition]:
         """Op that generates observation metadata for a source asset."""
         if self.observe_fn is None:
             return None
 
         if self._node_def is None:
             self._node_def = OpDefinition(
                 compute_fn=self._get_op_def_compute_fn(self.observe_fn),
                 name=self.key.to_python_identifier(),
                 description=self.description,
+                required_resource_keys=self._required_resource_keys,
             )
         return self._node_def
 
     def with_resources(self, resource_defs) -> "SourceAsset":
         from dagster._core.execution.resources_init import get_transitive_required_resource_keys
 
         overlapping_keys = get_resource_key_conflicts(self.resource_defs, resource_defs)
@@ -217,22 +232,26 @@
                 f"{sorted(list(overlapping_keys))}. Either remove the existing "
                 "resources from the asset or change the resource keys so that "
                 "they don't overlap."
             )
 
         merged_resource_defs = merge_dicts(resource_defs, self.resource_defs)
 
+        # Ensure top-level resource requirements are met - except for
+        # io_manager, since that is a default it can be resolved later.
+        ensure_requirements_satisfied(merged_resource_defs, list(self.get_resource_requirements()))
+
         io_manager_def = merged_resource_defs.get(self.get_io_manager_key())
         if not io_manager_def and self.get_io_manager_key() != DEFAULT_IO_MANAGER_KEY:
             raise DagsterInvalidDefinitionError(
                 f"SourceAsset with asset key {self.key} requires IO manager with key"
                 f" '{self.get_io_manager_key()}', but none was provided."
             )
         relevant_keys = get_transitive_required_resource_keys(
-            {self.get_io_manager_key()}, merged_resource_defs
+            {*self._required_resource_keys, self.get_io_manager_key()}, merged_resource_defs
         )
 
         relevant_resource_defs = {
             key: resource_def
             for key, resource_def in merged_resource_defs.items()
             if key in relevant_keys
         }
@@ -250,14 +269,15 @@
                 io_manager_key=io_manager_key,
                 description=self.description,
                 partitions_def=self.partitions_def,
                 metadata=self.raw_metadata,
                 resource_defs=relevant_resource_defs,
                 group_name=self.group_name,
                 observe_fn=self.observe_fn,
+                _required_resource_keys=self._required_resource_keys,
             )
 
     def with_group_name(self, group_name: str) -> "SourceAsset":
         if self.group_name != DEFAULT_GROUP_NAME:
             raise DagsterInvalidDefinitionError(
                 "A group name has already been provided to source asset"
                 f" {self.key.to_user_string()}"
@@ -272,17 +292,20 @@
                 io_manager_key=self.io_manager_key,
                 io_manager_def=self.io_manager_def,
                 description=self.description,
                 partitions_def=self.partitions_def,
                 group_name=group_name,
                 resource_defs=self.resource_defs,
                 observe_fn=self.observe_fn,
+                _required_resource_keys=self._required_resource_keys,
             )
 
     def get_resource_requirements(self) -> Iterator[ResourceRequirement]:
+        if self.node_def is not None:
+            yield from self.node_def.get_resource_requirements()
         yield SourceAssetIOManagerRequirement(
             key=self.get_io_manager_key(), asset_key=self.key.to_string()
         )
         for source_key, resource_def in self.resource_defs.items():
             yield from resource_def.get_resource_requirements(outer_context=source_key)
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/step_launcher.py` & `dagster-1.2.7/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/target.py` & `dagster-1.2.7/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.2.7/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.2.7/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.2.7/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,19 @@
         if not self.partitions_def:
             check.failed("Called run_request_for_partition on a non-partitioned job")
 
         partitioned_config = PartitionedConfig.from_flexible_config(
             self.config, self.partitions_def
         )
 
-        if isinstance(self.partitions_def, DynamicPartitionsDefinition) and not instance:
+        if (
+            isinstance(self.partitions_def, DynamicPartitionsDefinition)
+            and self.partitions_def.name
+            and not instance
+        ):
             check.failed(
                 "Must provide a dagster instance when calling run_request_for_partition on a "
                 "dynamic partition set"
             )
 
         partition = self.partitions_def.get_partition(
             partition_key, dynamic_partitions_store=instance, current_time=current_time
@@ -190,19 +194,14 @@
 
         asset_keys_by_partitions_def = defaultdict(set)
         for asset_key in selected_asset_keys:
             partitions_def = asset_graph.get_partitions_def(asset_key)
             if partitions_def is not None:
                 asset_keys_by_partitions_def[partitions_def].add(asset_key)
 
-        if len(asset_keys_by_partitions_def) == 0 and self.partitions_def:
-            raise DagsterInvalidDefinitionError(
-                "Tried to build a partitioned job, but none of the selected assets are partitioned."
-            )
-
         if len(asset_keys_by_partitions_def) > 1:
             keys_by_partitions_def_str = "\n".join(
                 f"{partitions_def}: {asset_keys}"
                 for partitions_def, asset_keys in asset_keys_by_partitions_def.items()
             )
             raise DagsterInvalidDefinitionError(
                 f"Multiple partitioned assets exist in assets job '{self.name}'. Selected assets"
```

### Comparing `dagster-1.2.6/dagster/_core/definitions/utils.py` & `dagster-1.2.7/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/definitions/version_strategy.py` & `dagster-1.2.7/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/errors.py` & `dagster-1.2.7/dagster/_core/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Dagster runtime.
 """
 
 from __future__ import annotations
 
 import sys
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Callable, Iterator, Optional, Type
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, Type
 
 import dagster._check as check
 from dagster._utils.interrupts import raise_interrupts_as
 
 if TYPE_CHECKING:
     from dagster._core.log_manager import DagsterLogManager
 
@@ -64,14 +64,82 @@
     """
 
 
 class DagsterInvalidDeserializationVersionError(DagsterError):
     """Indicates that a serialized value has an unsupported version and cannot be deserialized."""
 
 
+PYTHONIC_CONFIG_ERROR_VERBIAGE = """
+This config type can be a:
+    - Python primitive type
+        - int, float, bool, str, list
+    - A Python Dict or List type containing other valid types
+    - Custom data classes extending dagster.Config
+    - A Pydantic discriminated union type (https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions)
+"""
+
+PYTHONIC_RESOURCE_ADDITIONAL_TYPES = """
+
+If this config type represents a resource dependency, its annotation must either:
+    - Extend dagster.ConfigurableResource, dagster.ConfigurableIOManager, or
+    - Be wrapped in a ResourceDependency annotation, e.g. ResourceDependency[{invalid_type_str}]
+"""
+
+
+def _generate_pythonic_config_error_message(
+    config_class: Optional[Type],
+    field_name: Optional[str],
+    invalid_type: Any,
+    is_resource: bool = False,
+) -> str:
+    invalid_type_name = getattr(invalid_type, "__name__", "<my type>")
+    pythonic_config_error_verbiage = (
+        PYTHONIC_CONFIG_ERROR_VERBIAGE + (PYTHONIC_RESOURCE_ADDITIONAL_TYPES if is_resource else "")
+    ).format(invalid_type_str=invalid_type_name)
+
+    return (
+        """
+Error defining Dagster config class{config_class}{field_name}.
+Unable to resolve config type {invalid_type} to a supported Dagster config type.
+
+{PYTHONIC_CONFIG_ERROR_VERBIAGE}"""
+    ).format(
+        config_class=f" {repr(config_class)}" if config_class else "",
+        field_name=f" on field '{field_name}'" if field_name else "",
+        invalid_type=repr(invalid_type),
+        PYTHONIC_CONFIG_ERROR_VERBIAGE=pythonic_config_error_verbiage,
+    )
+
+
+class DagsterInvalidPythonicConfigDefinitionError(DagsterError):
+    """Indicates that you have attempted to construct a Pythonic config or resource class with an invalid value.
+    """
+
+    def __init__(
+        self,
+        config_class: Optional[Type],
+        field_name: Optional[str],
+        invalid_type: Any,
+        is_resource: bool = False,
+        **kwargs,
+    ):
+        self.invalid_type = invalid_type
+        self.field_name = field_name
+        self.config_class = config_class
+        super(DagsterInvalidPythonicConfigDefinitionError, self).__init__(
+            _generate_pythonic_config_error_message(
+                config_class=config_class,
+                field_name=field_name,
+                invalid_type=invalid_type,
+                is_resource=is_resource,
+            ),
+            **kwargs,
+        )
+
+
 CONFIG_ERROR_VERBIAGE = """
 This value can be a:
     - Field
     - Python primitive types that resolve to dagster config types
         - int, float, bool, str, list.
     - A dagster config type: Int, Float, Bool, Array, Optional, Selector, Shape, Permissive, Map
     - A bare python dictionary, which is wrapped in Field(Shape(...)). Any values
```

### Comparing `dagster-1.2.6/dagster/_core/event_api.py` & `dagster-1.2.7/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/events/__init__.py` & `dagster-1.2.7/dagster/_core/events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     ) -> "DagsterEvent":
         event = DagsterEvent(
             event_type_value=check.inst_param(event_type, "event_type", DagsterEventType).value,
             pipeline_name=step_context.pipeline_name,
             step_handle=step_context.step.handle,
             node_handle=step_context.step.node_handle,
             step_kind_value=step_context.step.kind.value,
-            logging_tags=step_context.logging_tags,
+            logging_tags=step_context.event_tags,
             event_specific_data=_validate_event_specific_data(event_type, event_specific_data),
             message=check.opt_str_param(message, "message"),
             pid=os.getpid(),
         )
 
         log_step_event(step_context, event)
 
@@ -1267,15 +1267,15 @@
 
         event = DagsterEvent(
             event_type_value=event_type.value,
             pipeline_name=step_context.pipeline_name,
             step_handle=step_context.step.handle,
             node_handle=step_context.step.node_handle,
             step_kind_value=step_context.step.kind.value,
-            logging_tags=step_context.logging_tags,
+            logging_tags=step_context.event_tags,
             message=(
                 'Finished the execution of hook "{hook_name}" triggered for "{solid_name}".'
             ).format(hook_name=hook_def.name, solid_name=step_context.solid.name),
         )
 
         step_context.log.log_dagster_event(
             level=logging.DEBUG, msg=event.message or "", dagster_event=event
@@ -1291,15 +1291,15 @@
 
         event = DagsterEvent(
             event_type_value=event_type.value,
             pipeline_name=step_context.pipeline_name,
             step_handle=step_context.step.handle,
             node_handle=step_context.step.node_handle,
             step_kind_value=step_context.step.kind.value,
-            logging_tags=step_context.logging_tags,
+            logging_tags=step_context.event_tags,
             event_specific_data=_validate_event_specific_data(
                 event_type,
                 HookErroredData(
                     error=serializable_error_info_from_exc_info(error.original_exc_info)
                 ),
             ),
         )
@@ -1316,15 +1316,15 @@
 
         event = DagsterEvent(
             event_type_value=event_type.value,
             pipeline_name=step_context.pipeline_name,
             step_handle=step_context.step.handle,
             node_handle=step_context.step.node_handle,
             step_kind_value=step_context.step.kind.value,
-            logging_tags=step_context.logging_tags,
+            logging_tags=step_context.event_tags,
             message=(
                 'Skipped the execution of hook "{hook_name}". It did not meet its triggering '
                 'condition during the execution of "{solid_name}".'
             ).format(hook_name=hook_def.name, solid_name=step_context.solid.name),
         )
 
         step_context.log.log_dagster_event(
@@ -1680,21 +1680,21 @@
 
 
 @whitelist_for_serdes(storage_field_names={"file_key": "log_key"})
 class ComputeLogsCaptureData(
     NamedTuple(
         "_ComputeLogsCaptureData",
         [
-            ("file_key", Sequence[str]),  # renamed log_key => file_key to avoid confusion
+            ("file_key", str),  # renamed log_key => file_key to avoid confusion
             ("step_keys", Sequence[str]),
             ("external_url", Optional[str]),
         ],
     )
 ):
-    def __new__(cls, file_key, step_keys, external_url=None):
+    def __new__(cls, file_key: str, step_keys: Sequence[str], external_url: Optional[str] = None):
         return super(ComputeLogsCaptureData, cls).__new__(
             cls,
             file_key=check.str_param(file_key, "file_key"),
             step_keys=check.opt_list_param(step_keys, "step_keys", of_type=str),
             external_url=check.opt_str_param(external_url, "external_url"),
         )
```

### Comparing `dagster-1.2.6/dagster/_core/events/log.py` & `dagster-1.2.7/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/events/utils.py` & `dagster-1.2.7/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/api.py` & `dagster-1.2.7/dagster/_core/execution/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,21 +51,19 @@
 from .execute_job_result import ExecuteJobResult
 from .results import PipelineExecutionResult
 
 ## Brief guide to the execution APIs
 # | function name               | operates over      | sync  | supports    | creates new DagsterRun  |
 # |                             |                    |       | reexecution | in instance             |
 # | --------------------------- | ------------------ | ----- | ----------- | ----------------------- |
-# | execute_pipeline_iterator   | IPipeline          | async | no          | yes                     |
-# | execute_pipeline            | IPipeline          | sync  | no          | yes                     |
+# | execute_job                 | ReconstructableJob | sync  | yes         | yes                     |
 # | execute_run_iterator        | DagsterRun         | async | (1)         | no                      |
 # | execute_run                 | DagsterRun         | sync  | (1)         | no                      |
 # | execute_plan_iterator       | ExecutionPlan      | async | (2)         | no                      |
 # | execute_plan                | ExecutionPlan      | sync  | (2)         | no                      |
-# | reexecute_pipeline          | IPipeline          | sync  | yes         | yes                     |
 #
 # Notes on reexecution support:
 # (1) The appropriate bits must be set on the DagsterRun passed to this function. Specifically,
 #     parent_run_id and root_run_id must be set and consistent, and if a solids_to_execute or
 #     step_keys_to_execute are set they must be consistent with the parent and root runs.
 # (2) As for (1), but the ExecutionPlan passed must also agree in all relevant bits.
 
@@ -296,89 +294,14 @@
             dagster_run,
             instance,
         ),
         output_capture=output_capture,
     )
 
 
-def execute_pipeline_iterator(
-    pipeline: Union[PipelineDefinition, IPipeline],
-    run_config: Optional[Mapping[str, object]] = None,
-    mode: Optional[str] = None,
-    preset: Optional[str] = None,
-    tags: Optional[Mapping[str, str]] = None,
-    solid_selection: Optional[Sequence[str]] = None,
-    instance: Optional[DagsterInstance] = None,
-) -> Iterator[DagsterEvent]:
-    """Execute a pipeline iteratively.
-
-    Rather than package up the result of running a pipeline into a single object, like
-    :py:func:`execute_pipeline`, this function yields the stream of events resulting from pipeline
-    execution.
-
-    This is intended to allow the caller to handle these events on a streaming basis in whatever
-    way is appropriate.
-
-    Parameters:
-        pipeline (Union[IPipeline, PipelineDefinition]): The pipeline to execute.
-        run_config (Optional[dict]): The configuration that parametrizes this run,
-            as a dict.
-        mode (Optional[str]): The name of the pipeline mode to use. You may not set both ``mode``
-            and ``preset``.
-        preset (Optional[str]): The name of the pipeline preset to use. You may not set both
-            ``mode`` and ``preset``.
-        tags (Optional[Dict[str, Any]]): Arbitrary key-value pairs that will be added to pipeline
-            logs.
-        solid_selection (Optional[List[str]]): A list of solid selection queries (including single
-            solid names) to execute. For example:
-
-            - ``['some_solid']``: selects ``some_solid`` itself.
-            - ``['*some_solid']``: select ``some_solid`` and all its ancestors (upstream dependencies).
-            - ``['*some_solid+++']``: select ``some_solid``, all its ancestors, and its descendants
-              (downstream dependencies) within 3 levels down.
-            - ``['*some_solid', 'other_solid_a', 'other_solid_b+']``: select ``some_solid`` and all its
-              ancestors, ``other_solid_a`` itself, and ``other_solid_b`` and its direct child solids.
-        instance (Optional[DagsterInstance]): The instance to execute against. If this is ``None``,
-            an ephemeral instance will be used, and no artifacts will be persisted from the run.
-
-    Returns:
-      Iterator[DagsterEvent]: The stream of events resulting from pipeline execution.
-    """
-    with ephemeral_instance_if_missing(instance) as execute_instance:
-        pipeline, repository_load_data = _pipeline_with_repository_load_data(pipeline)
-
-        (
-            pipeline,
-            run_config,
-            mode,
-            tags,
-            solids_to_execute,
-            solid_selection,
-        ) = _check_execute_pipeline_args(
-            pipeline=pipeline,
-            run_config=run_config,
-            mode=mode,
-            preset=preset,
-            tags=tags,
-            solid_selection=solid_selection,
-        )
-
-        dagster_run = execute_instance.create_run_for_pipeline(
-            pipeline_def=pipeline.get_definition(),
-            run_config=run_config,
-            mode=mode,
-            solid_selection=solid_selection,
-            solids_to_execute=solids_to_execute,
-            tags=tags,
-            repository_load_data=repository_load_data,
-        )
-
-        return execute_run_iterator(pipeline, dagster_run, execute_instance)
-
-
 @contextmanager
 def ephemeral_instance_if_missing(
     instance: Optional[DagsterInstance],
 ) -> Iterator[DagsterInstance]:
     if instance:
         yield instance
     else:
@@ -449,15 +372,15 @@
     execution. For most testing purposes, :py:meth:`~dagster.JobDefinition.
     execute_in_process` will be more suitable, but when wanting to run
     execution using an out-of-process executor (such as :py:class:`dagster.
     multiprocess_executor`), then `execute_job` is suitable.
 
     `execute_job` expects a persistent :py:class:`DagsterInstance` for
     execution, meaning the `$DAGSTER_HOME` environment variable must be set.
-    It als expects a reconstructable pointer to a :py:class:`JobDefinition` so
+    It also expects a reconstructable pointer to a :py:class:`JobDefinition` so
     that it can be reconstructed in separate processes. This can be done by
     wrapping the ``JobDefinition`` in a call to :py:func:`dagster.
     reconstructable`.
 
     .. code-block:: python
 
         from dagster import DagsterInstance, execute_job, job, reconstructable
@@ -536,229 +459,126 @@
       :py:class:`JobExecutionResult`: The result of job execution.
     """
     check.inst_param(job, "job", ReconstructablePipeline)
     check.inst_param(instance, "instance", DagsterInstance)
     check.opt_sequence_param(asset_selection, "asset_selection", of_type=AssetKey)
 
     # get the repository load data here because we call job.get_definition() later in this fn
-    job_def, _ = _pipeline_with_repository_load_data(job)
+    job_def, _ = _job_with_repository_load_data(job)
 
     if reexecution_options is not None and op_selection is not None:
         raise DagsterInvariantViolationError(
             "re-execution and op selection cannot be used together at this time."
         )
 
     if reexecution_options:
         if run_config is None:
             run = check.not_none(instance.get_run_by_id(reexecution_options.parent_run_id))
             run_config = run.run_config
-        result = reexecute_pipeline(
-            pipeline=job_def,
+        result = _reexecute_job(
+            job_arg=job_def,
             parent_run_id=reexecution_options.parent_run_id,
             run_config=run_config,
             step_selection=list(reexecution_options.step_selection),
-            mode=None,
-            preset=None,
             tags=tags,
             instance=instance,
             raise_on_error=raise_on_error,
         )
     else:
-        result = _logged_execute_pipeline(
-            pipeline=job_def,
+        result = _logged_execute_job(
+            job_arg=job_def,
             instance=instance,
             run_config=run_config,
-            mode=None,
-            preset=None,
             tags=tags,
-            solid_selection=op_selection,
+            op_selection=op_selection,
             raise_on_error=raise_on_error,
             asset_selection=asset_selection,
         )
 
     # We use PipelineExecutionResult to construct the JobExecutionResult.
     return ExecuteJobResult(
         job_def=cast(ReconstructableJob, job_def).get_definition(),
         reconstruct_context=result.reconstruct_context(),
         event_list=result.event_list,
         dagster_run=instance.get_run_by_id(result.run_id),
     )
 
 
-def execute_pipeline(
-    pipeline: Union[PipelineDefinition, IPipeline],
-    run_config: Optional[Mapping[str, object]] = None,
-    mode: Optional[str] = None,
-    preset: Optional[str] = None,
-    tags: Optional[Mapping[str, str]] = None,
-    solid_selection: Optional[Sequence[str]] = None,
-    instance: Optional[DagsterInstance] = None,
-    raise_on_error: bool = True,
-) -> PipelineExecutionResult:
-    """Execute a pipeline synchronously.
-
-    Users will typically call this API when testing pipeline execution, or running standalone
-    scripts.
-
-    Parameters:
-        pipeline (Union[IPipeline, PipelineDefinition]): The pipeline to execute.
-        run_config (Optional[dict]): The configuration that parametrizes this run,
-            as a dict.
-        mode (Optional[str]): The name of the pipeline mode to use. You may not set both ``mode``
-            and ``preset``.
-        preset (Optional[str]): The name of the pipeline preset to use. You may not set both
-            ``mode`` and ``preset``.
-        tags (Optional[Dict[str, Any]]): Arbitrary key-value pairs that will be added to pipeline
-            logs.
-        instance (Optional[DagsterInstance]): The instance to execute against. If this is ``None``,
-            an ephemeral instance will be used, and no artifacts will be persisted from the run.
-        raise_on_error (Optional[bool]): Whether or not to raise exceptions when they occur.
-            Defaults to ``True``, since this is the most useful behavior in test.
-        solid_selection (Optional[List[str]]): A list of solid selection queries (including single
-            solid names) to execute. For example:
-
-            - ``['some_solid']``: selects ``some_solid`` itself.
-            - ``['*some_solid']``: select ``some_solid`` and all its ancestors (upstream dependencies).
-            - ``['*some_solid+++']``: select ``some_solid``, all its ancestors, and its descendants
-              (downstream dependencies) within 3 levels down.
-            - ``['*some_solid', 'other_solid_a', 'other_solid_b+']``: select ``some_solid`` and all its
-              ancestors, ``other_solid_a`` itself, and ``other_solid_b`` and its direct child solids.
-
-    Returns:
-      :py:class:`PipelineExecutionResult`: The result of pipeline execution.
-
-    For the asynchronous version, see :py:func:`execute_pipeline_iterator`.
-    """
-    with ephemeral_instance_if_missing(instance) as execute_instance:
-        return _logged_execute_pipeline(
-            pipeline,
-            instance=execute_instance,
-            run_config=run_config,
-            mode=mode,
-            preset=preset,
-            tags=tags,
-            solid_selection=solid_selection,
-            raise_on_error=raise_on_error,
-        )
-
-
 @telemetry_wrapper
-def _logged_execute_pipeline(
-    pipeline: Union[IPipeline, PipelineDefinition],
+def _logged_execute_job(
+    job_arg: Union[IPipeline, PipelineDefinition],
     instance: DagsterInstance,
     run_config: Optional[Mapping[str, object]] = None,
-    mode: Optional[str] = None,
-    preset: Optional[str] = None,
     tags: Optional[Mapping[str, str]] = None,
-    solid_selection: Optional[Sequence[str]] = None,
+    op_selection: Optional[Sequence[str]] = None,
     raise_on_error: bool = True,
     asset_selection: Optional[Sequence[AssetKey]] = None,
 ) -> PipelineExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
-    pipeline, repository_load_data = _pipeline_with_repository_load_data(pipeline)
+    job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
     (
-        pipeline,
+        job_arg,
         run_config,
         mode,
         tags,
         solids_to_execute,
-        solid_selection,
-    ) = _check_execute_pipeline_args(
-        pipeline=pipeline,
+        op_selection,
+    ) = _check_execute_job_args(
+        job_arg=job_arg,
         run_config=run_config,
-        mode=mode,
-        preset=preset,
         tags=tags,
-        solid_selection=solid_selection,
+        op_selection=op_selection,
     )
 
-    log_repo_stats(instance=instance, pipeline=pipeline, source="execute_pipeline")
+    log_repo_stats(instance=instance, pipeline=job_arg, source="execute_pipeline")
 
     dagster_run = instance.create_run_for_pipeline(
-        pipeline_def=pipeline.get_definition(),
+        pipeline_def=job_arg.get_definition(),
         run_config=run_config,
         mode=mode,
-        solid_selection=solid_selection,
+        solid_selection=op_selection,
         solids_to_execute=solids_to_execute,
         tags=tags,
         pipeline_code_origin=(
-            pipeline.get_python_origin() if isinstance(pipeline, ReconstructablePipeline) else None
+            job_arg.get_python_origin() if isinstance(job_arg, ReconstructableJob) else None
         ),
         repository_load_data=repository_load_data,
         asset_selection=frozenset(asset_selection) if asset_selection else None,
     )
 
     return execute_run(
-        pipeline,
+        job_arg,
         dagster_run,
         instance,
         raise_on_error=raise_on_error,
     )
 
 
-def reexecute_pipeline(
-    pipeline: Union[IPipeline, PipelineDefinition],
+def _reexecute_job(
+    job_arg: Union[IPipeline, PipelineDefinition],
     parent_run_id: str,
     run_config: Optional[Mapping[str, object]] = None,
     step_selection: Optional[Sequence[str]] = None,
-    mode: Optional[str] = None,
-    preset: Optional[str] = None,
     tags: Optional[Mapping[str, str]] = None,
     instance: Optional[DagsterInstance] = None,
     raise_on_error: bool = True,
 ) -> PipelineExecutionResult:
-    """Reexecute an existing pipeline run.
-
-    Users will typically call this API when testing pipeline reexecution, or running standalone
-    scripts.
-
-    Parameters:
-        pipeline (Union[IPipeline, PipelineDefinition]): The pipeline to execute.
-        parent_run_id (str): The id of the previous run to reexecute. The run must exist in the
-            instance.
-        run_config (Optional[dict]): The configuration that parametrizes this run,
-            as a dict.
-        solid_selection (Optional[List[str]]): A list of solid selection queries (including single
-            solid names) to execute. For example:
-
-            - ``['some_solid']``: selects ``some_solid`` itself.
-            - ``['*some_solid']``: select ``some_solid`` and all its ancestors (upstream dependencies).
-            - ``['*some_solid+++']``: select ``some_solid``, all its ancestors, and its descendants
-              (downstream dependencies) within 3 levels down.
-            - ``['*some_solid', 'other_solid_a', 'other_solid_b+']``: select ``some_solid`` and all its
-              ancestors, ``other_solid_a`` itself, and ``other_solid_b`` and its direct child solids.
-
-        mode (Optional[str]): The name of the pipeline mode to use. You may not set both ``mode``
-            and ``preset``.
-        preset (Optional[str]): The name of the pipeline preset to use. You may not set both
-            ``mode`` and ``preset``.
-        tags (Optional[Dict[str, Any]]): Arbitrary key-value pairs that will be added to pipeline
-            logs.
-        instance (Optional[DagsterInstance]): The instance to execute against. If this is ``None``,
-            an ephemeral instance will be used, and no artifacts will be persisted from the run.
-        raise_on_error (Optional[bool]): Whether or not to raise exceptions when they occur.
-            Defaults to ``True``, since this is the most useful behavior in test.
-
-    Returns:
-      :py:class:`PipelineExecutionResult`: The result of pipeline execution.
-    """
+    """Reexecute an existing job run."""
     check.opt_sequence_param(step_selection, "step_selection", of_type=str)
 
     check.str_param(parent_run_id, "parent_run_id")
 
     with ephemeral_instance_if_missing(instance) as execute_instance:
-        pipeline, repository_load_data = _pipeline_with_repository_load_data(pipeline)
+        job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
-        (pipeline, run_config, mode, tags, _, _) = _check_execute_pipeline_args(
-            pipeline=pipeline,
+        (job_arg, run_config, mode, tags, _, _) = _check_execute_job_args(
+            job_arg=job_arg,
             run_config=run_config,
-            mode=mode,
-            preset=preset,
             tags=tags,
         )
 
         parent_dagster_run = execute_instance.get_run_by_id(parent_run_id)
         if parent_dagster_run is None:
             check.failed(
                 "No parent run with id {parent_run_id} found in instance.".format(
@@ -767,47 +587,45 @@
             )
 
         execution_plan: Optional[ExecutionPlan] = None
         # resolve step selection DSL queries using parent execution information
         if step_selection:
             execution_plan = _resolve_reexecute_step_selection(
                 execute_instance,
-                pipeline,
+                job_arg,
                 mode,
                 run_config,
                 cast(DagsterRun, parent_dagster_run),
                 step_selection,
             )
 
         if parent_dagster_run.asset_selection:
-            pipeline = pipeline.subset_for_execution(
+            job_arg = job_arg.subset_for_execution(
                 solid_selection=None, asset_selection=parent_dagster_run.asset_selection
             )
 
         dagster_run = execute_instance.create_run_for_pipeline(
-            pipeline_def=pipeline.get_definition(),
+            pipeline_def=job_arg.get_definition(),
             execution_plan=execution_plan,
             run_config=run_config,
             mode=mode,
             tags=tags,
             solid_selection=parent_dagster_run.solid_selection,
             asset_selection=parent_dagster_run.asset_selection,
             solids_to_execute=parent_dagster_run.solids_to_execute,
             root_run_id=parent_dagster_run.root_run_id or parent_dagster_run.run_id,
             parent_run_id=parent_dagster_run.run_id,
             pipeline_code_origin=(
-                pipeline.get_python_origin()
-                if isinstance(pipeline, ReconstructablePipeline)
-                else None
+                job_arg.get_python_origin() if isinstance(job_arg, ReconstructableJob) else None
             ),
             repository_load_data=repository_load_data,
         )
 
         return execute_run(
-            pipeline,
+            job_arg,
             dagster_run,
             execute_instance,
             raise_on_error=raise_on_error,
         )
     check.failed("Should not reach here.")
 
 
@@ -871,21 +689,21 @@
             dagster_run=dagster_run,
             instance=instance,
             retry_mode=retry_mode,
         )
     )
 
 
-def _check_pipeline(pipeline: Union[PipelineDefinition, IPipeline]) -> IPipeline:
+def _check_pipeline(job_arg: Union[PipelineDefinition, IPipeline]) -> IPipeline:
     # backcompat
-    if isinstance(pipeline, PipelineDefinition):
-        pipeline = InMemoryPipeline(pipeline)
+    if isinstance(job_arg, PipelineDefinition):
+        job_arg = InMemoryPipeline(job_arg)
 
-    check.inst_param(pipeline, "pipeline", IPipeline)
-    return pipeline
+    check.inst_param(job_arg, "job_arg", IPipeline)
+    return job_arg
 
 
 def _get_execution_plan_from_run(
     pipeline: IPipeline,
     dagster_run: DagsterRun,
     instance: DagsterInstance,
 ) -> ExecutionPlan:
@@ -1033,14 +851,20 @@
                     pipeline_context,
                     (
                         "Execution was interrupted unexpectedly. No user initiated termination"
                         " request was found, not treating as failure because run will be resumed."
                     ),
                     EngineEventData(),
                 )
+            elif reloaded_run and reloaded_run.status == DagsterRunStatus.FAILURE:
+                event = DagsterEvent.engine_event(
+                    pipeline_context,
+                    "Execution was interrupted for a run that was already in a failure state.",
+                    EngineEventData(),
+                )
             else:
                 event = DagsterEvent.pipeline_failure(
                     pipeline_context,
                     (
                         "Execution was interrupted unexpectedly. "
                         "No user initiated termination request was found, treating as failure."
                     ),
@@ -1109,117 +933,51 @@
                 raise
             finally:
                 for event in self.execution_context_manager.shutdown_context():
                     if not generator_closed:
                         yield event
 
 
-def _check_execute_pipeline_args(
-    pipeline: Union[PipelineDefinition, IPipeline],
+def _check_execute_job_args(
+    job_arg: Union[PipelineDefinition, IPipeline],
     run_config: Optional[Mapping[str, object]],
-    mode: Optional[str],
-    preset: Optional[str],
     tags: Optional[Mapping[str, str]],
-    solid_selection: Optional[Sequence[str]] = None,
+    op_selection: Optional[Sequence[str]] = None,
 ) -> Tuple[
     IPipeline,
     Optional[Mapping],
     Optional[str],
     Mapping[str, str],
     Optional[AbstractSet[str]],
     Optional[Sequence[str]],
 ]:
-    pipeline = _check_pipeline(pipeline)
-    pipeline_def = pipeline.get_definition()
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    job_arg = _check_pipeline(job_arg)
+    job_def = job_arg.get_definition()
+    check.inst_param(job_def, "job_def", JobDefinition)
 
     run_config = check.opt_mapping_param(run_config, "run_config")
-    check.opt_str_param(mode, "mode")
-    check.opt_str_param(preset, "preset")
-    check.invariant(
-        not (mode is not None and preset is not None),
-        "You may set only one of `mode` (got {mode}) or `preset` (got {preset}).".format(
-            mode=mode, preset=preset
-        ),
-    )
 
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
-    check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
+    check.opt_sequence_param(op_selection, "solid_selection", of_type=str)
 
-    if preset is not None:
-        pipeline_preset = pipeline_def.get_preset(preset)
+    mode = job_def.get_default_mode_name()
 
-        if pipeline_preset.run_config is not None:
-            check.invariant(
-                (not run_config) or (pipeline_preset.run_config == run_config),
-                "The environment set in preset '{preset}' does not agree with the environment "
-                "passed in the `run_config` argument.".format(preset=preset),
-            )
-
-            run_config = pipeline_preset.run_config
-
-        # load solid_selection from preset
-        if pipeline_preset.solid_selection is not None:
-            check.invariant(
-                solid_selection is None or solid_selection == pipeline_preset.solid_selection,
-                "The solid_selection set in preset '{preset}', {preset_subset}, does not agree with"
-                " the `solid_selection` argument: {solid_selection}".format(
-                    preset=preset,
-                    preset_subset=pipeline_preset.solid_selection,
-                    solid_selection=solid_selection,
-                ),
-            )
-            solid_selection = pipeline_preset.solid_selection
-
-        check.invariant(
-            mode is None or mode == pipeline_preset.mode,
-            "Mode {mode} does not agree with the mode set in preset '{preset}': "
-            "('{preset_mode}')".format(preset=preset, preset_mode=pipeline_preset.mode, mode=mode),
-        )
-
-        mode = pipeline_preset.mode
-
-        tags = merge_dicts(pipeline_preset.tags, tags)
-
-    if mode is not None:
-        if not pipeline_def.has_mode_definition(mode):
-            raise DagsterInvariantViolationError(
-                (
-                    "You have attempted to execute pipeline {name} with mode {mode}. "
-                    "Available modes: {modes}"
-                ).format(
-                    name=pipeline_def.name,
-                    mode=mode,
-                    modes=pipeline_def.available_modes,
-                )
-            )
-    else:
-        if pipeline_def.is_multi_mode:
-            raise DagsterInvariantViolationError(
-                (
-                    "Pipeline {name} has multiple modes (Available modes: {modes}) and you have "
-                    "attempted to execute it without specifying a mode. Set "
-                    "mode property on the DagsterRun object."
-                ).format(name=pipeline_def.name, modes=pipeline_def.available_modes)
-            )
-        mode = pipeline_def.get_default_mode_name()
-
-    tags = merge_dicts(pipeline_def.tags, tags)
+    tags = merge_dicts(job_def.tags, tags)
 
     # generate pipeline subset from the given solid_selection
-    if solid_selection:
-        pipeline = pipeline.subset_for_execution(solid_selection)
+    if op_selection:
+        job_arg = job_arg.subset_for_execution(op_selection)
 
     return (
-        pipeline,
+        job_arg,
         run_config,
         mode,
         tags,
-        pipeline.solids_to_execute,
-        solid_selection,
+        job_arg.solids_to_execute,
+        op_selection,
     )
 
 
 def _resolve_reexecute_step_selection(
     instance: DagsterInstance,
     pipeline: IPipeline,
     mode: Optional[str],
@@ -1246,19 +1004,19 @@
         step_keys_to_execute=list(step_keys_to_execute),
         known_state=state.update_for_step_selection(step_keys_to_execute),
         tags=parent_dagster_run.tags,
     )
     return execution_plan
 
 
-def _pipeline_with_repository_load_data(
-    pipeline: Union[PipelineDefinition, IPipeline],
+def _job_with_repository_load_data(
+    job_arg: Union[PipelineDefinition, IPipeline],
 ) -> Tuple[Union[PipelineDefinition, IPipeline], Optional[RepositoryLoadData]]:
     """For ReconstructablePipeline, generate and return any required RepositoryLoadData, alongside
     a ReconstructablePipeline with this repository load data baked in.
     """
-    if isinstance(pipeline, ReconstructablePipeline):
+    if isinstance(job_arg, ReconstructablePipeline):
         # Unless this ReconstructablePipeline alread has repository_load_data attached, this will
         # force the repository_load_data to be computed from scratch.
-        repository_load_data = pipeline.repository.get_definition().repository_load_data
-        return pipeline.with_repository_load_data(repository_load_data), repository_load_data
-    return pipeline, None
+        repository_load_data = job_arg.repository.get_definition().repository_load_data
+        return job_arg.with_repository_load_data(repository_load_data), repository_load_data
+    return job_arg, None
```

### Comparing `dagster-1.2.6/dagster/_core/execution/asset_backfill.py` & `dagster-1.2.7/dagster/_core/execution/asset_backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     find_parent_materialized_asset_partitions,
 )
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.definitions.assets_job import is_base_asset_job_name
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.mode import DEFAULT_MODE_NAME
+from dagster._core.definitions.partition import PartitionsSubset
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.errors import DagsterBackfillFailedError
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation import (
     ExternalExecutionPlan,
     ExternalPipeline,
@@ -86,14 +87,31 @@
             .sources()
             .resolve(self.target_subset.asset_graph)
         )
         return list(
             self.target_subset.filter_asset_keys(root_asset_keys).iterate_asset_partitions()
         )
 
+    def get_target_root_partitions_subset(self) -> PartitionsSubset:
+        """Returns the most upstream partitions subset that was targeted by the backfill."""
+        partitioned_asset_keys = {
+            asset_key
+            for asset_key in self.target_subset.asset_keys
+            if self.target_subset.asset_graph.get_partitions_def(asset_key) is not None
+        }
+
+        root_partitioned_asset_keys = (
+            AssetSelection.keys(*partitioned_asset_keys)
+            .sources()
+            .resolve(self.target_subset.asset_graph)
+        )
+
+        # Return the targeted partitions for the root partitioned asset keys
+        return self.target_subset.get_partitions_subset(next(iter(root_partitioned_asset_keys)))
+
     def get_num_partitions(self) -> Optional[int]:
         """Only valid when the same number of partitions are targeted in every asset.
 
         When not valid, returns None.
         """
         asset_partition_nums = {
             len(subset) for subset in self.target_subset.partitions_subsets_by_asset_key.values()
@@ -446,23 +464,30 @@
 
         next_latest_storage_id = instance_queryer.get_latest_storage_id(
             DagsterEventType.ASSET_MATERIALIZATION
         )
         updated_materialized_subset = AssetGraphSubset(asset_graph)
         failed_and_downstream_subset = AssetGraphSubset(asset_graph)
     else:
+        target_parent_asset_keys = {
+            parent
+            for target_asset_key in asset_backfill_data.target_subset.asset_keys
+            for parent in asset_graph.get_parents(target_asset_key)
+        }
+        target_asset_keys_and_parents = (
+            asset_backfill_data.target_subset.asset_keys | target_parent_asset_keys
+        )
         (
             parent_materialized_asset_partitions,
             next_latest_storage_id,
         ) = find_parent_materialized_asset_partitions(
             asset_graph=asset_graph,
             instance_queryer=instance_queryer,
-            target_asset_selection=AssetSelection.keys(
-                *asset_backfill_data.target_subset.asset_keys
-            ),
+            target_asset_keys=asset_backfill_data.target_subset.asset_keys,
+            target_asset_keys_and_parents=target_asset_keys_and_parents,
             latest_storage_id=asset_backfill_data.latest_storage_id,
         )
         initial_candidates.update(parent_materialized_asset_partitions)
 
         yield None
 
         recently_materialized_asset_partitions = AssetGraphSubset(asset_graph)
```

### Comparing `dagster-1.2.6/dagster/_core/execution/backfill.py` & `dagster-1.2.7/dagster/_core/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Mapping, NamedTuple, Optional, Sequence, Tuple
 
 from dagster import _check as check
 from dagster._core.definitions import AssetKey
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
+from dagster._core.definitions.partition import PartitionsSubset
 from dagster._core.errors import (
     DagsterDefinitionChangedDeserializationError,
 )
 from dagster._core.execution.bulk_actions import BulkActionType
 from dagster._core.host_representation.origin import ExternalPartitionSetOrigin
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.workspace.workspace import IWorkspace
@@ -160,14 +161,33 @@
                 )
                 for asset_key in partitions_status_counts_by_asset_key
             }
 
         else:
             return {}
 
+    def get_target_root_partitions_subset(
+        self, workspace: IWorkspace
+    ) -> Optional[PartitionsSubset]:
+        if not self.is_valid_serialization(workspace):
+            return None
+
+        if self.serialized_asset_backfill_data is not None:
+            try:
+                asset_backfill_data = AssetBackfillData.from_serialized(
+                    self.serialized_asset_backfill_data,
+                    ExternalAssetGraph.from_workspace(workspace),
+                )
+            except DagsterDefinitionChangedDeserializationError:
+                return None
+
+            return asset_backfill_data.get_target_root_partitions_subset()
+        else:
+            return None
+
     def get_num_partitions(self, workspace: IWorkspace) -> Optional[int]:
         if not self.is_valid_serialization(workspace):
             return 0
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
```

### Comparing `dagster-1.2.6/dagster/_core/execution/build_resources.py` & `dagster-1.2.7/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/compute_logs.py` & `dagster-1.2.7/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/compute.py` & `dagster-1.2.7/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/hook.py` & `dagster-1.2.7/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/init.py` & `dagster-1.2.7/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/input.py` & `dagster-1.2.7/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/invocation.py` & `dagster-1.2.7/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/logger.py` & `dagster-1.2.7/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/output.py` & `dagster-1.2.7/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/context/system.py` & `dagster-1.2.7/dagster/_core/execution/context/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,23 +143,27 @@
 
     @property
     def log(self) -> DagsterLogManager:
         raise NotImplementedError()
 
     @property
     def logging_tags(self) -> Mapping[str, str]:
-        return self.log.logging_metadata.to_tags()
+        return self.log.logging_metadata.all_tags()
+
+    @property
+    def event_tags(self) -> Mapping[str, str]:
+        return self.log.logging_metadata.event_tags()
 
     def has_tag(self, key: str) -> bool:
         check.str_param(key, "key")
-        return key in self.log.logging_metadata.pipeline_tags
+        return key in self.dagster_run.tags
 
     def get_tag(self, key: str) -> Optional[str]:
         check.str_param(key, "key")
-        return self.log.logging_metadata.pipeline_tags.get(key)
+        return self.dagster_run.tags.get(key)
 
 
 class PlanData(NamedTuple):
     """The data about a run that is available during both orchestration and execution.
 
     This object does not contain any information that requires access to user code, such as the
     pipeline definition and resources.
```

### Comparing `dagster-1.2.6/dagster/_core/execution/context_creation_pipeline.py` & `dagster-1.2.7/dagster/_core/execution/context_creation_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/execute_in_process.py` & `dagster-1.2.7/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.2.7/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/execute_job_result.py` & `dagster-1.2.7/dagster/_core/execution/execute_job_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/execution_result.py` & `dagster-1.2.7/dagster/_core/execution/execution_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,26 @@
         Returns:
             List[DagsterEvent]: A list of all dagster events associated with provided node name.
         """
         check.str_param(node_name, "node_name")
 
         return self._filter_events_by_handle(NodeHandle.from_string(node_name))
 
+    def is_node_success(self, node_str: str) -> bool:
+        return any(evt.is_step_success for evt in self.events_for_node(node_str))
+
+    def is_node_failed(self, node_str: str) -> bool:
+        return any(evt.is_step_failure for evt in self.events_for_node(node_str))
+
+    def is_node_skipped(self, node_str: str) -> bool:
+        return any(evt.is_step_skipped for evt in self.events_for_node(node_str))
+
+    def is_node_untouched(self, node_str: str) -> bool:
+        return len(self.events_for_node(node_str)) == 0
+
     def get_job_failure_event(self) -> DagsterEvent:
         """Returns a DagsterEvent with type DagsterEventType.PIPELINE_FAILURE if it ocurred during
         execution.
         """
         events = self.filter_events(
             lambda event: event.event_type == DagsterEventType.PIPELINE_FAILURE
         )
@@ -166,14 +178,17 @@
 
     def get_step_success_events(self) -> Sequence[DagsterEvent]:
         return [event for event in self.all_events if event.is_step_success]
 
     def get_step_skipped_events(self) -> Sequence[DagsterEvent]:
         return [event for event in self.all_events if event.is_step_skipped]
 
+    def get_step_failure_events(self) -> Sequence[DagsterEvent]:
+        return [event for event in self.all_events if event.is_step_failure]
+
     def get_failed_step_keys(self) -> AbstractSet[str]:
         failure_events = self.filter_events(
             lambda event: event.is_step_failure or event.is_resource_init_failure
         )
         keys: Set[str] = set()
         for event in failure_events:
             if event.step_key:
```

### Comparing `dagster-1.2.6/dagster/_core/execution/host_mode.py` & `dagster-1.2.7/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/job_backfill.py` & `dagster-1.2.7/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/memoization.py` & `dagster-1.2.7/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/active.py` & `dagster-1.2.7/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/compute.py` & `dagster-1.2.7/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.2.7/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.2.7/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/execute_step.py` & `dagster-1.2.7/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/external_step.py` & `dagster-1.2.7/dagster/_core/execution/plan/external_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         if os.path.exists(step_run_dir):
             shutil.rmtree(step_run_dir)
         os.makedirs(step_run_dir)
 
         step_run_ref_file_path = os.path.join(step_run_dir, PICKLED_STEP_RUN_REF_FILE_NAME)
         with open(step_run_ref_file_path, "wb") as step_pickle_file:
             pickle.dump(step_run_ref, step_pickle_file)
-
         command_tokens = [
             sys.executable,
             "-m",
             "dagster._core.execution.plan.local_external_step_main",
             step_run_ref_file_path,
         ]
         # If this is being called within a `capture_interrupts` context, allow interrupts
```

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/handle.py` & `dagster-1.2.7/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/inputs.py` & `dagster-1.2.7/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.2.7/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/objects.py` & `dagster-1.2.7/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/outputs.py` & `dagster-1.2.7/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/plan.py` & `dagster-1.2.7/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/state.py` & `dagster-1.2.7/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/step.py` & `dagster-1.2.7/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/plan/utils.py` & `dagster-1.2.7/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.2.7/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/resolve_versions.py` & `dagster-1.2.7/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/resources_init.py` & `dagster-1.2.7/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/results.py` & `dagster-1.2.7/dagster/_core/execution/results.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/retries.py` & `dagster-1.2.7/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.2.7/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/stats.py` & `dagster-1.2.7/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/tags.py` & `dagster-1.2.7/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/validate_run_config.py` & `dagster-1.2.7/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/watch_orphans.py` & `dagster-1.2.7/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/execution/with_resources.py` & `dagster-1.2.7/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/base.py` & `dagster-1.2.7/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/child_process_executor.py` & `dagster-1.2.7/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/in_process.py` & `dagster-1.2.7/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/init.py` & `dagster-1.2.7/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/multiprocess.py` & `dagster-1.2.7/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.2.7/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/__init__.py` & `dagster-1.2.7/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/code_location.py` & `dagster-1.2.7/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/external.py` & `dagster-1.2.7/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/external_data.py` & `dagster-1.2.7/dagster/_core/host_representation/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     PresetDefinition,
     RepositoryDefinition,
     ScheduleDefinition,
     SourceAsset,
 )
 from dagster._core.definitions.asset_layer import AssetOutputInfo
 from dagster._core.definitions.asset_sensor_definition import AssetSensorDefinition
-from dagster._core.definitions.assets_job import ASSET_BASE_JOB_PREFIX, is_base_asset_job_name
+from dagster._core.definitions.assets_job import is_base_asset_job_name
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.definition_config_schema import ConfiguredDefinitionConfigSchema
 from dagster._core.definitions.dependency import (
     GraphNode,
     Node,
     NodeHandle,
     NodeOutputHandle,
     OpNode,
@@ -1055,14 +1056,15 @@
             ("is_source", bool),
             ("is_observable", bool),
             # If a set of assets can't be materialized independently from each other, they will all
             # have the same atomic_execution_unit_id. This ID should be stable across reloads and
             # unique deployment-wide.
             ("atomic_execution_unit_id", Optional[str]),
             ("required_top_level_resources", Optional[Sequence[str]]),
+            ("auto_materialize_policy", Optional[AutoMaterializePolicy]),
         ],
     )
 ):
     """A definition of a node in the logical asset graph.
 
     A function for computing the asset and an identifier for that asset.
     """
@@ -1086,14 +1088,15 @@
         metadata: Optional[Mapping[str, MetadataValue]] = None,
         group_name: Optional[str] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
         is_source: Optional[bool] = None,
         is_observable: bool = False,
         atomic_execution_unit_id: Optional[str] = None,
         required_top_level_resources: Optional[Sequence[str]] = None,
+        auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     ):
         # backcompat logic to handle ExternalAssetNodes serialized without op_names/graph_name
         if not op_names:
             op_names = list(filter(None, [op_name]))
 
         # backcompat logic to handle ExternalAssetNodes serialzied without is_source
         if is_source is None:
@@ -1136,14 +1139,19 @@
             is_observable=check.bool_param(is_observable, "is_observable"),
             atomic_execution_unit_id=check.opt_str_param(
                 atomic_execution_unit_id, "atomic_execution_unit_id"
             ),
             required_top_level_resources=check.opt_sequence_param(
                 required_top_level_resources, "required_top_level_resources", of_type=str
             ),
+            auto_materialize_policy=check.opt_inst_param(
+                auto_materialize_policy,
+                "auto_materialize_policy",
+                AutoMaterializePolicy,
+            ),
         )
 
 
 ResourceJobUsageMap = Dict[str, List[ResourceJobUsageEntry]]
 
 
 class NodeHandleResourceUse(NamedTuple):
@@ -1289,14 +1297,15 @@
 ) -> Sequence[ExternalAssetNode]:
     node_defs_by_asset_key: Dict[
         AssetKey, List[Tuple[NodeOutputHandle, PipelineDefinition]]
     ] = defaultdict(list)
     asset_info_by_asset_key: Dict[AssetKey, AssetOutputInfo] = dict()
     freshness_policy_by_asset_key: Dict[AssetKey, FreshnessPolicy] = dict()
     metadata_by_asset_key: Dict[AssetKey, MetadataUserInput] = dict()
+    auto_materialize_policy_by_asset_key: Dict[AssetKey, AutoMaterializePolicy] = dict()
 
     deps: Dict[AssetKey, Dict[AssetKey, ExternalAssetDependency]] = defaultdict(dict)
     dep_by: Dict[AssetKey, Dict[AssetKey, ExternalAssetDependedBy]] = defaultdict(dict)
     all_upstream_asset_keys: Set[AssetKey] = set()
     op_names_by_asset_key: Dict[AssetKey, Sequence[str]] = {}
     code_version_by_asset_key: Dict[AssetKey, Optional[str]] = dict()
     group_name_by_asset_key: Dict[AssetKey, str] = {}
@@ -1338,14 +1347,15 @@
                 dep_by[upstream_key][output_key] = ExternalAssetDependedBy(
                     downstream_asset_key=output_key
                 )
 
         for assets_def in asset_layer.assets_defs_by_key.values():
             metadata_by_asset_key.update(assets_def.metadata_by_key)
             freshness_policy_by_asset_key.update(assets_def.freshness_policies_by_key)
+            auto_materialize_policy_by_asset_key.update(assets_def.auto_materialize_policies_by_key)
             descriptions_by_asset_key.update(assets_def.descriptions_by_key)
             if len(assets_def.keys) > 1 and not assets_def.can_subset:
                 atomic_execution_unit_id = assets_def.unique_id
 
                 for asset_key in assets_def.keys:
                     atomic_execution_unit_ids_by_asset_key[asset_key] = atomic_execution_unit_id
 
@@ -1365,20 +1375,29 @@
             code_version=code_version_by_asset_key.get(asset_key),
         )
         for asset_key in asset_keys_without_definitions
     ]
 
     for source_asset in source_assets_by_key.values():
         if source_asset.key not in node_defs_by_asset_key:
+            job_names = (
+                [
+                    job_def.name
+                    for job_def in pipelines
+                    if source_asset.key in job_def.asset_layer.source_assets_by_key
+                ]
+                if source_asset.node_def is not None
+                else []
+            )
             asset_nodes.append(
                 ExternalAssetNode(
                     asset_key=source_asset.key,
                     dependencies=list(deps[source_asset.key].values()),
                     depended_by=list(dep_by[source_asset.key].values()),
-                    job_names=[ASSET_BASE_JOB_PREFIX] if source_asset.node_def is not None else [],
+                    job_names=job_names,
                     op_description=source_asset.description,
                     metadata=source_asset.metadata,
                     group_name=source_asset.group_name,
                     is_source=True,
                     is_observable=source_asset.is_observable,
                     partitions_def_data=external_partitions_definition_from_def(
                         source_asset.partitions_def
@@ -1444,14 +1463,15 @@
                 output_name=output_def.name,
                 metadata=asset_metadata,
                 # assets defined by Out(asset_key="k") do not have any group
                 # name specified we default to DEFAULT_GROUP_NAME here to ensure
                 # such assets are part of the default group
                 group_name=group_name_by_asset_key.get(asset_key, DEFAULT_GROUP_NAME),
                 freshness_policy=freshness_policy_by_asset_key.get(asset_key),
+                auto_materialize_policy=auto_materialize_policy_by_asset_key.get(asset_key),
                 atomic_execution_unit_id=atomic_execution_unit_ids_by_asset_key.get(asset_key),
                 required_top_level_resources=required_top_level_resources,
             )
         )
 
     return asset_nodes
```

### Comparing `dagster-1.2.6/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.2.7/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.2.7/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/handle.py` & `dagster-1.2.7/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/historical.py` & `dagster-1.2.7/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/origin.py` & `dagster-1.2.7/dagster/_core/host_representation/origin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import (
     TYPE_CHECKING,
     Any,
-    Generator,
+    Iterator,
     Mapping,
     NamedTuple,
     NoReturn,
     Optional,
     Sequence,
     cast,
 )
@@ -237,15 +237,15 @@
             " in order to create a handle."
         )
 
     @contextmanager
     def create_single_location(
         self,
         instance: "DagsterInstance",
-    ) -> Generator["CodeLocation", None, None]:
+    ) -> Iterator["GrpcServerCodeLocation"]:
         from dagster._core.workspace.context import DAGIT_GRPC_SERVER_HEARTBEAT_TTL
 
         from .code_location import GrpcServerCodeLocation
         from .grpc_server_registry import GrpcServerRegistry
 
         with GrpcServerRegistry(
             instance=instance,
```

### Comparing `dagster-1.2.6/dagster/_core/host_representation/pipeline_index.py` & `dagster-1.2.7/dagster/_core/host_representation/pipeline_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/host_representation/represented.py` & `dagster-1.2.7/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/instance/__init__.py` & `dagster-1.2.7/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 import os
 import sys
 import time
-import warnings
 import weakref
 from collections import defaultdict
 from enum import Enum
 from tempfile import TemporaryDirectory
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
@@ -114,14 +113,15 @@
     )
     from dagster._core.host_representation.external import ExternalSchedule
     from dagster._core.launcher import RunLauncher
     from dagster._core.run_coordinator import RunCoordinator
     from dagster._core.scheduler import Scheduler, SchedulerDebugInfo
     from dagster._core.scheduler.instigation import (
         InstigatorState,
+        InstigatorStatus,
         InstigatorTick,
         TickData,
         TickStatus,
     )
     from dagster._core.secrets import SecretsLoader
     from dagster._core.snap import ExecutionPlanSnapshot, PipelineSnapshot
     from dagster._core.storage.compute_log_manager import ComputeLogManager
@@ -405,19 +405,14 @@
             self._secrets_loader.register_instance(self)
 
         self._ref = check.opt_inst_param(ref, "ref", InstanceRef)
 
         self._subscribers: Dict[str, List[Callable]] = defaultdict(list)
 
         run_monitoring_enabled = self.run_monitoring_settings.get("enabled", False)
-        if run_monitoring_enabled and not self.run_launcher.supports_check_run_worker_health:
-            run_monitoring_enabled = False
-            warnings.warn(
-                "The configured run launcher does not support run monitoring, disabling it.",
-            )
         self._run_monitoring_enabled = run_monitoring_enabled
         if self.run_monitoring_enabled and self.run_monitoring_max_resume_run_attempts:
             check.invariant(
                 self.run_launcher.supports_resume_run,
                 (
                     "The configured run launcher does not support resuming runs. Set"
                     " max_resume_run_attempts to 0 to use run monitoring. Any runs with a failed"
@@ -991,20 +986,20 @@
                     ),
                 )
             else:
                 # for cases when `create_run_for_pipeline` is directly called
                 pipeline_def = pipeline_def.get_pipeline_subset_def(
                     nodes_to_execute=solids_to_execute
                 )
-        if asset_selection and isinstance(pipeline_def, JobDefinition):
+        if isinstance(pipeline_def, JobDefinition) and (asset_selection or solid_selection):
             # for cases when `create_run_for_pipeline` is directly called
             pipeline_def = pipeline_def.get_job_def_for_subset_selection(
-                asset_selection=asset_selection
+                asset_selection=asset_selection,
+                op_selection=solid_selection,
             )
-
         step_keys_to_execute = None
 
         if execution_plan:
             step_keys_to_execute = execution_plan.step_keys_to_execute
 
         else:
             execution_plan = create_execution_plan(
@@ -1343,15 +1338,15 @@
                 solids_to_execute is None,
                 "Cannot pass both asset_selection and solids_to_execute",
             )
 
         # The "python origin" arguments exist so a job can be reconstructed in memory
         # after a DagsterRun has been fetched from the database.
         #
-        # There are cases (notably in _logged_execute_pipeline with Reconstructable pipelines)
+        # There are cases (notably in _logged_execute_job with Reconstructable jobs)
         # where pipeline_code_origin and is not. In some cloud test cases only
         # external_pipeline_origin is passed But they are almost always passed together.
         # If these are not set the created run will never be able to be relaunched from
         # the information just in the run or in another process.
 
         check.opt_inst_param(
             external_pipeline_origin, "external_pipeline_origin", ExternalPipelineOrigin
@@ -2122,15 +2117,14 @@
                 f"Could not load run {run_id} that was passed to launch_run"
             )
 
         launch_started_event = DagsterEvent(
             event_type_value=DagsterEventType.PIPELINE_STARTING.value,
             pipeline_name=run.pipeline_name,
         )
-
         self.report_dagster_event(launch_started_event, run_id=run.run_id)
 
         run = self.get_run_by_id(run_id)
         if run is None:
             check.failed(f"Failed to reload run {run_id}")
 
         try:
@@ -2314,19 +2308,20 @@
 
     @traced
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional[InstigatorType] = None,
+        instigator_statuses: Optional[Set[InstigatorStatus]] = None,
     ):
         if not self._schedule_storage:
             check.failed("Schedule storage not available")
         return self._schedule_storage.all_instigator_state(
-            repository_origin_id, repository_selector_id, instigator_type
+            repository_origin_id, repository_selector_id, instigator_type, instigator_statuses
         )
 
     @traced
     def get_instigator_state(self, origin_id: str, selector_id: str) -> Optional["InstigatorState"]:
         if not self._schedule_storage:
             check.failed("Schedule storage not available")
         return self._schedule_storage.get_instigator_state(origin_id, selector_id)
```

### Comparing `dagster-1.2.6/dagster/_core/instance/config.py` & `dagster-1.2.7/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/instance/ref.py` & `dagster-1.2.7/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/instance_for_test.py` & `dagster-1.2.7/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/launcher/base.py` & `dagster-1.2.7/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.2.7/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.2.7/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/log_manager.py` & `dagster-1.2.7/dagster/_core/log_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,18 +144,22 @@
 
     @property
     def log_source(self) -> str:
         if self.resource_name is None:
             return self.pipeline_name or "system"
         return f"resource:{self.resource_name}"
 
-    def to_tags(self) -> Mapping[str, str]:
+    def all_tags(self) -> Mapping[str, str]:
         # converts all values into strings
         return {k: str(v) for k, v in self._asdict().items()}
 
+    def event_tags(self) -> Mapping[str, str]:
+        # Exclude pipeline_tags since it can be quite large and can be found on the run
+        return {k: str(v) for k, v in self._asdict().items() if k != "pipeline_tags"}
+
 
 def construct_log_string(
     logging_metadata: DagsterLoggingMetadata, message_props: DagsterMessageProps
 ) -> str:
     from dagster._core.events import EVENT_TYPE_VALUE_TO_DISPLAY_STRING
 
     event_type_str = (
```

### Comparing `dagster-1.2.6/dagster/_core/nux.py` & `dagster-1.2.7/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/origin.py` & `dagster-1.2.7/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/run_coordinator/base.py` & `dagster-1.2.7/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.2.7/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.2.7/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/scheduler/__init__.py` & `dagster-1.2.7/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/scheduler/execution.py` & `dagster-1.2.7/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/scheduler/instigation.py` & `dagster-1.2.7/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/scheduler/scheduler.py` & `dagster-1.2.7/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/secrets/env_file.py` & `dagster-1.2.7/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/selector/subset_selector.py` & `dagster-1.2.7/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/__init__.py` & `dagster-1.2.7/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/config_types.py` & `dagster-1.2.7/dagster/_core/snap/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/dagster_types.py` & `dagster-1.2.7/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/dep_snapshot.py` & `dagster-1.2.7/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.2.7/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/mode.py` & `dagster-1.2.7/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/node.py` & `dagster-1.2.7/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/snap/pipeline_snapshot.py` & `dagster-1.2.7/dagster/_core/snap/pipeline_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/DEVELOPING.md` & `dagster-1.2.7/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/README.md` & `dagster-1.2.7/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/env.py` & `dagster-1.2.7/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.2.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/asset_value_loader.py` & `dagster-1.2.7/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/base_storage.py` & `dagster-1.2.7/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/captured_log_manager.py` & `dagster-1.2.7/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.2.7/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/compute_log_manager.py` & `dagster-1.2.7/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/config.py` & `dagster-1.2.7/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/db_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/__init__.py` & `dagster-1.2.7/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/base.py` & `dagster-1.2.7/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.2.7/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/migration.py` & `dagster-1.2.7/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.2.7/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/schema.py` & `dagster-1.2.7/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.2.7/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/file_manager.py` & `dagster-1.2.7/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/fs_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/input_manager.py` & `dagster-1.2.7/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/io_manager.py` & `dagster-1.2.7/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/legacy_storage.py` & `dagster-1.2.7/dagster/_core/storage/legacy_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     from dagster._core.events.log import EventLogEntry
     from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
     from dagster._core.execution.stats import RunStepKeyStatsSnapshot
     from dagster._core.host_representation.origin import ExternalPipelineOrigin
     from dagster._core.instance import DagsterInstance
     from dagster._core.scheduler.instigation import (
         InstigatorState,
+        InstigatorStatus,
         InstigatorTick,
         TickData,
         TickStatus,
     )
     from dagster._core.snap.execution_plan_snapshot import ExecutionPlanSnapshot
     from dagster._core.snap.pipeline_snapshot import PipelineSnapshot
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
@@ -576,16 +577,19 @@
         return self._storage.schedule_storage.wipe()
 
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional["InstigatorType"] = None,
+        instigator_statuses: Optional[Set["InstigatorStatus"]] = None,
     ) -> Iterable["InstigatorState"]:
-        return self._storage.schedule_storage.all_instigator_state()
+        return self._storage.schedule_storage.all_instigator_state(
+            repository_origin_id, repository_selector_id, instigator_type, instigator_statuses
+        )
 
     def get_instigator_state(self, origin_id: str, selector_id: str) -> Optional["InstigatorState"]:
         return self._storage.schedule_storage.get_instigator_state(origin_id, selector_id)
 
     def add_instigator_state(self, state: "InstigatorState") -> "InstigatorState":
         return self._storage.schedule_storage.add_instigator_state(state)
```

### Comparing `dagster-1.2.6/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.2.7/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/mem_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/migration/utils.py` & `dagster-1.2.7/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.2.7/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/output_manager.py` & `dagster-1.2.7/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/partition_status_cache.py` & `dagster-1.2.7/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/pipeline_run.py` & `dagster-1.2.7/dagster/_core/storage/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/root.py` & `dagster-1.2.7/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/root_input_manager.py` & `dagster-1.2.7/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/base.py` & `dagster-1.2.7/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/in_memory.py` & `dagster-1.2.7/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/migration.py` & `dagster-1.2.7/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/schema.py` & `dagster-1.2.7/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.2.7/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.2.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/base.py` & `dagster-1.2.7/dagster/_core/storage/schedules/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
-from typing import Mapping, Optional, Sequence
+from typing import Mapping, Optional, Sequence, Set
 
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.scheduler.instigation import (
     InstigatorState,
+    InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.sql import AlembicVersion
 from dagster._utils import PrintFn
 
@@ -22,21 +23,23 @@
 
     @abc.abstractmethod
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional[InstigatorType] = None,
+        instigator_statuses: Optional[Set[InstigatorStatus]] = None,
     ) -> Sequence[InstigatorState]:
         """Return all InstigationStates present in storage.
 
         Args:
             repository_origin_id (Optional[str]): The ExternalRepository target id to scope results to
             repository_selector_id (Optional[str]): The repository selector id to scope results to
             instigator_type (Optional[InstigatorType]): The InstigatorType to scope results to
+            instigator_statuses (Optional[Set[InstigatorStatus]]): The InstigatorStatuses to scope results to
         """
 
     @abc.abstractmethod
     def get_instigator_state(self, origin_id: str, selector_id: str) -> Optional[InstigatorState]:
         """Return the instigator state for the given id.
 
         Args:
```

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/migration.py` & `dagster-1.2.7/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/schema.py` & `dagster-1.2.7/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.2.7/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,30 @@
     Any,
     Callable,
     ContextManager,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
+    Set,
     Type,
     TypeVar,
 )
 
 import pendulum
 import sqlalchemy as db
 import sqlalchemy.exc as db_exc
 from sqlalchemy.engine import Connection
 
 import dagster._check as check
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.scheduler.instigation import (
     InstigatorState,
+    InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.sql import SqlAlchemyQuery, SqlAlchemyRow
 from dagster._serdes import serialize_value
 from dagster._serdes.serdes import deserialize_value
@@ -65,31 +67,41 @@
         return list(map(lambda r: deserialize_value(r[0], as_type), rows))
 
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional[InstigatorType] = None,
+        instigator_statuses: Optional[Set[InstigatorStatus]] = None,
     ) -> Sequence[InstigatorState]:
         check.opt_inst_param(instigator_type, "instigator_type", InstigatorType)
 
         if self.has_instigators_table() and self.has_built_index(SCHEDULE_JOBS_SELECTOR_ID):
             query = db.select([InstigatorsTable.c.instigator_body]).select_from(InstigatorsTable)
             if repository_selector_id:
                 query = query.where(
                     InstigatorsTable.c.repository_selector_id == repository_selector_id
                 )
             if instigator_type:
                 query = query.where(InstigatorsTable.c.instigator_type == instigator_type.value)
+            if instigator_statuses:
+                query = query.where(
+                    InstigatorsTable.c.status.in_([status.value for status in instigator_statuses])
+                )
+
         else:
             query = db.select([JobTable.c.job_body]).select_from(JobTable)
             if repository_origin_id:
                 query = query.where(JobTable.c.repository_origin_id == repository_origin_id)
             if instigator_type:
                 query = query.where(JobTable.c.job_type == instigator_type.value)
+            if instigator_statuses:
+                query = query.where(
+                    JobTable.c.status.in_([status.value for status in instigator_statuses])
+                )
 
         rows = self.execute(query)
         return self._deserialize_rows(rows, InstigatorState)
 
     def get_instigator_state(self, origin_id: str, selector_id: str) -> Optional[InstigatorState]:
         check.str_param(origin_id, "origin_id")
         check.str_param(selector_id, "selector_id")
```

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.2.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/sql.py` & `dagster-1.2.7/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/sqlite.py` & `dagster-1.2.7/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/sqlite_storage.py` & `dagster-1.2.7/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/tags.py` & `dagster-1.2.7/dagster/_core/storage/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,22 @@
 
 DOCKER_IMAGE_TAG = f"{SYSTEM_TAG_PREFIX}image"
 
 MAX_RETRIES_TAG = f"{SYSTEM_TAG_PREFIX}max_retries"
 RETRY_NUMBER_TAG = f"{SYSTEM_TAG_PREFIX}retry_number"
 RETRY_STRATEGY_TAG = f"{SYSTEM_TAG_PREFIX}retry_strategy"
 
-USER_EDITABLE_SYSTEM_TAGS = [PRIORITY_TAG, MAX_RETRIES_TAG, RETRY_STRATEGY_TAG]
+MAX_RUNTIME_SECONDS_TAG = f"{SYSTEM_TAG_PREFIX}max_runtime"
+
+USER_EDITABLE_SYSTEM_TAGS = [
+    PRIORITY_TAG,
+    MAX_RETRIES_TAG,
+    RETRY_STRATEGY_TAG,
+    MAX_RUNTIME_SECONDS_TAG,
+]
 
 
 class TagType(Enum):
     # Custom tag provided by a user
     USER_PROVIDED = "USER_PROVIDED"
 
     # Tags used by Dagster to manage execution that should be surfaced to users.
```

### Comparing `dagster-1.2.6/dagster/_core/storage/temp_file_manager.py` & `dagster-1.2.7/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/storage/upath_io_manager.py` & `dagster-1.2.7/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/system_config/composite_descent.py` & `dagster-1.2.7/dagster/_core/system_config/composite_descent.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,40 +330,37 @@
     )
 
 
 def raise_top_level_config_error(
     pipeline_def: PipelineDefinition, failed_config_value: object, evr: EvaluateValueResult
 ) -> NoReturn:
     message = (
-        f"In pipeline '{pipeline_def.name}', top level graph '{pipeline_def.graph.name}' has a "
+        f"In job '{pipeline_def.name}', top level graph '{pipeline_def.graph.name}' has a "
         "configuration error."
     )
 
     raise DagsterInvalidConfigError(message, evr.errors, failed_config_value)
 
 
 def raise_composite_descent_config_error(
     descent_stack: DescentStack, failed_config_value: object, evr: EvaluateValueResult
 ) -> NoReturn:
     check.inst_param(descent_stack, "descent_stack", DescentStack)
     check.inst_param(evr, "evr", EvaluateValueResult)
 
     solid = descent_stack.current_node
-    message = "In pipeline {pipeline_name} at stack {stack}: \n".format(
-        pipeline_name=descent_stack.pipeline_def.name,
+    message = "In job {job_name} at stack {stack}: \n".format(
+        job_name=descent_stack.pipeline_def.name,
         stack=":".join(descent_stack.handle.path),
     )
     message += (
-        'Solid "{solid_name}" with definition "{solid_def_name}" has a '
+        f'Op "{solid.name}" with definition "{solid.definition.name}" has a '
         "configuration error. "
         "It has produced config a via its config_fn that fails to "
         "pass validation in the solids that it contains. "
         "This indicates an error in the config mapping function itself. It must "
         "produce correct config for its constiuent solids in all cases. The correct "
         "resolution is to fix the mapping function. Details on the error (and the paths "
         'on this error are relative to config mapping function "root", not the entire document): '
-    ).format(
-        solid_name=solid.name,
-        solid_def_name=solid.definition.name,
     )
 
     raise DagsterInvalidConfigError(message, evr.errors, failed_config_value)
```

### Comparing `dagster-1.2.6/dagster/_core/system_config/objects.py` & `dagster-1.2.7/dagster/_core/system_config/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
 
         check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
         run_config = check.opt_mapping_param(run_config, "run_config")
         check.opt_str_param(mode, "mode")
 
         mode = mode or pipeline_def.get_default_mode_name()
         run_config_schema = pipeline_def.get_run_config_schema(mode)
-
         if run_config_schema.config_mapping:
             # add user code boundary
             run_config = run_config_schema.config_mapping.resolve_from_unvalidated_config(
                 run_config
             )
 
         config_evr = process_config(
```

### Comparing `dagster-1.2.6/dagster/_core/telemetry.py` & `dagster-1.2.7/dagster/_core/telemetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 STEP_SUCCESS_EVENT = "step_success_event"
 STEP_FAILURE_EVENT = "step_failure_event"
 OS_DESC = platform.platform()
 OS_PLATFORM = platform.system()
 
 
 TELEMETRY_WHITELISTED_FUNCTIONS = {
-    "_logged_execute_pipeline",
+    "_logged_execute_job",
     "execute_execute_command",
     "execute_launch_command",
     "_daemon_run_command",
     "execute_materialize_command",
 }
 
 KNOWN_CI_ENV_VAR_KEYS = {
@@ -213,15 +213,15 @@
     )
 ):
     """Schema for telemetry logs.
 
     Currently, log entries are coerced to the same schema to enable storing all entries in one DB
     table with unified schema.
 
-    action - Name of function called i.e. `execute_pipeline_started` (see: fn telemetry_wrapper)
+    action - Name of function called i.e. `execute_job_started` (see: fn telemetry_wrapper)
     client_time - Client time
     elapsed_time - Time elapsed between start of function and end of function call
     event_id - Unique id for the event
     instance_id - Unique id for dagster instance
     python_version - Python version
     metadata - More information i.e. pipeline success (boolean)
     version - Schema version
@@ -449,74 +449,116 @@
         return "<<unable_to_write_instance_id>>"
 
 
 def hash_name(name: str) -> str:
     return hashlib.sha256(name.encode("utf-8")).hexdigest()
 
 
+def get_stats_from_external_repo(external_repo: "ExternalRepository") -> Mapping[str, str]:
+    from dagster._core.host_representation.external_data import (
+        ExternalDynamicPartitionsDefinitionData,
+        ExternalMultiPartitionsDefinitionData,
+    )
+
+    num_pipelines_in_repo = len(external_repo.get_all_external_jobs())
+    num_schedules_in_repo = len(external_repo.get_external_schedules())
+    num_sensors_in_repo = len(external_repo.get_external_sensors())
+    external_asset_nodes = external_repo.get_external_asset_nodes()
+    num_assets_in_repo = len(external_asset_nodes)
+
+    num_partitioned_assets_in_repo = 0
+    num_multi_partitioned_assets_in_repo = 0
+    num_dynamic_partitioned_assets_in_repo = 0
+    num_assets_with_freshness_policies_in_repo = 0
+    num_source_assets_in_repo = 0
+    num_observable_source_assets_in_repo = 0
+    num_dbt_assets_in_repo = 0
+    num_assets_with_code_versions_in_repo = 0
+    for asset in external_asset_nodes:
+        if asset.partitions_def_data:
+            num_partitioned_assets_in_repo += 1
+
+            if isinstance(asset.partitions_def_data, ExternalDynamicPartitionsDefinitionData):
+                num_dynamic_partitioned_assets_in_repo += 1
+
+            if isinstance(asset.partitions_def_data, ExternalMultiPartitionsDefinitionData):
+                num_multi_partitioned_assets_in_repo += 1
+
+        if asset.freshness_policy is not None:
+            num_assets_with_freshness_policies_in_repo += 1
+
+        if asset.is_source:
+            num_source_assets_in_repo += 1
+
+            if asset.is_observable:
+                num_observable_source_assets_in_repo += 1
+
+        if asset.code_version is not None:
+            num_assets_with_code_versions_in_repo += 1
+
+        if asset.compute_kind == "dbt":
+            num_dbt_assets_in_repo += 1
+
+    num_asset_reconciliation_sensors_in_repo = sum(
+        1
+        for external_sensor in external_repo.get_external_sensors()
+        if external_sensor.name == "asset_reconciliation_sensor"
+    )
+
+    return {
+        "num_pipelines_in_repo": str(num_pipelines_in_repo),
+        "num_schedules_in_repo": str(num_schedules_in_repo),
+        "num_sensors_in_repo": str(num_sensors_in_repo),
+        "num_assets_in_repo": str(num_assets_in_repo),
+        "num_source_assets_in_repo": str(num_source_assets_in_repo),
+        "num_partitioned_assets_in_repo": str(num_partitioned_assets_in_repo),
+        "num_dynamic_partitioned_assets_in_repo": str(num_dynamic_partitioned_assets_in_repo),
+        "num_multi_partitioned_assets_in_repo": str(num_multi_partitioned_assets_in_repo),
+        "num_assets_with_freshness_policies_in_repo": str(
+            num_assets_with_freshness_policies_in_repo
+        ),
+        "num_observable_source_assets_in_repo": str(num_observable_source_assets_in_repo),
+        "num_dbt_assets_in_repo": str(num_dbt_assets_in_repo),
+        "num_assets_with_code_versions_in_repo": str(num_assets_with_code_versions_in_repo),
+        "num_asset_reconciliation_sensors_in_repo": str(num_asset_reconciliation_sensors_in_repo),
+    }
+
+
 def log_external_repo_stats(
     instance: DagsterInstance,
     source: str,
     external_repo: "ExternalRepository",
     external_pipeline: Optional["ExternalPipeline"] = None,
 ):
     from dagster._core.host_representation.external import ExternalPipeline, ExternalRepository
-    from dagster._core.host_representation.external_data import (
-        ExternalAssetNode,
-        ExternalDynamicPartitionsDefinitionData,
-    )
 
     check.inst_param(instance, "instance", DagsterInstance)
     check.str_param(source, "source")
     check.inst_param(external_repo, "external_repo", ExternalRepository)
     check.opt_inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
 
-    def _get_num_dynamic_partitioned_assets(
-        external_asset_nodes: Sequence[ExternalAssetNode],
-    ) -> int:
-        return sum(
-            1
-            for asset in external_asset_nodes
-            if asset.partitions_def_data
-            and isinstance(asset.partitions_def_data, ExternalDynamicPartitionsDefinitionData)
-        )
-
     if _get_instance_telemetry_enabled(instance):
         instance_id = get_or_set_instance_id()
 
         pipeline_name_hash = hash_name(external_pipeline.name) if external_pipeline else ""
         repo_hash = hash_name(external_repo.name)
         location_name_hash = hash_name(external_repo.handle.location_name)
-        num_pipelines_in_repo = len(external_repo.get_all_external_jobs())
-        num_schedules_in_repo = len(external_repo.get_external_schedules())
-        num_sensors_in_repo = len(external_repo.get_external_sensors())
-        external_asset_nodes = external_repo.get_external_asset_nodes()
-        num_assets_in_repo = len(external_asset_nodes)
-        num_dynamic_partitioned_assets_in_repo = _get_num_dynamic_partitioned_assets(
-            external_asset_nodes
-        )
 
         write_telemetry_log_line(
             TelemetryEntry(
                 action=UPDATE_REPO_STATS,
                 client_time=str(datetime.datetime.now()),
                 event_id=str(uuid.uuid4()),
                 instance_id=instance_id,
                 metadata={
+                    **get_stats_from_external_repo(external_repo),
                     "source": source,
                     "pipeline_name_hash": pipeline_name_hash,
-                    "num_pipelines_in_repo": str(num_pipelines_in_repo),
-                    "num_schedules_in_repo": str(num_schedules_in_repo),
-                    "num_sensors_in_repo": str(num_sensors_in_repo),
-                    "num_assets_in_repo": str(num_assets_in_repo),
                     "repo_hash": repo_hash,
                     "location_name_hash": location_name_hash,
-                    "num_dynamic_partitioned_assets_in_repo": str(
-                        num_dynamic_partitioned_assets_in_repo
-                    ),
                 },
             )._asdict()
         )
 
 
 def log_repo_stats(
     instance: DagsterInstance,
```

### Comparing `dagster-1.2.6/dagster/_core/telemetry_upload.py` & `dagster-1.2.7/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/test_utils.py` & `dagster-1.2.7/dagster/_core/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,75 @@
 import asyncio
 import os
 import re
 import time
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import contextmanager
-from typing import Any, Generator, Mapping, NamedTuple, Optional, Sequence, TypeVar
+from signal import Signals
+from typing import (
+    TYPE_CHECKING,
+    AbstractSet,
+    Any,
+    Dict,
+    Iterator,
+    Mapping,
+    NamedTuple,
+    NoReturn,
+    Optional,
+    Sequence,
+    TypeVar,
+)
 
 import pendulum
 from typing_extensions import Self
 
 from dagster import (
     Permissive,
     Shape,
     _check as check,
     fs_io_manager,
 )
 from dagster._config import Array, Field
 from dagster._core.definitions.decorators import op
 from dagster._core.definitions.decorators.graph_decorator import graph
+from dagster._core.definitions.graph_definition import GraphDefinition
+from dagster._core.definitions.node_definition import NodeDefinition
 from dagster._core.errors import DagsterUserCodeUnreachableError
+from dagster._core.events import DagsterEvent
 from dagster._core.host_representation.origin import (
     ExternalPipelineOrigin,
     InProcessCodeLocationOrigin,
 )
 from dagster._core.instance import DagsterInstance
 from dagster._core.launcher import RunLauncher
 from dagster._core.run_coordinator import RunCoordinator, SubmitRunContext
 from dagster._core.secrets import SecretsLoader
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus, RunsFilter
-from dagster._core.workspace.context import WorkspaceProcessContext
+from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
+from dagster._core.workspace.context import WorkspaceProcessContext, WorkspaceRequestContext
 from dagster._core.workspace.load_target import WorkspaceLoadTarget
-from dagster._legacy import ModeDefinition, pipeline
+from dagster._legacy import ModeDefinition
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 from dagster._seven.compat.pendulum import create_pendulum_time, mock_pendulum_timezone
 from dagster._utils import Counter, get_terminate_signal, traced, traced_counter
 from dagster._utils.log import configure_loggers
 
 # test utils from separate light weight file since are exported top level
 from .instance_for_test import (
     cleanup_test_instance as cleanup_test_instance,
     environ as environ,
     instance_for_test as instance_for_test,
 )
 
+if TYPE_CHECKING:
+    from pendulum.datetime import DateTime
+
+T = TypeVar("T")
 T_NamedTuple = TypeVar("T_NamedTuple", bound=NamedTuple)
 
 
 def assert_namedtuple_lists_equal(
     t1_list: Sequence[T_NamedTuple],
     t2_list: Sequence[T_NamedTuple],
     exclude_fields: Optional[Sequence[str]] = None,
@@ -62,50 +83,50 @@
 ) -> None:
     exclude_fields = exclude_fields or []
     for field in type(t1)._fields:
         if field not in exclude_fields:
             assert getattr(t1, field) == getattr(t2, field)
 
 
-def step_output_event_filter(pipe_iterator):
+def step_output_event_filter(pipe_iterator: Iterator[DagsterEvent]):
     for step_event in pipe_iterator:
         if step_event.is_successful_output:
             yield step_event
 
 
-def nesting_graph_pipeline(depth, num_children, *args, **kwargs):
+def nesting_graph(depth: int, num_children: int, name: Optional[str] = None) -> GraphDefinition:
     """Creates a pipeline of nested composite solids up to "depth" layers, with a fan-out of
     num_children at each layer.
 
     Total number of solids will be num_children ^ depth
     """
 
     @op
     def leaf_node(_):
         return 1
 
-    def create_wrap(inner, name):
+    def create_wrap(inner: NodeDefinition, name: str) -> GraphDefinition:
         @graph(name=name)
         def wrap():
             for i in range(num_children):
                 solid_alias = "%s_node_%d" % (name, i)
                 inner.alias(solid_alias)()
 
         return wrap
 
-    @pipeline(*args, **kwargs)
-    def nested_pipeline():
-        comp_solid = create_wrap(leaf_node, "layer_%d" % depth)
+    @graph(name=name)
+    def nested_graph():
+        graph_def = create_wrap(leaf_node, "layer_%d" % depth)
 
         for i in range(depth):
-            comp_solid = create_wrap(comp_solid, "layer_%d" % (depth - (i + 1)))
+            graph_def = create_wrap(graph_def, "layer_%d" % (depth - (i + 1)))
 
-        comp_solid.alias("outer")()
+        graph_def.alias("outer")()
 
-    return nested_pipeline
+    return nested_graph
 
 
 TEST_PIPELINE_NAME = "_test_pipeline_"
 
 
 def create_run_for_test(
     instance: DagsterInstance,
@@ -120,14 +141,16 @@
     root_run_id=None,
     parent_run_id=None,
     pipeline_snapshot=None,
     execution_plan_snapshot=None,
     parent_pipeline_snapshot=None,
     external_pipeline_origin=None,
     pipeline_code_origin=None,
+    asset_selection=None,
+    solid_selection=None,
 ):
     return instance.create_run(
         pipeline_name=pipeline_name,
         run_id=run_id,
         run_config=run_config,
         mode=mode,
         solids_to_execute=solids_to_execute,
@@ -137,16 +160,16 @@
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         pipeline_snapshot=pipeline_snapshot,
         execution_plan_snapshot=execution_plan_snapshot,
         parent_pipeline_snapshot=parent_pipeline_snapshot,
         external_pipeline_origin=external_pipeline_origin,
         pipeline_code_origin=pipeline_code_origin,
-        asset_selection=None,
-        solid_selection=None,
+        asset_selection=asset_selection,
+        solid_selection=solid_selection,
     )
 
 
 def register_managed_run_for_test(
     instance,
     pipeline_name=TEST_PIPELINE_NAME,
     run_id=None,
@@ -173,15 +196,17 @@
         parent_run_id,
         pipeline_snapshot,
         execution_plan_snapshot,
         parent_pipeline_snapshot,
     )
 
 
-def wait_for_runs_to_finish(instance, timeout=20, run_tags=None):
+def wait_for_runs_to_finish(
+    instance: DagsterInstance, timeout: float = 20, run_tags: Optional[Mapping[str, str]] = None
+) -> None:
     total_time = 0
     interval = 0.1
 
     filters = RunsFilter(tags=run_tags) if run_tags else None
 
     while True:
         runs = instance.get_runs(filters)
@@ -192,15 +217,20 @@
             raise Exception("Timed out")
 
         time.sleep(interval)
         total_time += interval
         interval = interval * 2
 
 
-def poll_for_finished_run(instance, run_id=None, timeout=20, run_tags=None):
+def poll_for_finished_run(
+    instance: DagsterInstance,
+    run_id: Optional[str] = None,
+    timeout: float = 20,
+    run_tags: Optional[Mapping[str, str]] = None,
+) -> DagsterRun:
     total_time = 0
     interval = 0.01
 
     filters = RunsFilter(
         run_ids=[run_id] if run_id else None,
         tags=run_tags,
         statuses=[
@@ -217,84 +247,90 @@
         else:
             time.sleep(interval)
             total_time += interval
             if total_time > timeout:
                 raise Exception("Timed out")
 
 
-def poll_for_step_start(instance, run_id, timeout=30):
+def poll_for_step_start(instance: DagsterInstance, run_id: str, timeout: float = 30):
     poll_for_event(instance, run_id, event_type="STEP_START", message=None, timeout=timeout)
 
 
-def poll_for_event(instance, run_id, event_type, message, timeout=30):
+def poll_for_event(
+    instance: DagsterInstance,
+    run_id: str,
+    event_type: str,
+    message: Optional[str],
+    timeout: float = 30,
+) -> None:
     total_time = 0
     backoff = 0.01
 
     while True:
         time.sleep(backoff)
         logs = instance.all_logs(run_id)
         matching_events = [
-            log_record.dagster_event
+            log_record.get_dagster_event()
             for log_record in logs
             if log_record.is_dagster_event
-            and log_record.dagster_event.event_type_value == event_type
+            and log_record.get_dagster_event().event_type_value == event_type
         ]
         if matching_events:
             if message is None:
                 return
             for matching_message in (event.message for event in matching_events):
-                if message in matching_message:
+                if matching_message and message in matching_message:
                     return
 
         total_time += backoff
         backoff = backoff * 2
         if total_time > timeout:
             raise Exception("Timed out")
 
 
 @contextmanager
-def new_cwd(path):
+def new_cwd(path: str) -> Iterator[None]:
     old = os.getcwd()
     try:
         os.chdir(path)
         yield
     finally:
         os.chdir(old)
 
 
-def today_at_midnight(timezone_name="UTC"):
+def today_at_midnight(timezone_name="UTC") -> "DateTime":
     check.str_param(timezone_name, "timezone_name")
     now = pendulum.now(timezone_name)
     return create_pendulum_time(now.year, now.month, now.day, tz=now.timezone.name)
 
 
 class ExplodingRunLauncher(RunLauncher, ConfigurableClass):
     def __init__(self, inst_data: Optional[ConfigurableClassData] = None):
         self._inst_data = inst_data
 
         super().__init__()
 
     @property
-    def inst_data(self):
+    def inst_data(self) -> Optional[ConfigurableClassData]:
         return self._inst_data
 
     @classmethod
-    def config_type(cls):
+    def config_type(cls) -> Mapping[str, Any]:
         return {}
 
     @classmethod
     def from_config_value(
         cls, inst_data: ConfigurableClassData, config_value: Mapping[str, Any]
     ) -> Self:
         return ExplodingRunLauncher(inst_data=inst_data)
 
-    def launch_run(self, context):
+    def launch_run(self, context) -> NoReturn:
         raise NotImplementedError("The entire purpose of this is to throw on launch")
 
-    def join(self, timeout=30):
+    def join(self, timeout: float = 30) -> None:
         """Nothing to join on since all executions are synchronous."""
 
     def terminate(self, run_id):
         check.not_implemented("Termination not supported")
 
 
 class MockedRunLauncher(RunLauncher, ConfigurableClass):
@@ -385,72 +421,72 @@
         return self._inst_data
 
     def cancel_run(self, run_id):
         check.not_implemented("Cancellation not supported")
 
 
 class TestSecretsLoader(SecretsLoader, ConfigurableClass):
-    def __init__(
-        self,
-        inst_data,
-        env_vars,
-    ):
+    def __init__(self, inst_data: Optional[ConfigurableClassData], env_vars: Dict[str, str]):
         self._inst_data = inst_data
         self.env_vars = env_vars
 
-    def get_secrets_for_environment(self, location_name):
+    def get_secrets_for_environment(self, location_name: str) -> Dict[str, str]:
         return self.env_vars.copy()
 
     @property
-    def inst_data(self):
+    def inst_data(self) -> Optional[ConfigurableClassData]:
         return self._inst_data
 
     @classmethod
-    def config_type(cls):
+    def config_type(cls) -> Mapping[str, Any]:
         return {"env_vars": Field(Permissive())}
 
     @classmethod
     def from_config_value(
         cls, inst_data: ConfigurableClassData, config_value: Mapping[str, Any]
     ) -> Self:
         return TestSecretsLoader(inst_data=inst_data, **config_value)
 
 
-def get_crash_signals():
+def get_crash_signals() -> Sequence[Signals]:
     return [get_terminate_signal()]
 
 
-_mocked_system_timezone = {"timezone": None}
+_mocked_system_timezone: Dict[str, Optional[str]] = {"timezone": None}
 
 
 @contextmanager
-def mock_system_timezone(override_timezone):
+def mock_system_timezone(override_timezone: str) -> Iterator[None]:
     with mock_pendulum_timezone(override_timezone):
         try:
             _mocked_system_timezone["timezone"] = override_timezone
             yield
         finally:
             _mocked_system_timezone["timezone"] = None
 
 
-def get_mocked_system_timezone():
+def get_mocked_system_timezone() -> Optional[str]:
     return _mocked_system_timezone["timezone"]
 
 
 # Test utility for creating a test workspace for a function
 class InProcessTestWorkspaceLoadTarget(WorkspaceLoadTarget):
     def __init__(self, origin: InProcessCodeLocationOrigin):
         self._origin = origin
 
-    def create_origins(self):
+    def create_origins(self) -> Sequence[InProcessCodeLocationOrigin]:
         return [self._origin]
 
 
 @contextmanager
-def in_process_test_workspace(instance, loadable_target_origin, container_image=None):
+def in_process_test_workspace(
+    instance: DagsterInstance,
+    loadable_target_origin: LoadableTargetOrigin,
+    container_image: Optional[str] = None,
+) -> Iterator[WorkspaceRequestContext]:
     with WorkspaceProcessContext(
         instance,
         InProcessTestWorkspaceLoadTarget(
             InProcessCodeLocationOrigin(
                 loadable_target_origin,
                 container_image=container_image,
             ),
@@ -459,30 +495,30 @@
         yield workspace_process_context.create_request_context()
 
 
 @contextmanager
 def create_test_daemon_workspace_context(
     workspace_load_target: WorkspaceLoadTarget,
     instance: DagsterInstance,
-) -> Generator[WorkspaceProcessContext, None, None]:
+) -> Iterator[WorkspaceProcessContext]:
     """Creates a DynamicWorkspace suitable for passing into a DagsterDaemon loop when running tests.
     """
     from dagster._daemon.controller import create_daemon_grpc_server_registry
 
     configure_loggers()
     with create_daemon_grpc_server_registry(instance) as grpc_server_registry:
         with WorkspaceProcessContext(
             instance,
             workspace_load_target,
             grpc_server_registry=grpc_server_registry,
         ) as workspace_process_context:
             yield workspace_process_context
 
 
-def remove_none_recursively(obj):
+def remove_none_recursively(obj: T) -> T:
     """Remove none values from a dict. This can be used to support comparing provided config vs.
     config we retrive from kubernetes, which returns all fields, even those which have no value
     configured.
     """
     if isinstance(obj, (list, tuple, set)):
         return type(obj)(remove_none_recursively(x) for x in obj if x is not None)
     elif isinstance(obj, dict):
@@ -492,52 +528,53 @@
             if k is not None and v is not None
         )
     else:
         return obj
 
 
 default_mode_def_for_test = ModeDefinition(resource_defs={"io_manager": fs_io_manager})
+default_resources_for_test = {"io_manager": fs_io_manager}
 
 
-def strip_ansi(input_str):
+def strip_ansi(input_str: str) -> str:
     ansi_escape = re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]")
     return ansi_escape.sub("", input_str)
 
 
-def get_logger_output_from_capfd(capfd, logger_name):
+def get_logger_output_from_capfd(capfd: Any, logger_name: str) -> str:
     return "\n".join(
         [
             line
             for line in strip_ansi(capfd.readouterr().out.replace("\r\n", "\n")).split("\n")
             if logger_name in line
         ]
     )
 
 
-def _step_events(instance, run):
+def _step_events(instance: DagsterInstance, run: DagsterRun) -> Mapping[str, AbstractSet[str]]:
     events_by_step = defaultdict(set)
     logs = instance.all_logs(run.run_id)
     for record in logs:
         if not record.is_dagster_event or not record.step_key:
             continue
-        events_by_step[record.step_key] = record.dagster_event.event_type_value
+        events_by_step[record.step_key].add(record.get_dagster_event().event_type_value)
     return events_by_step
 
 
-def step_did_not_run(instance, run, step_name):
+def step_did_not_run(instance: DagsterInstance, run: DagsterRun, step_name: str) -> bool:
     step_events = _step_events(instance, run)[step_name]
     return len(step_events) == 0
 
 
-def step_succeeded(instance, run, step_name):
+def step_succeeded(instance: DagsterInstance, run: DagsterRun, step_name: str) -> bool:
     step_events = _step_events(instance, run)[step_name]
     return "STEP_SUCCESS" in step_events
 
 
-def step_failed(instance, run, step_name):
+def step_failed(instance: DagsterInstance, run: DagsterRun, step_name: str) -> bool:
     step_events = _step_events(instance, run)[step_name]
     return "STEP_FAILURE" in step_events
 
 
 def test_counter():
     @traced
     async def foo():
@@ -563,15 +600,15 @@
     counter = traced_counter.get()
     assert isinstance(counter, Counter)
     counts = counter.counts()
     assert counts["foo"] == 20
     assert counts["bar"] == 10
 
 
-def wait_for_futures(futures, timeout=None):
+def wait_for_futures(futures: Dict[str, Future], timeout: Optional[float] = None):
     start_time = time.time()
     for target_id, future in futures.copy().items():
         if timeout is not None:
             future_timeout = max(0, timeout - (time.time() - start_time))
         else:
             future_timeout = None
```

### Comparing `dagster-1.2.6/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.2.7/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/config_schema.py` & `dagster-1.2.7/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/dagster_type.py` & `dagster-1.2.7/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/decorator.py` & `dagster-1.2.7/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/loadable_target_origin.py` & `dagster-1.2.7/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/primitive_mapping.py` & `dagster-1.2.7/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/python_dict.py` & `dagster-1.2.7/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/python_set.py` & `dagster-1.2.7/dagster/_core/types/python_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dagster._config import Array
 from dagster._core.types.dagster_type import DagsterTypeKind
 
 from .config_schema import DagsterTypeLoader
 from .dagster_type import DagsterType, PythonObjectDagsterType, resolve_dagster_type
 
 PythonSet = PythonObjectDagsterType(
-    set, "PythonSet", description="""Represents a python dictionary to pass between solids"""
+    set, "PythonSet", description="""Represents a python dictionary to pass between ops"""
 )
 
 
 class TypedSetLoader(DagsterTypeLoader):
     def __init__(self, item_dagster_type):
         self._item_dagster_type = check.inst_param(
             item_dagster_type, "item_dagster_type", DagsterType
```

### Comparing `dagster-1.2.6/dagster/_core/types/python_tuple.py` & `dagster-1.2.7/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/types/transform_typing.py` & `dagster-1.2.7/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/utils.py` & `dagster-1.2.7/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/autodiscovery.py` & `dagster-1.2.7/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/config_schema.py` & `dagster-1.2.7/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/context.py` & `dagster-1.2.7/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/load.py` & `dagster-1.2.7/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/load_target.py` & `dagster-1.2.7/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/permissions.py` & `dagster-1.2.7/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_core/workspace/workspace.py` & `dagster-1.2.7/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/__init__.py` & `dagster-1.2.7/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.2.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from typing import Iterator, Optional, Sequence, Tuple, cast
 
 from dagster._core.definitions.metadata import MetadataValue
+from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.events import EngineEventData
 from dagster._core.execution.plan.resume_retry import ReexecutionStrategy
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus, RunRecord
 from dagster._core.storage.tags import MAX_RETRIES_TAG, RETRY_NUMBER_TAG, RETRY_STRATEGY_TAG
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._utils.error import serializable_error_info_from_exc_info
@@ -115,15 +116,25 @@
                 f"Could not find job {failed_run.pipeline_name} in repository {repo_name}, unable"
                 " to retry the run. It was likely renamed or deleted."
             ),
             failed_run,
         )
         return
 
-    external_pipeline = external_repo.get_full_external_job(failed_run.pipeline_name)
+    external_pipeline = code_location.get_external_pipeline(
+        PipelineSelector(
+            location_name=origin.code_location_origin.location_name,
+            repository_name=repo_name,
+            pipeline_name=failed_run.pipeline_name,
+            solid_selection=failed_run.solid_selection,
+            asset_selection=None
+            if failed_run.asset_selection is None
+            else list(failed_run.asset_selection),
+        )
+    )
 
     strategy = get_reexecution_strategy(failed_run, instance) or DEFAULT_REEXECUTION_POLICY
 
     new_run = instance.create_reexecuted_run(
         parent_run=failed_run,
         code_location=code_location,
         external_pipeline=external_pipeline,
```

### Comparing `dagster-1.2.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.2.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/backfill.py` & `dagster-1.2.7/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/cli/__init__.py` & `dagster-1.2.7/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/controller.py` & `dagster-1.2.7/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/daemon.py` & `dagster-1.2.7/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.2.7/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import logging
 import sys
 import time
 from typing import Iterator, Optional
 
+import pendulum
+
 from dagster import (
     DagsterInstance,
     _check as check,
 )
-from dagster._core.events import DagsterEventType
+from dagster._core.events import DagsterEventType, EngineEventData
 from dagster._core.launcher import WorkerStatus
 from dagster._core.storage.pipeline_run import (
     IN_PROGRESS_RUN_STATUSES,
-    DagsterRun,
     DagsterRunStatus,
+    RunRecord,
     RunsFilter,
 )
+from dagster._core.storage.tags import MAX_RUNTIME_SECONDS_TAG
 from dagster._core.workspace.context import IWorkspace, IWorkspaceProcessContext
 from dagster._utils import DebugCrashFlags
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 RESUME_RUN_LOG_MESSAGE = "Launching a new run worker to resume run"
 
 
 def monitor_starting_run(
-    instance: DagsterInstance, run: DagsterRun, logger: logging.Logger
+    instance: DagsterInstance, run_record: RunRecord, logger: logging.Logger
 ) -> None:
+    run = run_record.dagster_run
     check.invariant(run.status == DagsterRunStatus.STARTING)
     run_stats = instance.get_run_stats(run.run_id)
 
     launch_time = check.not_none(
         run_stats.launch_time, "Run in status STARTING doesn't have a launch time."
     )
     if time.time() - launch_time >= instance.run_monitoring_start_timeout_seconds:
@@ -55,97 +59,153 @@
     events = instance.all_logs(run_id, of_type=DagsterEventType.ENGINE_EVENT)
     return len([event for event in events if event.message == RESUME_RUN_LOG_MESSAGE])
 
 
 def monitor_started_run(
     instance: DagsterInstance,
     workspace: IWorkspace,
-    run: DagsterRun,
+    run_record: RunRecord,
     logger: logging.Logger,
 ) -> None:
+    run = run_record.dagster_run
     check.invariant(run.status == DagsterRunStatus.STARTED)
-    check_health_result = instance.run_launcher.check_run_worker_health(run)
-    if check_health_result.status not in [WorkerStatus.RUNNING, WorkerStatus.SUCCESS]:
-        num_prev_attempts = count_resume_run_attempts(instance, run.run_id)
-        recheck_run = check.not_none(instance.get_run_by_id(run.run_id))
-        status_changed = run.status != recheck_run.status
-        if status_changed:
-            msg = (
-                "Detected run status changed during monitoring loop: "
-                f"{run.status} -> {recheck_run.status}, disregarding for now"
-            )
-            logger.info(msg)
-            return
-        if num_prev_attempts < instance.run_monitoring_max_resume_run_attempts:
-            msg = (
-                f"Detected run worker status {check_health_result}. Resuming run {run.run_id} with "
-                "a new worker."
-            )
-            logger.info(msg)
-            instance.report_engine_event(msg, run)
-            attempt_number = num_prev_attempts + 1
-            instance.resume_run(
-                run.run_id,
-                workspace,
-                attempt_number,
-            )
-        else:
-            debug_info = ""
-            try:
-                debug_info = instance.run_launcher.get_run_worker_debug_info(run)
-            except Exception:
-                logger.exception("Failure fetching debug info for failed run worker")
-
-            if instance.run_launcher.supports_resume_run:
+    if instance.run_launcher.supports_check_run_worker_health:
+        check_health_result = instance.run_launcher.check_run_worker_health(run)
+        if check_health_result.status not in [WorkerStatus.RUNNING, WorkerStatus.SUCCESS]:
+            num_prev_attempts = count_resume_run_attempts(instance, run.run_id)
+            recheck_run = check.not_none(instance.get_run_by_id(run.run_id))
+            status_changed = run.status != recheck_run.status
+            if status_changed:
                 msg = (
-                    f"Detected run worker status {check_health_result}. Marking run {run.run_id} as"
-                    " failed, because it has surpassed the configured maximum attempts to resume"
-                    f" the run: {instance.run_monitoring_max_resume_run_attempts}."
-                    + (f"\n{debug_info}" if debug_info else "")
+                    "Detected run status changed during monitoring loop: "
+                    f"{run.status} -> {recheck_run.status}, disregarding for now"
                 )
-            else:
+                logger.info(msg)
+                return
+            if num_prev_attempts < instance.run_monitoring_max_resume_run_attempts:
                 msg = (
-                    f"Detected run worker status {check_health_result}. Marking run {run.run_id} as"
-                    " failed."
-                    + (f"\n{debug_info}" if debug_info else "")
+                    f"Detected run worker status {check_health_result}. Resuming run"
+                    f" {run.run_id} with a new worker."
+                )
+                logger.info(msg)
+                instance.report_engine_event(msg, run)
+                attempt_number = num_prev_attempts + 1
+                instance.resume_run(
+                    run.run_id,
+                    workspace,
+                    attempt_number,
                 )
-            logger.info(msg)
-            instance.report_run_failed(run, msg)
+                # Return rather than immediately checking for a timeout, since we only just resumed
+                return
+            else:
+                if instance.run_launcher.supports_resume_run:
+                    msg = (
+                        f"Detected run worker status {check_health_result}. Marking run"
+                        f" {run.run_id} as failed, because it has surpassed the configured maximum"
+                        " attempts to resume the run:"
+                        f" {instance.run_monitoring_max_resume_run_attempts}."
+                    )
+                else:
+                    msg = (
+                        f"Detected run worker status {check_health_result}. Marking run"
+                        f" {run.run_id} as failed."
+                    )
+                logger.info(msg)
+                instance.report_run_failed(run, msg)
+                # Return rather than immediately checking for a timeout, since we just failed
+                return
+    check_run_timeout(instance, run_record, logger)
 
 
 def execute_monitoring_iteration(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     _debug_crash_flags: Optional[DebugCrashFlags] = None,
 ) -> Iterator[Optional[SerializableErrorInfo]]:
     instance = workspace_process_context.instance
-    check.invariant(
-        instance.run_launcher.supports_check_run_worker_health, "Must use a supported run launcher"
-    )
 
     # TODO: consider limiting number of runs to fetch
-    runs = list(instance.get_runs(filters=RunsFilter(statuses=IN_PROGRESS_RUN_STATUSES)))
+    run_records = list(
+        instance.get_run_records(filters=RunsFilter(statuses=IN_PROGRESS_RUN_STATUSES))
+    )
 
-    if not runs:
+    if not run_records:
         return
 
-    logger.info(f"Collected {len(runs)} runs for monitoring")
+    logger.info(f"Collected {len(run_records)} runs for monitoring")
     workspace = workspace_process_context.create_request_context()
-    for run in runs:
+    for run_record in run_records:
         try:
-            logger.info(f"Checking run {run.run_id}")
+            logger.info(f"Checking run {run_record.dagster_run.run_id}")
 
-            if run.status == DagsterRunStatus.STARTING:
-                monitor_starting_run(instance, run, logger)
-            elif run.status == DagsterRunStatus.STARTED:
-                monitor_started_run(instance, workspace, run, logger)
-            elif run.status == DagsterRunStatus.CANCELING:
+            if run_record.dagster_run.status == DagsterRunStatus.STARTING:
+                monitor_starting_run(instance, run_record, logger)
+            elif run_record.dagster_run.status == DagsterRunStatus.STARTED:
+                monitor_started_run(instance, workspace, run_record, logger)
+            elif run_record.dagster_run.status == DagsterRunStatus.CANCELING:
                 # TODO: implement canceling timeouts
                 pass
             else:
-                check.invariant(False, f"Unexpected run status: {run.status}")
+                check.invariant(False, f"Unexpected run status: {run_record.dagster_run.status}")
         except Exception:
             error_info = serializable_error_info_from_exc_info(sys.exc_info())
-            logger.error(f"Hit error while monitoring run {run.run_id}: {str(error_info)}")
+            logger.error(
+                f"Hit error while monitoring run {run_record.dagster_run.run_id}: {str(error_info)}"
+            )
             yield error_info
         else:
             yield
+
+
+def check_run_timeout(
+    instance: DagsterInstance, run_record: RunRecord, logger: logging.Logger
+) -> None:
+    max_time_str = run_record.dagster_run.tags.get(
+        MAX_RUNTIME_SECONDS_TAG,
+    )
+    if not max_time_str:
+        return
+
+    max_time = float(max_time_str)
+
+    if (
+        run_record.start_time is not None
+        and pendulum.now("UTC").timestamp() - run_record.start_time > max_time
+    ):
+        logger.info(
+            f"Run {run_record.dagster_run.run_id} has exceeded maximum runtime of"
+            f" {max_time} seconds: terminating run."
+        )
+
+        instance.report_run_canceling(
+            run_record.dagster_run,
+            message=f"Canceling due to exceeding maximum runtime of {int(max_time)} seconds.",
+        )
+        try:
+            if instance.run_launcher.terminate(run_id=run_record.dagster_run.run_id):
+                instance.report_run_failed(
+                    run_record.dagster_run, f"Exceeded maximum runtime of {int(max_time)} seconds."
+                )
+        except:
+            instance.report_engine_event(
+                "Exception while attempting to terminate run. Run will still be marked as failed.",
+                pipeline_name=run_record.dagster_run.job_name,
+                run_id=run_record.dagster_run.run_id,
+                engine_event_data=EngineEventData(
+                    error=serializable_error_info_from_exc_info(sys.exc_info()),
+                ),
+            )
+        _force_mark_as_failed(instance, run_record.dagster_run.run_id)
+
+
+def _force_mark_as_failed(instance: DagsterInstance, run_id: str) -> None:
+    reloaded_record = check.not_none(
+        instance.get_run_record_by_id(run_id), f"Could not reload run record with run_id {run_id}."
+    )
+
+    if not reloaded_record.dagster_run.is_finished:
+        message = (
+            "This job is being forcibly marked as failed. The "
+            "computational resources created by the run may not have been fully cleaned up."
+        )
+        instance.report_run_failed(reloaded_record.dagster_run, message=message)
+        reloaded_record = check.not_none(instance.get_run_record_by_id(run_id))
```

### Comparing `dagster-1.2.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.2.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/sensor.py` & `dagster-1.2.7/dagster/_daemon/sensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,20 @@
 )
 
 import pendulum
 from typing_extensions import Self, TypeAlias
 
 import dagster._check as check
 import dagster._seven as seven
-from dagster._core.definitions.run_request import InstigatorType, RunRequest
+from dagster._core.definitions.run_request import (
+    AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest,
+    InstigatorType,
+    RunRequest,
+)
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.definitions.sensor_definition import DefaultSensorStatus, SensorExecutionData
 from dagster._core.definitions.utils import validate_tags
 from dagster._core.errors import DagsterError
 from dagster._core.host_representation.code_location import CodeLocation
 from dagster._core.host_representation.external import ExternalPipeline, ExternalSensor
 from dagster._core.host_representation.external_data import ExternalTargetData
@@ -578,14 +583,37 @@
 
     yield
 
     if sensor_runtime_data.captured_log_key:
         context.add_log_info(sensor_runtime_data.captured_log_key)
 
     assert isinstance(sensor_runtime_data, SensorExecutionData)
+
+    if sensor_runtime_data.dynamic_partitions_requests:
+        for request in sensor_runtime_data.dynamic_partitions_requests:
+            if isinstance(request, AddDynamicPartitionsRequest):
+                instance.add_dynamic_partitions(
+                    request.partitions_def_name,
+                    request.partition_keys,
+                )
+                context.logger.info(
+                    "Added partition keys to dynamic partitions definition"
+                    f" '{request.partitions_def_name}': {request.partition_keys}"
+                )
+            elif isinstance(request, DeleteDynamicPartitionsRequest):
+                # TODO add a bulk delete method to the instance
+                for partition in request.partition_keys:
+                    instance.delete_dynamic_partition(request.partitions_def_name, partition)
+
+                context.logger.info(
+                    "Deleted partition keys from dynamic partitions definition"
+                    f" '{request.partitions_def_name}': {request.partition_keys}"
+                )
+            else:
+                check.failed(f"Unexpected action {request.action} for dynamic partition request")
     if not sensor_runtime_data.run_requests:
         if sensor_runtime_data.pipeline_run_reactions:
             for pipeline_run_reaction in sensor_runtime_data.pipeline_run_reactions:
                 origin_run_id = check.not_none(pipeline_run_reaction.pipeline_run).run_id
                 if pipeline_run_reaction.error:
                     context.logger.error(
                         f"Got a reaction request for run {origin_run_id} but execution errorred:"
```

### Comparing `dagster-1.2.6/dagster/_daemon/types.py` & `dagster-1.2.7/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_daemon/workspace.py` & `dagster-1.2.7/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_generate/download.py` & `dagster-1.2.7/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_generate/generate.py` & `dagster-1.2.7/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.2.7/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.2.7/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/__init__.py` & `dagster-1.2.7/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/client.py` & `dagster-1.2.7/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/compile.py` & `dagster-1.2.7/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/impl.py` & `dagster-1.2.7/dagster/_grpc/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,15 @@
         }
         with ScheduleEvaluationContext(
             instance_ref,
             scheduled_execution_time,
             repo_def.name,
             schedule_name,
             resources=resources_to_build,
+            repository_def=repo_def,
         ) as schedule_context:
             with user_code_error_boundary(
                 ScheduleExecutionError,
                 lambda: "Error occurred during the execution function for schedule {schedule_name}".format(
                     schedule_name=schedule_def.name
                 ),
             ):
@@ -412,26 +413,22 @@
         (
             _,
             partitions_def,
             partitioned_config,
         ) = _get_job_partitions_and_config_for_partition_set_name(repo_def, partition_set_name)
 
         with _instance_from_ref_for_dynamic_partitions(instance_ref, partitions_def) as instance:
-            partition = partitions_def.get_partition(
-                partition_key, dynamic_partitions_store=instance
-            )
-
             with user_code_error_boundary(
                 PartitionExecutionError,
                 lambda: f"Error occurred during the evaluation of the `run_config_for_partition` function for partition set {partition_set_name}",
             ):
                 run_config = partitioned_config.get_run_config_for_partition_key(
                     partition_key, dynamic_partitions_store=instance
                 )
-                return ExternalPartitionConfigData(name=partition.name, run_config=run_config)
+                return ExternalPartitionConfigData(name=partition_key, run_config=run_config)
     except Exception:
         return ExternalPartitionExecutionErrorData(
             serializable_error_info_from_exc_info(sys.exc_info())
         )
 
 
 def get_partition_names(
@@ -469,25 +466,23 @@
             partitioned_config,
         ) = _get_job_partitions_and_config_for_partition_set_name(repo_def, partition_set_name)
 
         # Certain gRPC servers do not have access to the instance, so we only attempt to instantiate
         # the instance when necessary for dynamic partitions: https://github.com/dagster-io/dagster/issues/12440
 
         with _instance_from_ref_for_dynamic_partitions(instance_ref, partitions_def) as instance:
-            partition = partitions_def.get_partition(
-                partition_name, dynamic_partitions_store=instance
-            )
             with user_code_error_boundary(
                 PartitionExecutionError,
                 lambda: f"Error occurred during the evaluation of the `tags_for_partition` function for partitioned config on job '{job_def.name}'",
             ):
                 tags = partitioned_config.get_tags_for_partition_key(
-                    partition.name, job_name=job_def.name, dynamic_partitions_store=instance
+                    partition_name, job_name=job_def.name, dynamic_partitions_store=instance
                 )
-                return ExternalPartitionTagsData(name=partition.name, tags=tags)
+                return ExternalPartitionTagsData(name=partition_name, tags=tags)
+
     except Exception:
         return ExternalPartitionExecutionErrorData(
             serializable_error_info_from_exc_info(sys.exc_info())
         )
 
 
 def get_external_execution_plan_snapshot(
```

### Comparing `dagster-1.2.6/dagster/_grpc/protos/api.proto` & `dagster-1.2.7/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/server.py` & `dagster-1.2.7/dagster/_grpc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1196,15 +1196,15 @@
 
         self.loadable_target_origin = check.opt_inst_param(
             loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin
         )
         check.bool_param(force_port, "force_port")
         check.int_param(max_retries, "max_retries")
         check.opt_int_param(max_workers, "max_workers")
-        check.bool_param(heartbeat, "heartbeat")
+        self._heartbeat = check.bool_param(heartbeat, "heartbeat")
         check.int_param(heartbeat_timeout, "heartbeat_timeout")
         check.invariant(heartbeat_timeout > 0, "heartbeat_timeout must be greater than 0")
         check.opt_str_param(fixed_server_id, "fixed_server_id")
         check.int_param(startup_timeout, "startup_timeout")
         check.invariant(
             max_workers is None or max_workers > 1 if heartbeat else True,
             (
@@ -1281,20 +1281,20 @@
             if self.server_process.poll() is None:
                 try:
                     self.create_client().shutdown_server()
                 except DagsterUserCodeUnreachableError:
                     pass
 
     def __del__(self):
-        if not self._shutdown:
+        if not self._shutdown and not self._heartbeat:
             warnings.warn(
-                "GrpcServerProcess is being destroyed without signalling to server that "
-                "it should shut down. This may result in server processes living longer than "
-                "they need to. To fix this, wrap the GrpcServerProcess in a contextmanager or "
-                "call shutdown_server on it."
+                "GrpcServerProcess without a heartbeat is being destroyed without signalling to the"
+                " server that it should shut down. This may result in server processes living"
+                " longer than they need to. To fix this, wrap the GrpcServerProcess in a"
+                " contextmanager or call shutdown_server on it."
             )
 
         if not self._waited and os.getenv("STRICT_GRPC_SERVER_PROCESS_WAIT"):
             warnings.warn(
                 "GrpcServerProcess is being destroyed without waiting for the process to "
                 + "fully terminate. This can cause test instability."
             )
```

### Comparing `dagster-1.2.6/dagster/_grpc/server_watcher.py` & `dagster-1.2.7/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_grpc/types.py` & `dagster-1.2.7/dagster/_grpc/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 import zlib
-from typing import Any, FrozenSet, Mapping, NamedTuple, Optional, Sequence
+from typing import AbstractSet, Any, Mapping, NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.code_pointer import CodePointer
 from dagster._core.definitions.events import AssetKey
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.retries import RetryMode
 from dagster._core.host_representation.origin import (
@@ -27,29 +27,29 @@
             ("solid_selection", Sequence[str]),
             ("run_config", Mapping[str, object]),
             ("mode", str),
             ("step_keys_to_execute", Optional[Sequence[str]]),
             ("pipeline_snapshot_id", str),
             ("known_state", Optional[KnownExecutionState]),
             ("instance_ref", Optional[InstanceRef]),
-            ("asset_selection", Optional[FrozenSet[AssetKey]]),
+            ("asset_selection", Optional[AbstractSet[AssetKey]]),
         ],
     )
 ):
     def __new__(
         cls,
         pipeline_origin: ExternalPipelineOrigin,
         solid_selection: Sequence[str],
         run_config: Mapping[str, object],
         mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         pipeline_snapshot_id: str,
         known_state: Optional[KnownExecutionState] = None,
         instance_ref: Optional[InstanceRef] = None,
-        asset_selection: Optional[FrozenSet[AssetKey]] = None,
+        asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ):
         return super(ExecutionPlanSnapshotArgs, cls).__new__(
             cls,
             pipeline_origin=check.inst_param(
                 pipeline_origin, "pipeline_origin", ExternalPipelineOrigin
             ),
             solid_selection=check.opt_sequence_param(
```

### Comparing `dagster-1.2.6/dagster/_grpc/utils.py` & `dagster-1.2.7/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_loggers/__init__.py` & `dagster-1.2.7/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_module_alias_map.py` & `dagster-1.2.7/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_scheduler/scheduler.py` & `dagster-1.2.7/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_scheduler/stale.py` & `dagster-1.2.7/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_serdes/__init__.py` & `dagster-1.2.7/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_serdes/config_class.py` & `dagster-1.2.7/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_serdes/ipc.py` & `dagster-1.2.7/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_serdes/serdes.py` & `dagster-1.2.7/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_serdes/utils.py` & `dagster-1.2.7/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_seven/__init__.py` & `dagster-1.2.7/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_seven/abc.py` & `dagster-1.2.7/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_seven/compat/pendulum.py` & `dagster-1.2.7/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/__init__.py` & `dagster-1.2.7/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/alert.py` & `dagster-1.2.7/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/backcompat.py` & `dagster-1.2.7/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/backoff.py` & `dagster-1.2.7/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/cached_method.py` & `dagster-1.2.7/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/caching_instance_queryer.py` & `dagster-1.2.7/dagster/_utils/caching_instance_queryer.py`

 * *Files 22% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     ####################
 
     @cached_method
     def get_observation_record(
         self,
         *,
         asset_key: AssetKey,
-        before_cursor: int,
+        before_cursor: Optional[int],
     ) -> Optional["EventLogRecord"]:
         from dagster._core.event_api import EventRecordsFilter
 
         return next(
             iter(
                 self.instance.get_event_records(
                     EventRecordsFilter(
@@ -309,15 +309,15 @@
         )
 
     @cached_method
     def next_version_record(
         self,
         *,
         asset_key: AssetKey,
-        after_cursor: int,
+        after_cursor: Optional[int],
         data_version: DataVersion,
     ) -> Optional["EventLogRecord"]:
         from dagster._core.event_api import EventRecordsFilter
 
         for record in self.instance.get_event_records(
             EventRecordsFilter(
                 event_type=DagsterEventType.ASSET_OBSERVATION,
@@ -329,14 +329,75 @@
             record_version = extract_data_version_from_entry(record.event_log_entry)
             if record_version is not None and record_version != data_version:
                 return record
 
         # no records found with a new data version
         return None
 
+    def new_version_exists(
+        self,
+        observable_source_asset_key: AssetKey,
+        after_cursor: Optional[int] = None,
+    ) -> bool:
+        """Returns True if there is an asset observation of the given observable source asset key
+        after the specified cursor.
+
+        Args:
+            observable_source_asset_key (AssetKeyPartitionKey): The observable source asset to query.
+            after_cursor (Optional[int]): Filter parameter such that only records with a storage_id
+                greater than this value will be considered.
+        """
+        previous_version_record = self.get_observation_record(
+            asset_key=observable_source_asset_key,
+            # we're looking for if a new version exists after `after_cursor`, so we need to know
+            # what the version was before `after_cursor`
+            before_cursor=after_cursor,
+        )
+        if previous_version_record is None:
+            return False
+        previous_version = extract_data_version_from_entry(previous_version_record.event_log_entry)
+        if previous_version is None:
+            return False
+
+        next_version_record = self.next_version_record(
+            asset_key=observable_source_asset_key,
+            after_cursor=after_cursor,
+            data_version=previous_version,
+        )
+        return next_version_record is not None
+
+    def _new_version_of_source_exists_after_asset_partition(
+        self,
+        observable_source_asset_key: AssetKey,
+        asset_partition: AssetKeyPartitionKey,
+    ) -> bool:
+        """Returns True if there is a new version of a given observable source asset after the latest
+        materialization record for a given asset partition.
+
+        Attempts to optimize cases where the downstream asset is partitioned, and we expect
+        this to be called multiple times for the same inputs, only varying the partitioned asset's key.
+
+        Args:
+            observable_source_asset_key (AssetKeyPartitionKey): The observable source asset.
+            asset_partition (AssetKeyPartitionKey): The downstream asset partition.
+        """
+        # TODO: this assumes that each observation record will have a distinct data version, which
+        # is not always the case. In the "next_version_record" implementation, we have the benefit
+        # of having an explicit start cursor, but here the corresponding implementation would require
+        # loading all historical observation records. We'll have to do our own pagination here.
+        latest_observation_record = self.get_observation_record(
+            asset_key=observable_source_asset_key,
+            before_cursor=None,
+        )
+        if latest_observation_record is None:
+            return False
+        return not self.materialization_exists(
+            asset_partition, after_cursor=latest_observation_record.storage_id
+        )
+
     ####################
     # RUNS
     ####################
 
     @cached_method
     def _get_run_record_by_id(self, *, run_id: str) -> Optional[RunRecord]:
         return self.instance.get_run_record_by_id(run_id)
@@ -511,16 +572,22 @@
 
         for parent in asset_graph.get_parents_partitions(
             self,
             asset_partition.asset_key,
             asset_partition.partition_key,
         ):
             if asset_graph.is_source(parent.asset_key):
-                continue
-
-            if self._materialization_of_a_exists_after_b(a=parent, b=asset_partition):
+                if asset_graph.is_observable(
+                    parent.asset_key
+                ) and self._new_version_of_source_exists_after_asset_partition(
+                    observable_source_asset_key=parent.asset_key,
+                    asset_partition=asset_partition,
+                ):
+                    return False
+                else:
+                    continue
+            elif self._materialization_of_a_exists_after_b(a=parent, b=asset_partition):
                 return False
-
-            if not self.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
+            elif not self.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
                 return False
 
         return True
```

### Comparing `dagster-1.2.6/dagster/_utils/dagster_type.py` & `dagster-1.2.7/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/error.py` & `dagster-1.2.7/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/external.py` & `dagster-1.2.7/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/forked_pdb.py` & `dagster-1.2.7/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/hosted_user_process.py` & `dagster-1.2.7/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/indenting_printer.py` & `dagster-1.2.7/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/interrupts.py` & `dagster-1.2.7/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/log.py` & `dagster-1.2.7/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/merger.py` & `dagster-1.2.7/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/net.py` & `dagster-1.2.7/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/schedules.py` & `dagster-1.2.7/dagster/_utils/schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,17 @@
     """Generator of execution datetimes >= start_timestamp for the given schedule.
 
     Here cron_schedule is either a cron string or a sequence of cron strings. In the latter case,
     the next execution datetime is obtained by computing the next cron datetime
     after the current execution datetime for each cron string in the sequence, and then choosing
     the earliest among them.
     """
-    check.invariant(is_valid_cron_schedule(cron_schedule))
+    check.invariant(
+        is_valid_cron_schedule(cron_schedule), desc=f"{cron_schedule} must be a valid cron schedule"
+    )
 
     if isinstance(cron_schedule, str):
         yield from cron_string_iterator(
             start_timestamp, cron_schedule, execution_timezone
         ) if ascending else reverse_cron_string_iterator(
             start_timestamp, cron_schedule, execution_timezone
         )
```

### Comparing `dagster-1.2.6/dagster/_utils/tags.py` & `dagster-1.2.7/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/temp_file.py` & `dagster-1.2.7/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/test/mysql_instance.py` & `dagster-1.2.7/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/test/postgres_instance.py` & `dagster-1.2.7/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/test/schedule_storage.py` & `dagster-1.2.7/dagster/_utils/test/schedule_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,17 +98,21 @@
         assert schedule.instigator_name == "my_schedule"
         assert schedule.instigator_data.cron_schedule == "* * * * *"
         assert schedule.instigator_data.start_timestamp is None
 
     def test_add_multiple_schedules(self, storage):
         assert storage
 
-        schedule = self.build_schedule("my_schedule", "* * * * *")
-        schedule_2 = self.build_schedule("my_schedule_2", "* * * * *")
-        schedule_3 = self.build_schedule("my_schedule_3", "* * * * *")
+        schedule = self.build_schedule("my_schedule", "* * * * *", status=InstigatorStatus.RUNNING)
+        schedule_2 = self.build_schedule(
+            "my_schedule_2", "* * * * *", status=InstigatorStatus.STOPPED
+        )
+        schedule_3 = self.build_schedule(
+            "my_schedule_3", "* * * * *", status=InstigatorStatus.AUTOMATICALLY_RUNNING
+        )
 
         storage.add_instigator_state(schedule)
         storage.add_instigator_state(schedule_2)
         storage.add_instigator_state(schedule_3)
 
         schedules = storage.all_instigator_state(
             self.fake_repo_target().get_id(),
@@ -117,14 +121,33 @@
         )
         assert len(schedules) == 3
 
         assert any(s.instigator_name == "my_schedule" for s in schedules)
         assert any(s.instigator_name == "my_schedule_2" for s in schedules)
         assert any(s.instigator_name == "my_schedule_3" for s in schedules)
 
+        running = storage.all_instigator_state(
+            self.fake_repo_target().get_id(),
+            self.fake_repo_target().get_selector_id(),
+            InstigatorType.SCHEDULE,
+            {InstigatorStatus.RUNNING, InstigatorStatus.AUTOMATICALLY_RUNNING},
+        )
+        assert len(running) == 2
+        assert "my_schedule" in [state.instigator_name for state in running]
+        assert "my_schedule_3" in [state.instigator_name for state in running]
+
+        stopped = storage.all_instigator_state(
+            self.fake_repo_target().get_id(),
+            self.fake_repo_target().get_selector_id(),
+            InstigatorType.SCHEDULE,
+            {InstigatorStatus.STOPPED},
+        )
+        assert len(stopped) == 1
+        assert stopped[0].instigator_name == "my_schedule_2"
+
     def test_get_schedule_state(self, storage):
         assert storage
 
         state = self.build_schedule("my_schedule", "* * * * *")
         storage.add_instigator_state(state)
         schedule = storage.get_instigator_state(state.instigator_origin_id, state.selector_id)
```

### Comparing `dagster-1.2.6/dagster/_utils/timing.py` & `dagster-1.2.7/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/typing_api.py` & `dagster-1.2.7/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster/_utils/yaml_utils.py` & `dagster-1.2.7/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/dagster.egg-info/PKG-INFO` & `dagster-1.2.7/dagster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.2.6
+Version: 1.2.7
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.2.6/dagster.egg-info/SOURCES.txt` & `dagster-1.2.7/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 dagster/_core/definitions/asset_layer.py
 dagster/_core/definitions/asset_out.py
 dagster/_core/definitions/asset_reconciliation_sensor.py
 dagster/_core/definitions/asset_selection.py
 dagster/_core/definitions/asset_sensor_definition.py
 dagster/_core/definitions/assets.py
 dagster/_core/definitions/assets_job.py
+dagster/_core/definitions/auto_materialize_policy.py
 dagster/_core/definitions/cacheable_assets.py
 dagster/_core/definitions/composition.py
 dagster/_core/definitions/config.py
 dagster/_core/definitions/configurable.py
 dagster/_core/definitions/data_time.py
 dagster/_core/definitions/data_version.py
 dagster/_core/definitions/definition_config_schema.py
@@ -163,15 +164,14 @@
 dagster/_core/definitions/decorators/__init__.py
 dagster/_core/definitions/decorators/asset_decorator.py
 dagster/_core/definitions/decorators/config_mapping_decorator.py
 dagster/_core/definitions/decorators/graph_decorator.py
 dagster/_core/definitions/decorators/hook_decorator.py
 dagster/_core/definitions/decorators/job_decorator.py
 dagster/_core/definitions/decorators/op_decorator.py
-dagster/_core/definitions/decorators/pipeline_decorator.py
 dagster/_core/definitions/decorators/repository_decorator.py
 dagster/_core/definitions/decorators/schedule_decorator.py
 dagster/_core/definitions/decorators/sensor_decorator.py
 dagster/_core/definitions/decorators/source_asset_decorator.py
 dagster/_core/definitions/metadata/__init__.py
 dagster/_core/definitions/metadata/table.py
 dagster/_core/definitions/repository_definition/__init__.py
```

### Comparing `dagster-1.2.6/dagster.egg-info/requires.txt` & `dagster-1.2.7/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.2.6/setup.py` & `dagster-1.2.7/setup.py`

 * *Files identical despite different names*

