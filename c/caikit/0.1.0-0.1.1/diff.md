# Comparing `tmp/caikit-0.1.0.tar.gz` & `tmp/caikit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.1.0.tar", last modified: Wed Apr 12 20:41:43 2023, max compression
+gzip compressed data, was "caikit-0.1.1.tar", last modified: Wed Apr 12 22:28:30 2023, max compression
```

## Comparing `caikit-0.1.0.tar` & `caikit-0.1.1.tar`

### file list

```diff
@@ -1,299 +1,299 @@
--rw-r--r--   0        0        0       60 2023-04-12 20:41:33.294004 caikit-0.1.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0     1272 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-12 20:41:33.294004 caikit-0.1.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      191 2023-04-12 20:41:33.294004 caikit-0.1.0/.gitignore
--rw-r--r--   0        0        0      299 2023-04-12 20:41:33.294004 caikit-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-12 20:41:33.294004 caikit-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-12 20:41:33.294004 caikit-0.1.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-12 20:41:33.294004 caikit-0.1.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-12 20:41:33.294004 caikit-0.1.0/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-12 20:41:33.294004 caikit-0.1.0/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-12 20:41:33.294004 caikit-0.1.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     6510 2023-04-12 20:41:33.294004 caikit-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-12 20:41:33.294004 caikit-0.1.0/LICENSE
--rw-r--r--   0        0        0       18 2023-04-12 20:41:33.294004 caikit-0.1.0/OWNERS
--rw-r--r--   0        0        0     5155 2023-04-12 20:41:33.294004 caikit-0.1.0/README.md
--rw-r--r--   0        0        0    44878 2023-04-12 20:41:33.294004 caikit-0.1.0/caikit-overview.png
--rw-r--r--   0        0        0      323 2023-04-12 20:41:33.294004 caikit-0.1.0/caikit/__init__.py
--rw-r--r--   0        0        0     1861 2023-04-12 20:41:33.294004 caikit-0.1.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-12 20:41:33.294004 caikit-0.1.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1104 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/config/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/config/config.py
--rw-r--r--   0        0        0     1010 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/config/config.yml
--rw-r--r--   0        0        0      962 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29225 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    12141 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20773 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0    51860 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module.py
--rw-r--r--   0        0        0     7643 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5493 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1110 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0     1787 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/config_utils.py
--rw-r--r--   0        0        0      637 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18275 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     5439 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/extension_utils.py
--rw-r--r--   0        0        0     4935 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1864 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0      630 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/performance/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/performance/json_test_data.py
--rw-r--r--   0        0        0     4278 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/performance/performance.py
--rw-r--r--   0        0        0     1013 2023-04-12 20:41:33.298004 caikit-0.1.0/caikit/core/toolkit/performance/test_data.py
--rw-r--r--   0        0        0     1476 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/toolkit/performance/text_test_data.py
--rw-r--r--   0        0        0      950 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/toolkit/performance_metrics.py
--rw-r--r--   0        0        0    32214 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     5379 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/config/config.yml
--rw-r--r--   0        0        0     1716 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13853 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6068 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12138 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4194 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    17113 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     2947 2023-04-12 20:41:33.302004 caikit-0.1.0/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5611 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12289 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5750 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0     9693 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    11398 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4850 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     7128 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12326 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14525 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10554 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1696 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/utils/config_parser.py
--rw-r--r--   0        0        0     6692 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0     1686 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/utils/log_config.py
--rw-r--r--   0        0        0    17900 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-12 20:41:33.306004 caikit-0.1.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      837 2023-04-12 20:41:33.306004 caikit-0.1.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0      989 2023-04-12 20:41:37.674016 caikit-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-12 20:41:33.306004 caikit-0.1.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-12 20:41:33.306004 caikit-0.1.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/base.py
--rw-r--r--   0        0        0     8909 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    12705 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26028 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-12 20:41:33.306004 caikit-0.1.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    11977 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     2909 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     3080 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_config.py
--rw-r--r--   0        0        0      521 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    18331 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17316 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_module.py
--rw-r--r--   0        0        0     4751 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8440 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0     1953 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_config_utils.py
--rw-r--r--   0        0        0    14999 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4408 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_extension_utils.py
--rw-r--r--   0        0        0     4972 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    15632 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0       27 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-12 20:41:33.310004 caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      176 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1852 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2411 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1404 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2498 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      202 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/config.py
--rw-r--r--   0        0        0      141 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      933 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/fixtures/studio_models/studio_block
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6439 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11774 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18079 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5053 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4762 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3295 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18350 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     1387 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9667 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    12985 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3533 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7386 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29820 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5570 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     3891 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/utils/test_configs.py
--rw-r--r--   0        0        0     5047 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26472 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-12 20:41:33.314004 caikit-0.1.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-12 20:41:33.318004 caikit-0.1.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1025 2023-04-12 20:41:33.318004 caikit-0.1.0/tox.ini
--rw-r--r--   0        0        0     6155 1970-01-01 00:00:00.000000 caikit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-12 22:28:23.919434 caikit-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0     1272 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      191 2023-04-12 22:28:23.919434 caikit-0.1.1/.gitignore
+-rw-r--r--   0        0        0      299 2023-04-12 22:28:23.919434 caikit-0.1.1/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-12 22:28:23.919434 caikit-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-12 22:28:23.919434 caikit-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-12 22:28:23.919434 caikit-0.1.1/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-12 22:28:23.919434 caikit-0.1.1/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-12 22:28:23.923434 caikit-0.1.1/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-12 22:28:23.923434 caikit-0.1.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     6510 2023-04-12 22:28:23.923434 caikit-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-12 22:28:23.923434 caikit-0.1.1/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-12 22:28:23.923434 caikit-0.1.1/OWNERS
+-rw-r--r--   0        0        0     5206 2023-04-12 22:28:23.923434 caikit-0.1.1/README.md
+-rw-r--r--   0        0        0    44878 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit-overview.png
+-rw-r--r--   0        0        0      323 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/__init__.py
+-rw-r--r--   0        0        0     1861 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1104 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/config.py
+-rw-r--r--   0        0        0     1010 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/config.yml
+-rw-r--r--   0        0        0      962 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29225 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    12141 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20773 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    51860 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module.py
+-rw-r--r--   0        0        0     7643 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5493 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1110 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0     1787 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/config_utils.py
+-rw-r--r--   0        0        0      637 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18275 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     5439 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/extension_utils.py
+-rw-r--r--   0        0        0     4935 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1864 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0      630 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/json_test_data.py
+-rw-r--r--   0        0        0     4278 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/performance.py
+-rw-r--r--   0        0        0     1013 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/test_data.py
+-rw-r--r--   0        0        0     1476 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/text_test_data.py
+-rw-r--r--   0        0        0      950 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance_metrics.py
+-rw-r--r--   0        0        0    32214 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     5379 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/config/config.yml
+-rw-r--r--   0        0        0     1716 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13853 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4703 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6068 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12138 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4194 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    17113 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     2947 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5611 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12289 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5750 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0     9693 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    11398 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4850 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     7128 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12326 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    14525 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10554 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1696 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/config_parser.py
+-rw-r--r--   0        0        0     6692 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0     1686 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/log_config.py
+-rw-r--r--   0        0        0    17900 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      837 2023-04-12 22:28:23.931434 caikit-0.1.1/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1069 2023-04-12 22:28:26.883463 caikit-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-12 22:28:23.931434 caikit-0.1.1/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-12 22:28:23.931434 caikit-0.1.1/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3783 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/base.py
+-rw-r--r--   0        0        0     8909 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    12705 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26028 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    11977 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     2909 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     3080 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_config.py
+-rw-r--r--   0        0        0      521 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_imports.py
+-rw-r--r--   0        0        0    18331 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17316 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module.py
+-rw-r--r--   0        0        0     4751 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8440 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0     1953 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_config_utils.py
+-rw-r--r--   0        0        0    14999 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4408 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_extension_utils.py
+-rw-r--r--   0        0        0     4972 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    15632 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      176 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1852 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2411 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1404 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2498 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      202 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/config.py
+-rw-r--r--   0        0        0      141 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      933 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/studio_models/studio_block
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6439 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11774 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18079 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5053 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4762 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3295 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18350 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     1387 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9667 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    12985 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3533 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7386 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    29820 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5570 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     3891 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_configs.py
+-rw-r--r--   0        0        0     5047 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26472 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1025 2023-04-12 22:28:23.935434 caikit-0.1.1/tox.ini
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 caikit-0.1.1/PKG-INFO
```

### Comparing `caikit-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.1.1/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.github/workflows/build-library.yml` & `caikit-0.1.1/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.github/workflows/lint-code.yml` & `caikit-0.1.1/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.github/workflows/publish-library.yml` & `caikit-0.1.1/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/.pylintrc` & `caikit-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/CODE-OF-CONDUCT.md` & `caikit-0.1.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/CONTRIBUTING.md` & `caikit-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/LICENSE` & `caikit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/README.md` & `caikit-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Caikit
 
 Caikit is an AI toolkit that enables users to manage AI models through a set of developer friendly APIs. It provides a consistent format for AI model deployment, consumption and evolution.
 
-![Caikit Overview](./caikit-overview.png)
+![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
 
 ## Capabilities
 
 Caikit streamlines the management of AI models for application usage. Think of it as REST API for applications to AI models.
 
 - Hosts AI models for inference and training so that models can be accessed through APIs
 - Provides access to the different training techniques as supported by a model
```

### Comparing `caikit-0.1.0/caikit-overview.png` & `caikit-0.1.1/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/__init__.py` & `caikit-0.1.1/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/__init__.py` & `caikit-0.1.1/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/base.py` & `caikit-0.1.1/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.1.1/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.1.1/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.1.1/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.1.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.1.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/blocks/__init__.py` & `caikit-0.1.1/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/blocks/base.py` & `caikit-0.1.1/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/config/__init__.py` & `caikit-0.1.1/caikit/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/config/config.py` & `caikit-0.1.1/caikit/core/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/config/config.yml` & `caikit-0.1.1/caikit/core/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/__init__.py` & `caikit-0.1.1/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/base.py` & `caikit-0.1.1/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.1.1/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.1.1/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.1.1/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/dataobject.py` & `caikit-0.1.1/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/enums.py` & `caikit-0.1.1/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/producer.py` & `caikit-0.1.1/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.1.1/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.1.1/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/converter.py` & `caikit-0.1.1/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.1.1/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.1.1/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.1.1/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/data_model/streams/validator.py` & `caikit-0.1.1/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/model_manager.py` & `caikit-0.1.1/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module.py` & `caikit-0.1.1/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_backend_config.py` & `caikit-0.1.1/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_backends/__init__.py` & `caikit-0.1.1/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_backends/backend_types.py` & `caikit-0.1.1/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_backends/base.py` & `caikit-0.1.1/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_backends/local_backend.py` & `caikit-0.1.1/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_config.py` & `caikit-0.1.1/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/module_meta.py` & `caikit-0.1.1/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/resources/__init__.py` & `caikit-0.1.1/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/resources/base.py` & `caikit-0.1.1/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/__init__.py` & `caikit-0.1.1/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/compatibility.py` & `caikit-0.1.1/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/config_utils.py` & `caikit-0.1.1/caikit/core/toolkit/config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.1.1/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.1.1/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.1.1/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/extension_utils.py` & `caikit-0.1.1/caikit/core/toolkit/extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/fileio.py` & `caikit-0.1.1/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/isa.py` & `caikit-0.1.1/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/logging.py` & `caikit-0.1.1/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance/__init__.py` & `caikit-0.1.1/caikit/core/toolkit/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance/json_test_data.py` & `caikit-0.1.1/caikit/core/toolkit/performance/json_test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance/performance.py` & `caikit-0.1.1/caikit/core/toolkit/performance/performance.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance/test_data.py` & `caikit-0.1.1/caikit/core/toolkit/performance/test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance/text_test_data.py` & `caikit-0.1.1/caikit/core/toolkit/performance/text_test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/performance_metrics.py` & `caikit-0.1.1/caikit/core/toolkit/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.1.1/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/serializers.py` & `caikit-0.1.1/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.1.1/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/workflows/__init__.py` & `caikit-0.1.1/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/core/workflows/base.py` & `caikit-0.1.1/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/__init__.py` & `caikit-0.1.1/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/common/__init__.py` & `caikit-0.1.1/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.1.1/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.1.1/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.1.1/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.1.1/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.1.1/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/__init__.py` & `caikit-0.1.1/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/config/config.yml` & `caikit-0.1.1/caikit/runtime/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/dump_services.py` & `caikit-0.1.1/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/grpc_server.py` & `caikit-0.1.1/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.1.1/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.1.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/metrics/__init__.py` & `caikit-0.1.1/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.1.1/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/metrics/throughput.py` & `caikit-0.1.1/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/__init__.py` & `caikit-0.1.1/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/batcher.py` & `caikit-0.1.1/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.1.1/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.1.1/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.1.1/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.1.1/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.1.1/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.1.1/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.1.1/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.1.1/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.1.1/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.1.1/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.1.1/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_factory.py` & `caikit-0.1.1/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.1.1/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.1.1/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/create_service.py` & `caikit-0.1.1/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.1.1/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/primitives.py` & `caikit-0.1.1/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/serializers.py` & `caikit-0.1.1/caikit/runtime/service_generation/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.1.1/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/__init__.py` & `caikit-0.1.1/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.1.1/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.1.1/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.1.1/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.1.1/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.1.1/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/types/__init__.py` & `caikit-0.1.1/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.1.1/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.1.1/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.1.1/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/utils/__init__.py` & `caikit-0.1.1/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/utils/config_parser.py` & `caikit-0.1.1/caikit/runtime/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/utils/import_util.py` & `caikit-0.1.1/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/utils/log_config.py` & `caikit-0.1.1/caikit/runtime/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/utils/servicer_util.py` & `caikit-0.1.1/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/work_management/__init__.py` & `caikit-0.1.1/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.1.1/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.1.1/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.1.1/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.1.1/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/pyproject.toml` & `caikit-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
-readme = "README.md"
+# Not the actual current version: overwritten by CI
+version = "0.1.1"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
+license = {text = "Apache-2.0"}
+readme = "README.md"
+repository = "https://github.com/caikit/caikit"
 requires-python = "~=3.8"
-# Not the actual current version: overwritten by CI
-version = "0.1.0"
 dependencies = [
     "alchemy-config>=1.0.0",
     "alchemy-logging>=1.0.4",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.2.0",
     "munch>=2.5.0,<3.0",
-    "protobuf>=3.20.0,<4",
+    "protobuf>=3.20.1,<5",
     "prometheus_client==0.12.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<3.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
```

### Comparing `caikit-0.1.0/scripts/fmt.sh` & `caikit-0.1.1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/__init__.py` & `caikit-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/base.py` & `caikit-0.1.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/conftest.py` & `caikit-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.1.1/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.1.1/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/blocks/__init__.py` & `caikit-0.1.1/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/blocks/test_base.py` & `caikit-0.1.1/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.1.1/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.1.1/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.1.1/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.1.1/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.1.1/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.1.1/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/test_base.py` & `caikit-0.1.1/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/data_model/test_dataobject.py` & `caikit-0.1.1/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/helpers.py` & `caikit-0.1.1/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.1.1/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_config.py` & `caikit-0.1.1/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_imports.py` & `caikit-0.1.1/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_model_manager.py` & `caikit-0.1.1/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_module.py` & `caikit-0.1.1/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_module_backend_config.py` & `caikit-0.1.1/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_module_metadata.py` & `caikit-0.1.1/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/test_no_write_permissions.py` & `caikit-0.1.1/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.1.1/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_config_utils.py` & `caikit-0.1.1/tests/core/toolkit/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.1.1/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_extension_utils.py` & `caikit-0.1.1/tests/core/toolkit/test_extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_fileio.py` & `caikit-0.1.1/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.1.1/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_serializers.py` & `caikit-0.1.1/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.1.1/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/workflows/__init__.py` & `caikit-0.1.1/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/core/workflows/test_base.py` & `caikit-0.1.1/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/data_model_helpers.py` & `caikit-0.1.1/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_block.zip` & `caikit-0.1.1/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_block/config.yml` & `caikit-0.1.1/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.1.1/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_resource.zip` & `caikit-0.1.1/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_workflow.zip` & `caikit-0.1.1/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/fixtures.py` & `caikit-0.1.1/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/invalid.zip` & `caikit-0.1.1/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/linux.txt` & `caikit-0.1.1/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/primitive_party.proto` & `caikit-0.1.1/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.1.1/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.1.1/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/fixtures/studio_models/studio_block` & `caikit-0.1.1/tests/fixtures/studio_models/studio_block`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/generated/__init__.py` & `caikit-0.1.1/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/metrics/__init__.py` & `caikit-0.1.1/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.1.1/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/metrics/test_throughput.py` & `caikit-0.1.1/tests/runtime/metrics/test_throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/__init__.py` & `caikit-0.1.1/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.1.1/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.1.1/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.1.1/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.1.1/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.1.1/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.1/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.1.1/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.1.1/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.1.1/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.1.1/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/__init__.py` & `caikit-0.1.1/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.1.1/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.1.1/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.1.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.1.1/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.1.1/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/test_grpc_server.py` & `caikit-0.1.1/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/test_service_factory.py` & `caikit-0.1.1/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/utils/__init__.py` & `caikit-0.1.1/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/utils/test_configs.py` & `caikit-0.1.1/tests/runtime/utils/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/utils/test_import_util.py` & `caikit-0.1.1/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.1.1/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/work_management/__init__.py` & `caikit-0.1.1/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.1.1/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.1.1/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.1.1/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/tox.ini` & `caikit-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.1.0/PKG-INFO` & `caikit-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: alchemy-config>=1.0.0
 Requires-Dist: alchemy-logging>=1.0.4
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.2.0
 Requires-Dist: munch>=2.5.0,<3.0
-Requires-Dist: protobuf>=3.20.0,<4
+Requires-Dist: protobuf>=3.20.1,<5
 Requires-Dist: prometheus_client==0.12.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<3.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
@@ -24,15 +24,15 @@
 Requires-Dist: jtd-to-proto>=0.11.4,<0.12.0
 Requires-Dist: import-tracker>=3.1.5,<4
 
 # Caikit
 
 Caikit is an AI toolkit that enables users to manage AI models through a set of developer friendly APIs. It provides a consistent format for AI model deployment, consumption and evolution.
 
-![Caikit Overview](./caikit-overview.png)
+![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
 
 ## Capabilities
 
 Caikit streamlines the management of AI models for application usage. Think of it as REST API for applications to AI models.
 
 - Hosts AI models for inference and training so that models can be accessed through APIs
 - Provides access to the different training techniques as supported by a model
```

