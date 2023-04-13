# Comparing `tmp/ai_transform-0.30.4.tar.gz` & `tmp/ai_transform-0.30.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.4.tar", last modified: Wed Apr 12 06:58:56 2023, max compression
+gzip compressed data, was "ai_transform-0.30.5.tar", last modified: Thu Apr 13 01:30:40 2023, max compression
```

## Comparing `ai_transform-0.30.4.tar` & `ai_transform-0.30.5.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-12 06:58:38.000000 ai_transform-0.30.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 06:58:56.312854 ai_transform-0.30.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-12 06:58:38.000000 ai_transform-0.30.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.292854 ai_transform-0.30.4/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32516 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.300854 ai_transform-0.30.4/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.304854 ai_transform-0.30.4/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.304854 ai_transform-0.30.4/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-12 06:58:38.000000 ai_transform-0.30.4/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.296854 ai_transform-0.30.4/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 06:58:56.000000 ai_transform-0.30.4/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:58:56.312854 ai_transform-0.30.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-12 06:58:38.000000 ai_transform-0.30.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.308854 ai_transform-0.30.4/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:56.312854 ai_transform-0.30.4/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 06:58:38.000000 ai_transform-0.30.4/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-13 01:30:19.000000 ai_transform-0.30.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 01:30:40.951236 ai_transform-0.30.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-13 01:30:19.000000 ai_transform-0.30.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.939236 ai_transform-0.30.5/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.939236 ai_transform-0.30.5/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 01:30:19.000000 ai_transform-0.30.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 01:30:40.951236 ai_transform-0.30.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 01:30:19.000000 ai_transform-0.30.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.4/LICENSE` & `ai_transform-0.30.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/README.md` & `ai_transform-0.30.5/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/ai_transform/__init__.py` & `ai_transform-0.30.5/ai_transform/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.4"
+__version__ = "0.30.5"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.4/ai_transform/api/api.py` & `ai_transform-0.30.5/ai_transform/api/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 from json import JSONDecodeError
 from functools import wraps
 
 from typing import Any, Dict, List, Optional, Literal
 
 from ai_transform.logger import format_logging_info
 from ai_transform.utils import document
-from ai_transform.types import (
-    Credentials,
-    FieldTransformer,
-    Filter,
-    Schema,
-)
+from ai_transform.types import Credentials, FieldTransformer, Filter, Schema
 
 from ai_transform import __version__
 
 
 LOG_REQUESTS = bool(os.getenv("LOG_REQUESTS"))
 if LOG_REQUESTS:
     # Get the current Unix timestamp as a string
@@ -65,17 +60,15 @@
     # get a json response
     # if errors - print what the response contains
     if response.status_code == 200:
         try:
             return response.json()
         except Exception as e:
             logger.exception(e)
-            logger.error(
-                format_logging_info({"x-trace-id": response.headers["x-trace-id"]})
-            )
+            logger.error(format_logging_info({"x-trace-id": response.headers["x-trace-id"]}))
             raise e
     else:
         datum = {"error": response.content.decode("utf-8")}
         if "x-trace-id" in response.headers:
             datum["x-trace-id"] = response.headers["x-trace-id"]
 
         try:
@@ -121,24 +114,19 @@
 
         return function_wrapper
 
     return _retry
 
 
 class API:
-    def __init__(
-        self, credentials: Credentials, job_id: str = None, name: str = None
-    ) -> None:
+    def __init__(self, credentials: Credentials, job_id: str = None, name: str = None) -> None:
         self._credentials = credentials
-        self._base_url = (
-            f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
-        )
+        self._base_url = f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
         self._headers = dict(
-            Authorization=f"{self.credentials.project}:{self.credentials.api_key}",
-            ai_transform_version=__version__,
+            Authorization=f"{self.credentials.project}:{self.credentials.api_key}", ai_transform_version=__version__
         )
         if job_id is not None:
             self.headers.update(ai_transform_job_id=job_id)
         if name is not None:
             self.headers.update(ai_transform_name=name)
 
         self.session = requests.Session()
@@ -152,24 +140,16 @@
         return self._base_url
 
     @property
     def headers(self) -> Dict[str, str]:
         return self._headers
 
     @retry()
-    def _request(
-        self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs
-    ) -> Response:
-        request = requests.Request(
-            method=method,
-            url=self.base_url + suffix,
-            headers=self.headers,
-            *args,
-            **kwargs,
-        )
+    def _request(self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs) -> Response:
+        request = requests.Request(method=method, url=self.base_url + suffix, headers=self.headers, *args, **kwargs)
         prepared_request = request.prepare()
 
         if LOG_REQUESTS:
             log_request(prepared_request)
 
         response = self.session.send(prepared_request)
 
@@ -185,23 +165,18 @@
         return self._request(method="POST", suffix=suffix, *args, **kwargs)
 
     def _list_datasets(self):
         response = self.get(suffix="/datasets/list")
         return get_response(response)
 
     def _create_dataset(
-        self,
-        dataset_id: str,
-        schema: Optional[Schema] = None,
-        upsert: bool = True,
-        expire: bool = False,
+        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
     ) -> Any:
         response = self.post(
-            suffix=f"/datasets/create",
-            json=dict(id=dataset_id, schema=schema, upsert=upsert, expire=expire),
+            suffix=f"/datasets/create", json=dict(id=dataset_id, schema=schema, upsert=upsert, expire=expire)
         )
         return get_response(response)
 
     def _delete_dataset(self, dataset_id: str) -> Any:
         response = self.post(suffix=f"/datasets/{dataset_id}/delete")
         return get_response(response)
 
@@ -223,17 +198,15 @@
         response = self.post(
             suffix=f"/datasets/{dataset_id}/documents/bulk_insert",
             json=dict(
                 documents=documents,
                 insert_date=insert_date,
                 overwrite=overwrite,
                 update_schema=update_schema,
-                field_transformers=[]
-                if field_transformers is None
-                else field_transformers,
+                field_transformers=[] if field_transformers is None else field_transformers,
                 ingest_in_background=ingest_in_background,
                 wait_for_update=wait_for_update,
             ),
         )
         return get_response(response)
 
     def _bulk_update(
@@ -280,58 +253,40 @@
                 is_random=is_random,
                 after_id=[] if after_id is None else after_id,
                 worker_number=worker_number,
             ),
         )
         return get_response(response)
 
-    def _delete_where(
-        self,
-        dataset_id: str,
-        filters: Optional[List[Filter]] = None,
-    ):
+    def _delete_where(self, dataset_id: str, filters: Optional[List[Filter]] = None):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/documents/delete_where",
-            json=dict(
-                filters=[] if filters is None else filters,
-            ),
+            json=dict(filters=[] if filters is None else filters),
         )
         return get_response(response)
 
     def _update_dataset_metadata(self, dataset_id: str, metadata: Dict[str, Any]):
         """
         Edit and add metadata about a dataset. Notably description, data source, etc
         """
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/metadata",
-            json=dict(dataset_id=dataset_id, metadata=metadata),
+            suffix=f"/datasets/{dataset_id}/metadata", json=dict(dataset_id=dataset_id, metadata=metadata)
         )
         return get_response(response)
 
     def _get_metadata(self, dataset_id: str) -> Dict[str, Any]:
-        response = self.get(
-            suffix=f"/datasets/{dataset_id}/metadata",
-        )
+        response = self.get(suffix=f"/datasets/{dataset_id}/metadata")
         return get_response(response)
 
     def _insert_centroids(
-        self,
-        dataset_id: str,
-        cluster_centers: List[document.Document],
-        vector_fields: List[str],
-        alias: str,
+        self, dataset_id: str, cluster_centers: List[document.Document], vector_fields: List[str], alias: str
     ):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/cluster/centroids/insert",
-            json=dict(
-                dataset_id=dataset_id,
-                cluster_centers=cluster_centers,
-                vector_fields=vector_fields,
-                alias=alias,
-            ),
+            json=dict(dataset_id=dataset_id, cluster_centers=cluster_centers, vector_fields=vector_fields, alias=alias),
         )
         return get_response(response)
 
     def _get_centroids(
         self,
         dataset_id: str,
         vector_fields: List[str],
@@ -367,17 +322,15 @@
         email: Dict[str, Any] = None,
         user_errors: str = None,
     ):
         # add edge case for API
         if job_id == "":
             return
         if status not in {"inprogress", "complete", "failed"}:
-            raise ValueError(
-                "state should be one of `['inprogress', 'complete', 'failed']`"
-            )
+            raise ValueError("state should be one of `['inprogress', 'complete', 'failed']`")
         parameters = dict(
             status=status,
             workflow_name=workflow_name,
             additional_information=additional_information,
             send_email=send_email,
         )
         # metadata can't be an empty dictionary as it overwrites
@@ -400,18 +353,15 @@
             assert "url" in email["secondary_cta"]
             assert "text" in email["secondary_cta"]
 
             parameters["email"] = email
 
         logger.debug(format_logging_info(parameters))
 
-        response = self.post(
-            suffix=f"/workflows/{job_id}/status",
-            json=parameters,
-        )
+        response = self.post(suffix=f"/workflows/{job_id}/status", json=parameters)
         return get_response(response)
 
     def _set_field_children(
         self,
         dataset_id: str,
         fieldchildren_id: str,
         field: str,
@@ -432,77 +382,55 @@
         params = dict(
             field=field,
             field_children=field_children,
             category=fieldchildren_id,
             metadata={} if metadata is None else metadata,
         )
         logger.debug(format_logging_info(params))
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/field_children/{str(uuid.uuid4())}/update",
-            json=params,
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{str(uuid.uuid4())}/update", json=params)
         return get_response(response)
 
     def _delete_field_children(self, dataset_id: str, fieldchildren_id: str):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/field_children/{fieldchildren_id}/delete",
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{fieldchildren_id}/delete")
         return get_response(response)
 
-    def _list_field_children(
-        self, dataset_id: str, page: int = 1, page_size: int = 10000, sort=None
-    ):
+    def _list_field_children(self, dataset_id: str, page: int = 1, page_size: int = 10000, sort=None):
         parameters = {"page": page, "page_size": page_size}
 
         if sort:
             parameters["sort"] = sort
 
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/field_children/list",
-            json=parameters,
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/list", json=parameters)
         return get_response(response)
 
     def _get_health(self, dataset_id: str):
-        response = self.get(
-            suffix=f"/datasets/{dataset_id}/monitor/health",
-        )
+        response = self.get(suffix=f"/datasets/{dataset_id}/monitor/health")
         return get_response(response)
 
     def _get_workflow_status(self, job_id: str):
         response = self.post(suffix=f"/workflows/{job_id}/get")
         return get_response(response)
 
     def _update_workflow_metadata(self, job_id: str, metadata: Dict[str, Any]):
-        response = self.post(
-            suffix=f"/workflows/{job_id}/metadata",
-            json=dict(metadata=metadata),
-        )
+        response = self.post(suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata))
         return get_response(response)
 
     def _get_file_upload_urls(self, dataset_id: str, files: List[str]):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/get_file_upload_urls",
-            json=dict(files=files),
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/get_file_upload_urls", json=dict(files=files))
         return get_response(response)
 
     def _get_temp_file_upload_url(self):
         """Use this for temporary file uploads.
         returns: {'download_url': ..., 'upload_url': ...}
         """
-        response = self.post(
-            suffix=f"/services/get_temporary_file_upload_url",
-        )
+        response = self.post(suffix=f"/services/get_temporary_file_upload_url")
         return get_response(response)
 
     def _upload_temporary_media(self, presigned_url: str, media_content: bytes):
-        return requests.put(
-            presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content
-        )
+        return requests.put(presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content)
 
     def _upload_media(self, presigned_url: str, media_content: bytes):
         # dont use get response since response cannot be json decoded
         return requests.put(presigned_url, data=media_content)
 
     def _trigger(
         self,
@@ -514,20 +442,15 @@
         host_type: str = None,
         version: str = "production_version",
     ):
         """
         trigger a workflow
         """
 
-        data = dict(
-            params=params,
-            dataset_id=dataset_id,
-            workflow_id=workflow_id,
-            version=version,
-        )
+        data = dict(params=params, dataset_id=dataset_id, workflow_id=workflow_id, version=version)
         if notebook_path is not None:
             data["notebook_path"] = notebook_path
         if instance_type is not None:
             data["instance_type"] = instance_type
         if host_type is not None:
             data["host_type"] = host_type
         return self.post(suffix=f"/workflows/trigger", json=data).json()
@@ -583,28 +506,20 @@
         """
         if worker_number is None:
             worker_number = 0
 
         if n_processed_pricing:
             params["n_processed_pricing "] = n_processed_pricing
 
-        params = dict(
-            worker_number=worker_number,
-            step=step,
-            n_processed=n_processed,
-            n_total=n_total,
-        )
+        params = dict(worker_number=worker_number, step=step, n_processed=n_processed, n_total=n_total)
 
         logger.debug("adding progress...")
         logger.debug(format_logging_info(params))
 
-        response = self.post(
-            suffix=f"/workflows/{workflow_id}/progress",
-            json=params,
-        )
+        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
         return get_response(response)
 
     def _update_workflow_pricing(
         self,
         workflow_id: str,
         worker_number: int = 0,
         step: str = "Workflow",
@@ -614,131 +529,72 @@
         Pricing endpoint is really part of progress endpoint but this is being
         abstracted away for now due to the fact that the pricing is actually
         something outside of progress.
         """
         if worker_number is None:
             worker_number = 0
 
-        params = dict(
-            worker_number=worker_number,
-            step=step,
-            n_processed_pricing=n_processed_pricing,
-        )
+        params = dict(worker_number=worker_number, step=step, n_processed_pricing=n_processed_pricing)
         logger.debug("adding progress...")
         logger.debug(format_logging_info(params))
-        response = self.post(
-            suffix=f"/workflows/{workflow_id}/progress",
-            json=params,
-        )
+        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
         return get_response(response)
 
-    def _append_tags(
-        self,
-        dataset_id: str,
-        field: str,
-        tags_to_add: List[str],
-        filters: List[Filter],
-    ):
+    def _append_tags(self, dataset_id: str, field: str, tags_to_add: List[str], filters: List[Filter]):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/tags/append",
-            json=dict(
-                field=field,
-                tags_to_add=tags_to_add,
-                filters=filters,
-            ),
+            json=dict(field=field, tags_to_add=tags_to_add, filters=filters),
         )
         return get_response(response)
 
-    def _delete_tags(
-        self,
-        dataset_id: str,
-        field: str,
-        tags_to_delete: List[str],
-        filters: List[Filter],
-    ):
+    def _delete_tags(self, dataset_id: str, field: str, tags_to_delete: List[str], filters: List[Filter]):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/tags/delete",
-            json=dict(
-                field=field,
-                tags_to_delete=tags_to_delete,
-                filters=filters,
-            ),
+            json=dict(field=field, tags_to_delete=tags_to_delete, filters=filters),
         )
         return get_response(response)
 
-    def _merge_tags(
-        self,
-        dataset_id: str,
-        field: str,
-        tags_to_merge: Dict[str, str],
-        filters: List[Filter],
-    ):
+    def _merge_tags(self, dataset_id: str, field: str, tags_to_merge: Dict[str, str], filters: List[Filter]):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/tags/merge",
-            json=dict(
-                field=field,
-                tags_to_merge=tags_to_merge,
-                filters=filters,
-            ),
+            json=dict(field=field, tags_to_merge=tags_to_merge, filters=filters),
         )
         return get_response(response)
 
-    def _bulk_update_keyphrase(
-        self,
-        dataset_id: str,
-        field: str,
-        alias: str,
-        updates: List,
-    ):
+    def _bulk_update_keyphrase(self, dataset_id: str, field: str, alias: str, updates: List):
         """
         Update keyphrases
         """
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_update",
-            json=dict(updates=updates),
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_update", json=dict(updates=updates)
         )
         return get_response(response)
 
-    def _bulk_delete_keyphrase(
-        self,
-        dataset_id: str,
-        field: str,
-        alias: str,
-        ids: List[str],
-    ):
+    def _bulk_delete_keyphrase(self, dataset_id: str, field: str, alias: str, ids: List[str]):
         """
         Update keyphrases
         """
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_delete",
-            json=dict(ids=ids),
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_delete", json=dict(ids=ids)
         )
         return get_response(response)
 
-    def _get_keyphrase(
-        self, dataset_id: str, field: str, alias: str, keyphrase_id: str
-    ):
+    def _get_keyphrase(self, dataset_id: str, field: str, alias: str, keyphrase_id: str):
         """
         Get keyphrase
         """
         if isinstance(keyphrase_id, str) and keyphrase_id != "":
-            response = self.get(
-                suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/get",
-            )
+            response = self.get(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/get")
             return get_response(response)
 
-    def _delete_keyphrase(
-        self, dataset_id: str, field: str, keyphrase_id: str, alias: str
-    ):
+    def _delete_keyphrase(self, dataset_id: str, field: str, keyphrase_id: str, alias: str):
         """
         Deleting Keyphrases
         """
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/delete",
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/delete")
         return get_response(response)
 
     def _update_keyphrase(
         self,
         dataset_id: str,
         field: str,
         keyphrase_id: str,
@@ -765,128 +621,79 @@
         if ancestors is not None:
             params["ancestors"] = ancestors
         if parents is not None:
             params["parents"] = parents
         if metadata is not None:
             params["metadata"] = metadata
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/update",
-            json=params,
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/update", json=params
         )
         return get_response(response)
 
     def _list_keyphrase(
-        self,
-        dataset_id: str,
-        field: str,
-        alias: str,
-        page: int = 0,
-        page_size: int = 100,
-        sort: list = None,
+        self, dataset_id: str, field: str, alias: str, page: int = 0, page_size: int = 100, sort: list = None
     ):
         """
         List keyphrases
         """
-        params = {
-            "page": page,
-            "page_size": min(9999, page_size),
-        }
+        params = {"page": page, "page_size": min(9999, page_size)}
         if sort is not None:
             params["sort"] = sort
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/list",
-            json=params,
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/list", json=params)
         return get_response(response)
 
     def _facets(
         self,
         dataset_id: str,
         fields: List[str],
         data_interval: str = "monthly",
         page_size: int = 1000,
         asc: bool = False,
     ):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/facets",
-            json=dict(
-                fields=fields,
-                data_interval=data_interval,
-                page_size=min(9999, page_size),
-                asc=asc,
-            ),
+            json=dict(fields=fields, data_interval=data_interval, page_size=min(9999, page_size), asc=asc),
         )
         return get_response(response)
 
-    def _upsert_dataset_settings(
-        self,
-        dataset_id: str,
-        settings: Optional[Dict[str, Any]] = None,
-    ):
+    def _upsert_dataset_settings(self, dataset_id: str, settings: Optional[Dict[str, Any]] = None):
         response = self.post(
-            suffix=f"/datasets/{dataset_id}/settings",
-            json=dict(settings={} if settings is None else settings),
+            suffix=f"/datasets/{dataset_id}/settings", json=dict(settings={} if settings is None else settings)
         )
         return get_response(response)
 
-    def _get_dataset_settings(
-        self,
-        dataset_id: str,
-    ):
-        response = self.get(
-            suffix=f"/datasets/{dataset_id}/settings",
-        )
+    def _get_dataset_settings(self, dataset_id: str):
+        response = self.get(suffix=f"/datasets/{dataset_id}/settings")
         return get_response(response)
 
-    def _create_deployable(
-        self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None
-    ):
+    def _create_deployable(self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None):
         response = self.post(
             suffix="/deployables/create",
-            json=dict(
-                dataset_id=dataset_id,
-                configuration={} if config is None else config,
-            ),
+            json=dict(dataset_id=dataset_id, configuration={} if config is None else config),
         )
         return get_response(response)
 
     def _share_dashboard(self, deployable_id: str):
-        response = self.post(
-            suffix=f"/deployablegroups/{deployable_id}/share",
-        )
+        response = self.post(suffix=f"/deployablegroups/{deployable_id}/share")
         return get_response(response)
 
     def _unshare_dashboard(self, deployable_id: str):
-        response = self.post(
-            suffix=f"/deployablegroups/{deployable_id}/private",
-        )
+        response = self.post(suffix=f"/deployablegroups/{deployable_id}/private")
         return get_response(response)
 
     def _get_deployable(self, deployable_id: str):
-        response = self.get(
-            suffix=f"/deployables/{deployable_id}/get",
-        )
+        response = self.get(suffix=f"/deployables/{deployable_id}/get")
         return get_response(response)
 
     def _delete_deployable(self, deployable_id: str):
-        response = self.post(
-            suffix=f"/deployables/delete",
-            json=dict(
-                id=deployable_id,
-            ),
-        )
+        response = self.post(suffix=f"/deployables/delete", json=dict(id=deployable_id))
         return get_response(response)
 
     def _list_deployables(self, page_size: int):
-        response = self.get(
-            suffix="/deployables/list",
-            params=dict(
-                page_size=min(9999, page_size),
-            ),
-        )
+        response = self.get(suffix="/deployables/list", params=dict(page_size=min(9999, page_size)))
         return get_response(response)
 
     def _label_openai(
         self,
         dataset_id: str,
         vector_field: str,
         field: str,
@@ -915,18 +722,15 @@
                         "question_suffix": question_suffix,
                     },
                 }
             ],
         }
         if filters is not None:
             params["filters"] = filters
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/labels/create",
-            json=params,
-        )
+        response = self.post(suffix=f"/datasets/{dataset_id}/cluster/centroids/labels/create", json=params)
         return get_response(response)
 
     def _aggregate(
         self,
         dataset_id: str,
         page_size: str = 20,
         page: str = 1,
@@ -978,76 +782,49 @@
                 page=page,
                 similarity_metric=similarity_metric,
                 min_score=min_score,
                 include_vector=include_vector,
                 include_count=include_count,
                 include_relevance=include_relevance,
                 page_size=min(9999, page_size),
-                cluster_properties_filter=cluster_properties_filter
-                if cluster_properties_filter is not None
-                else {},
+                cluster_properties_filter=cluster_properties_filter if cluster_properties_filter is not None else {},
                 filters=filters if filters is not None else [],
                 cluster_ids=cluster_ids if cluster_ids is not None else [],
                 select_fields=select_fields if select_fields is not None else [],
             ),
         )
         return get_response(response)
 
     def _list_project_keys(self):
-        response = self.get(
-            suffix="/projects/keys/list",
-        )
+        response = self.get(suffix="/projects/keys/list")
         return get_response(response)
 
     def _get_project_key(self, key: str, token: str):
-        response = self.post(
-            suffix="/projects/keys/get",
-            json=dict(key=key, token=token),
-        )
+        response = self.post(suffix="/projects/keys/get", json=dict(key=key, token=token))
         return get_response(response)
 
     def _set_project_key(self, key: str, value: str):
-        response = self.post(
-            suffix="/projects/keys/set",
-            json=dict(key=key, value=value),
-        )
+        response = self.post(suffix="/projects/keys/set", json=dict(key=key, value=value))
         return get_response(response)
 
     def _delete_project_key(self, key: str):
-        response = self.post(
-            suffix="/projects/keys/delete",
-            json=dict(key=key),
-        )
+        response = self.post(suffix="/projects/keys/delete", json=dict(key=key))
         return get_response(response)
 
-    def _update_version_aliases(
-        self, development_version: str, production_version: str
-    ):
+    def _update_version_aliases(self, development_version: str, production_version: str):
         response = self.post(
             suffix="/workflows/types/version_aliases/update",
-            json={
-                "aliases": {
-                    "development_version": development_version,
-                    "production_version": production_version,
-                },
-            },
+            json={"aliases": {"development_version": development_version, "production_version": production_version}},
         )
         return get_response(response)
 
     def _openai_completion(
-        self,
-        workflows_admin_token: str,
-        body: dict,
-        suffix: str = "/admin/proxy/openai/v1/completions",
+        self, workflows_admin_token: str, body: dict, suffix: str = "/admin/proxy/openai/v1/completions"
     ):
-        response = self.post(
-            suffix=suffix,
-            json={"token": workflows_admin_token, "body": body},
-        )
+        response = self.post(suffix=suffix, json={"token": workflows_admin_token, "body": body})
         return get_response(response)
 
     def _proxy_openai(self, workflows_admin_token: str, endpoint: str, body: dict):
         response = self.post(
-            suffix="/admin/proxy/openai" + endpoint,
-            json={"token": workflows_admin_token, "body": body},
+            suffix="/admin/proxy/openai" + endpoint, json={"token": workflows_admin_token, "body": body}
         )
         return get_response(response)
```

### Comparing `ai_transform-0.30.4/ai_transform/api/client.py` & `ai_transform-0.30.5/ai_transform/api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,18 @@
     def api(self) -> API:
         return self._api
 
     def list_datasets(self):
         return self.api._list_datasets()
 
     def create_dataset(
-        self,
-        dataset_id: str,
-        schema: Optional[Schema] = None,
-        upsert: bool = True,
-        expire: bool = False,
+        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
     ) -> None:
         return self.api._create_dataset(
-            dataset_id=dataset_id,
-            schema={} if schema is None else schema,
-            upsert=upsert,
-            expire=expire,
+            dataset_id=dataset_id, schema={} if schema is None else schema, upsert=upsert, expire=expire
         )
 
     def delete_dataset(self, dataset_id: str) -> None:
         return self.api._delete_dataset(dataset_id=dataset_id)
 
     def Dataset(self, dataset_id: str, expire: bool = False) -> Dataset:
         self.create_dataset(dataset_id=dataset_id, expire=expire)
@@ -88,18 +81,15 @@
         Insert temporary local media.
         """
         data = self.api._get_temp_file_upload_url()
         upload_url = data["upload_url"]
         download_url = data["download_url"]
         with open(file_path, "rb") as fn_byte:
             media_content = bytes(fn_byte.read())
-        response = self.api._upload_temporary_media(
-            presigned_url=upload_url,
-            media_content=media_content,
-        )
+        response = self.api._upload_temporary_media(presigned_url=upload_url, media_content=media_content)
         logger.debug(response.content)
         return {"download_url": download_url}
 
     def list_project_keys(self):
         return self.api._list_project_keys()
 
     def get_project_key(self, key: str, token: str):
@@ -120,14 +110,8 @@
         model: str = "text-davinci-003",
         workflows_admin_token: str = None,
         max_tokens: int = 20,
         temperature: float = 0.0,
     ):
         if workflows_admin_token is None:
             workflows_admin_token = os.getenv("WORKFLOWS_ADMIN_TOKEN")
-        return self.api._openai_completion(
-            workflows_admin_token,
-            model,
-            prompt,
-            max_tokens,
-            temperature,
-        )
+        return self.api._openai_completion(workflows_admin_token, model, prompt, max_tokens, temperature)
```

### Comparing `ai_transform-0.30.4/ai_transform/api/helpers.py` & `ai_transform-0.30.5/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/ai_transform/api/wrappers.py` & `ai_transform-0.30.5/ai_transform/api/wrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,20 +36,15 @@
         retry_func = lambda result: False
 
     for n in range(1, num_retries + 1):
         try:
             result = fn(*args, **kwargs)
 
             if result.status_code != 200:
-                to_log = format_logging_info(
-                    {
-                        "message": result.content.decode(),
-                        "status_code": result.status_code,
-                    }
-                )
+                to_log = format_logging_info({"message": result.content.decode(), "status_code": result.status_code})
                 if output_to_stdout:
                     print(to_log)
                 else:
                     logger.debug(to_log)
 
                 raise ValueError(to_log)
```

### Comparing `ai_transform-0.30.4/ai_transform/components/components.py` & `ai_transform-0.30.5/ai_transform/components/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
     All components are here
 """
 from dataclasses import dataclass, asdict, field
 from typing import Any, List
 
-COLAB_PREFIX = (
-    "https://colab.research.google.com/github/RelevanceAI/workflows/blob/main/"
-)
+COLAB_PREFIX = "https://colab.research.google.com/github/RelevanceAI/workflows/blob/main/"
 
 # This is useful if you are ignoring
 GENERATED_TYPES = ["sentiment", "cluster", "tag", "emotion"]
 
 
 @dataclass
 class Component:
@@ -89,20 +87,15 @@
 
     def _add_only_types(self, doc: dict):
         doc["props"]["onlyTypes"] = self.only_types
         return doc
 
     @property
     def hooks(self):
-        return [
-            self._add_optional,
-            self._add_only_types,
-            self._add_multiple,
-            self._add_exclude_types,
-        ]
+        return [self._add_optional, self._add_only_types, self._add_multiple, self._add_exclude_types]
 
 
 @dataclass
 class FileUpload(Component):
     title: str = "Upload your files."
     description: str = "You can upload your files here."
     value_key: str = "images"
@@ -160,56 +153,35 @@
 
 @dataclass
 class BaseDropdown(Component):
     title: str = ""
     description: str = ""
     value_key: str = ""
     options: List[Option] = field(
-        default_factory=lambda x: [
-            Option(label="Yes", value=True),
-            Option(label="No", value=False),
-        ]
+        default_factory=lambda x: [Option(label="Yes", value=True), Option(label="No", value=False)]
     )
     type: str = "baseDropdown"
 
 
 @dataclass
 class BoolDropdown(Component):
     title: str = ""
     description: str = ""
     value_key: str = ""
     type: str = "baseDropdown"
-    options: list = field(
-        default_factory=lambda x: [
-            {
-                "label": "Yes",
-                "value": True,
-            },
-            {
-                "label": "No",
-                "value": False,
-            },
-        ],
-    )
+    options: list = field(default_factory=lambda x: [{"label": "Yes", "value": True}, {"label": "No", "value": False}])
 
     def _add_options(self):
         self.doc["props"]["options"] = self.options
 
     @property
     def hooks(self):
-        return [
-            self._add_optional,
-            self._add_multiple,
-            self._add_options,
-            self._add_default_value,
-        ]
+        return [self._add_optional, self._add_multiple, self._add_options, self._add_default_value]
 
-    props: dict = field(
-        default_factory=lambda: {"multiple": False, "optional": True, "value": True}
-    )
+    props: dict = field(default_factory=lambda: {"multiple": False, "optional": True, "value": True})
 
 
 @dataclass
 class TagsInput(Component):
     title: str = ""
     description: str = ""
     value_key: str = "tagsToDelete"
@@ -248,21 +220,15 @@
         doc["props"]["min"] = self.min
         if "min" in doc:
             doc.pop("min")
         return doc
 
     @property
     def hooks(self):
-        return [
-            self._add_type,
-            self._add_default_value,
-            self._add_max,
-            self._add_min,
-            self._add_optional,
-        ]
+        return [self._add_type, self._add_default_value, self._add_max, self._add_min, self._add_optional]
 
 
 @dataclass
 class DynamicTextInput(Component):
     title: str = ""
     description: str = ""
     value_key: str = ""
@@ -341,19 +307,15 @@
         doc["props"]["maxRunResults"] = self.max_run_results
         if "max_run_results" in doc:
             doc.pop("max_run_results")
         return doc
 
     @property
     def hooks(self):
-        return [
-            self._add_aggregation_query,
-            self._add_aggregation_result_field,
-            self._add_max_run_results,
-        ]
+        return [self._add_aggregation_query, self._add_aggregation_result_field, self._add_max_run_results]
 
 
 @dataclass
 class AggregateSelector(Component):
     title: str = "Add some tags"
     description: str = "Here's where you can add some tags."
     type: str = "aggregateSelector"
@@ -409,55 +371,37 @@
     description: str = "Do not include spaces or capital letters or full stops."
     value_key: str = "dataset_input"
     type: str = "datasetNameInput"
 
 
 @dataclass
 class EmailDropdown(Component):
-    title: str = (
-        "Do you want to receive an notification email when the workflow is completed?"
-    )
+    title: str = "Do you want to receive an notification email when the workflow is completed?"
     description: str = "If you choose yes, then we will send you an email when the workflow is successfully completed."
     value_key: str = "send_email"
     type: str = "baseDropdown"
     props: dict = field(
         default_factory=lambda: {
-            "options": [
-                {
-                    "label": "Yes",
-                    "value": True,
-                },
-                {
-                    "label": "No",
-                    "value": False,
-                },
-            ],
+            "options": [{"label": "Yes", "value": True}, {"label": "No", "value": False}],
             "multiple": False,
             "optional": True,
             "value": True,
         }
     )
 
 
 @dataclass
 class RefreshComponent(Component):
     title: str = "Do you want to refresh?"
-    description: str = "If you choose False, then we will run it on new rows only. If True, we will run it on the whole dataset."
+    description: str = (
+        "If you choose False, then we will run it on new rows only. If True, we will run it on the whole dataset."
+    )
     value_key: str = "refresh"
     type: str = "baseDropdown"
     props: dict = field(
         default_factory=lambda: {
-            "options": [
-                {
-                    "label": "Yes",
-                    "value": True,
-                },
-                {
-                    "label": "No",
-                    "value": False,
-                },
-            ],
+            "options": [{"label": "Yes", "value": True}, {"label": "No", "value": False}],
             "multiple": False,
             "optional": True,
             "value": False,
         }
     )
```

### Comparing `ai_transform-0.30.4/ai_transform/config.py` & `ai_transform-0.30.5/ai_transform/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,22 @@
 
         result = SentimentConfig.to_schema()
 
     """
 
     authorizationToken: str = None
     dataset_id: Optional[str] = None
-    job_id: Optional[str] = Field(
-        default_factory=generate_random_string, description="the job ID"
-    )
+    job_id: Optional[str] = Field(default_factory=generate_random_string, description="the job ID")
     total_workers: Optional[int] = Field(default=None, description="Total workers.")
     send_email: Optional[bool] = Field(
-        default=True,
-        description="If True, sends an email upon completion. Otherwise, False.",
-    )
-    additional_information: Optional[str] = Field(
-        default="", description="What to include in the e-mail."
+        default=True, description="If True, sends an email upon completion. Otherwise, False."
     )
+    additional_information: Optional[str] = Field(default="", description="What to include in the e-mail.")
     filters: Optional[list] = Field(default=[], description="Filters to apply.")
-    documents: Optional[list] = Field(
-        default=None,
-        description="You can submit documents and have it run immediately.",
-    )
+    documents: Optional[list] = Field(default=None, description="You can submit documents and have it run immediately.")
 
     @classmethod
     def to_schema(self):
         return self.schema_json()
 
     def read_from_argparser(self, argparser: argparse.ArgumentParser):
         # Enables behavior such
@@ -98,29 +90,22 @@
     """
     Same as BaseConfig but a few more additional attributes.
     This is suitable for basic transformations that go through
     the same pulling, transforming and then pushing (e.g. sentiment or emotion workflows)
     """
 
     pull_chunksize: Optional[int] = Field(
-        default=1000,
-        description="How many do you want to download and upload to the server.",
-    )
-    transform_chunksize: Optional[int] = Field(
-        default=20, description="How many do you want to transform each time?"
-    )
-    refresh: Optional[bool] = Field(
-        default=False,
-        description="If True, re-runs the workflow on the entire dataset.",
+        default=1000, description="How many do you want to download and upload to the server."
     )
+    transform_chunksize: Optional[int] = Field(default=20, description="How many do you want to transform each time?")
+    refresh: Optional[bool] = Field(default=False, description="If True, re-runs the workflow on the entire dataset.")
     output_to_status: Optional[bool] = Field(
         default=False, description="If True, it will output results to status object."
     )
     documents: Optional[List[object]] = Field(
-        default_factory=lambda: [],
-        description="If passed in, documents will be used instead of dataset.",
+        default_factory=lambda: [], description="If passed in, documents will be used instead of dataset."
     )
     limit_documents: Optional[int] = Field(
         default=None,
         description="If passed in, the transform will be limited to the number of documents specified here",
     )
     webhook_url: str = None
```

### Comparing `ai_transform-0.30.4/ai_transform/dataset/dataset.py` & `ai_transform-0.30.5/ai_transform/dataset/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from json import JSONDecodeError
 from typing import Any, Dict, List, Optional, Union
 
 from ai_transform.api.api import API
 from ai_transform.api.helpers import process_token
 from ai_transform.types import Filter, Schema, GroupBy, Metric
 from ai_transform.errors import MaxRetriesError
-from ai_transform.dataset.field import (
-    Field,
-    KeyphraseField,
-    ClusterField,
-)
+from ai_transform.dataset.field import Field, KeyphraseField, ClusterField
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 from concurrent.futures import ThreadPoolExecutor
 
 
 logging.basicConfig(level=logging.DEBUG)
@@ -38,18 +34,15 @@
 
     @property
     def token(self):
         return self.api.credentials.token
 
     def __getitem__(self, index: str) -> Field:
         if isinstance(index, str):
-            if (
-                index.startswith(("_cluster_", "_cluster_otm_"))
-                or "_cluster_id_" in index
-            ):
+            if index.startswith(("_cluster_", "_cluster_otm_")) or "_cluster_id_" in index:
                 return ClusterField(dataset=self, field=index)
             elif "_keyphrase_" in index:
                 return KeyphraseField(dataset=self, field=index)
             else:
                 return Field(dataset=self, field=index)
         else:
             raise NotImplementedError("index must of type `str` (field in dataset)")
@@ -71,55 +64,39 @@
     def create(self):
         return self.api._create_dataset(self._dataset_id)
 
     def delete(self):
         return self.api._delete_dataset(self._dataset_id)
 
     def bulk_insert(
-        self,
-        documents: Union[List[Document], DocumentList],
-        insert_chunksize: int = 20,
-        max_workers: int = 2,
-        **kwargs
+        self, documents: Union[List[Document], DocumentList], insert_chunksize: int = 20, max_workers: int = 2, **kwargs
     ):
         def chunk_documents_with_kwargs(documents):
             for i in range(len(documents) // insert_chunksize + 1):
-                yield {
-                    "documents": documents[
-                        i * insert_chunksize : (i + 1) * insert_chunksize
-                    ],
-                    **kwargs,
-                }
+                yield {"documents": documents[i * insert_chunksize : (i + 1) * insert_chunksize], **kwargs}
 
         results = {}
         with ThreadPoolExecutor(max_workers=max_workers) as executor:
-            futures = executor.map(
-                lambda kw: self.insert_documents(**kw),
-                chunk_documents_with_kwargs(documents),
-            )
+            futures = executor.map(lambda kw: self.insert_documents(**kw), chunk_documents_with_kwargs(documents))
 
         results = {"inserted": 0, "failed_documents": []}
         for result in futures:
             results["inserted"] += result["inserted"]
             results["failed_documents"] += result["failed_documents"]
 
         return results
 
-    def insert_documents(
-        self, documents: Union[List[Document], DocumentList], *args, **kwargs
-    ) -> Dict[str, Any]:
+    def insert_documents(self, documents: Union[List[Document], DocumentList], *args, **kwargs) -> Dict[str, Any]:
         if hasattr(documents, "to_json"):
             documents = documents.to_json()
         else:
             for index in range(len(documents)):
                 if hasattr(documents[index], "to_json"):
                     documents[index] = documents[index].to_json()
-        return self.api._bulk_insert(
-            dataset_id=self._dataset_id, documents=documents, *args, **kwargs
-        )
+        return self.api._bulk_insert(dataset_id=self._dataset_id, documents=documents, *args, **kwargs)
 
     def update_documents(
         self,
         documents: Union[List[Document], DocumentList],
         insert_date: bool = True,
         ingest_in_background: bool = True,
         update_schema: bool = True,
@@ -226,23 +203,18 @@
         res["documents"] = DocumentList(documents)
         return res
 
     def len(self, *args, **kwargs):
         """
         Get length of dataset, usually used with filters
         """
-        return self.api._get_where(
-            dataset_id=self._dataset_id, page_size=1, *args, **kwargs
-        )["count"]
+        return self.api._get_where(dataset_id=self._dataset_id, page_size=1, *args, **kwargs)["count"]
 
     def insert_metadata(self, metadata: Dict[str, Any]):
-        return self.api._update_dataset_metadata(
-            dataset_id=self._dataset_id,
-            metadata=metadata,
-        )
+        return self.api._update_dataset_metadata(dataset_id=self._dataset_id, metadata=metadata)
 
     def update_metadata(self, metadata: Dict[str, Any]):
         old_metadata: dict = self.get_metadata()["results"]
 
         def merge_dicts(dict1, dict2):
             """Recursively merges dict2 into dict1"""
             if not isinstance(dict1, dict) or not isinstance(dict2, dict):
@@ -251,53 +223,36 @@
                 if k in dict1:
                     dict1[k] = merge_dicts(dict1[k], dict2[k])
                 else:
                     dict1[k] = dict2[k]
             return dict1
 
         return self.api._update_dataset_metadata(
-            dataset_id=self._dataset_id,
-            metadata=merge_dicts(old_metadata, metadata),
+            dataset_id=self._dataset_id, metadata=merge_dicts(old_metadata, metadata)
         )
 
     def get_metadata(self) -> Dict[str, Any]:
         return self.api._get_metadata(dataset_id=self._dataset_id)
 
     def insert_local_medias(self, file_paths: List[str]) -> List[str]:
-        presigned_urls = self.api._get_file_upload_urls(
-            self.dataset_id,
-            files=file_paths,
-        )
+        presigned_urls = self.api._get_file_upload_urls(self.dataset_id, files=file_paths)
         urls = []
         for index, file_path in enumerate(file_paths):
             url = presigned_urls["files"][index]["url"]
             upload_url = presigned_urls["files"][index]["upload_url"]
             with open(file_path, "rb") as fn_byte:
                 media_content = bytes(fn_byte.read())
             urls.append(url)
-            response = self.api._upload_media(
-                presigned_url=upload_url,
-                media_content=media_content,
-            )
+            response = self.api._upload_media(presigned_url=upload_url, media_content=media_content)
             assert response.status_code == 200
         return urls
 
-    def facets(
-        self,
-        fields: List[str],
-        data_interval: str = "monthly",
-        page_size: int = 10000,
-        asc: bool = False,
-    ):
+    def facets(self, fields: List[str], data_interval: str = "monthly", page_size: int = 10000, asc: bool = False):
         return self.api._facets(
-            dataset_id=self.dataset_id,
-            fields=fields,
-            data_interval=data_interval,
-            page_size=page_size,
-            asc=asc,
+            dataset_id=self.dataset_id, fields=fields, data_interval=data_interval, page_size=page_size, asc=asc
         )
 
     def set_field_children(
         self,
         fieldchildren_id: str,
         field: str,
         field_children: List[str],
@@ -311,37 +266,22 @@
             field_children=field_children,
             metadata=metadata,
         )
         if recursive:
             parent_fields = self[field].list_field_parents()
             for parent_field in parent_fields:
                 self[parent_field].add_field_children(
-                    field_children=field_children,
-                    fieldchildren_id=fieldchildren_id,
-                    recursive=recursive,
+                    field_children=field_children, fieldchildren_id=fieldchildren_id, recursive=recursive
                 )
 
-    def list_field_children(
-        self,
-        page: int = 1,
-        page_size: int = 10000,
-        sort=None,
-    ):
-        return self.api._list_field_children(
-            dataset_id=self._dataset_id,
-            page=page,
-            page_size=page_size,
-            sort=sort,
-        )
+    def list_field_children(self, page: int = 1, page_size: int = 10000, sort=None):
+        return self.api._list_field_children(dataset_id=self._dataset_id, page=page, page_size=page_size, sort=sort)
 
     def delete_field_children(self, fieldchildren_id: str):
-        return self.api._delete_field_children(
-            dataset_id=self._dataset_id,
-            fieldchildren_id=fieldchildren_id,
-        )
+        return self.api._delete_field_children(dataset_id=self._dataset_id, fieldchildren_id=fieldchildren_id)
 
     def aggregate(
         self,
         page_size: str = 20,
         page: str = 1,
         asc: str = False,
         groupby: List[GroupBy] = None,
@@ -364,10 +304,8 @@
             filters=filters,
         )
 
     def get_settings(self):
         return self.api._get_dataset_settings(self.dataset_id)
 
     def update_settings(self, settings: Dict[str, Any]):
-        return self.api._upsert_dataset_settings(
-            dataset_id=self.dataset_id, settings=settings
-        )
+        return self.api._upsert_dataset_settings(dataset_id=self.dataset_id, settings=settings)
```

### Comparing `ai_transform-0.30.4/ai_transform/dataset/field.py` & `ai_transform-0.30.5/ai_transform/dataset/field.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,175 +73,80 @@
             filter_type = "date"
         elif self._dtype is None:
             filter_type = "ids"
         else:
             filter_type = "exact_match"
         return filter_type
 
-    def __eq__(
-        self,
-        other: Union[str, float, int, bool, None],
-        filter_type: Optional[str] = None,
-    ) -> Filter:
+    def __eq__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
         if filter_type is None:
             filter_type = self._filter_type
-        return [
-            {
-                "field": self._field,
-                "filter_type": filter_type,
-                "condition": "==",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": filter_type, "condition": "==", "condition_value": other}]
 
-    def __lt__(
-        self,
-        other: Union[str, float, int, bool, None],
-        filter_type: Optional[str] = None,
-    ) -> Filter:
+    def __lt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
         if filter_type is None:
             filter_type = self._filter_type
-        return [
-            {
-                "field": self._field,
-                "filter_type": filter_type,
-                "condition": "<",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": filter_type, "condition": "<", "condition_value": other}]
 
-    def __le__(
-        self,
-        other: Union[str, float, int, bool, None],
-        filter_type: Optional[str] = None,
-    ) -> Filter:
+    def __le__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
         if filter_type is None:
             filter_type = self._filter_type
-        return [
-            {
-                "field": self._field,
-                "filter_type": filter_type,
-                "condition": "<=",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": filter_type, "condition": "<=", "condition_value": other}]
 
-    def __gt__(
-        self,
-        other: Union[str, float, int, bool, None],
-        filter_type: Optional[str] = None,
-    ) -> Filter:
+    def __gt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
         if filter_type is None:
             filter_type = self._filter_type
-        return [
-            {
-                "field": self._field,
-                "filter_type": filter_type,
-                "condition": ">",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": filter_type, "condition": ">", "condition_value": other}]
 
-    def __ge__(
-        self,
-        other: Union[str, float, int, bool, None],
-        filter_type: Optional[str] = None,
-    ) -> Filter:
+    def __ge__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
         if filter_type is None:
             filter_type = self._filter_type
-        return [
-            {
-                "field": self._field,
-                "filter_type": filter_type,
-                "condition": ">=",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": filter_type, "condition": ">=", "condition_value": other}]
 
     def contains(self, other: str) -> Filter:
-        return [
-            {
-                "field": self._field,
-                "filter_type": "contains",
-                "condition": "==",
-                "condition_value": other,
-            }
-        ]
+        return [{"field": self._field, "filter_type": "contains", "condition": "==", "condition_value": other}]
 
     def exists(self) -> Filter:
         if "_chunk_" in self._field:
             count = self._field.count(".")
             if count:
                 parent_field = self._field.split(".")[0]
             else:
                 parent_field = self._field
 
-            return [
-                {
-                    "chunk": {
-                        "path": parent_field,
-                        "filters": [{"fieldExists": {"field": self._field}}],
-                    }
-                }
-            ]
-        return [
-            {
-                "field": self._field,
-                "filter_type": "exists",
-                "condition": "==",
-                "condition_value": " ",
-            }
-        ]
+            return [{"chunk": {"path": parent_field, "filters": [{"fieldExists": {"field": self._field}}]}}]
+        return [{"field": self._field, "filter_type": "exists", "condition": "==", "condition_value": " "}]
 
     def not_exists(self) -> Filter:
-        return [
-            {
-                "field": self._field,
-                "filter_type": "exists",
-                "condition": "!=",
-                "condition_value": " ",
-            }
-        ]
+        return [{"field": self._field, "filter_type": "exists", "condition": "!=", "condition_value": " "}]
 
     def insert_centroids(self, centroid_documents: DocumentList):
-        raise NotImplementedError(
-            f"`insert_centroids` not available for non-vector fields"
-        )
+        raise NotImplementedError(f"`insert_centroids` not available for non-vector fields")
 
     def label_openai(
         self,
         field: str,
         question_suffix: str,
         accuracy: int = 4,
         cluster_ids: list = None,
         dont_save_summaries: bool = True,
         filters: list = None,
     ):
         raise NotImplementedError(f"`label_openai` not available for non-vector fields")
 
     def get_centroids(
-        self,
-        page_size: int = 5,
-        page: int = 1,
-        cluster_ids: Optional[List] = None,
-        include_vector: bool = False,
+        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
     ):
-        raise NotImplementedError(
-            f"`get_centroids` not available for non-vector fields"
-        )
+        raise NotImplementedError(f"`get_centroids` not available for non-vector fields")
 
     def get_all_centroids(self):
-        raise NotImplementedError(
-            f"`get_all_centroids` not available for non-vector fields"
-        )
+        raise NotImplementedError(f"`get_all_centroids` not available for non-vector fields")
 
     def create_centroid_documents(self):
-        raise NotImplementedError(
-            f"`create_centroid_documents` not available for non-vector fields"
-        )
+        raise NotImplementedError(f"`create_centroid_documents` not available for non-vector fields")
 
     def list_closest_to_center(
         self,
         centroid_vector_fields: List[str],
         cluster_field: str,
         approx: int = 0,
         sum_fields: bool = True,
@@ -253,97 +158,74 @@
         include_relevance: bool = False,
         page_size: int = 20,
         cluster_properties_filter: Dict[str, Any] = None,
         cluster_ids: List[str] = None,
         filters: List[Filter] = None,
         select_fields: List[str] = None,
     ):
-        raise NotImplementedError(
-            "`list_closest_to_center` not available for non-vector fields"
-        )
+        raise NotImplementedError("`list_closest_to_center` not available for non-vector fields")
 
     def get_keyphrase(self, keyphrase_id: str):
-        raise NotImplementedError(
-            f"`get_keyphrase` not available for non-keyphrase fields"
-        )
+        raise NotImplementedError(f"`get_keyphrase` not available for non-keyphrase fields")
 
     def update_keyphrase(
         self,
         keyphrase_id: str,
         alias: str,
         keyphrase: str,
         frequency: int = 0,
         ancestors: list = None,
         parents: list = None,
         metadata: dict = None,
         keyphrase_score: float = 0,
         level: int = 0,
     ):
-        raise NotImplementedError(
-            f"`update_keyphrase` not available for non-keyphrase fields"
-        )
+        raise NotImplementedError(f"`update_keyphrase` not available for non-keyphrase fields")
 
     def delete_keyphrase(self, keyphrase_id: str):
-        raise NotImplementedError(
-            f"`delete_keyphrase` not available for non-keyphrase fields"
-        )
+        raise NotImplementedError(f"`delete_keyphrase` not available for non-keyphrase fields")
 
     def bulk_update_keyphrases(self, updates: List[Union[Keyphrase, dict]]):
-        raise NotImplementedError(
-            f"`bulk_update_keyphrases` not available for non-keyphrase fields"
-        )
+        raise NotImplementedError(f"`bulk_update_keyphrases` not available for non-keyphrase fields")
 
     def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
-        raise NotImplementedError(
-            f"`list_keyphrases` not available for non-keyphrase fields"
-        )
+        raise NotImplementedError(f"`list_keyphrases` not available for non-keyphrase fields")
 
 
 class ClusterField(Field):
     def __init__(self, dataset, field: str):
         super().__init__(dataset=dataset, field=field)
         _, *middle_fields, alias = field.split(".")
         self._cluster_field = ".".join(middle_fields)
         self._cluster_alias = alias
 
-    def insert_centroids(
-        self, centroid_documents: Union[List[Dict[str, Any]], DocumentList]
-    ):
+    def insert_centroids(self, centroid_documents: Union[List[Dict[str, Any]], DocumentList]):
         if isinstance(centroid_documents, DocumentList):
             centroid_documents = centroid_documents.to_json()
         return self._dataset.api._insert_centroids(
             dataset_id=self.dataset_id,
             cluster_centers=centroid_documents,
             vector_fields=[self._cluster_field],
             alias=self._cluster_alias,
         )
 
     def get_centroids(
-        self,
-        page_size: int = 5,
-        page: int = 1,
-        cluster_ids: Optional[List] = None,
-        include_vector: bool = False,
+        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
     ):
         return self._dataset.api._get_centroids(
             dataset_id=self.dataset_id,
             vector_fields=[self._cluster_field],
             alias=self._cluster_alias,
             page_size=page_size,
             page=page,
             cluster_ids=cluster_ids,
             include_vector=include_vector,
         )
 
-    def get_all_centroids(
-        self,
-        page_size: int = 5,
-        cluster_ids: Optional[List] = None,
-        include_vector: bool = False,
-    ):
+    def get_all_centroids(self, page_size: int = 5, cluster_ids: Optional[List] = None, include_vector: bool = False):
         """
         Get all centroids and returns as a dictionary for easy access
         """
         all_centroids = {"results": []}
         page = 1
         while True:
             res = self._dataset.api._get_centroids(
@@ -381,17 +263,15 @@
             cluster_ids=cluster_ids if cluster_ids is not None else [],
             dont_save_summaries=dont_save_summaries,
             filters=filters if filters is not None else [],
         )
 
     def create_centroid_documents(self):
 
-        documents = self._dataset.get_all_documents(
-            select_fields=[self._cluster_field, self._field]
-        )
+        documents = self._dataset.get_all_documents(select_fields=[self._cluster_field, self._field])
         documents = documents["documents"]
 
         vectors = np.array([document[self._cluster_field] for document in documents])
 
         labels = [document[self._field] for document in documents]
 
         label_map = {}
@@ -407,18 +287,15 @@
 
         label_indices = np.array([label_map[label] for label in labels])
 
         for index in range(n_clusters):
             selected_vectors = vectors[label_indices == index]
             centroid_vector = selected_vectors.mean(0)
 
-            centroid_document = {
-                "_id": f"cluster_{index}",
-                f"{self._cluster_field}": centroid_vector.tolist(),
-            }
+            centroid_document = {"_id": f"cluster_{index}", f"{self._cluster_field}": centroid_vector.tolist()}
             centroid_documents.append(centroid_document)
 
         return centroid_documents
 
     def list_closest_to_center(
         self,
         centroid_vector_fields: List[str] = None,
@@ -513,18 +390,15 @@
         updates_list = []
         for update in updates:
             if isinstance(update, Keyphrase):
                 updates_list.append(asdict(update))
             elif isinstance(update, dict):
                 updates_list.append(update)
         return self._dataset.api._bulk_update_keyphrase(
-            dataset_id=self.dataset_id,
-            field=self._keyphrase_field,
-            alias=self._keyphrase_alias,
-            updates=updates_list,
+            dataset_id=self.dataset_id, field=self._keyphrase_field, alias=self._keyphrase_alias, updates=updates_list
         )
 
     def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
         return self._dataset.api._list_keyphrase(
             dataset_id=self.dataset_id,
             field=self._keyphrase_field,
             alias=self._keyphrase_alias,
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.5/ai_transform/engine/abstract_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 from ai_transform.operator.abstract_operator import AbstractOperator
 
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 from ai_transform.errors import MaxRetriesError
 
-logging.basicConfig(
-    level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s"
-)
+logging.basicConfig(level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 logger = logging.getLogger(__name__)
 
 
 class AbstractEngine(ABC):
     MAX_SCHEMA_UPDATE_LIMITER: int = 1
 
     def __init__(
@@ -48,17 +46,15 @@
             # We set this to a warning so that workflows that are adding
             # onto an existing field don't need this. For example - adding tags
             # to existing tags. If existing tags don't exist - it shouldn't break
             # the whole workflow. This allows for multiple workflows to be run in parallel
             # without worrying about breaking things.
             if check_for_missing_fields:
                 assert all(
-                    field in dataset.schema
-                    for field in select_fields
-                    if field not in {"_id", "insert_date_"}
+                    field in dataset.schema for field in select_fields if field not in {"_id", "insert_date_"}
                 ), f"Some fields not in dataset schema - namely {select_fields}. If this is not desired behavior, set check_for_missing_fields=False."
             else:
                 for field in select_fields:
                     if field not in ["_id", "insert_date_"]:
                         if field not in dataset.schema:
                             warnings.warn(f"Not all fields were found. Missing {field}")
 
@@ -83,24 +79,19 @@
 
         self._limit_documents = limit_documents
 
         if isinstance(pull_chunksize, int):
             assert pull_chunksize > 0, "Chunksize should be a Positive Integer"
             self._pull_chunksize = pull_chunksize
         else:
-            warnings.warn(
-                f"`chunksize=None` assumes the operation transforms on the entire dataset at once"
-            )
+            warnings.warn(f"`chunksize=None` assumes the operation transforms on the entire dataset at once")
             self._pull_chunksize = self._size
 
         # If limiting documents, make sure pull chunk size is not larger than document count
-        if (
-            self._limit_documents is not None
-            and self._limit_documents < self._pull_chunksize
-        ):
+        if self._limit_documents is not None and self._limit_documents < self._pull_chunksize:
             self._pull_chunksize = self.limit_documents
 
         self._output_to_status = output_to_status  # Whether we should output_to_status
         self._output_documents = []  # document store for output
 
         # Empty unless documents passed into run on instead of dataset
         self._documents = DocumentList(documents)
@@ -113,29 +104,23 @@
             self._operators = [operator]
         else:
             self._operator = None
             self._operators = operators
 
         if filters is None:
             filters = []
-        assert isinstance(
-            filters, list
-        ), "Filters must be applied as a list of Dictionaries"
+        assert isinstance(filters, list), "Filters must be applied as a list of Dictionaries"
 
         if not refresh:
             filters += self._get_refresh_filter(select_fields, dataset)
         filters += self._get_workflow_filter()
 
         self._filters = filters
 
-        self._size = (
-            dataset.len(filters=filters)
-            if self._limit_documents is None
-            else self._limit_documents
-        )
+        self._size = dataset.len(filters=filters) if self._limit_documents is None else self._limit_documents
 
         self._refresh = refresh
         self._after_id = after_id
 
         self._successful_documents = 0
         self._success_ratio = None
 
@@ -208,51 +193,41 @@
 
     def _operate(self, mini_batch):
         try:
             # note: do not put an IF inside ths try-except-else loop - the if code will not work
             transformed_batch = self.operator(mini_batch)
         except Exception as e:
             logger.exception(e)
-            logger.error(
-                format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)})
-            )
+            logger.error(format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)}))
         else:
             # if there is no exception then this block will be executed
             # we only update schema on the first chunk
             # otherwise it breaks down how the backend handles
             # schema updates
             self._successful_documents += len(mini_batch)
             return transformed_batch
 
     def _get_refresh_filter(self, select_fields: List[str], dataset: Dataset):
         # initialize the refresh filter container
-        refresh_filters = {
-            "filter_type": "or",
-            "condition_value": [],
-        }
+        refresh_filters = {"filter_type": "or", "condition_value": []}
 
         # initialize where the filters are going
         input_field_filters = []
-        output_field_filters = {
-            "filter_type": "or",
-            "condition_value": [],
-        }
+        output_field_filters = {"filter_type": "or", "condition_value": []}
 
         # We want documents where all select_fields exists
         # as these are needed for operator ...
         for field in select_fields:
             input_field_filters += dataset[field].exists()
 
         # ... and where any of its output_fields dont exist
         for operator in self.operators:
             if operator.output_fields is not None:
                 for output_field in operator.output_fields:
-                    output_field_filters["condition_value"] += dataset[
-                        output_field
-                    ].not_exists()
+                    output_field_filters["condition_value"] += dataset[output_field].not_exists()
 
         # We construct this as:
         #
         #   input_field1 and input_field2 and (not output_field1 or not output_field2)
         #
         # This use case here is for two input fields and two output fields
         # tho this extends to arbitrarily many.
@@ -264,34 +239,24 @@
 
     def _get_workflow_filter(self, field: str = "_id"):
         # Get the required workflow filter as an environment variable
         # WORKER_NUMBER is passed into execute function
         # total number of workers must be greater than 1 for data sharding to work
         if self.worker_number is not None and self.total_workers is not None:
             if self.total_workers > 1:
-                return [
-                    {
-                        "matchModulo": {
-                            "field": field,
-                            "modulo": self.total_workers,
-                            "value": self.worker_number,
-                        }
-                    }
-                ]
+                return [{"matchModulo": {"field": field, "modulo": self.total_workers, "value": self.worker_number}}]
         return []
 
     def get_iterator(self) -> Iterator:
         if self.documents is None or len(self.documents) == 0:
             # Iterate through dataset
             iterator = self.iterate()
         else:
             # Iterate through passed in documents
-            iterator = self.chunk_documents(
-                chunksize=min(100, len(self.documents)), documents=self.documents
-            )
+            iterator = self.chunk_documents(chunksize=min(100, len(self.documents)), documents=self.documents)
         return iterator
 
     def iterate(
         self,
         filters: Optional[List[Filter]] = None,
         select_fields: Optional[List[str]] = None,
         max_retries: int = 5,
@@ -310,18 +275,15 @@
 
         retry_count = 0
         documents_processed = 0
 
         while True:
             try:
                 # Adjust chunksize to get correct amount of documents
-                if (
-                    self.limit_documents is None
-                    or documents_processed + self.pull_chunksize < self.limit_documents
-                ):
+                if self.limit_documents is None or documents_processed + self.pull_chunksize < self.limit_documents:
                     pull_chunksize = self._pull_chunksize
                 else:
                     pull_chunksize = self.limit_documents - documents_processed
 
                 chunk = self._dataset.get_documents(
                     page_size=pull_chunksize,
                     filters=filters,
@@ -349,18 +311,15 @@
                 documents = self._filter_for_non_empty_list(documents)
                 if documents:
                     yield documents
 
                 retry_count = 0
                 # If document limit is hit, break the loop
                 documents_processed += chunk["count"]
-                if (
-                    self.limit_documents is not None
-                    and documents_processed >= self.limit_documents
-                ):
+                if self.limit_documents is not None and documents_processed >= self.limit_documents:
                     break
 
     @staticmethod
     def chunk_documents(chunksize: int, documents: List[Document]):
         num_chunks = len(documents) // chunksize + 1
         for i in range(num_chunks):
             start = i * chunksize
@@ -376,17 +335,15 @@
         ingest_in_background: bool = True,
         update_schema: bool = False,
     ):
         if chunk:
             for _ in range(max_retries):
                 try:
                     update_json = self._dataset.update_documents(
-                        documents=chunk,
-                        ingest_in_background=ingest_in_background,
-                        update_schema=update_schema,
+                        documents=chunk, ingest_in_background=ingest_in_background, update_schema=update_schema
                     )
                 except Exception as e:
                     logger.exception(e)
                 else:
                     return update_json
 
             raise MaxRetriesError("max number of retries exceeded")
@@ -403,37 +360,26 @@
         assert pass_index >= 0, "`pass_index` must be strictly positive"
 
         if n_total is None:
             n_total = self.size
 
         total = n_total * n_passes
         inital_value = pass_index * n_total
-        self.update_progress(
-            n_processed=inital_value,
-            n_total=total,
-        )
+        self.update_progress(n_processed=inital_value, n_total=total)
 
         desc = " -> ".join([repr(operator) for operator in self.operators])
 
-        tqdm_bar = tqdm(
-            range(total),
-            desc=desc,
-            disable=(not show_progress_bar),
-            total=total,
-        )
+        tqdm_bar = tqdm(range(total), desc=desc, disable=(not show_progress_bar), total=total)
         tqdm_bar.update(inital_value)
 
         total_so_far = 0
         for batch in iterator:
             yield batch
             api_n_processed = total_so_far + len(batch) + pass_index * n_total
-            self.update_progress(
-                n_processed=api_n_processed,
-                n_total=total,
-            )
+            self.update_progress(n_processed=api_n_processed, n_total=total)
             total_so_far += len(batch)
             tqdm_bar.update(len(batch))
 
     def update_progress(self, n_processed: int, n_total: int = None):
         """
         n_process: int
             the number of documents that have been processed:
@@ -452,32 +398,27 @@
                 n_processed=n_processed,
                 n_total=n_total,
             )
 
     def update_engine_props(self, job_id: str, workflow_name: str):
         self._job_id = job_id
         self._workflow_name = workflow_name
-        self.dataset.api.headers.update(
-            ai_transform_job_id=job_id,
-            ai_transform_name=workflow_name,
-        )
+        self.dataset.api.headers.update(ai_transform_job_id=job_id, ai_transform_name=workflow_name)
 
     def set_success_ratio(self) -> None:
         if self.size:
             denominator = self.size * len(self.operators)
             self._success_ratio = self._successful_documents / denominator
         else:
             self._success_ratio = 1
         logger.debug(format_logging_info({"success_ratio": self._success_ratio}))
 
     @staticmethod
     def _filter_for_non_empty_list(documents: List[Document]) -> List[Document]:
         # if there are more keys than just _id in each document
         # then return that as a list of Documents
         # length of a dictionary is just 1 if there is only 1 key
-        return DocumentList(
-            [document for document in documents if len(document.keys()) > 1]
-        )
+        return DocumentList([document for document in documents if len(document.keys()) > 1])
 
     @staticmethod
     def _get_chunks_ids(documents: List[Document]) -> List[Document]:
         return [document["_id"] for document in documents]
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.5/ai_transform/engine/dense_output_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,22 @@
         iterator = self.get_iterator()
 
         output_dataset_ids = []
 
         self.operator.pre_hooks(self._dataset)
 
         for mega_batch in self.api_progress(iterator):
-            for mini_batch in AbstractEngine.chunk_documents(
-                self._transform_chunksize, mega_batch
-            ):
+            for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
                 document_mapping = self._operate(mini_batch)
                 for dataset_id, documents in document_mapping.items():
                     output_dataset_ids.append(dataset_id)
                     dataset = Dataset.from_details(dataset_id, self.token)
                     result = dataset.bulk_insert(documents)
                     logger.debug({"dataset_id": dataset_id, "result": result})
 
         self.operator.post_hooks(self._dataset)
 
         output_datasets = self.datasets_from_ids(output_dataset_ids)
         self.operator.store_dataset_relationship(self.dataset, output_datasets)
 
     def datasets_from_ids(self, dataset_ids: Sequence[str]) -> Sequence[Dataset]:
-        return [
-            Dataset.from_details(dataset_id, self.token) for dataset_id in dataset_ids
-        ]
+        return [Dataset.from_details(dataset_id, self.token) for dataset_id in dataset_ids]
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.5/ai_transform/engine/in_memory_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
             documents += batch
 
         documents_to_insert = self._operate(documents)
 
         # Update this in series
         for batch_index, batch in enumerate(
             self.api_progress(
-                AbstractEngine.chunk_documents(
-                    self.pull_chunksize, documents_to_insert
-                ),
+                AbstractEngine.chunk_documents(self.pull_chunksize, documents_to_insert),
                 show_progress_bar=self._show_progress_bar,
             )
         ):
             if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
                 update_schema = True
             else:
                 update_schema = False
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.5/ai_transform/engine/multipass_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         This functions handles the reinsertion of new transformed data back
         into the dataset. This could happen for two reasons:
             1. For a regular workflow
             2. For outputting to status
         """
         if self.output_to_status:
             # Store in output documents
-            self.extend_output_documents(
-                [document.to_json() for document in batch_to_insert]
-            )
+            self.extend_output_documents([document.to_json() for document in batch_to_insert])
         else:
             # Store in dataset
             # We want to make sure the schema updates
             # on the first chunk upserting
             if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
                 ingest_in_background = False
             else:
@@ -80,17 +78,15 @@
 
     def _operate(self, operator: AbstractOperator, mini_batch: List[Document]):
         try:
             # note: do not put an IF inside ths try-except-else loop - the if code will not work
             transformed_batch = operator(mini_batch)
         except Exception as e:
             logger.exception(e)
-            logger.error(
-                format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)})
-            )
+            logger.error(format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)}))
         else:
             # if there is no exception then this block will be executed
             # we only update schema on the first chunk
             # otherwise it breaks down how the backend handles
             # schema updates
             self._successful_documents += len(mini_batch)
             return transformed_batch
@@ -101,25 +97,19 @@
         """
         for operator_index, operator in enumerate(self.operators):
             operator.pre_hooks(self._dataset)
 
             iterator = self.get_iterator()
 
             for batch_index, mega_batch in enumerate(
-                self.api_progress(
-                    iterator,
-                    pass_index=operator_index,
-                    n_passes=len(self.operators),
-                )
+                self.api_progress(iterator, pass_index=operator_index, n_passes=len(self.operators))
             ):
                 batch_to_insert: List[Document] = []
 
-                for mini_batch in AbstractEngine.chunk_documents(
-                    self._transform_chunksize, mega_batch
-                ):
+                for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
                     transformed_batch = self._operate(operator, mini_batch)
                     if transformed_batch is not None:
                         batch_to_insert += transformed_batch
 
                 if batch_to_insert:
                     self.handle_upsert(batch_index, batch_to_insert)
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.5/ai_transform/engine/small_batch_stable_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,17 @@
         self,
         dataset: Dataset,
         operator: AbstractOperator,
         pull_chunksize: int = 5,
         transform_threshold: int = 1000,
         transform_chunksize: int = 20,
         *args,
-        **kwargs
+        **kwargs,
     ):
-        super().__init__(
-            dataset=dataset,
-            operator=operator,
-            pull_chunksize=pull_chunksize,
-            *args,
-            **kwargs
-        )
+        super().__init__(dataset=dataset, operator=operator, pull_chunksize=pull_chunksize, *args, **kwargs)
 
         self._transform_threshold = transform_threshold
         self._transform_chunksize = transform_chunksize
 
         self._show_progress_bar = kwargs.pop("show_progress_bar", True)
 
     def _filter_for_non_empty_list(self, docs: DocumentList):
@@ -88,18 +82,15 @@
         iterator = self.iterate()
 
         batch = []
 
         self.operator.pre_hooks(self.dataset)
 
         upload_index = 0
-        for minibatch in self.api_progress(
-            iterator,
-            show_progress_bar=self._show_progress_bar,
-        ):
+        for minibatch in self.api_progress(iterator, show_progress_bar=self._show_progress_bar):
             batch += minibatch
 
             if len(batch) >= self._transform_threshold:
                 self._transform_and_upsert(upload_index, batch)
                 upload_index += 1
                 batch = []
```

### Comparing `ai_transform-0.30.4/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.5/ai_transform/engine/stable_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 
         self._transform_chunksize = min(self.pull_chunksize, transform_chunksize)
         self._show_progress_bar = show_progress_bar
 
     def handle_upsert(self, batch_index: int, batch_to_insert: List[Document]):
         if self.output_to_status:
             # Store in output documents
-            self.extend_output_documents(
-                [document.to_json() for document in batch_to_insert]
-            )
+            self.extend_output_documents([document.to_json() for document in batch_to_insert])
         else:
             # Store in dataset
             # We want to make sure the schema updates
             # on the first chunk upserting
             if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
                 ingest_in_background = False
             else:
@@ -89,17 +87,15 @@
         """
         iterator = self.get_iterator()
 
         self.operator.pre_hooks(self._dataset)
         for batch_index, mega_batch in enumerate(self.api_progress(iterator)):
             batch_to_insert: List[Document] = []
 
-            for mini_batch in AbstractEngine.chunk_documents(
-                self._transform_chunksize, mega_batch
-            ):
+            for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
                 transformed_batch = self._operate(mini_batch)
                 if transformed_batch is not None:
                     batch_to_insert += transformed_batch
 
             self.handle_upsert(batch_index, batch_to_insert)
 
         self.operator.post_hooks(self._dataset)
```

### Comparing `ai_transform-0.30.4/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.5/ai_transform/operator/abstract_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,19 @@
 def is_different(field: str, value1: Any, value2: Any) -> bool:
     """
     An all purpose function that checks if two values are different
     """
     # TODO: Implement a better fix for chunks - but this will do for now
     if isinstance(value1, list) and isinstance(value2, list):
         return any(
-            is_different(field, chunk1_value, chunk2_value)
-            for chunk1_value, chunk2_value in zip(value1, value2)
+            is_different(field, chunk1_value, chunk2_value) for chunk1_value, chunk2_value in zip(value1, value2)
         )
 
     # check if its a vector field but only if it ends with it
-    elif (
-        field.endswith(("_vector_", "_chunkvector_"))
-        and isinstance(value1, list)
-        and isinstance(value2, list)
-    ):
+    elif field.endswith(("_vector_", "_chunkvector_")) and isinstance(value1, list) and isinstance(value2, list):
         return are_vectors_similar(value1, value2)
 
     elif isinstance(value1, dict) and isinstance(value2, dict):
         return json.dumps(value1, sort_keys=True) != json.dumps(value2, sort_keys=True)
 
     else:
         return value1 != value2
@@ -79,38 +74,28 @@
         input_fields: Optional[List[str]] = None,
         output_fields: Optional[Union[Dict[str, str], List[str]]] = None,
         enable_postprocess: Optional[bool] = True,
     ):
 
         if input_fields is not None and output_fields is not None:
             if any(input_field in output_fields for input_field in input_fields):
-                detected_fields = [
-                    input_field
-                    for input_field in input_fields
-                    if input_field in output_fields
-                ]
-                warnings.warn(
-                    f"Some input fields are present in the output fields, namely {str(detected_fields)}"
-                )
+                detected_fields = [input_field for input_field in input_fields if input_field in output_fields]
+                warnings.warn(f"Some input fields are present in the output fields, namely {str(detected_fields)}")
                 for field in detected_fields:
                     output_fields.remove(field)
 
         if input_fields is not None:
-            assert isinstance(
-                input_fields, list
-            ), "`input_fields` must be of type list or dict"
+            assert isinstance(input_fields, list), "`input_fields` must be of type list or dict"
             for field_index, input_field in enumerate(input_fields):
                 assert isinstance(
                     input_field, str
                 ), f"input_field at index {field_index} of `input_fields` is not of type string"
 
         if output_fields is not None:
-            assert isinstance(
-                output_fields, list
-            ), "`output_fields`  must be of type list or dict"
+            assert isinstance(output_fields, list), "`output_fields`  must be of type list or dict"
             for field_index, output_field in enumerate(output_fields):
                 assert isinstance(
                     output_field, str
                 ), f"output_field at index {field_index} of `output_fields` is not of type string"
 
         self._input_fields = input_fields
         self._output_fields = output_fields
```

### Comparing `ai_transform-0.30.4/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.5/ai_transform/operator/dense_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,30 @@
 logger = logging.getLogger(__file__)
 
 
 DatasetID = str
 DenseOperatorOutput = Dict[DatasetID, Sequence[Document]]
 
 
-BAD_OPERATOR_MESSAGE = "please ensure the output of the operator is a dict that is a mapping of dataset_ids to documents"
+BAD_OPERATOR_MESSAGE = (
+    "please ensure the output of the operator is a dict that is a mapping of dataset_ids to documents"
+)
 
 
 class DenseOperator(AbstractOperator):
     def __call__(self, old_documents: DocumentList) -> DenseOperatorOutput:
         datum = self.transform(old_documents)
         assert isinstance(datum, dict), BAD_OPERATOR_MESSAGE
         for _, documents in datum.items():
             assert isinstance(documents, Sequence)
         return datum
 
     @abstractmethod
     def transform(self, documents: DocumentList) -> DenseOperatorOutput:
         raise NotImplementedError
 
-    def store_dataset_relationship(
-        self, input_dataset: Dataset, output_datasets: Sequence[Dataset]
-    ):
+    def store_dataset_relationship(self, input_dataset: Dataset, output_datasets: Sequence[Dataset]):
         input_dataset.update_metadata(
-            {
-                "_child_datasets_": [
-                    output_dataset.dataset_id for output_dataset in output_datasets
-                ]
-            }
+            {"_child_datasets_": [output_dataset.dataset_id for output_dataset in output_datasets]}
         )
         for output_dataset in output_datasets:
-            output_dataset.update_metadata(
-                {"_parent_dataset_": input_dataset.dataset_id}
-            )
+            output_dataset.update_metadata({"_parent_dataset_": input_dataset.dataset_id})
```

### Comparing `ai_transform-0.30.4/ai_transform/timer.py` & `ai_transform-0.30.5/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/ai_transform/types.py` & `ai_transform-0.30.5/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/ai_transform/utils/document.py` & `ai_transform-0.30.5/ai_transform/utils/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,40 +148,29 @@
 
         document_list = DocumentList(self.get(chunk_field, default=default))
         # Get the field across chunks
         if field is None:
             return document_list
         return [d.get(field, default=default) for d in document_list.data]
 
-    def _create_chunk_documents(
-        self,
-        field: str,
-        values: list,
-        generate_id: bool = False,
-    ):
+    def _create_chunk_documents(self, field: str, values: list, generate_id: bool = False):
         """
         create chunk documents based on a given field and value.
         """
         from ai_transform.utils.document_list import DocumentList
 
         if generate_id:
-            docs = [
-                {"_id": uuid.uuid4().__str__(), field: values[i], "_order_": i}
-                for i in range(len(values))
-            ]
+            docs = [{"_id": uuid.uuid4().__str__(), field: values[i], "_order_": i} for i in range(len(values))]
         else:
             docs = [{field: values[i], "_order_": i} for i in range(len(values))]
         return DocumentList(docs)
 
     def _calculate_offset(self, text_to_find, string):
         try:
-            result = [
-                {"start": m.start(), "end": m.end()}
-                for m in re.finditer(text_to_find, string)
-            ]
+            result = [{"start": m.start(), "end": m.end()} for m in re.finditer(text_to_find, string)]
         except Exception as e:
             import traceback
 
             traceback.print_exc()
             # this is the error this exception aims to solve
             #     for m in re.finditer(text_to_find, string)
             #     return _compile(pattern, flags).finditer(string)
@@ -194,34 +183,24 @@
             # instead, we will use fuzzysearch
             from fuzzysearch import find_near_matches
 
             matches = find_near_matches(text_to_find, string, max_l_dist=2)
             result = [{"start": m.start, "end": m.end} for m in matches]
         return result
 
-    def set_chunk(
-        self,
-        chunk_field: str,
-        field: str,
-        values: list,
-        generate_id: bool = False,
-    ):
+    def set_chunk(self, chunk_field: str, field: str, values: list, generate_id: bool = False):
         """
         doc.list_chunks()
         doc.get_chunk("value_chunk_", field="sentence") # returns a list of values
         doc.set_chunk("value_chunk_", field="sentence", values=["hey", "test"])
         """
         # We use upsert behavior for now
         from ai_transform.utils.document_list import DocumentList
 
-        new_chunk_docs = self._create_chunk_documents(
-            field,
-            values=values,
-            generate_id=generate_id,
-        )
+        new_chunk_docs = self._create_chunk_documents(field, values=values, generate_id=generate_id)
         # Update on the old chunk docs
         old_chunk_docs = DocumentList(self.get(chunk_field))
         # Relying on immutable property
         [d.update(new_chunk_docs[i]) for i, d in enumerate(old_chunk_docs.data)]
 
     def split(
         self,
@@ -238,32 +217,25 @@
         The split operation returns to us a list of possible values.
         The chunk documents are then created automatically for you.
         """
         if default is None:
             default = []
         value = self.get(field, default)
         split_values = split_operation(value)
-        chunk_documents = self._create_chunk_documents(
-            field=field, values=split_values, generate_id=generate_id
-        )
+        chunk_documents = self._create_chunk_documents(field=field, values=split_values, generate_id=generate_id)
 
         if include_offsets:
             for i, d in enumerate(chunk_documents):
                 offsets = self._calculate_offset(d[field], value)
                 d["_offsets_"] = offsets
 
         self.set(chunk_field, chunk_documents)
 
     def operate_on_chunk(
-        self,
-        operator_function: callable,
-        chunk_field: str,
-        field: str,
-        output_field: str,
-        default: Any = None,
+        self, operator_function: callable, chunk_field: str, field: str, output_field: str, default: Any = None
     ):
         """
         Add an operate function.
         """
         values = self.get_chunk(chunk_field=chunk_field, field=field, default=default)
         results = operator_function(values)
         self.set_chunk(chunk_field=chunk_field, field=output_field, values=results)
```

### Comparing `ai_transform-0.30.4/ai_transform/utils/document_list.py` & `ai_transform-0.30.5/ai_transform/utils/document_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,15 @@
     def to_json(self):
         return [document.to_json() for document in self.data]
 
     def _flatten_list(self, list_of_lists):
         flat_list = itertools.chain(*list_of_lists)
         return list(flat_list)
 
-    def set_chunk_values(
-        self,
-        chunk_field: str,
-        output_field: str,
-        chunk_values: List[List[Any]],
-        sortby: str = None,
-    ):
+    def set_chunk_values(self, chunk_field: str, output_field: str, chunk_values: List[List[Any]], sortby: str = None):
         if sortby is None:
             if any("_order_" in key for key in self.data[0].keys()):
                 sortby = "_order_"
 
         assert len(chunk_values) == len(
             self.data
         ), "The length of your values array should be the same as your documents"
@@ -96,17 +90,15 @@
                 chunk_doc = Document(chunk_doc)
                 chunk_doc.set(field, values[chunk_counter])
                 chunk_docs.append(chunk_doc)
                 chunk_counter += 1
             doc.set(chunk_field, chunk_docs)
 
         if chunk_counter > len(values):
-            raise ValueError(
-                "Number of chunks do not match with number of values - check logic."
-            )
+            raise ValueError("Number of chunks do not match with number of values - check logic.")
 
     def get_chunks_as_flat(self, chunk_field: str, field: str, default=None):
         """
         Set chunks from a flat list.
         Note that this is only possible if there is pre-existing
         chunk documents.
         """
@@ -136,17 +128,15 @@
             old_tags = document.get(tag_field, [])
             for tag_json in old_tags:
                 if tag_json.get(remove_field) != value:
                     new_tags.append(tag_json)
 
             document[tag_field] = new_tags
 
-    def append_tag(
-        self, field: str, value: Union[Dict[str, Any], List[Dict[str, Any]]]
-    ) -> None:
+    def append_tag(self, field: str, value: Union[Dict[str, Any], List[Dict[str, Any]]]) -> None:
         warnings.warn("This behaviour is experimental and is subject to change")
 
         if isinstance(value, list):
             for document, tag in zip(self.data, value):
                 document[field].append(tag)
         else:
             for document in self.data:
@@ -159,11 +149,9 @@
         tag_field = ".".join(tag_fields)
 
         for document in self.data:
             tags = document.get(tag_field)
 
             if tags is not None:
                 document[tag_field] = sorted(
-                    document[tag_field],
-                    key=lambda tag_json: tag_json[sort_field],
-                    reverse=reverse,
+                    document[tag_field], key=lambda tag_json: tag_json[sort_field], reverse=reverse
                 )
```

### Comparing `ai_transform-0.30.4/ai_transform/utils/example_documents.py` & `ai_transform-0.30.5/ai_transform/utils/example_documents.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,15 @@
 def create_id():
     return str(uuid.uuid4())
 
 
 def generate_random_string(string_length: int = 5) -> str:
 
     """Generate a random string of letters and numbers"""
-    return "".join(
-        random.choice(string.ascii_uppercase + string.digits)
-        for _ in range(string_length)
-    )
+    return "".join(random.choice(string.ascii_uppercase + string.digits) for _ in range(string_length))
 
 
 def generate_random_vector(vector_length: int = 5) -> Vector:
     """Generate a random list of floats"""
     return [random.random() for _ in range(vector_length)]
 
 
@@ -84,20 +81,15 @@
         "sample_3_description": generate_random_string(),
         "sample_1_vector_": generate_random_vector(),
         "sample_2_vector_": generate_random_vector(),
         "sample_3_vector_": generate_random_vector(),
         "sample_1_value": generate_random_integer(),
         "sample_2_value": generate_random_integer(),
         "sample_3_value": generate_random_integer(),
-        "_chunk_": [
-            {
-                "label": generate_random_label(),
-                "label_chunkvector_": generate_random_vector(),
-            }
-        ],
+        "_chunk_": [{"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}],
     }
 
     return Document(document)
 
 
 def mock_documents(n: int = 100, vector_length: int = 5) -> DocumentList:
     return DocumentList([vector_document(vector_length) for _ in range(n)])
@@ -108,16 +100,15 @@
 
 
 def tag_document(n_tags: int = 5):
     document = {
         "text": "This is some random text",
         "_surveytag_": {
             "text": [
-                {"label": generate_random_label(), "value": random.random()}
-                for _ in range(random.randint(0, n_tags))
+                {"label": generate_random_label(), "value": random.random()} for _ in range(random.randint(0, n_tags))
             ]
         },
     }
     return Document(document)
 
 
 def tag_documents(n: int = 100):
```

### Comparing `ai_transform-0.30.4/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.5/ai_transform/utils/json_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,15 @@
 """
 import math
 import datetime
 import dataclasses
 import collections
 import pandas as pd
 
-from ipaddress import (
-    IPv4Address,
-    IPv4Interface,
-    IPv4Network,
-    IPv6Address,
-    IPv6Interface,
-    IPv6Network,
-)
+from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 
 from enum import Enum
 from types import GeneratorType
 from uuid import UUID
 from collections import deque
 from pathlib import Path
 from pathlib import PurePath
```

### Comparing `ai_transform-0.30.4/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.5/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.5/ai_transform/workflow/abstract_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         name: Optional[str] = "Workflow",
         metadata: Optional[Dict[str, Any]] = None,
         additional_information: str = "",
         send_email: bool = True,
         success_threshold: float = 0.8,
         email: dict = None,
         output: dict = None,
-        webhook_url: str = None,
         **kwargs,  # TODO: Update workflows, This for deprecated arguments
     ):
 
         if job_id is None:
             job_id = str(uuid.uuid4())
             warnings.warn(f"No job id supplied, using {job_id}")
 
@@ -43,20 +42,14 @@
         self._additional_information = additional_information
         self._send_email = send_email
 
         self._success_threshold = success_threshold
         self._email = email
         self._output = output
 
-        self._webhook_url = webhook_url
-
-    @property
-    def webhook_url(self):
-        return self._webhook_url
-
     @property
     def success_threshold(self):
         return self._success_threshold
 
     @property
     def name(self):
         return self._name
@@ -109,15 +102,14 @@
             email=self.email,
             success_threshold=self.success_threshold,
             operators=self.operators,
             metadata=self.metadata,
             engine=self.engine,
             dataset=self.dataset,
             output=self._output,
-            webhook_url=self._webhook_url,
         ):
             self.engine()
 
     def get_status(self):
         return self.api._get_workflow_status(self._job_id)
 
     def update_metadata(self, metadata: Dict[str, Any]):
```

### Comparing `ai_transform-0.30.4/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.5/ai_transform/workflow/context_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 from ai_transform.types import Credentials
 from ai_transform.dataset import dataset
 from ai_transform.operator import abstract_operator
 from ai_transform.engine import abstract_engine
 from ai_transform.logger import format_logging_info
 from ai_transform.api.wrappers import request_wrapper
 
-logging.basicConfig(
-    level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s"
-)
+logging.basicConfig(level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 
 logger = logging.getLogger(__file__)
 
 
 WORKFLOW_FAIL_MESSAGE = (
-    "Workflow processed {:.2f}%"
-    + " of documents. This is less than the success threshold of {:.2f}%"
+    "Workflow processed {:.2f}%" + " of documents. This is less than the success threshold of {:.2f}%"
 )
 
 
 class WorkflowContextManager:
 
     FAILED = "failed"
     COMPLETE = "complete"
@@ -44,15 +41,14 @@
         # a Simple Workflow or a Regular one. They are initialized to None.
         credentials: Credentials = None,
         dataset: dataset.Dataset = None,
         operators: List[abstract_operator.AbstractOperator] = None,
         engine: abstract_engine.AbstractEngine = None,
         metadata: Dict[str, Any] = None,
         output: dict = None,
-        webhook_url: str = None,
     ):
 
         self.credentials = credentials
         self.engine = engine
         self.dataset = dataset
 
         if self.dataset is not None:
@@ -63,23 +59,25 @@
         self.workflow_name = workflow_name
         self.operators = operators
         self.job_id = job_id
         self.additional_information = additional_information
         self.send_email = send_email
         self.email = email
         self.success_threshold = success_threshold
+
+        if output is not None:
+            assert isinstance(output, dict), "When specifying an `output` object, please make sure it of type `dict`"
         self.output = output
 
         from ai_transform import __version__
 
         self.metadata = metadata if metadata is not None else {}
         self.metadata["ai_transform_version"] = __version__
 
         self._n_processed_pricing = None
-        self._webhook_url = webhook_url
 
     @property
     def worker_number(self) -> int:
         if self.engine is not None:
             return self.engine.worker_number
         else:
             return 0
@@ -91,75 +89,64 @@
         else:
             return None
 
     @property
     def field_children_metadata(self) -> Dict[str, str]:
         script_path = os.getenv("script_path", "")
         workflow_id = script_path.split("/")[0]
-        return {
-            "job_id": self.job_id,
-            "workflow_id": workflow_id,
-        }
+        return {"job_id": self.job_id, "workflow_id": workflow_id}
 
     def _set_field_children_recursively(self):
         for operator in self.operators:
             if operator.update_field_children:
                 for input_field in operator.input_fields:
 
                     metadata = {}
                     metadata.update(self.field_children_metadata)
                     if isinstance(operator.output_fields, dict):
                         metadata.update(operator.output_fields)
 
                     output_fields = list(operator.output_fields)
 
                     res = self.dataset[input_field].add_field_children(
-                        field_children=output_fields,
-                        fieldchildren_id=self.job_id,
-                        metadata=metadata,
-                        recursive=True,
+                        field_children=output_fields, fieldchildren_id=self.job_id, metadata=metadata, recursive=True
                     )
                     logger.debug(format_logging_info(res))
 
-    def set_workflow_status(self, status: str):
+    def _get_output_to_status_obj(self):
         if self.output is not None:
             output = self.output
+            if self.output_documents is not None:
+                output["documents"] = self.output_documents
         else:
             output = self.output_documents
+        return output
+
+    def set_workflow_status(self, status: str):
         result = self.api._set_workflow_status(
             status=status,
             job_id=self.job_id,
             metadata=self.metadata,
             workflow_name=self.workflow_name,
             additional_information=self.additional_information,
             send_email=self.send_email,
             email=self.email,
             worker_number=self.worker_number,
-            output=output,
+            output=self._get_output_to_status_obj(),
         )
-        if self._webhook_url is not None:
-            request_wrapper(
-                requests.post,
-                kwargs=dict(
-                    url=self._webhook_url,
-                    json={"status": status, "id": self.workflow_name},
-                ),
-            )
         logger.debug(format_logging_info(result))
         return result
 
     def __enter__(self):
         if self.operators is not None:
             self._set_field_children_recursively()
         self.set_workflow_status(status=self.IN_PROGRESS)
         return self
 
-    def _handle_workflow_fail(
-        self, exc_type: type, exc_value: BaseException, traceback: Traceback
-    ):
+    def _handle_workflow_fail(self, exc_type: type, exc_value: BaseException, traceback: Traceback):
         logger.exception(exc_value)
         self.set_workflow_status(status=self.FAILED)
         return False
 
     def _handle_workflow_complete(self):
         self.set_workflow_status(status=self.COMPLETE)
         return True
```

### Comparing `ai_transform-0.30.4/ai_transform/workflow/helpers.py` & `ai_transform-0.30.5/ai_transform/workflow/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,15 @@
     Example health object looks like this:
     {"exists": 300, "missing": 100}
     """
     return safe_divide(health["exists"], (health["exists"] + health["missing"]))
 
 
 def poll_until_health_updates(
-    dataset: Dataset,
-    field: str,
-    minimum_coverage: float = 0.95,
-    sleep_timer: int = 10,
-    max_time: int = 600,
+    dataset: Dataset, field: str, minimum_coverage: float = 0.95, sleep_timer: int = 10, max_time: int = 600
 ):
     """
     Poll until the dataset has all required dataset.
     """
     health = dataset.health()
     field_health = health[field]
     proportion = calculate_health_proportion(field_health)
@@ -101,17 +97,13 @@
             required based on the input field
         sleep_timer:
             the time in between each poll request
     """
     input_field_health = dataset.health()[input_field]
     min_coverage = calculate_health_proportion(input_field_health) * minimum_coverage
     return poll_until_health_updates(
-        dataset=dataset,
-        field=output_field,
-        minimum_coverage=min_coverage,
-        sleep_timer=sleep_timer,
-        max_time=max_time,
+        dataset=dataset, field=output_field, minimum_coverage=min_coverage, sleep_timer=sleep_timer, max_time=max_time
     )
 
 
 def encode_config(data: dict):
     return base64.b64encode(json.dumps(data).encode()).decode()
```

### Comparing `ai_transform-0.30.4/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.5/ai_transform.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 ai_transform/__init__.py
 ai_transform/config.py
 ai_transform/constants.py
 ai_transform/errors.py
 ai_transform/logger.py
 ai_transform/timer.py
```

### Comparing `ai_transform-0.30.4/setup.py` & `ai_transform-0.30.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,31 @@
 from setuptools import find_packages, setup
 
 from ai_transform import __version__
 
-requirements = [
-    "tqdm>=4.49.0",
-    "requests>=2.0.0",
-    "pandas>=1.5.0",
-    "pydantic>=1.10.2",
-]
-
-ray_requirements = [
-    "numpy>=1.19.0",
-    "pyarrow==9.0.0",
-    "ray==2.0.0",
-]
+requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2"]
+
+ray_requirements = ["numpy>=1.19.0", "pyarrow==9.0.0", "ray==2.0.0"]
 
 core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov", "sentence-splitter"]
 
-example_test_requirements = core_test_requirements + [
-    "torch",
-    "scikit-learn>=0.20.0",
-    "transformers[torch]==4.18.0",
-]
+example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
 
 chunk_requirements = ["fuzzysearch==0.7.3"]
 
 setup(
     name="ai_transform",
     version=__version__,
     url="https://tryrelevance.com/",
     author="Relevance AI",
     author_email="dev@tryrelevance.com",
     packages=find_packages(),
     setup_requires=["wheel"],
     install_requires=requirements,
-    package_data={
-        "": [
-            "*.ini",
-        ]
-    },
+    package_data={"": ["*.ini"]},
     extras_require=dict(
         core_tests=core_test_requirements,
         example_tests=example_test_requirements,
         ray=ray_requirements,
         chunk=chunk_requirements,
     ),
 )
```

### Comparing `ai_transform-0.30.4/tests/conftest.py` & `ai_transform-0.30.5/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 from ai_transform.api.helpers import process_token
 from ai_transform.engine.stable_engine import StableEngine
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.operator.dense_operator import DenseOperator
 from ai_transform.engine.stable_engine import StableEngine
-from ai_transform.utils.example_documents import (
-    mock_documents,
-    static_documents,
-    tag_documents,
-)
+from ai_transform.utils.example_documents import mock_documents, static_documents, tag_documents
 
 TEST_TOKEN = os.getenv("TEST_TOKEN")
 test_creds = process_token(TEST_TOKEN)
 
 
 @pytest.fixture(scope="session")
 def test_token() -> str:
@@ -115,18 +111,15 @@
     dataset = test_client.Dataset((dataset_id), expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="function")
 def test_document() -> Document:
-    raw_dict = {
-        "field1": {"field2": 1},
-        "field3": 3,
-    }
+    raw_dict = {"field1": {"field2": 1}, "field3": 3}
     return Document(raw_dict)
 
 
 @pytest.fixture(scope="function")
 def test_documents() -> DocumentList:
     return mock_documents()
 
@@ -173,18 +166,15 @@
 
             return documents
 
     return ExampleOperator()
 
 
 @pytest.fixture(scope="function")
-def test_dense_operator(
-    dense_output_dataset1: Dataset,
-    dense_output_dataset2: Dataset,
-) -> DenseOperator:
+def test_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
     class TestDenseOperator(DenseOperator):
         def __init__(self, output_dataset_ids: Sequence[str]):
             self.output_dataset_ids = output_dataset_ids
             super().__init__()
 
         def transform(self, documents: DocumentList) -> DocumentList:
             """
@@ -194,48 +184,31 @@
                 if "new_field" not in document:
                     document["new_field"] = 0
 
                 document["new_field"] += 3
 
             return {dataset_id: documents for dataset_id in self.output_dataset_ids}
 
-    output_dataset_ids = (
-        dense_output_dataset1.dataset_id,
-        dense_output_dataset2.dataset_id,
-    )
+    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
     return TestDenseOperator(output_dataset_ids)
 
 
 @pytest.fixture(scope="function")
 def test_engine(full_dataset: Dataset, test_operator: AbstractOperator) -> StableEngine:
-    return StableEngine(
-        dataset=full_dataset,
-        operator=test_operator,
-    )
+    return StableEngine(dataset=full_dataset, operator=test_operator)
 
 
 @pytest.fixture(scope="function")
-def test_paid_engine(
-    full_dataset: Dataset, test_paid_operator: AbstractOperator
-) -> StableEngine:
-    return StableEngine(
-        dataset=full_dataset,
-        operator=test_paid_operator,
-    )
+def test_paid_engine(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
+    return StableEngine(dataset=full_dataset, operator=test_paid_operator)
 
 
 @pytest.fixture(scope="function")
-def test_paid_engine_no_refresh(
-    full_dataset: Dataset, test_paid_operator: AbstractOperator
-) -> StableEngine:
-    return StableEngine(
-        dataset=full_dataset,
-        operator=test_paid_operator,
-        refresh=False,
-    )
+def test_paid_engine_no_refresh(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
+    return StableEngine(dataset=full_dataset, operator=test_paid_operator, refresh=False)
 
 
 @pytest.fixture(scope="function")
 def test_sentiment_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset((dataset_id), expire=True)
@@ -277,18 +250,15 @@
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset((dataset_id), expire=True)
     dataset.insert_documents(mock_documents(20))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
-        job_id=job_id,
-        authorizationToken=test_client.credentials.token,
-        dataset_id=dataset_id,
-        send_email=True,
+        job_id=job_id, authorizationToken=test_client.credentials.token, dataset_id=dataset_id, send_email=True
     )
     config_string = json.dumps(config)
     config_bytes = config_string.encode()
     workflow_token = base64.b64encode(config_bytes).decode()
     yield workflow_token
     test_client.delete_dataset(dataset_id)
```

### Comparing `ai_transform-0.30.4/tests/core/test_api/test_client.py` & `ai_transform-0.30.5/tests/core/test_api/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,15 @@
     def test_delete_where(self, test_client: Client, test_dataset_id: str):
         dataset = test_client.Dataset(test_dataset_id)
 
         n_test_docs = 20
         n_to_delete = 10
 
         documents = mock_documents(n_test_docs)
-        _ids = list(
-            set(
-                [
-                    document["_id"]
-                    for document in random.choices(documents, k=n_to_delete)
-                ]
-            )
-        )
+        _ids = list(set([document["_id"] for document in random.choices(documents, k=n_to_delete)]))
 
         dataset.insert_documents(documents)
         dataset.delete_documents(filters=dataset["_id"] == _ids)
 
         time.sleep(2)
 
         all_documents = dataset.get_all_documents()["documents"]
```

### Comparing `ai_transform-0.30.4/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.5/tests/core/test_api/test_endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 def test_proxy_openai(test_client: Client):
     body = {
         "model": f"gpt-3.5-turbo",
         "messages": [
             {"role": "system", "content": "You are a translator."},
             {
                 "role": "assistant",
-                "content": """Example response: 
+                "content": """Example response:
 {"detected_language" : The detected language, "translated_text": The translated text}
 """,
             },
             {"role": "user", "content": "Example"},
         ],
         "temperature": 0,
         "n": 1,
         "presence_penalty": 0,
         "frequency_penalty": 0,
     }
     response = test_client._api._proxy_openai(
-        workflows_admin_token=os.environ["WORKFLOW_ADMIN_TOKEN"],
-        body=body,
-        endpoint="/v1/chat/completions",
+        workflows_admin_token=os.environ["WORKFLOW_ADMIN_TOKEN"], body=body, endpoint="/v1/chat/completions"
     )
     assert "choices" in response
```

### Comparing `ai_transform-0.30.4/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.5/tests/core/test_api/test_keyphrase.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,21 @@
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.api.client import Client
 from ai_transform.utils.keyphrase import Keyphrase
 
 # write a few tests
 class TestClient:
     def test_upsert_keyphrases(
-        self,
-        test_client: Client,
-        test_keyphrase_dataset: Dataset,
-        test_keyphrases: List[Keyphrase],
+        self, test_client: Client, test_keyphrase_dataset: Dataset, test_keyphrases: List[Keyphrase]
     ):
         # Test that upserting keyphrases is good
         field = "sample_1_label"
         alias = "default"
         test_dataset_id = test_keyphrase_dataset.dataset_id
 
         result = test_client.api._bulk_update_keyphrase(
-            dataset_id=test_dataset_id,
-            field=field,
-            alias=alias,
-            updates=test_keyphrases,
+            dataset_id=test_dataset_id, field=field, alias=alias, updates=test_keyphrases
         )
         # Now that that we saw the actual dataset
-        result = test_client.api._get_keyphrase(
-            test_dataset_id, field=field, alias=alias, keyphrase_id="word"
-        )
+        result = test_client.api._get_keyphrase(test_dataset_id, field=field, alias=alias, keyphrase_id="word")
         print(result)
         assert result["text"] == "word" and result["keyphrase_score"] == 10, result
```

### Comparing `ai_transform-0.30.4/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.5/tests/core/test_api/test_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 
 class TestWrappers:
     def test_request_wrapper_fail_with_error_in_logs(self):
         f = io.StringIO()
         saved_stdout = sys.stdout
         sys.stdout = f
         resp = request_wrapper(
-            requests.post,
-            args=["https://www.google.com"],
-            num_retries=1,
-            timeout=1,
-            output_to_stdout=True,
+            requests.post, args=["https://www.google.com"], num_retries=1, timeout=1, output_to_stdout=True
         )
         output = f.getvalue()
         sys.stdout = saved_stdout
         assert "status_code" in output
         assert "message" in output
 
     def test_request_wrapper_fail_2(self):
@@ -37,17 +33,15 @@
                 timeout=1,
             )
 
         assert "status_code" in str(u.getvalue()) + str(f.getvalue())
         assert "message" in str(u.getvalue()) + str(f.getvalue())
 
     def test_request_wrapper_pass(self):
-        resp = request_wrapper(
-            requests.get, ("https://www.google.com",), timeout=1, num_retries=2
-        )
+        resp = request_wrapper(requests.get, ("https://www.google.com",), timeout=1, num_retries=2)
         if resp is None:
             raise ValueError("Resp should not be None")
         assert resp.status_code == 200
 
     def test_request_wrapper_lambda(self):
         f = io.StringIO()
         u = io.StringIO()
@@ -88,19 +82,15 @@
                     placeholder = requests.Response()
                     placeholder.status_code = 429
                     placeholder._content = b"Simulated Rate Error"
                     return placeholder
 
         with redirect_stdout(f), redirect_stderr(u):
             resp = request_wrapper(
-                TestRequest(),
-                ("https://www.google.com",),
-                num_retries=3,
-                timeout=1,
-                output_to_stdout=True,
+                TestRequest(), ("https://www.google.com",), num_retries=3, timeout=1, output_to_stdout=True
             )
 
         assert resp.status_code == 200
 
         logs = str(u.getvalue()) + str(f.getvalue())
 
         assert logs.count("Simulated Rate Error") == 2
```

### Comparing `ai_transform-0.30.4/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.5/tests/core/test_dataset/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 
 
 @pytest.mark.usefixtures("full_dataset")
 class TestDataset2:
     def test_schema(self, full_dataset: Dataset):
         documents = mock_documents(5)
         keys = documents[0].keys()
-        keys = [
-            ".".join([sf for sf in nested_field.split(".") if not sf.isdigit()])
-            for nested_field in keys
-        ]
+        keys = [".".join([sf for sf in nested_field.split(".") if not sf.isdigit()]) for nested_field in keys]
         schema = full_dataset.schema
         assert all([key in schema for key in keys if key not in ["_id"]])
 
     def test_series(self, full_dataset: Dataset):
         schema = full_dataset.schema
         series = full_dataset[random.choice(list(schema.keys()))]
         assert True
@@ -130,17 +127,15 @@
         filters = static_dataset["insert_date_"] == random.choice(dates)
         res = static_dataset.get_documents(page_size=20, filters=filters)
         assert res["count"] == 1
 
 
 class TestDatasetMedia:
     def test_upload_medias(self, empty_dataset: Dataset):
-        urls = empty_dataset.insert_local_medias(
-            ["hierarchy.png", "hierarchy.png", "hierarchy.png"]
-        )
+        urls = empty_dataset.insert_local_medias(["hierarchy.png", "hierarchy.png", "hierarchy.png"])
         assert len(urls) == 3
 
 
 class TestChunkFilters:
     def test_chunk_filters(self, mixed_dataset: Dataset):
         filters = mixed_dataset["_chunk_.label"].exists()
         filtered = mixed_dataset.get_documents(100, filters=filters)
```

### Comparing `ai_transform-0.30.4/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.5/tests/core/test_dataset/test_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,19 @@
 
 from ai_transform.api.client import Client
 from ai_transform.dataset.field import Field, ClusterField, KeyphraseField
 from ai_transform.utils.example_documents import mock_documents
 
 
 def list_methods(cls):
-    return set(
-        x
-        for x, y in cls.__dict__.items()
-        if isinstance(y, (FunctionType, classmethod, staticmethod))
-    )
+    return set(x for x, y in cls.__dict__.items() if isinstance(y, (FunctionType, classmethod, staticmethod)))
 
 
 def list_parent_methods(cls):
-    return set(
-        itertools.chain.from_iterable(
-            list_methods(c).union(list_parent_methods(c)) for c in cls.__bases__
-        )
-    )
+    return set(itertools.chain.from_iterable(list_methods(c).union(list_parent_methods(c)) for c in cls.__bases__))
 
 
 def list_subclass_methods(cls, is_narrow: bool = False):
     methods = list_methods(cls)
     if is_narrow:
         parentMethods = list_parent_methods(cls)
         return set(cls for cls in methods if not (cls in parentMethods))
```

### Comparing `ai_transform-0.30.4/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.5/tests/core/test_dataset/test_keyphrase.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,33 +6,24 @@
 
 @pytest.mark.usefixtures("full_dataset")
 class TestKeyphraseCrud:
     def test_crud(self, full_dataset: Dataset):
         keyphrase_field = full_dataset["_keyphrase_.sample_1_label.default"]
 
         keyphrase1 = Keyphrase(
-            text="cat",
-            _id="cat",
-            ancestors=[],
-            parents=[],
-            level=0,
-            keyphrase_score=1.1,
-            frequency=2,
-            metadata={},
+            text="cat", _id="cat", ancestors=[], parents=[], level=0, keyphrase_score=1.1, frequency=2, metadata={}
         )
         keyphrase2 = Keyphrase(
             text="cat",
             _id="dog",
             ancestors=["cat"],
             parents=["cat"],
             level=1,
             keyphrase_score=1.1,
             frequency=1,
             metadata={},
         )
         updates = [keyphrase1, keyphrase2]
-        response = keyphrase_field.bulk_update_keyphrases(
-            updates=updates,
-        )
+        response = keyphrase_field.bulk_update_keyphrases(updates=updates)
 
         keyphrase = keyphrase_field.get_keyphrase(keyphrase_id="cat")
         assert "cat" == keyphrase["text"]
```

### Comparing `ai_transform-0.30.4/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.5/tests/core/test_engine/test_dense_output_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,16 @@
     def test_dense_output_engine(
         self,
         test_dense_operator: AbstractOperator,
         dense_input_dataset: Dataset,
         dense_output_dataset1: Dataset,
         dense_output_dataset2: Dataset,
     ):
-        engine = DenseOutputEngine(
-            dataset=dense_input_dataset,
-            operator=test_dense_operator,
-        )
-        workflow = Workflow(
-            name="workflow_test123",
-            engine=engine,
-            job_id="test_job123",
-        )
+        engine = DenseOutputEngine(dataset=dense_input_dataset, operator=test_dense_operator)
+        workflow = Workflow(name="workflow_test123", engine=engine, job_id="test_job123")
         workflow.run()
 
         time.sleep(4)
 
         documents = dense_input_dataset.get_all_documents(select_fields=["new_field"])
         assert len(documents["documents"]) == 2
         for document in documents["documents"]:
```

### Comparing `ai_transform-0.30.4/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.5/tests/core/test_engine/test_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,23 @@
                 return
 
         engine = ExampleEngine(full_dataset, test_operator)
 
         assert isinstance(engine.operator, AbstractOperator)
         assert len(ExampleEngine.__abstractmethods__) == 0
 
-    def test_engine_abstract(
-        self, full_dataset: Dataset, test_operator: AbstractOperator
-    ):
+    def test_engine_abstract(self, full_dataset: Dataset, test_operator: AbstractOperator):
         class ExampleEngine(AbstractEngine):
             pass
 
         try:
             engine = ExampleEngine(full_dataset, test_operator)
         except:
             assert True
 
-    def test_engine_select_fields(
-        self, full_dataset: Dataset, test_operator: AbstractOperator
-    ):
+    def test_engine_select_fields(self, full_dataset: Dataset, test_operator: AbstractOperator):
         class ExampleEngine(AbstractEngine):
             def apply(self) -> Any:
                 return
 
-        engine = ExampleEngine(
-            full_dataset, test_operator, select_fields=["_id", "_chunk_.label"]
-        )
+        engine = ExampleEngine(full_dataset, test_operator, select_fields=["_id", "_chunk_.label"])
         assert "_chunk_" in engine._select_fields
```

### Comparing `ai_transform-0.30.4/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.5/tests/core/test_engine/test_engine_playground.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,17 @@
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.engine.stable_engine import StableEngine
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.utils import mock_documents
 
 
 class TestEnginePlayground:
-    def test_engine_playground(
-        self,
-        full_dataset: Dataset,
-        test_operator: AbstractOperator,
-    ):
-
-        engine = StableEngine(
-            full_dataset,
-            test_operator,
-            documents=mock_documents(1000),
-        )
+    def test_engine_playground(self, full_dataset: Dataset, test_operator: AbstractOperator):
+
+        engine = StableEngine(full_dataset, test_operator, documents=mock_documents(1000))
 
         assert engine.output_to_status
 
         engine()
 
         assert engine.output_documents
         for document in engine.output_documents:
```

### Comparing `ai_transform-0.30.4/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.5/tests/core/test_engine/test_multipass_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,29 +10,17 @@
     from ai_transform.dataset.dataset import Dataset
     from ai_transform.engine.multipass_engine import MultiPassEngine
 
     from ai_transform.operator.abstract_operator import AbstractOperator
     from ai_transform.workflow.abstract_workflow import Workflow
 
     class TestMultiPassEngine:
-        def test_multipass_engine(
-            self, full_dataset: Dataset, test_operator: AbstractOperator
-        ):
-            engine = MultiPassEngine(
-                dataset=full_dataset,
-                operators=[
-                    test_operator,
-                    test_operator,
-                ],
-            )
-            workflow = Workflow(
-                name="test_multipass_engine",
-                engine=engine,
-                job_id="test_multipass_engine",
-            )
+        def test_multipass_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
+            engine = MultiPassEngine(dataset=full_dataset, operators=[test_operator, test_operator])
+            workflow = Workflow(name="test_multipass_engine", engine=engine, job_id="test_multipass_engine")
             workflow.run()
 
             time.sleep(4)
 
             documents = full_dataset.get_all_documents(select_fields=["new_field"])
             for document in documents["documents"]:
                 assert document["new_field"] == 6
@@ -43,34 +31,26 @@
             class FitOperator(AbstractOperator):
                 def __init__(self, model: MiniBatchKMeans, vector_field: str):
                     self._model = model
                     self._vector_field = vector_field
                     super().__init__(input_fields=[vector_field], output_fields=[])
 
                 def transform(self, documents):
-                    vectors = np.array(
-                        [document[self._vector_field] for document in documents]
-                    )
+                    vectors = np.array([document[self._vector_field] for document in documents])
                     self._model.partial_fit(vectors)
 
             class PredictOperator(AbstractOperator):
-                def __init__(
-                    self, model: MiniBatchKMeans, vector_field: str, output_field: str
-                ):
+                def __init__(self, model: MiniBatchKMeans, vector_field: str, output_field: str):
                     self._model = model
                     self._vector_field = vector_field
                     self._output_field = output_field
-                    super().__init__(
-                        input_fields=[vector_field], output_fields=[output_field]
-                    )
+                    super().__init__(input_fields=[vector_field], output_fields=[output_field])
 
                 def transform(self, documents):
-                    vectors = np.array(
-                        [document[self._vector_field] for document in documents]
-                    )
+                    vectors = np.array([document[self._vector_field] for document in documents])
                     labels = self._model.predict(vectors)
                     for document, label in zip(documents, labels):
                         document[self._output_field] = f"cluster_{label}"
 
                     return documents
 
             vector_field = "sample_1_vector_"
@@ -79,20 +59,15 @@
 
             batch_size = 5
             kmeans_model = MiniBatchKMeans(n_clusters=3, batch_size=batch_size)
             fit_operator = FitOperator(kmeans_model, vector_field)
             predict_operator = PredictOperator(kmeans_model, vector_field, output_field)
 
             engine = MultiPassEngine(
-                dataset=full_dataset,
-                operators=[
-                    fit_operator,
-                    predict_operator,
-                ],
-                transform_chunksize=batch_size,
+                dataset=full_dataset, operators=[fit_operator, predict_operator], transform_chunksize=batch_size
             )
             workflow = Workflow(
                 name="test_multipass_engine_with_clustering",
                 engine=engine,
                 job_id="test_multipass_engine_with_clustering",
             )
             workflow.run()
```

### Comparing `ai_transform-0.30.4/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.5/tests/core/test_engine/test_stable_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,18 @@
 from ai_transform.engine.small_batch_stable_engine import SmallBatchStableEngine
 
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.workflow.abstract_workflow import AbstractWorkflow
 
 
 class TestStableEngine:
-    def test_stable_engine(
-        self, full_dataset: Dataset, test_operator: AbstractOperator
-    ):
+    def test_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
         engine = StableEngine(full_dataset, test_operator, worker_number=0)
-        workflow = AbstractWorkflow(
-            name="workflow_test123",
-            engine=engine,
-            job_id="test_job123",
-        )
+        workflow = AbstractWorkflow(name="workflow_test123", engine=engine, job_id="test_job123")
         workflow.run()
         assert engine.success_ratio == 1
 
-    def test_small_batch_stable_engine(
-        self, full_dataset: Dataset, test_operator: AbstractOperator
-    ):
+    def test_small_batch_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
         engine = SmallBatchStableEngine(full_dataset, test_operator)
-        workflow = AbstractWorkflow(
-            name="workflow_test123",
-            engine=engine,
-            job_id="test_job123",
-        )
+        workflow = AbstractWorkflow(name="workflow_test123", engine=engine, job_id="test_job123")
         workflow.run()
         assert engine.success_ratio == 1
```

### Comparing `ai_transform-0.30.4/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.5/tests/core/test_operator/test_document_diff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 import json
 import random
 
 from copy import deepcopy
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.utils.document import Document
-from ai_transform.utils.example_documents import (
-    mock_documents,
-    generate_random_label,
-    generate_random_vector,
-)
+from ai_transform.utils.example_documents import mock_documents, generate_random_label, generate_random_vector
 
 
 class TestDocumentDiff:
     def test_diff1(self):
         old_documents = mock_documents(3)
         new_documents = deepcopy(old_documents)
 
         expected_diff = []
 
         for document in new_documents:
-            new_chunk = {
-                "label": generate_random_label(),
-                "label_chunkvector_": generate_random_vector(),
-            }
+            new_chunk = {"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}
             document["_chunk_"].append(new_chunk)
-            expected_diff.append(
-                {"_id": document["_id"], "_chunk_": document["_chunk_"]}
-            )
+            expected_diff.append({"_id": document["_id"], "_chunk_": document["_chunk_"]})
 
         diff = AbstractOperator._postprocess(new_documents, old_documents).to_json()
         diff = list(sorted(diff, key=lambda x: x["_id"]))
         expected_diff = list(sorted(expected_diff, key=lambda x: x["_id"]))
 
-        assert json.dumps(diff, sort_keys=True) == json.dumps(
-            expected_diff, sort_keys=True
-        )
+        assert json.dumps(diff, sort_keys=True) == json.dumps(expected_diff, sort_keys=True)
 
     def test_update_diff(self):
         old_documents = [Document({"label": "yes"}) for _ in range(5)]
         new_documents = deepcopy(old_documents)
         for document in new_documents:
             document["label"] = "no"
 
@@ -49,18 +38,15 @@
 
     def test_no_diff(self):
         documents = [Document({"value": 10})]
         diff = AbstractOperator._postprocess(documents, documents)
         assert not diff
 
     def test_chunk_diff(self):
-        old_documents = [
-            Document({"example_vector_": [random.random() for _ in range(5)]})
-            for _ in range(5)
-        ]
+        old_documents = [Document({"example_vector_": [random.random() for _ in range(5)]}) for _ in range(5)]
         new_documents = deepcopy(old_documents)
         for document in new_documents:
             document["label"] = "yes"
 
         diff = AbstractOperator._postprocess(new_documents, old_documents)
         expected_diff = json.dumps({"label": "yes"})
```

### Comparing `ai_transform-0.30.4/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.5/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.4/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.5/tests/core/test_workflow/test_workflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,107 +5,78 @@
 from ai_transform.api.client import Client
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.workflow.abstract_workflow import Workflow
 from ai_transform.config import BaseConfig
 
 
 class SimpleWorkflowConfig(BaseConfig):
-    input_field: str = Field(
-        "test_input_field",
-        description="The field you want to are using to transform on",
-    )
-    output_field: str = Field(
-        "test_output_field",
-        description="The output field",
-    )
+    input_field: str = Field("test_input_field", description="The field you want to are using to transform on")
+    output_field: str = Field("test_output_field", description="The output field")
     minimum_coverage: float = Field(
-        0.95,
-        description="The minimum amount of coverage of the output field relative to the input field.",
-    )
-    max_time: float = Field(
-        6000, description="THe maximum amount of time to allow for this to poll."
-    )
-    sleep_timer: float = Field(
-        10,
-        description="How long to wait before each poll",
+        0.95, description="The minimum amount of coverage of the output field relative to the input field."
     )
+    max_time: float = Field(6000, description="THe maximum amount of time to allow for this to poll.")
+    sleep_timer: float = Field(10, description="How long to wait before each poll")
     parent_job_id: str = Field(
         None,
         description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
     )
     parent_job_name: str = Field(
         None,
         description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
     )
 
 
 class TestWorkflow:
     def test_workflow(self, test_paid_engine: AbstractEngine):
 
         workflow_name = "test_workflow"
-        workflow = Workflow(
-            name=workflow_name,
-            engine=test_paid_engine,
-            job_id="test_job1",
-        )
+        workflow = Workflow(name=workflow_name, engine=test_paid_engine, job_id="test_job1")
         res = workflow.run()
         assert res is None
 
         status = workflow.get_status()
         assert status["steps"][workflow_name]["n_processed_pricing"] == 20
 
     def test_workflow_no_refresh(self, test_paid_engine_no_refresh: AbstractEngine):
 
         workflow_name = "test_workflow"
-        workflow = Workflow(
-            name=workflow_name,
-            engine=test_paid_engine_no_refresh,
-            job_id="test_job2",
-        )
+        workflow = Workflow(name=workflow_name, engine=test_paid_engine_no_refresh, job_id="test_job2")
         res = workflow.run()
         assert res is None
 
         status = workflow.get_status()
         assert status["steps"][workflow_name]["n_processed_pricing"] == 20
 
 
 class TestSimpleWorkflow:
-    def test_simple_workflow_simple_case(
-        self, test_client: Client, test_simple_workflow_token: str
-    ):
+    def test_simple_workflow_simple_case(self, test_client: Client, test_simple_workflow_token: str):
         config = SimpleWorkflowConfig.read_token(test_simple_workflow_token)
 
         x = 0
         with test_client.SimpleWorkflow(
             workflow_name="Simple Workflow",
             job_id=config.job_id,
             additional_information=config.additional_information,
             send_email=config.send_email,
         ):
             x += 1
         assert x == 1
 
     def test_simple_workflow(self, test_client: Client):
-        simple_workflow_dataset = test_client.Dataset(
-            "test-simple-workflow-dataset", expire=True
-        )
+        simple_workflow_dataset = test_client.Dataset("test-simple-workflow-dataset", expire=True)
         simple_workflow_dataset.insert_documents([{"_id": "0", "value": 0}])
 
         workflow_name = "Simple Workflow"
         time_sleep_value = 10
 
-        with test_client.SimpleWorkflow(
-            workflow_name=workflow_name,
-            job_id="test-simple-workflow",
-        ) as workflow:
+        with test_client.SimpleWorkflow(workflow_name=workflow_name, job_id="test-simple-workflow") as workflow:
 
             time.sleep(time_sleep_value)
-            simple_workflow_dataset.update_documents(
-                [{"_id": "0", "value": 1}], ingest_in_background=False
-            )
+            simple_workflow_dataset.update_documents([{"_id": "0", "value": 1}], ingest_in_background=False)
 
         status = workflow.get_status()
         assert status["status"] == "complete"
         assert status["steps"][workflow_name]["n_processed_pricing"] >= time_sleep_value
 
         documents = simple_workflow_dataset.get_all_documents()["documents"]
         assert documents[0]["value"] == 1
```

