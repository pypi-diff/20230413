# Comparing `tmp/keras-tuner-1.3.4.tar.gz` & `tmp/keras-tuner-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-tuner-1.3.4.tar", last modified: Sun Apr  2 22:35:13 2023, max compression
+gzip compressed data, was "keras-tuner-1.3.5.tar", last modified: Thu Apr 13 04:36:47 2023, max compression
```

## Comparing `keras-tuner-1.3.4.tar` & `keras-tuner-1.3.5.tar`

### file list

```diff
@@ -1,102 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.983317 keras-tuner-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-02 22:35:13.983317 keras-tuner-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.971316 keras-tuner-1.3.4/keras_tuner/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.975316 keras-tuner-1.3.4/keras_tuner/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/augment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/efficientnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/applications/xception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.975316 keras-tuner-1.3.4/keras_tuner/distribute/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/oracle_chief.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/oracle_chief_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/oracle_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/oracle_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/distribute/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.979317 keras-tuner-1.3.4/keras_tuner/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/base_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/base_tuner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/conditions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hypermodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.979317 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.979317 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/boolean_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/boolean_hp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/choice_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/choice_hp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/fixed_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/fixed_hp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/float_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/float_hp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/int_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/int_hp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/metrics_tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/metrics_tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/multi_execution_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/objective_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/oracle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/stateful.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/trial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    46833 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/tuner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/tuner_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/engine/tuner_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.979317 keras-tuner-1.3.4/keras_tuner/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.983317 keras-tuner-1.3.4/keras_tuner/protos/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61874 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/protos/keras_tuner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/protos/keras_tuner_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/protos/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/protos/service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.983317 keras-tuner-1.3.4/keras_tuner/tuners/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/bayesian_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/gridsearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/hyperband_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/randomsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/randomsearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/sklearn_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/tuners/sklearn_tuner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/keras_tuner/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 22:35:13.971316 keras-tuner-1.3.4/keras_tuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-02 22:35:13.000000 keras-tuner-1.3.4/keras_tuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-02 22:35:13.000000 keras-tuner-1.3.4/keras_tuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 22:35:13.000000 keras-tuner-1.3.4/keras_tuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-02 22:35:13.000000 keras-tuner-1.3.4/keras_tuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-02 22:35:13.000000 keras-tuner-1.3.4/keras_tuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-02 22:35:13.983317 keras-tuner-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-02 22:35:03.000000 keras-tuner-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.473099 keras-tuner-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-13 04:36:47.473099 keras-tuner-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.461099 keras-tuner-1.3.5/keras_tuner/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.465099 keras-tuner-1.3.5/keras_tuner/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/augment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/efficientnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/applications/xception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.465099 keras-tuner-1.3.5/keras_tuner/distribute/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/oracle_chief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/oracle_chief_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/oracle_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/oracle_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/distribute/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/base_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/base_tuner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/conditions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hypermodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/boolean_hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/boolean_hp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/choice_hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/choice_hp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/fixed_hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/fixed_hp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/float_hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/float_hp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/int_hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/int_hp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/metrics_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/metrics_tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/objective_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/oracle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/trial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46833 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/tuner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/tuner_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/engine/tuner_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.469099 keras-tuner-1.3.5/keras_tuner/protos/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v3/keras_tuner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v3/keras_tuner_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v3/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v3/service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.473099 keras-tuner-1.3.5/keras_tuner/protos/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v4/keras_tuner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v4/keras_tuner_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v4/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/protos/v4/service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.473099 keras-tuner-1.3.5/keras_tuner/tuners/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/bayesian_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/gridsearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/hyperband_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/randomsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/randomsearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/sklearn_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/tuners/sklearn_tuner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/keras_tuner/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:36:47.461099 keras-tuner-1.3.5/keras_tuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-13 04:36:47.000000 keras-tuner-1.3.5/keras_tuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-13 04:36:47.000000 keras-tuner-1.3.5/keras_tuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:36:47.000000 keras-tuner-1.3.5/keras_tuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 04:36:47.000000 keras-tuner-1.3.5/keras_tuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 04:36:47.000000 keras-tuner-1.3.5/keras_tuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-13 04:36:47.473099 keras-tuner-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 04:36:36.000000 keras-tuner-1.3.5/setup.py
```

### Comparing `keras-tuner-1.3.4/LICENSE` & `keras-tuner-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/PKG-INFO` & `keras-tuner-1.3.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-tuner
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Hyperparameter Tuning Library for Keras
 Home-page: https://github.com/keras-team/keras-tuner
 Author: The KerasTuner authors
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,11 +13,13 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Provides-Extra: tensorflow
+Provides-Extra: tensorflow-cpu
 Provides-Extra: tests
 Provides-Extra: bayesian
 Provides-Extra: build
 License-File: LICENSE
```

### Comparing `keras-tuner-1.3.4/README.md` & `keras-tuner-1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 * [Getting started with KerasTuner](https://keras.io/guides/keras_tuner/getting_started)
 * [KerasTuner developer guides](https://keras.io/guides/keras_tuner/)
 * [KerasTuner API reference](https://keras.io/api/keras_tuner/)
 
 
 ## Installation
 
-KerasTuner requires **Python 3.7+** and **TensorFlow 2.0+**.
+KerasTuner requires **Python 3.8+** and **TensorFlow 2.0+**.
 
 Install the latest release:
 
 ```
-pip install keras-tuner --upgrade
+pip install keras-tuner
 ```
 
 You can also check out other versions in our
 [GitHub repository](https://github.com/keras-team/keras-tuner).
 
 
 ## Quick introduction
```

### Comparing `keras-tuner-1.3.4/keras_tuner/__init__.py` & `keras-tuner-1.3.5/keras_tuner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 from keras_tuner.tuners import Hyperband
 from keras_tuner.tuners import RandomSearch
 from keras_tuner.tuners import SklearnTuner
 from keras_tuner.utils import check_tf_version
 
 check_tf_version()
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
```

### Comparing `keras-tuner-1.3.4/keras_tuner/api_export.py` & `keras-tuner-1.3.5/keras_tuner/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/__init__.py` & `keras-tuner-1.3.5/keras_tuner/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/augment.py` & `keras-tuner-1.3.5/keras_tuner/applications/augment.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/augment_test.py` & `keras-tuner-1.3.5/keras_tuner/applications/augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/efficientnet.py` & `keras-tuner-1.3.5/keras_tuner/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/efficientnet_test.py` & `keras-tuner-1.3.5/keras_tuner/applications/efficientnet_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/resnet.py` & `keras-tuner-1.3.5/keras_tuner/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/resnet_test.py` & `keras-tuner-1.3.5/keras_tuner/applications/resnet_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/xception.py` & `keras-tuner-1.3.5/keras_tuner/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/applications/xception_test.py` & `keras-tuner-1.3.5/keras_tuner/applications/xception_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/config.py` & `keras-tuner-1.3.5/keras_tuner/config.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/conftest.py` & `keras-tuner-1.3.5/keras_tuner/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/__init__.py` & `keras-tuner-1.3.5/keras_tuner/distribute/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/file_utils.py` & `keras-tuner-1.3.5/keras_tuner/distribute/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/oracle_chief.py` & `keras-tuner-1.3.5/keras_tuner/distribute/oracle_chief.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/oracle_chief_test.py` & `keras-tuner-1.3.5/keras_tuner/distribute/oracle_chief_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/oracle_client.py` & `keras-tuner-1.3.5/keras_tuner/distribute/oracle_client.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/oracle_client_test.py` & `keras-tuner-1.3.5/keras_tuner/distribute/oracle_client_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/utils.py` & `keras-tuner-1.3.5/keras_tuner/distribute/utils.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/distribute/utils_test.py` & `keras-tuner-1.3.5/keras_tuner/distribute/utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/__init__.py` & `keras-tuner-1.3.5/keras_tuner/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/base_tuner.py` & `keras-tuner-1.3.5/keras_tuner/engine/base_tuner.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/base_tuner_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/base_tuner_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/conditions.py` & `keras-tuner-1.3.5/keras_tuner/engine/conditions.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/conditions_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/conditions_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hypermodel.py` & `keras-tuner-1.3.5/keras_tuner/engine/hypermodel.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/__init__.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/__init__.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/boolean_hp.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/boolean_hp.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/boolean_hp_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/boolean_hp_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/choice_hp.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/choice_hp.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/choice_hp_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/choice_hp_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/fixed_hp.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/fixed_hp.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/fixed_hp_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/fixed_hp_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/float_hp.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/float_hp.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/float_hp_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/float_hp_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/int_hp.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/int_hp.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/int_hp_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/int_hp_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_types/numerical.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_types/numerical.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_utils.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_utils.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hp_utils_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hp_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameter.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameter_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameter_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameters.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/hyperparameters/hyperparameters_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/hyperparameters/hyperparameters_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/metrics_tracking.py` & `keras-tuner-1.3.5/keras_tuner/engine/metrics_tracking.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/metrics_tracking_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/metrics_tracking_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/multi_execution_tuner.py` & `keras-tuner-1.3.5/keras_tuner/protos/v3/keras_tuner_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_tuner.engine import tuner
-
-
-class MultiExecutionTuner(tuner.Tuner):
-    """Keep this class for backward compatibility.
-
-    Currently, the Tuner class behavoir is the same as the old
-    MultiExecutionTuner.
-    """
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
```

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/objective.py` & `keras-tuner-1.3.5/keras_tuner/engine/objective.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/objective_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/objective_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/oracle.py` & `keras-tuner-1.3.5/keras_tuner/engine/oracle.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/oracle_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/oracle_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/stateful.py` & `keras-tuner-1.3.5/keras_tuner/engine/stateful.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/trial.py` & `keras-tuner-1.3.5/keras_tuner/engine/trial.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/trial_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/trial_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/tuner.py` & `keras-tuner-1.3.5/keras_tuner/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/tuner_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/tuner_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/tuner_utils.py` & `keras-tuner-1.3.5/keras_tuner/engine/tuner_utils.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/engine/tuner_utils_test.py` & `keras-tuner-1.3.5/keras_tuner/engine/tuner_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/errors.py` & `keras-tuner-1.3.5/keras_tuner/errors.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/oracles/__init__.py` & `keras-tuner-1.3.5/keras_tuner/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/protos/__init__.py` & `keras-tuner-1.3.5/keras_tuner/protos/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """KerasTuner protos."""
 
+from contextlib import contextmanager
 
-def get_proto():
-    from keras_tuner.protos import keras_tuner_pb2
+# v3 is generated with protobuf==3.20.3 and grpcio-tools==1.48.0
+# v4 is generated with protobuf==4.22.1 and grpcio-tools==1.53.0
+try:
+    from keras_tuner.protos import v4 as protos
+except ImportError:
+    from keras_tuner.protos import v3 as protos
 
-    return keras_tuner_pb2
 
+def get_proto():
+    return protos.keras_tuner_pb2
 
-def get_service():
-    from keras_tuner.protos import service_pb2
 
-    return service_pb2
+def get_service():
+    return protos.service_pb2
 
 
 def get_service_grpc():
-    from keras_tuner.protos import service_pb2_grpc
-
-    return service_pb2_grpc
+    return protos.service_pb2_grpc
```

### Comparing `keras-tuner-1.3.4/keras_tuner/protos/keras_tuner_pb2_grpc.py` & `keras-tuner-1.3.5/keras_tuner/protos/v4/keras_tuner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/protos/service_pb2_grpc.py` & `keras-tuner-1.3.5/keras_tuner/protos/v3/service_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from keras_tuner.protos import (
+from keras_tuner.protos.v3 import (
     service_pb2 as keras__tuner_dot_protos_dot_service__pb2,
 )
 
 
 class OracleStub(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -164,188 +164,202 @@
     @staticmethod
     def GetSpace(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/GetSpace",
             keras__tuner_dot_protos_dot_service__pb2.GetSpaceRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.GetSpaceResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def UpdateSpace(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/UpdateSpace",
             keras__tuner_dot_protos_dot_service__pb2.UpdateSpaceRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.UpdateSpaceResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def CreateTrial(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/CreateTrial",
             keras__tuner_dot_protos_dot_service__pb2.CreateTrialRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.CreateTrialResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def UpdateTrial(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/UpdateTrial",
             keras__tuner_dot_protos_dot_service__pb2.UpdateTrialRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.UpdateTrialResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def EndTrial(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/EndTrial",
             keras__tuner_dot_protos_dot_service__pb2.EndTrialRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.EndTrialResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def GetBestTrials(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/GetBestTrials",
             keras__tuner_dot_protos_dot_service__pb2.GetBestTrialsRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.GetBestTrialsResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
     def GetTrial(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
+        insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/keras_tuner.Oracle/GetTrial",
             keras__tuner_dot_protos_dot_service__pb2.GetTrialRequest.SerializeToString,
             keras__tuner_dot_protos_dot_service__pb2.GetTrialResponse.FromString,
             options,
             channel_credentials,
+            insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
```

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/__init__.py` & `keras-tuner-1.3.5/keras_tuner/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/bayesian.py` & `keras-tuner-1.3.5/keras_tuner/tuners/bayesian.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/bayesian_test.py` & `keras-tuner-1.3.5/keras_tuner/tuners/bayesian_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/gridsearch.py` & `keras-tuner-1.3.5/keras_tuner/tuners/gridsearch.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/gridsearch_test.py` & `keras-tuner-1.3.5/keras_tuner/tuners/gridsearch_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/hyperband.py` & `keras-tuner-1.3.5/keras_tuner/tuners/hyperband.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/hyperband_test.py` & `keras-tuner-1.3.5/keras_tuner/tuners/hyperband_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/randomsearch.py` & `keras-tuner-1.3.5/keras_tuner/tuners/randomsearch.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/randomsearch_test.py` & `keras-tuner-1.3.5/keras_tuner/tuners/randomsearch_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/sklearn_tuner.py` & `keras-tuner-1.3.5/keras_tuner/tuners/sklearn_tuner.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/tuners/sklearn_tuner_test.py` & `keras-tuner-1.3.5/keras_tuner/tuners/sklearn_tuner_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/utils.py` & `keras-tuner-1.3.5/keras_tuner/utils.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner/utils_test.py` & `keras-tuner-1.3.5/keras_tuner/utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/keras_tuner.egg-info/PKG-INFO` & `keras-tuner-1.3.5/keras_tuner.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-tuner
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Hyperparameter Tuning Library for Keras
 Home-page: https://github.com/keras-team/keras-tuner
 Author: The KerasTuner authors
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,11 +13,13 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Provides-Extra: tensorflow
+Provides-Extra: tensorflow-cpu
 Provides-Extra: tests
 Provides-Extra: bayesian
 Provides-Extra: build
 License-File: LICENSE
```

### Comparing `keras-tuner-1.3.4/keras_tuner.egg-info/SOURCES.txt` & `keras-tuner-1.3.5/keras_tuner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 keras_tuner/engine/base_tuner.py
 keras_tuner/engine/base_tuner_test.py
 keras_tuner/engine/conditions.py
 keras_tuner/engine/conditions_test.py
 keras_tuner/engine/hypermodel.py
 keras_tuner/engine/metrics_tracking.py
 keras_tuner/engine/metrics_tracking_test.py
-keras_tuner/engine/multi_execution_tuner.py
 keras_tuner/engine/objective.py
 keras_tuner/engine/objective_test.py
 keras_tuner/engine/oracle.py
 keras_tuner/engine/oracle_test.py
 keras_tuner/engine/stateful.py
 keras_tuner/engine/trial.py
 keras_tuner/engine/trial_test.py
@@ -69,18 +68,24 @@
 keras_tuner/engine/hyperparameters/hp_types/float_hp.py
 keras_tuner/engine/hyperparameters/hp_types/float_hp_test.py
 keras_tuner/engine/hyperparameters/hp_types/int_hp.py
 keras_tuner/engine/hyperparameters/hp_types/int_hp_test.py
 keras_tuner/engine/hyperparameters/hp_types/numerical.py
 keras_tuner/oracles/__init__.py
 keras_tuner/protos/__init__.py
-keras_tuner/protos/keras_tuner_pb2.py
-keras_tuner/protos/keras_tuner_pb2_grpc.py
-keras_tuner/protos/service_pb2.py
-keras_tuner/protos/service_pb2_grpc.py
+keras_tuner/protos/v3/__init__.py
+keras_tuner/protos/v3/keras_tuner_pb2.py
+keras_tuner/protos/v3/keras_tuner_pb2_grpc.py
+keras_tuner/protos/v3/service_pb2.py
+keras_tuner/protos/v3/service_pb2_grpc.py
+keras_tuner/protos/v4/__init__.py
+keras_tuner/protos/v4/keras_tuner_pb2.py
+keras_tuner/protos/v4/keras_tuner_pb2_grpc.py
+keras_tuner/protos/v4/service_pb2.py
+keras_tuner/protos/v4/service_pb2_grpc.py
 keras_tuner/tuners/__init__.py
 keras_tuner/tuners/bayesian.py
 keras_tuner/tuners/bayesian_test.py
 keras_tuner/tuners/gridsearch.py
 keras_tuner/tuners/gridsearch_test.py
 keras_tuner/tuners/hyperband.py
 keras_tuner/tuners/hyperband_test.py
```

### Comparing `keras-tuner-1.3.4/setup.cfg` & `keras-tuner-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-tuner-1.3.4/setup.py` & `keras-tuner-1.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 # limitations under the License.
 
 """Setup script."""
 
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 setup(
     name="keras-tuner",
     description="A Hyperparameter Tuning Library for Keras",
     url="https://github.com/keras-team/keras-tuner",
     author="The KerasTuner authors",
     license="Apache License 2.0",
     version=__version__,
     install_requires=[
         "packaging",
-        "tensorflow>=2.0",
         "requests",
         "kt-legacy",
-        "protobuf<=3.20.3",
     ],
     extras_require={
+        "tensorflow": [
+            "tensorflow>=2.0",
+        ],
+        "tensorflow-cpu": [
+            "tensorflow-cpu>=2.0",
+        ],
         "tests": [
             "black",
             "flake8",
             "isort",
             "ipython",
             "pandas",
             "portpicker",
```

