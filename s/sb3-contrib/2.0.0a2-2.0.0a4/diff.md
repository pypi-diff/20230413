# Comparing `tmp/sb3_contrib-2.0.0a2.tar.gz` & `tmp/sb3_contrib-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb3_contrib-2.0.0a2.tar", last modified: Wed Apr  5 18:56:51 2023, max compression
+gzip compressed data, was "sb3_contrib-2.0.0a4.tar", last modified: Thu Apr 13 14:51:19 2023, max compression
```

## Comparing `sb3_contrib-2.0.0a2.tar` & `sb3_contrib-2.0.0a4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.329553 sb3_contrib-2.0.0a2/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1078 2020-09-20 20:10:25.000000 sb3_contrib-2.0.0a2/LICENSE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-05 18:56:51.325553 sb3_contrib-2.0.0a2/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3584 2022-11-28 21:39:26.000000 sb3_contrib-2.0.0a2/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1877 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.317553 sb3_contrib-2.0.0a2/sb3_contrib/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      525 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.317553 sb3_contrib-2.0.0a2/sb3_contrib/ars/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      145 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/ars/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    16834 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/ars/ars.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4299 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/ars/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.317553 sb3_contrib-2.0.0a2/sb3_contrib/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-11-13 12:40:30.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.317553 sb3_contrib-2.0.0a2/sb3_contrib/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      262 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4261 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/envs/invalid_actions_env.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8740 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5744 2023-02-13 13:32:37.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11653 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7006 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    19411 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1080 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17764 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26968 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      778 2023-04-03 13:50:28.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7022 2023-04-03 13:03:38.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       85 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8405 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/vec_env/async_eval.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1139 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/action_masker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4085 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/time_feature.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/ppo_mask/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      208 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_mask/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      294 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_mask/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    24110 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_mask/ppo_mask.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.321553 sb3_contrib-2.0.0a2/sb3_contrib/ppo_recurrent/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      249 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_recurrent/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      313 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_recurrent/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21599 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/ppo_recurrent/ppo_recurrent.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2020-09-25 09:51:52.000000 sb3_contrib-2.0.0a2/sb3_contrib/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.325553 sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      187 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11626 2023-04-05 18:46:59.000000 sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13427 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/qrdqn.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.325553 sb3_contrib-2.0.0a2/sb3_contrib/tqc/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      177 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/tqc/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    23190 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/sb3_contrib/tqc/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15447 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/tqc/tqc.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.325553 sb3_contrib-2.0.0a2/sb3_contrib/trpo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      182 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a2/sb3_contrib/trpo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      302 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a2/sb3_contrib/trpo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20106 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/sb3_contrib/trpo/trpo.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-05 18:19:06.000000 sb3_contrib-2.0.0a2/sb3_contrib/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.317553 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-05 18:56:51.000000 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1893 2023-04-05 18:56:51.000000 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-05 18:56:51.000000 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       27 2023-04-05 18:56:51.000000 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       12 2023-04-05 18:56:51.000000 sb3_contrib-2.0.0a2/sb3_contrib.egg-info/top_level.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-05 18:56:51.329553 sb3_contrib-2.0.0a2/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4146 2023-04-05 18:19:10.000000 sb3_contrib-2.0.0a2/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:56:51.325553 sb3_contrib-2.0.0a2/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7675 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2385 2023-02-13 13:36:17.000000 sb3_contrib-2.0.0a2/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9174 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11090 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a2/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1366 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9645 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_invalid_actions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6862 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_lstm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4994 2023-04-05 18:18:04.000000 sb3_contrib-2.0.0a2/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17613 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9974 2023-04-05 18:18:01.000000 sb3_contrib-2.0.0a2/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2165 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a2/tests/test_utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1078 2020-09-20 20:10:25.000000 sb3_contrib-2.0.0a4/LICENSE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3584 2022-11-28 21:39:26.000000 sb3_contrib-2.0.0a4/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1789 2023-04-13 14:13:11.000000 sb3_contrib-2.0.0a4/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      525 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/ars/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      145 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    16834 2023-04-13 14:13:09.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/ars.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4299 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ars/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-11-13 12:40:30.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      262 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4261 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/envs/invalid_actions_env.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8740 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5744 2023-02-13 13:32:37.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11653 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7006 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    19187 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1080 2021-09-23 13:16:47.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17764 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26968 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      778 2023-04-03 13:50:28.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7022 2023-04-03 13:03:38.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       85 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8405 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/async_eval.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1139 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/action_masker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4085 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/time_feature.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.771164 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      208 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      294 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    24110 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/ppo_mask.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      249 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      313 2022-10-31 12:56:26.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21599 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/ppo_recurrent.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2020-09-25 09:51:52.000000 sb3_contrib-2.0.0a4/sb3_contrib/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      187 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11417 2023-04-13 13:57:06.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14168 2023-04-13 13:57:14.000000 sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/qrdqn.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/tqc/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      177 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    23495 2023-04-13 14:23:36.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15637 2023-04-13 14:22:39.000000 sb3_contrib-2.0.0a4/sb3_contrib/tqc/tqc.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.775164 sb3_contrib-2.0.0a4/sb3_contrib/trpo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      182 2022-12-19 11:07:58.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      302 2022-04-13 18:24:59.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20271 2023-04-13 14:25:24.000000 sb3_contrib-2.0.0a4/sb3_contrib/trpo/trpo.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 13:50:37.000000 sb3_contrib-2.0.0a4/sb3_contrib/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.767164 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3408 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1893 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       27 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       12 2023-04-13 14:51:19.000000 sb3_contrib-2.0.0a4/sb3_contrib.egg-info/top_level.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4146 2023-04-13 14:50:50.000000 sb3_contrib-2.0.0a4/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:51:19.779164 sb3_contrib-2.0.0a4/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7675 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2385 2023-02-13 13:36:17.000000 sb3_contrib-2.0.0a4/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9174 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11090 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a4/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1366 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9645 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_invalid_actions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6862 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_lstm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4994 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17613 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9974 2023-04-12 14:32:51.000000 sb3_contrib-2.0.0a4/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2165 2022-02-22 17:36:32.000000 sb3_contrib-2.0.0a4/tests/test_utils.py
```

### Comparing `sb3_contrib-2.0.0a2/LICENSE` & `sb3_contrib-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/PKG-INFO` & `sb3_contrib-2.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb3_contrib
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: Contrib package of Stable Baselines3, experimental code.
 Home-page: https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: Documentation, https://sb3-contrib.readthedocs.io/
```

### Comparing `sb3_contrib-2.0.0a2/README.md` & `sb3_contrib-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/pyproject.toml` & `sb3_contrib-2.0.0a4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -33,17 +33,14 @@
 	| sb3_contrib/common/recurrent/buffers.py$
 	| sb3_contrib/common/maskable/distributions.py$
 	| sb3_contrib/common/maskable/callbacks.py$
 	| sb3_contrib/common/maskable/policies.py$
 	| sb3_contrib/common/maskable/buffers.py$
 	| sb3_contrib/common/envs/invalid_actions_env.py$
 	| sb3_contrib/common/vec_env/async_eval.py$
-	| sb3_contrib/tqc/tqc.py$
-	| sb3_contrib/tqc/policies.py$
-	| sb3_contrib/trpo/trpo.py$
 	| sb3_contrib/ppo_mask/ppo_mask.py$
 	| tests/test_train_eval_mode.py$
   )"""
 
 [tool.pytest.ini_options]
 # Deterministic ordering for tests; useful for pytest-xdist.
 env = [
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/__init__.py` & `sb3_contrib-2.0.0a4/sb3_contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/ars/ars.py` & `sb3_contrib-2.0.0a4/sb3_contrib/ars/ars.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/ars/policies.py` & `sb3_contrib-2.0.0a4/sb3_contrib/ars/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/envs/invalid_actions_env.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/envs/invalid_actions_env.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/buffers.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/buffers.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/callbacks.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/callbacks.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/distributions.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/distributions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/evaluation.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/evaluation.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/policies.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,20 +266,14 @@
         :param state: The last states (can be None, used in recurrent policies)
         :param episode_start: The last masks (can be None, used in recurrent policies)
         :param deterministic: Whether or not to return deterministic actions.
         :param action_masks: Action masks to apply to the action distribution
         :return: the model's action and the next state
             (used in recurrent policies)
         """
-        # TODO (GH/1): add support for RNN policies
-        # if state is None:
-        #     state = self.initial_state
-        # if episode_start is None:
-        #     episode_start = [False for _ in range(self.n_envs)]
-
         # Switch to eval mode (this affects batch norm / dropout)
         self.set_training_mode(False)
 
         observation, vectorized_env = self.obs_to_tensor(observation)
 
         with th.no_grad():
             actions = self._predict(observation, deterministic=deterministic, action_masks=action_masks)
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/maskable/utils.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/maskable/utils.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/buffers.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/buffers.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/policies.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/policies.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/recurrent/type_aliases.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/recurrent/type_aliases.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/utils.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/utils.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/vec_env/async_eval.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/vec_env/async_eval.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/action_masker.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/action_masker.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/common/wrappers/time_feature.py` & `sb3_contrib-2.0.0a4/sb3_contrib/common/wrappers/time_feature.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/ppo_mask/ppo_mask.py` & `sb3_contrib-2.0.0a4/sb3_contrib/ppo_mask/ppo_mask.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/ppo_recurrent/ppo_recurrent.py` & `sb3_contrib-2.0.0a4/sb3_contrib/ppo_recurrent/ppo_recurrent.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/policies.py` & `sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     :param n_quantiles: Number of quantiles
     :param net_arch: The specification of the network architecture.
     :param activation_fn: Activation function
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     """
 
+    action_space: spaces.Discrete
+
     def __init__(
         self,
         observation_space: spaces.Space,
         action_space: spaces.Discrete,
         features_extractor: BaseFeaturesExtractor,
         features_dim: int,
         n_quantiles: int = 200,
@@ -48,29 +50,25 @@
         if net_arch is None:
             net_arch = [64, 64]
 
         self.net_arch = net_arch
         self.activation_fn = activation_fn
         self.features_dim = features_dim
         self.n_quantiles = n_quantiles
-        assert isinstance(self.action_space, spaces.Discrete)
         action_dim = int(self.action_space.n)  # number of actions
         quantile_net = create_mlp(self.features_dim, action_dim * self.n_quantiles, self.net_arch, self.activation_fn)
         self.quantile_net = nn.Sequential(*quantile_net)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         """
         Predict the quantiles.
 
         :param obs: Observation
         :return: The estimated quantiles for each action.
         """
-        # For type checker:
-        assert isinstance(self.features_extractor, BaseFeaturesExtractor)
-        assert isinstance(self.action_space, spaces.Discrete)
         quantiles = self.quantile_net(self.extract_features(obs, self.features_extractor))
         return quantiles.view(-1, self.n_quantiles, int(self.action_space.n))
 
     def _predict(self, observation: th.Tensor, deterministic: bool = True) -> th.Tensor:
         q_values = self(observation).mean(dim=1)
         # Greedy action
         action = q_values.argmax(dim=1).reshape(-1)
@@ -108,14 +106,17 @@
          dividing by 255.0 (True by default)
     :param optimizer_class: The optimizer to use,
         ``th.optim.Adam`` by default
     :param optimizer_kwargs: Additional keyword arguments,
         excluding the learning rate, to pass to the optimizer
     """
 
+    quantile_net: QuantileNetwork
+    quantile_net_target: QuantileNetwork
+
     def __init__(
         self,
         observation_space: spaces.Space,
         action_space: spaces.Discrete,
         lr_schedule: Schedule,
         n_quantiles: int = 200,
         net_arch: Optional[List[int]] = None,
@@ -150,17 +151,14 @@
             "observation_space": self.observation_space,
             "action_space": self.action_space,
             "n_quantiles": self.n_quantiles,
             "net_arch": self.net_arch,
             "activation_fn": self.activation_fn,
             "normalize_images": normalize_images,
         }
-
-        self.quantile_net: QuantileNetwork
-        self.quantile_net_target: QuantileNetwork
         self._build(lr_schedule)
 
     def _build(self, lr_schedule: Schedule) -> None:
         """
         Create the network and the optimizer.
 
         :param lr_schedule: Learning rate schedule
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/qrdqn/qrdqn.py` & `sb3_contrib-2.0.0a4/sb3_contrib/qrdqn/qrdqn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import warnings
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 import torch as th
 from gymnasium import spaces
 from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 from stable_baselines3.common.utils import get_linear_fn, get_parameters_by_name, polyak_update
 
 from sb3_contrib.common.utils import quantile_huber_loss
-from sb3_contrib.qrdqn.policies import CnnPolicy, MlpPolicy, MultiInputPolicy, QRDQNPolicy
+from sb3_contrib.qrdqn.policies import CnnPolicy, MlpPolicy, MultiInputPolicy, QRDQNPolicy, QuantileNetwork
 
 SelfQRDQN = TypeVar("SelfQRDQN", bound="QRDQN")
 
 
 class QRDQN(OffPolicyAlgorithm):
     """
     Quantile Regression Deep Q-Network (QR-DQN)
@@ -60,14 +61,19 @@
     """
 
     policy_aliases: Dict[str, Type[BasePolicy]] = {
         "MlpPolicy": MlpPolicy,
         "CnnPolicy": CnnPolicy,
         "MultiInputPolicy": MultiInputPolicy,
     }
+    # Linear schedule will be defined in `_setup_model()`
+    exploration_schedule: Schedule
+    quantile_net: QuantileNetwork
+    quantile_net_target: QuantileNetwork
+    policy: QRDQNPolicy
 
     def __init__(
         self,
         policy: Union[str, Type[QRDQNPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 5e-5,
         buffer_size: int = 1000000,  # 1e6
@@ -119,21 +125,19 @@
             support_multi_env=True,
         )
 
         self.exploration_initial_eps = exploration_initial_eps
         self.exploration_final_eps = exploration_final_eps
         self.exploration_fraction = exploration_fraction
         self.target_update_interval = target_update_interval
+        # For updating the target network with multiple envs:
+        self._n_calls = 0
         self.max_grad_norm = max_grad_norm
         # "epsilon" for the epsilon-greedy exploration
         self.exploration_rate = 0.0
-        # Linear schedule will be defined in `_setup_model()`
-        self.exploration_schedule: Schedule
-        self.quantile_net: th.nn.Module
-        self.quantile_net_target: th.nn.Module
 
         if "optimizer_class" not in self.policy_kwargs:
             self.policy_kwargs["optimizer_class"] = th.optim.Adam
             # Proposed in the QR-DQN paper where `batch_size = 32`
             self.policy_kwargs["optimizer_kwargs"] = dict(eps=0.01 / batch_size)
 
         if _init_setup_model:
@@ -144,28 +148,39 @@
         self._create_aliases()
         # Copy running stats, see https://github.com/DLR-RM/stable-baselines3/issues/996
         self.batch_norm_stats = get_parameters_by_name(self.quantile_net, ["running_"])
         self.batch_norm_stats_target = get_parameters_by_name(self.quantile_net_target, ["running_"])
         self.exploration_schedule = get_linear_fn(
             self.exploration_initial_eps, self.exploration_final_eps, self.exploration_fraction
         )
+        # Account for multiple environments
+        # each call to step() corresponds to n_envs transitions
+        if self.n_envs > 1:
+            if self.n_envs > self.target_update_interval:
+                warnings.warn(
+                    "The number of environments used is greater than the target network "
+                    f"update interval ({self.n_envs} > {self.target_update_interval}), "
+                    "therefore the target network will be updated after each call to env.step() "
+                    f"which corresponds to {self.n_envs} steps."
+                )
+
+            self.target_update_interval = max(self.target_update_interval // self.n_envs, 1)
 
     def _create_aliases(self) -> None:
-        # For type checker:
-        assert isinstance(self.policy, QRDQNPolicy)
         self.quantile_net = self.policy.quantile_net
         self.quantile_net_target = self.policy.quantile_net_target
         self.n_quantiles = self.policy.n_quantiles
 
     def _on_step(self) -> None:
         """
         Update the exploration rate and target network if needed.
         This method is called in ``collect_rollouts()`` after each step in the environment.
         """
-        if self.num_timesteps % self.target_update_interval == 0:
+        self._n_calls += 1
+        if self._n_calls % self.target_update_interval == 0:
             polyak_update(self.quantile_net.parameters(), self.quantile_net_target.parameters(), self.tau)
             # Copy running stats, see https://github.com/DLR-RM/stable-baselines3/issues/996
             polyak_update(self.batch_norm_stats, self.batch_norm_stats_target, 1.0)
 
         self.exploration_rate = self.exploration_schedule(self._current_progress_remaining)
         self.logger.record("rollout/exploration_rate", self.exploration_rate)
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/tqc/policies.py` & `sb3_contrib-2.0.0a4/sb3_contrib/tqc/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,20 @@
         a positive standard deviation (cf paper). It allows to keep variance
         above zero and prevent it from growing too fast. In practice, ``exp()`` is usually enough.
     :param clip_mean: Clip the mean output when using gSDE to avoid numerical instability.
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     """
 
+    action_space: spaces.Box
+
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         net_arch: List[int],
         features_extractor: nn.Module,
         features_dim: int,
         activation_fn: Type[nn.Module] = nn.ReLU,
         use_sde: bool = False,
         log_std_init: float = -3,
         full_std: bool = True,
@@ -91,17 +93,17 @@
                 latent_dim=last_layer_dim, latent_sde_dim=last_layer_dim, log_std_init=log_std_init
             )
             # Avoid numerical issues by limiting the mean of the Gaussian
             # to be in [-clip_mean, clip_mean]
             if clip_mean > 0.0:
                 self.mu = nn.Sequential(self.mu, nn.Hardtanh(min_val=-clip_mean, max_val=clip_mean))
         else:
-            self.action_dist = SquashedDiagGaussianDistribution(action_dim)
+            self.action_dist = SquashedDiagGaussianDistribution(action_dim)  # type: ignore[assignment]
             self.mu = nn.Linear(last_layer_dim, action_dim)
-            self.log_std = nn.Linear(last_layer_dim, action_dim)
+            self.log_std = nn.Linear(last_layer_dim, action_dim)  # type: ignore[assignment]
 
     def _get_constructor_parameters(self) -> Dict[str, Any]:
         data = super()._get_constructor_parameters()
 
         data.update(
             dict(
                 net_arch=self.net_arch,
@@ -152,15 +154,15 @@
         features = self.extract_features(obs, self.features_extractor)
         latent_pi = self.latent_pi(features)
         mean_actions = self.mu(latent_pi)
 
         if self.use_sde:
             return mean_actions, self.log_std, dict(latent_sde=latent_pi)
         # Unstructured exploration (Original implementation)
-        log_std = self.log_std(latent_pi)
+        log_std = self.log_std(latent_pi)  # type: ignore[operator]
         # Original Implementation to cap the standard deviation
         log_std = th.clamp(log_std, LOG_STD_MIN, LOG_STD_MAX)
         return mean_actions, log_std, {}
 
     def forward(self, obs: th.Tensor, deterministic: bool = False) -> th.Tensor:
         mean_actions, log_std, kwargs = self.get_action_dist_params(obs)
         # Note: the action is squashed
@@ -188,20 +190,23 @@
     :param activation_fn: Activation function
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     :param share_features_extractor: Whether the features extractor is shared or not
         between the actor and the critic (this saves computation time)
     """
 
+    action_space: spaces.Box
+    features_extractor: BaseFeaturesExtractor
+
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         net_arch: List[int],
-        features_extractor: nn.Module,
+        features_extractor: BaseFeaturesExtractor,
         features_dim: int,
         activation_fn: Type[nn.Module] = nn.ReLU,
         normalize_images: bool = True,
         n_quantiles: int = 25,
         n_critics: int = 2,
         share_features_extractor: bool = False,
     ):
@@ -217,20 +222,20 @@
         self.share_features_extractor = share_features_extractor
         self.q_networks = []
         self.n_quantiles = n_quantiles
         self.n_critics = n_critics
         self.quantiles_total = n_quantiles * n_critics
 
         for i in range(n_critics):
-            qf_net = create_mlp(features_dim + action_dim, n_quantiles, net_arch, activation_fn)
-            qf_net = nn.Sequential(*qf_net)
+            qf_net_list = create_mlp(features_dim + action_dim, n_quantiles, net_arch, activation_fn)
+            qf_net = nn.Sequential(*qf_net_list)
             self.add_module(f"qf{i}", qf_net)
             self.q_networks.append(qf_net)
 
-    def forward(self, obs: th.Tensor, action: th.Tensor) -> List[th.Tensor]:
+    def forward(self, obs: th.Tensor, action: th.Tensor) -> th.Tensor:
         # Learn the features extractor using the policy loss only
         # when the features_extractor is shared with the actor
         with th.set_grad_enabled(not self.share_features_extractor):
             features = self.extract_features(obs, self.features_extractor)
         qvalue_input = th.cat([features, action], dim=1)
         quantiles = th.stack(tuple(qf(qvalue_input) for qf in self.q_networks), dim=1)
         return quantiles
@@ -262,18 +267,22 @@
         excluding the learning rate, to pass to the optimizer
     :param n_quantiles: Number of quantiles for the critic.
     :param n_critics: Number of critic networks to create.
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
+    actor: Actor
+    critic: Critic
+    critic_target: Critic
+
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
         use_sde: bool = False,
         log_std_init: float = -3,
         use_expln: bool = False,
         clip_mean: float = 2.0,
@@ -324,43 +333,49 @@
         tqc_kwargs = {
             "n_quantiles": n_quantiles,
             "n_critics": n_critics,
             "net_arch": critic_arch,
             "share_features_extractor": share_features_extractor,
         }
         self.critic_kwargs.update(tqc_kwargs)
-        self.actor, self.actor_target = None, None
-        self.critic, self.critic_target = None, None
         self.share_features_extractor = share_features_extractor
 
         self._build(lr_schedule)
 
     def _build(self, lr_schedule: Schedule) -> None:
         self.actor = self.make_actor()
-        self.actor.optimizer = self.optimizer_class(self.actor.parameters(), lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.actor.optimizer = self.optimizer_class(  # type: ignore[call-arg]
+            self.actor.parameters(),
+            lr=lr_schedule(1),
+            **self.optimizer_kwargs,
+        )
 
         if self.share_features_extractor:
             self.critic = self.make_critic(features_extractor=self.actor.features_extractor)
             # Do not optimize the shared features extractor with the critic loss
             # otherwise, there are gradient computation issues
             critic_parameters = [param for name, param in self.critic.named_parameters() if "features_extractor" not in name]
         else:
             # Create a separate features extractor for the critic
             # this requires more memory and computation
             self.critic = self.make_critic(features_extractor=None)
-            critic_parameters = self.critic.parameters()
+            critic_parameters = list(self.critic.parameters())
 
         # Critic target should not share the feature extactor with critic
         self.critic_target = self.make_critic(features_extractor=None)
         self.critic_target.load_state_dict(self.critic.state_dict())
 
         # Target networks should always be in eval mode
         self.critic_target.set_training_mode(False)
 
-        self.critic.optimizer = self.optimizer_class(critic_parameters, lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.critic.optimizer = self.optimizer_class(  # type: ignore[call-arg]
+            critic_parameters,
+            lr=lr_schedule(1),
+            **self.optimizer_kwargs,
+        )
 
     def _get_constructor_parameters(self) -> Dict[str, Any]:
         data = super()._get_constructor_parameters()
 
         data.update(
             dict(
                 net_arch=self.net_arch,
@@ -443,15 +458,15 @@
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
         use_sde: bool = False,
         log_std_init: float = -3,
         use_expln: bool = False,
         clip_mean: float = 2.0,
@@ -512,15 +527,15 @@
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
         use_sde: bool = False,
         log_std_init: float = -3,
         use_expln: bool = False,
         clip_mean: float = 2.0,
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/tqc/tqc.py` & `sb3_contrib-2.0.0a4/sb3_contrib/tqc/tqc.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback
 from stable_baselines3.common.utils import get_parameters_by_name, polyak_update
 
 from sb3_contrib.common.utils import quantile_huber_loss
-from sb3_contrib.tqc.policies import CnnPolicy, MlpPolicy, MultiInputPolicy, TQCPolicy
+from sb3_contrib.tqc.policies import Actor, CnnPolicy, Critic, MlpPolicy, MultiInputPolicy, TQCPolicy
 
 SelfTQC = TypeVar("SelfTQC", bound="TQC")
 
 
 class TQC(OffPolicyAlgorithm):
     """
 
@@ -69,29 +69,33 @@
     """
 
     policy_aliases: Dict[str, Type[BasePolicy]] = {
         "MlpPolicy": MlpPolicy,
         "CnnPolicy": CnnPolicy,
         "MultiInputPolicy": MultiInputPolicy,
     }
+    policy: TQCPolicy
+    actor: Actor
+    critic: Critic
+    critic_target: Critic
 
     def __init__(
         self,
         policy: Union[str, Type[TQCPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Callable] = 3e-4,
         buffer_size: int = 1000000,  # 1e6
         learning_starts: int = 100,
         batch_size: int = 256,
         tau: float = 0.005,
         gamma: float = 0.99,
         train_freq: int = 1,
         gradient_steps: int = 1,
         action_noise: Optional[ActionNoise] = None,
-        replay_buffer_class: Optional[ReplayBuffer] = None,
+        replay_buffer_class: Optional[Type[ReplayBuffer]] = None,
         replay_buffer_kwargs: Optional[Dict[str, Any]] = None,
         optimize_memory_usage: bool = False,
         ent_coef: Union[str, float] = "auto",
         target_update_interval: int = 1,
         target_entropy: Union[str, float] = "auto",
         top_quantiles_to_drop_per_net: int = 2,
         use_sde: bool = False,
@@ -135,15 +139,15 @@
 
         self.target_entropy = target_entropy
         self.log_ent_coef = None  # type: Optional[th.Tensor]
         # Entropy coefficient / Entropy temperature
         # Inverse of the reward scale
         self.ent_coef = ent_coef
         self.target_update_interval = target_update_interval
-        self.ent_coef_optimizer = None
+        self.ent_coef_optimizer: Optional[th.optim.Adam] = None
         self.top_quantiles_to_drop_per_net = top_quantiles_to_drop_per_net
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
@@ -151,15 +155,15 @@
         # Running mean and running var
         self.batch_norm_stats = get_parameters_by_name(self.critic, ["running_"])
         self.batch_norm_stats_target = get_parameters_by_name(self.critic_target, ["running_"])
 
         # Target entropy is used when learning the entropy coefficient
         if self.target_entropy == "auto":
             # automatically set target entropy if needed
-            self.target_entropy = -np.prod(self.env.action_space.shape).astype(np.float32)
+            self.target_entropy = -np.prod(self.env.action_space.shape).astype(np.float32)  # type: ignore
         else:
             # Force conversion
             # this will also throw an error for unexpected string
             self.target_entropy = float(self.target_entropy)
 
         # The entropy coefficient or entropy can be learned automatically
         # see Automating Entropy Adjustment for Maximum Entropy RL section
@@ -198,41 +202,40 @@
         self._update_learning_rate(optimizers)
 
         ent_coef_losses, ent_coefs = [], []
         actor_losses, critic_losses = [], []
 
         for gradient_step in range(gradient_steps):
             # Sample replay buffer
-            replay_data = self.replay_buffer.sample(batch_size, env=self._vec_normalize_env)
+            replay_data = self.replay_buffer.sample(batch_size, env=self._vec_normalize_env)  # type: ignore[union-attr]
 
             # We need to sample because `log_std` may have changed between two gradient steps
             if self.use_sde:
                 self.actor.reset_noise()
 
             # Action by the current actor for the sampled state
             actions_pi, log_prob = self.actor.action_log_prob(replay_data.observations)
             log_prob = log_prob.reshape(-1, 1)
 
             ent_coef_loss = None
-            if self.ent_coef_optimizer is not None:
+            if self.ent_coef_optimizer is not None and self.log_ent_coef is not None:
                 # Important: detach the variable from the graph
                 # so we don't change it with other losses
                 # see https://github.com/rail-berkeley/softlearning/issues/60
                 ent_coef = th.exp(self.log_ent_coef.detach())
                 ent_coef_loss = -(self.log_ent_coef * (log_prob + self.target_entropy).detach()).mean()
                 ent_coef_losses.append(ent_coef_loss.item())
             else:
                 ent_coef = self.ent_coef_tensor
 
             ent_coefs.append(ent_coef.item())
-            self.replay_buffer.ent_coef = ent_coef.item()
 
             # Optimize entropy coefficient, also called
             # entropy temperature or alpha in the paper
-            if ent_coef_loss is not None:
+            if ent_coef_loss is not None and self.ent_coef_optimizer is not None:
                 self.ent_coef_optimizer.zero_grad()
                 ent_coef_loss.backward()
                 self.ent_coef_optimizer.step()
 
             with th.no_grad():
                 # Select action according to policy
                 next_actions, next_log_prob = self.actor.action_log_prob(replay_data.next_observations)
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib/trpo/trpo.py` & `sb3_contrib-2.0.0a4/sb3_contrib/trpo/trpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,24 +174,24 @@
 
         :param kl_div: The KL divergence objective
         :param policy_objective: The surrogate objective ("classic" policy gradient)
         :return: List of actor params, gradients and gradients shape.
         """
         # This is necessary because not all the parameters in the policy have gradients w.r.t. the KL divergence
         # The policy objective is also called surrogate objective
-        policy_objective_gradients = []
+        policy_objective_gradients_list = []
         # Contains the gradients of the KL divergence
-        grad_kl = []
+        grad_kl_list = []
         # Contains the shape of the gradients of the KL divergence w.r.t each parameter
         # This way the flattened gradient can be reshaped back into the original shapes and applied to
         # the parameters
-        grad_shape = []
+        grad_shape: List[Tuple[int, ...]] = []
         # Contains the parameters which have non-zeros KL divergence gradients
         # The list is used during the line-search to apply the step to each parameters
-        actor_params = []
+        actor_params: List[nn.Parameter] = []
 
         for name, param in self.policy.named_parameters():
             # Skip parameters related to value function based on name
             # this work for built-in policies only (not custom ones)
             if "value" in name:
                 continue
 
@@ -209,21 +209,21 @@
             if kl_param_grad is not None:
                 # If the parameter impacts the KL divergence (i.e. the policy)
                 # we compute the gradient of the policy objective w.r.t to the parameter
                 # this avoids computing the gradient if it's not going to be used in the conjugate gradient step
                 policy_objective_grad, *_ = th.autograd.grad(policy_objective, param, retain_graph=True, only_inputs=True)
 
                 grad_shape.append(kl_param_grad.shape)
-                grad_kl.append(kl_param_grad.reshape(-1))
-                policy_objective_gradients.append(policy_objective_grad.reshape(-1))
+                grad_kl_list.append(kl_param_grad.reshape(-1))
+                policy_objective_gradients_list.append(policy_objective_grad.reshape(-1))
                 actor_params.append(param)
 
         # Gradients are concatenated before the conjugate gradient step
-        policy_objective_gradients = th.cat(policy_objective_gradients)
-        grad_kl = th.cat(grad_kl)
+        policy_objective_gradients = th.cat(policy_objective_gradients_list)
+        grad_kl = th.cat(grad_kl_list)
         return actor_params, policy_objective_gradients, grad_kl, grad_shape
 
     def train(self) -> None:
         """
         Update policy using the currently gathered rollout buffer.
         """
         # Switch to train mode (this affects batch norm / dropout)
@@ -239,18 +239,18 @@
         # This will only loop once (get all data in one go)
         for rollout_data in self.rollout_buffer.get(batch_size=None):
             # Optional: sub-sample data for faster computation
             if self.sub_sampling_factor > 1:
                 rollout_data = RolloutBufferSamples(
                     rollout_data.observations[:: self.sub_sampling_factor],
                     rollout_data.actions[:: self.sub_sampling_factor],
-                    None,  # old values, not used here
+                    None,  # type: ignore[arg-type]  # old values, not used here
                     rollout_data.old_log_prob[:: self.sub_sampling_factor],
                     rollout_data.advantages[:: self.sub_sampling_factor],
-                    None,  # returns, not used here
+                    None,  # type: ignore[arg-type]  # returns, not used here
                 )
 
             actions = rollout_data.actions
             if isinstance(self.action_space, spaces.Discrete):
                 # Convert discrete action from float to long
                 actions = rollout_data.actions.long().flatten()
 
@@ -297,15 +297,15 @@
             )
 
             # Maximal step length
             line_search_max_step_size = 2 * self.target_kl
             line_search_max_step_size /= th.matmul(
                 search_direction, hessian_vector_product_fn(search_direction, retain_graph=False)
             )
-            line_search_max_step_size = th.sqrt(line_search_max_step_size)
+            line_search_max_step_size = th.sqrt(line_search_max_step_size)  # type: ignore[assignment, arg-type]
 
             line_search_backtrack_coeff = 1.0
             original_actor_params = [param.detach().clone() for param in actor_params]
 
             is_line_search_success = False
             with th.no_grad():
                 # Line-search (backtracking)
@@ -347,15 +347,15 @@
 
                 if not is_line_search_success:
                     # If the line-search wasn't successful we revert to the original parameters
                     for param, original_param in zip(actor_params, original_actor_params):
                         param.data = original_param.data.clone()
 
                     policy_objective_values.append(policy_objective.item())
-                    kl_divergences.append(0)
+                    kl_divergences.append(0.0)
                 else:
                     policy_objective_values.append(new_policy_objective.item())
                     kl_divergences.append(kl_div.item())
 
         # Critic update
         for _ in range(self.n_critic_updates):
             for rollout_data in self.rollout_buffer.get(self.batch_size):
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib.egg-info/PKG-INFO` & `sb3_contrib-2.0.0a4/sb3_contrib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb3-contrib
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: Contrib package of Stable Baselines3, experimental code.
 Home-page: https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
 Project-URL: Documentation, https://sb3-contrib.readthedocs.io/
```

### Comparing `sb3_contrib-2.0.0a2/sb3_contrib.egg-info/SOURCES.txt` & `sb3_contrib-2.0.0a4/sb3_contrib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/setup.py` & `sb3_contrib-2.0.0a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 setup(
     name="sb3_contrib",
     packages=[package for package in find_packages() if package.startswith("sb3_contrib")],
     package_data={"sb3_contrib": ["py.typed", "version.txt"]},
     install_requires=[
-        "stable_baselines3>=2.0.0a2",
+        "stable_baselines3>=2.0.0a4",
     ],
     description="Contrib package of Stable Baselines3, experimental code.",
     author="Antonin Raffin",
     url="https://github.com/Stable-Baselines-Team/stable-baselines3-contrib",
     author_email="antonin.raffin@dlr.de",
     keywords="reinforcement-learning-algorithms reinforcement-learning machine-learning "
     "gym openai stable baselines toolbox python data-science",
```

### Comparing `sb3_contrib-2.0.0a2/tests/test_cnn.py` & `sb3_contrib-2.0.0a4/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_deterministic.py` & `sb3_contrib-2.0.0a4/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_dict_env.py` & `sb3_contrib-2.0.0a4/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_distributions.py` & `sb3_contrib-2.0.0a4/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_identity.py` & `sb3_contrib-2.0.0a4/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_invalid_actions.py` & `sb3_contrib-2.0.0a4/tests/test_invalid_actions.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_lstm.py` & `sb3_contrib-2.0.0a4/tests/test_lstm.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_run.py` & `sb3_contrib-2.0.0a4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_save_load.py` & `sb3_contrib-2.0.0a4/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_train_eval_mode.py` & `sb3_contrib-2.0.0a4/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `sb3_contrib-2.0.0a2/tests/test_utils.py` & `sb3_contrib-2.0.0a4/tests/test_utils.py`

 * *Files identical despite different names*

