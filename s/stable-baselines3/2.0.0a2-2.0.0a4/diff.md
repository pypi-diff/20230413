# Comparing `tmp/stable_baselines3-2.0.0a2.tar.gz` & `tmp/stable_baselines3-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable_baselines3-2.0.0a2.tar", last modified: Wed Apr  5 18:36:12 2023, max compression
+gzip compressed data, was "stable_baselines3-2.0.0a4.tar", last modified: Thu Apr 13 14:50:21 2023, max compression
```

## Comparing `stable_baselines3-2.0.0a2.tar` & `stable_baselines3-2.0.0a4.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.128048 stable_baselines3-2.0.0a2/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a2/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a2/NOTICE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-05 18:36:12.128048 stable_baselines3-2.0.0a2/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14112 2023-03-29 22:22:11.000000 stable_baselines3-2.0.0a2/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3280 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/pyproject.toml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-05 18:36:12.128048 stable_baselines3-2.0.0a2/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5706 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.112048 stable_baselines3-2.0.0a2/stable_baselines3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.112048 stable_baselines3-2.0.0a2/stable_baselines3/a2c/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/a2c/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/a2c/a2c.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a2/stable_baselines3/a2c/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.116048 stable_baselines3-2.0.0a2/stable_baselines3/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/atari_wrappers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    36580 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/base_class.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    33738 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26477 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    27288 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20728 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7539 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/env_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.116048 stable_baselines3-2.0.0a2/stable_baselines3/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8103 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/envs/bit_flipping_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6033 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/envs/identity_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6453 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/envs/multi_input_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6406 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    23428 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5545 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/noise.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26137 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11643 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    40339 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/results_plotter.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/running_mean_std.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20674 2023-03-19 19:46:04.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/save_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.116048 stable_baselines3-2.0.0a2/stable_baselines3/common/sb2_compat/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/sb2_compat/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5631 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/torch_layers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3182 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20989 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15804 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/base_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7073 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/dummy_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/patch_gym.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8237 2023-04-05 18:12:25.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/stacked_observations.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10631 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/subproc_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2986 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/util.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      755 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2062 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_frame_stack.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3807 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_transpose.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_video_recorder.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a2/stable_baselines3/ddpg/ddpg.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/ddpg/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12993 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10819 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/her/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/her/__init__.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a2/stable_baselines3/her/goal_selection_strategy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-05 18:11:00.000000 stable_baselines3-2.0.0a2/stable_baselines3/her/her_replay_buffer.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a2/stable_baselines3/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14876 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a2/stable_baselines3/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20434 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15538 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.120048 stable_baselines3-2.0.0a2/stable_baselines3/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/stable_baselines3/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14330 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/stable_baselines3/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10957 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/stable_baselines3/td3/td3.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-05 18:06:08.000000 stable_baselines3-2.0.0a2/stable_baselines3/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.112048 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-05 18:36:12.000000 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-04-05 18:36:12.000000 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-05 18:36:12.000000 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      744 2023-04-05 18:36:12.000000 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-04-05 18:36:12.000000 stable_baselines3-2.0.0a2/stable_baselines3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-05 18:36:12.124048 stable_baselines3-2.0.0a2/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5687 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/tests/test_custom_policy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a2/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3739 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9887 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_gae.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-05 18:19:07.000000 stable_baselines3-2.0.0a2/tests/test_her.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14793 2023-04-05 18:05:58.000000 stable_baselines3-2.0.0a2/tests/test_logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3756 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_predict.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26907 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a2/tests/test_sde.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4338 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_spaces.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a2/tests/test_tensorboard.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22564 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1389 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20064 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1457 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-05 18:05:55.000000 stable_baselines3-2.0.0a2/tests/test_vec_stacked_obs.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a4/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a4/NOTICE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14112 2023-03-29 22:22:11.000000 stable_baselines3-2.0.0a4/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2893 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/pyproject.toml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5706 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3/a2c/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/a2c.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/atari_wrappers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    37082 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/base_class.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    33755 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26487 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27242 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20619 2023-04-13 10:43:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7539 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/env_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8099 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/bit_flipping_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/identity_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6449 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/multi_input_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    23428 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5545 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/noise.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26104 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12001 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    40200 2023-04-13 14:18:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/results_plotter.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/running_mean_std.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20664 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/save_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5631 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/torch_layers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3117 2023-04-13 13:46:31.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20971 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15814 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/base_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7073 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/patch_gym.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8298 2023-04-13 10:53:06.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/stacked_observations.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10631 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2986 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/util.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-12 13:21:02.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2062 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3807 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_transpose.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/ddpg.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12908 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10673 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/her/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/goal_selection_strategy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/her_replay_buffer.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14928 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20669 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15920 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14471 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11193 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/td3.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 13:45:04.000000 stable_baselines3-2.0.0a4/stable_baselines3/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      744 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5687 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/tests/test_custom_policy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a4/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3739 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9887 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_gae.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_her.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14793 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3756 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_predict.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26907 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a4/tests/test_sde.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4338 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_spaces.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/tests/test_tensorboard.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22809 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1389 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20064 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2231 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_stacked_obs.py
```

### Comparing `stable_baselines3-2.0.0a2/LICENSE` & `stable_baselines3-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/NOTICE` & `stable_baselines3-2.0.0a4/NOTICE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/PKG-INFO` & `stable_baselines3-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.0.0a2/README.md` & `stable_baselines3-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/pyproject.toml` & `stable_baselines3-2.0.0a4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -31,25 +31,22 @@
 disable = ["pyi-error"]
 
 [tool.mypy]
 ignore_missing_imports = true
 follow_imports = "silent"
 show_error_codes = true
 exclude = """(?x)(
-    stable_baselines3/a2c/a2c.py$
-    | stable_baselines3/common/base_class.py$
-    | stable_baselines3/common/buffers.py$
+    stable_baselines3/common/buffers.py$
     | stable_baselines3/common/callbacks.py$
     | stable_baselines3/common/distributions.py$
     | stable_baselines3/common/envs/bit_flipping_env.py$
     | stable_baselines3/common/envs/identity_env.py$
     | stable_baselines3/common/envs/multi_input_envs.py$
     | stable_baselines3/common/logger.py$
     | stable_baselines3/common/off_policy_algorithm.py$
-    | stable_baselines3/common/on_policy_algorithm.py$
     | stable_baselines3/common/policies.py$
     | stable_baselines3/common/save_util.py$
     | stable_baselines3/common/sb2_compat/rmsprop_tf_like.py$
     | stable_baselines3/common/utils.py$
     | stable_baselines3/common/vec_env/__init__.py$
     | stable_baselines3/common/vec_env/base_vec_env.py$
     | stable_baselines3/common/vec_env/dummy_vec_env.py$
@@ -58,19 +55,14 @@
     | stable_baselines3/common/vec_env/vec_extract_dict_obs.py$
     | stable_baselines3/common/vec_env/vec_frame_stack.py$
     | stable_baselines3/common/vec_env/vec_monitor.py$
     | stable_baselines3/common/vec_env/vec_normalize.py$
     | stable_baselines3/common/vec_env/vec_transpose.py$
     | stable_baselines3/common/vec_env/vec_video_recorder.py$
     | stable_baselines3/her/her_replay_buffer.py$
-    | stable_baselines3/ppo/ppo.py$
-    | stable_baselines3/sac/policies.py$
-    | stable_baselines3/sac/sac.py$
-    | stable_baselines3/td3/policies.py$
-    | stable_baselines3/td3/td3.py$
     | tests/test_logger.py$
     | tests/test_train_eval_mode.py$
   )"""
 
 [tool.pytest.ini_options]
 # Deterministic ordering for tests; useful for pytest-xdist.
 env = [
@@ -78,15 +70,14 @@
 ]
 
 filterwarnings = [
     # Tensorboard warnings
     "ignore::DeprecationWarning:tensorboard",
     # Gymnasium warnings
     "ignore::UserWarning:gymnasium",
-    # "ignore::DeprecationWarning:.*passive_env_checker.*",
 ]
 markers = [
     "expensive: marks tests as expensive (deselect with '-m \"not expensive\"')"
 ]
 
 [tool.coverage.run]
 disable_warnings = ["couldnt-parse"]
```

### Comparing `stable_baselines3-2.0.0a2/setup.py` & `stable_baselines3-2.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/__init__.py` & `stable_baselines3-2.0.0a4/stable_baselines3/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/a2c/a2c.py` & `stable_baselines3-2.0.0a4/stable_baselines3/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/atari_wrappers.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/base_class.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/base_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from stable_baselines3.common.env_util import is_wrapped
 from stable_baselines3.common.logger import Logger
 from stable_baselines3.common.monitor import Monitor
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.preprocessing import check_for_nested_spaces, is_image_space, is_image_space_channels_first
 from stable_baselines3.common.save_util import load_from_zip_file, recursive_getattr, recursive_setattr, save_to_zip_file
-from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
+from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule, TensorDict
 from stable_baselines3.common.utils import (
     check_for_correct_spaces,
     get_device,
     get_schedule_fn,
     get_system_info,
     set_random_seed,
     update_learning_rate,
@@ -40,29 +40,30 @@
     unwrap_vec_normalize,
 )
 from stable_baselines3.common.vec_env.patch_gym import _convert_space, _patch_env
 
 SelfBaseAlgorithm = TypeVar("SelfBaseAlgorithm", bound="BaseAlgorithm")
 
 
-def maybe_make_env(env: Union[GymEnv, str, None], verbose: int) -> Optional[GymEnv]:
+def maybe_make_env(env: Union[GymEnv, str], verbose: int) -> GymEnv:
     """If env is a string, make the environment; otherwise, return env.
 
     :param env: The environment to learn from.
     :param verbose: Verbosity level: 0 for no output, 1 for indicating if envrironment is created
     :return A Gym (vector) environment.
     """
     if isinstance(env, str):
+        env_id = env
         if verbose >= 1:
-            print(f"Creating environment from the given name '{env}'")
+            print(f"Creating environment from the given name '{env_id}'")
         # Set render_mode to `rgb_array` as default, so we can record video
         try:
-            env = gym.make(env, render_mode="rgb_array")
+            env = gym.make(env_id, render_mode="rgb_array")
         except TypeError:
-            env = gym.make(env)
+            env = gym.make(env_id)
     return env
 
 
 class BaseAlgorithm(ABC):
     """
     The base of RL algorithms
 
@@ -91,14 +92,19 @@
         Default: -1 (only sample at the beginning of the rollout)
     :param supported_action_spaces: The action spaces supported by the algorithm.
     """
 
     # Policy aliases (see _get_policy_from_name())
     policy_aliases: Dict[str, Type[BasePolicy]] = {}
     policy: BasePolicy
+    observation_space: spaces.Space
+    action_space: spaces.Space
+    n_envs: int
+    lr_schedule: Schedule
+    _logger: Logger
 
     def __init__(
         self,
         policy: Union[str, Type[BasePolicy]],
         env: Union[GymEnv, str, None],
         learning_rate: Union[float, Schedule],
         policy_kwargs: Optional[Dict[str, Any]] = None,
@@ -107,76 +113,73 @@
         verbose: int = 0,
         device: Union[th.device, str] = "auto",
         support_multi_env: bool = False,
         monitor_wrapper: bool = True,
         seed: Optional[int] = None,
         use_sde: bool = False,
         sde_sample_freq: int = -1,
-        supported_action_spaces: Optional[Tuple[spaces.Space, ...]] = None,
-    ):
+        supported_action_spaces: Optional[Tuple[Type[spaces.Space], ...]] = None,
+    ) -> None:
         if isinstance(policy, str):
             self.policy_class = self._get_policy_from_name(policy)
         else:
             self.policy_class = policy
 
         self.device = get_device(device)
         if verbose >= 1:
             print(f"Using {self.device} device")
 
-        self.env = None  # type: Optional[GymEnv]
-        # get VecNormalize object if needed
-        self._vec_normalize_env = unwrap_vec_normalize(env)
         self.verbose = verbose
         self.policy_kwargs = {} if policy_kwargs is None else policy_kwargs
-        self.observation_space: spaces.Space
-        self.action_space: spaces.Space
-        self.n_envs: int
+
         self.num_timesteps = 0
         # Used for updating schedules
         self._total_timesteps = 0
         # Used for computing fps, it is updated at each call of learn()
         self._num_timesteps_at_start = 0
         self.seed = seed
         self.action_noise: Optional[ActionNoise] = None
-        self.start_time = None
+        self.start_time = 0.0
         self.learning_rate = learning_rate
         self.tensorboard_log = tensorboard_log
-        self.lr_schedule = None  # type: Optional[Schedule]
         self._last_obs = None  # type: Optional[Union[np.ndarray, Dict[str, np.ndarray]]]
         self._last_episode_starts = None  # type: Optional[np.ndarray]
         # When using VecNormalize:
         self._last_original_obs = None  # type: Optional[Union[np.ndarray, Dict[str, np.ndarray]]]
         self._episode_num = 0
         # Used for gSDE only
         self.use_sde = use_sde
         self.sde_sample_freq = sde_sample_freq
         # Track the training progress remaining (from 1 to 0)
         # this is used to update the learning rate
-        self._current_progress_remaining = 1
+        self._current_progress_remaining = 1.0
         # Buffers for logging
         self._stats_window_size = stats_window_size
         self.ep_info_buffer = None  # type: Optional[deque]
         self.ep_success_buffer = None  # type: Optional[deque]
         # For logging (and TD3 delayed updates)
         self._n_updates = 0  # type: int
-        # The logger object
-        self._logger = None  # type: Logger
         # Whether the user passed a custom logger or not
         self._custom_logger = False
+        self.env: Optional[VecEnv] = None
+        self._vec_normalize_env: Optional[VecNormalize] = None
 
         # Create and wrap the env if needed
         if env is not None:
             env = maybe_make_env(env, self.verbose)
             env = self._wrap_env(env, self.verbose, monitor_wrapper)
 
             self.observation_space = env.observation_space
             self.action_space = env.action_space
             self.n_envs = env.num_envs
             self.env = env
 
+            # get VecNormalize object if needed
+            self._vec_normalize_env = unwrap_vec_normalize(env)
+
             if supported_action_spaces is not None:
                 assert isinstance(self.action_space, supported_action_spaces), (
                     f"The algorithm only supports {supported_action_spaces} as action spaces "
                     f"but {self.action_space} was provided"
                 )
 
             if not support_multi_env and self.n_envs > 1:
@@ -213,32 +216,32 @@
             env = _patch_env(env)
             if not is_wrapped(env, Monitor) and monitor_wrapper:
                 if verbose >= 1:
                     print("Wrapping the env with a `Monitor` wrapper")
                 env = Monitor(env)
             if verbose >= 1:
                 print("Wrapping the env in a DummyVecEnv.")
-            env = DummyVecEnv([lambda: env])
+            env = DummyVecEnv([lambda: env])  # type: ignore[list-item, return-value]
 
         # Make sure that dict-spaces are not nested (not supported)
         check_for_nested_spaces(env.observation_space)
 
         if not is_vecenv_wrapped(env, VecTransposeImage):
             wrap_with_vectranspose = False
             if isinstance(env.observation_space, spaces.Dict):
                 # If even one of the keys is a image-space in need of transpose, apply transpose
                 # If the image spaces are not consistent (for instance one is channel first,
                 # the other channel last), VecTransposeImage will throw an error
                 for space in env.observation_space.spaces.values():
                     wrap_with_vectranspose = wrap_with_vectranspose or (
-                        is_image_space(space) and not is_image_space_channels_first(space)
+                        is_image_space(space) and not is_image_space_channels_first(space)  # type: ignore[arg-type]
                     )
             else:
                 wrap_with_vectranspose = is_image_space(env.observation_space) and not is_image_space_channels_first(
-                    env.observation_space
+                    env.observation_space  # type: ignore[arg-type]
                 )
 
             if wrap_with_vectranspose:
                 if verbose >= 1:
                     print("Wrapping the env in a VecTransposeImage.")
                 env = VecTransposeImage(env)
 
@@ -412,15 +415,18 @@
             # Make sure training timesteps are ahead of the internal counter
             total_timesteps += self.num_timesteps
         self._total_timesteps = total_timesteps
         self._num_timesteps_at_start = self.num_timesteps
 
         # Avoid resetting the environment when calling ``.learn()`` consecutive times
         if reset_num_timesteps or self._last_obs is None:
-            self._last_obs = self.env.reset()  # pytype: disable=annotation-type-mismatch
+            assert self.env is not None
+            # pytype: disable=annotation-type-mismatch
+            self._last_obs = self.env.reset()  # type: ignore[assignment]
+            # pytype: enable=annotation-type-mismatch
             self._last_episode_starts = np.ones((self.env.num_envs,), dtype=bool)
             # Retrieve unnormalized observation for saving into the buffer
             if self._vec_normalize_env is not None:
                 self._last_original_obs = self._vec_normalize_env.get_original_obs()
 
         # Configure logger's outputs if no logger was passed
         if not self._custom_logger:
@@ -435,14 +441,17 @@
         """
         Retrieve reward, episode length, episode success and update the buffer
         if using Monitor wrapper or a GoalEnv.
 
         :param infos: List of additional information about the transition.
         :param dones: Termination signals
         """
+        assert self.ep_info_buffer is not None
+        assert self.ep_success_buffer is not None
+
         if dones is None:
             dones = np.array([False] * len(infos))
         for idx, info in enumerate(infos):
             maybe_ep_info = info.get("episode")
             maybe_is_success = info.get("is_success")
             if maybe_ep_info is not None:
                 self.ep_info_buffer.extend([maybe_ep_info])
@@ -558,15 +567,15 @@
         self.action_space.seed(seed)
         # self.env is always a VecEnv
         if self.env is not None:
             self.env.seed(seed)
 
     def set_parameters(
         self,
-        load_path_or_dict: Union[str, Dict[str, Dict]],
+        load_path_or_dict: Union[str, TensorDict],
         exact_match: bool = True,
         device: Union[th.device, str] = "auto",
     ) -> None:
         """
         Load parameters from a given zip-file or a nested dictionary containing parameters for
         different modules (see ``get_parameters``).
 
@@ -574,15 +583,15 @@
             dictionary containing nn.Module parameters used by the policy. The dictionary maps
             object names to a state-dictionary returned by ``torch.nn.Module.state_dict()``.
         :param exact_match: If True, the given parameters should include parameters for each
             module and each of their parameters, otherwise raises an Exception. If set to False, this
             can be used to update only specific parameters.
         :param device: Device on which the code should run.
         """
-        params = None
+        params = {}
         if isinstance(load_path_or_dict, dict):
             params = load_path_or_dict
         else:
             _, params, _ = load_from_zip_file(load_path_or_dict, device=device)
 
         # Keep track which objects were updated.
         # `_get_torch_save_params` returns [params, other_pytorch_variables].
@@ -612,15 +621,15 @@
                 # mess.
                 #
                 # TL;DR: We might not be able to reliably say
                 # if given state-dict is missing keys.
                 #
                 # Solution: Just load the state-dict as is, and trust
                 # the user has provided a sensible state dictionary.
-                attr.load_state_dict(params[name])
+                attr.load_state_dict(params[name])  # type: ignore[arg-type]
             else:
                 # Assume attr is th.nn.Module
                 attr.load_state_dict(params[name], strict=exact_match)
             updated_objects.add(name)
 
         if exact_match and updated_objects != objects_needing_update:
             raise ValueError(
@@ -670,14 +679,17 @@
         data, params, pytorch_variables = load_from_zip_file(
             path,
             device=device,
             custom_objects=custom_objects,
             print_system_info=print_system_info,
         )
 
+        assert data is not None, "No data found in the saved file"
+        assert params is not None, "No params found in the saved file"
+
         # Remove stored device information and replace with ours
         if "policy_kwargs" in data:
             if "device" in data["policy_kwargs"]:
                 del data["policy_kwargs"]["device"]
             # backward compatibility, convert to new format
             if "net_arch" in data["policy_kwargs"] and len(data["policy_kwargs"]["net_arch"]) > 0:
                 saved_net_arch = data["policy_kwargs"]["net_arch"]
@@ -710,21 +722,22 @@
             if data is not None:
                 data["n_envs"] = env.num_envs
         else:
             # Use stored env, if one exists. If not, continue as is (can be used for predict)
             if "env" in data:
                 env = data["env"]
 
-        # noinspection PyArgumentList
-        model = cls(  # pytype: disable=not-instantiable,wrong-keyword-args
+        # pytype: disable=not-instantiable,wrong-keyword-args
+        model = cls(
             policy=data["policy_class"],
             env=env,
             device=device,
-            _init_setup_model=False,  # pytype: disable=not-instantiable,wrong-keyword-args
+            _init_setup_model=False,  # type: ignore[call-arg]
         )
+        # pytype: enable=not-instantiable,wrong-keyword-args
 
         # load parameters
         model.__dict__.update(data)
         model.__dict__.update(kwargs)
         model._setup_model()
 
         try:
@@ -754,20 +767,20 @@
                 # SAC has an entropy coefficient which can be fixed or optimized.
                 # If it is optimized, an additional PyTorch variable `log_ent_coef` is defined,
                 # otherwise it is initialized to `None`.
                 if pytorch_variables[name] is None:
                     continue
                 # Set the data attribute directly to avoid issue when using optimizers
                 # See https://github.com/DLR-RM/stable-baselines3/issues/391
-                recursive_setattr(model, name + ".data", pytorch_variables[name].data)
+                recursive_setattr(model, f"{name}.data", pytorch_variables[name].data)
 
         # Sample gSDE exploration matrix, so it uses the right device
         # see issue #44
         if model.use_sde:
-            model.policy.reset_noise()  # pytype: disable=attribute-error
+            model.policy.reset_noise()  # type: ignore[operator]  # pytype: disable=attribute-error
         return model
 
     def get_parameters(self) -> Dict[str, Dict]:
         """
         Return the parameters of the agent. This includes parameters from different networks, e.g.
         critics (value functions) and policies (pi functions).
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/buffers.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,29 +331,36 @@
     :param device: PyTorch device
     :param gae_lambda: Factor for trade-off of bias vs variance for Generalized Advantage Estimator
         Equivalent to classic advantage when set to 1.
     :param gamma: Discount factor
     :param n_envs: Number of parallel environments
     """
 
+    observations: np.ndarray
+    actions: np.ndarray
+    rewards: np.ndarray
+    advantages: np.ndarray
+    returns: np.ndarray
+    episode_starts: np.ndarray
+    log_probs: np.ndarray
+    values: np.ndarray
+
     def __init__(
         self,
         buffer_size: int,
         observation_space: spaces.Space,
         action_space: spaces.Space,
         device: Union[th.device, str] = "auto",
         gae_lambda: float = 1,
         gamma: float = 0.99,
         n_envs: int = 1,
     ):
         super().__init__(buffer_size, observation_space, action_space, device, n_envs=n_envs)
         self.gae_lambda = gae_lambda
         self.gamma = gamma
-        self.observations, self.actions, self.rewards, self.advantages = None, None, None, None
-        self.returns, self.episode_starts, self.values, self.log_probs = None, None, None, None
         self.generator_ready = False
         self.reset()
 
     def reset(self) -> None:
         self.observations = np.zeros((self.buffer_size, self.n_envs, *self.obs_shape), dtype=np.float32)
         self.actions = np.zeros((self.buffer_size, self.n_envs, self.action_dim), dtype=np.float32)
         self.rewards = np.zeros((self.buffer_size, self.n_envs), dtype=np.float32)
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/callbacks.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
     """
     Convert functional callback (old-style) to object.
 
     :param callback:
     :param verbose: Verbosity level: 0 for no output, 1 for info messages, 2 for debug messages
     """
 
-    def __init__(self, callback: Callable[[Dict[str, Any], Dict[str, Any]], bool], verbose: int = 0):
+    def __init__(self, callback: Optional[Callable[[Dict[str, Any], Dict[str, Any]], bool]], verbose: int = 0):
         super().__init__(verbose)
         self.callback = callback
 
     def _on_step(self) -> bool:
         if self.callback is not None:
             return self.callback(self.locals, self.globals)
         return True
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/distributions.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,14 @@
         return actions, log_prob
 
 
 class TanhBijector:
     """
     Bijective transformation of a probability distribution
     using a squashing function (tanh)
-    TODO: use Pyro instead (https://pyro.ai/)
 
     :param epsilon: small value to avoid NaN due to numerical imprecision.
     """
 
     def __init__(self, epsilon: float = 1e-6):
         super().__init__()
         self.epsilon = epsilon
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/env_checker.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/env_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,16 +362,15 @@
         if warn:
             warnings.warn(
                 "No render modes was declared in the environment "
                 "(env.metadata['render_modes'] is None or not defined), "
                 "you may have trouble when calling `.render()`"
             )
 
-    # TODO: if we want to check all declared render modes,
-    # we need to initialize new environments so the class should be passed as argument.
+    # Only check currrent render mode
     if env.render_mode:
         env.render()
     env.close()
 
 
 def check_env(env: gym.Env, warn: bool = True, skip_render_check: bool = True) -> None:
     """
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/env_util.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/env_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/envs/__init__.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/envs/bit_flipping_env.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/bit_flipping_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import OrderedDict
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 from gymnasium import Env, spaces
 from gymnasium.envs.registration import EnvSpec
 
-from stable_baselines3.common.type_aliases import Gym26StepReturn
+from stable_baselines3.common.type_aliases import GymStepReturn
 
 
 class BitFlippingEnv(Env):
     """
     Simple bit flipping env, useful to test HER.
     The goal is to flip all the bits to get a vector of ones.
     In the continuous variant, if the ith action component has a value > 0,
@@ -162,15 +162,15 @@
     ) -> Tuple[Dict[str, Union[int, np.ndarray]], Dict]:
         if seed is not None:
             self.obs_space.seed(seed)
         self.current_step = 0
         self.state = self.obs_space.sample()
         return self._get_obs(), {}
 
-    def step(self, action: Union[np.ndarray, int]) -> Gym26StepReturn:
+    def step(self, action: Union[np.ndarray, int]) -> GymStepReturn:
         """
         Step into the env.
 
         :param action:
         :return:
         """
         if self.continuous:
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/envs/identity_env.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/identity_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Generic, Optional, Tuple, TypeVar, Union
 
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
 
-from stable_baselines3.common.type_aliases import Gym26StepReturn
+from stable_baselines3.common.type_aliases import GymStepReturn
 
 T = TypeVar("T", int, np.ndarray)
 
 
 class IdentityEnv(gym.Env, Generic[T]):
     def __init__(self, dim: Optional[int] = None, space: Optional[spaces.Space] = None, ep_length: int = 100):
         """
@@ -144,15 +144,15 @@
 
     def reset(self, *, seed: Optional[int] = None, options: Optional[Dict] = None) -> Tuple[np.ndarray, Dict]:
         if seed is not None:
             super().reset(seed=seed)
         self.current_step = 0
         return self.observation_space.sample(), {}
 
-    def step(self, action: Union[np.ndarray, int]) -> Gym26StepReturn:
+    def step(self, action: Union[np.ndarray, int]) -> GymStepReturn:
         reward = 0.0
         self.current_step += 1
         terminated = False
         truncated = self.current_step >= self.ep_length
         return self.observation_space.sample(), reward, terminated, truncated, {}
 
     def render(self, mode: str = "human") -> None:
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/envs/multi_input_envs.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/multi_input_envs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Optional, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
 
-from stable_baselines3.common.type_aliases import Gym26StepReturn
+from stable_baselines3.common.type_aliases import GymStepReturn
 
 
 class SimpleMultiObsEnv(gym.Env):
     """
     Base class for GridWorld-based MultiObs Environments 4x4  grid world.
 
     .. code-block:: text
@@ -117,15 +117,15 @@
         in order to define the transitions of the environment
         """
         self.left_possible = [1, 2, 3, 13, 14, 15]
         self.down_possible = [0, 4, 8, 3, 7, 11]
         self.right_possible = [0, 1, 2, 12, 13, 14]
         self.up_possible = [4, 8, 12, 7, 11, 15]
 
-    def step(self, action: Union[float, np.ndarray]) -> Gym26StepReturn:
+    def step(self, action: Union[float, np.ndarray]) -> GymStepReturn:
         """
         Run one timestep of the environment's dynamics. When end of
         episode is reached, you are responsible for calling `reset()`
         to reset this environment's state.
         Accepts an action and returns a tuple (observation, reward, done, info).
 
         :param action:
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/evaluation.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     while (episode_counts < episode_count_targets).any():
         actions, states = model.predict(
             observations,  # type: ignore[arg-type]
             state=states,
             episode_start=episode_starts,
             deterministic=deterministic,
         )
-        observations, rewards, dones, infos = env.step(actions)
+        new_observations, rewards, dones, infos = env.step(actions)
         current_rewards += rewards
         current_lengths += 1
         for i in range(n_envs):
             if episode_counts[i] < episode_count_targets[i]:
                 # unpack values so that the callback can access the local variables
                 reward = rewards[i]
                 done = dones[i]
@@ -121,14 +121,16 @@
                     else:
                         episode_rewards.append(current_rewards[i])
                         episode_lengths.append(current_lengths[i])
                         episode_counts[i] += 1
                     current_rewards[i] = 0
                     current_lengths[i] = 0
 
+        observations = new_observations
+
         if render:
             env.render()
 
     mean_reward = np.mean(episode_rewards)
     std_reward = np.std(episode_rewards)
     if reward_threshold is not None:
         assert mean_reward > reward_threshold, "Mean reward below threshold: " f"{mean_reward:.2f} < {reward_threshold:.2f}"
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/logger.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/monitor.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/noise.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/noise.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/off_policy_algorithm.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/off_policy_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         Default: -1 (only sample at the beginning of the rollout)
     :param use_sde_at_warmup: Whether to use gSDE instead of uniform sampling
         during the warm up phase (before learning starts)
     :param sde_support: Whether the model support gSDE or not
     :param supported_action_spaces: The action spaces supported by the algorithm.
     """
 
+    actor: th.nn.Module
+
     def __init__(
         self,
         policy: Union[str, Type[BasePolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule],
         buffer_size: int = 1_000_000,  # 1e6
         learning_starts: int = 100,
@@ -125,23 +127,22 @@
         self.batch_size = batch_size
         self.learning_starts = learning_starts
         self.tau = tau
         self.gamma = gamma
         self.gradient_steps = gradient_steps
         self.action_noise = action_noise
         self.optimize_memory_usage = optimize_memory_usage
+        self.replay_buffer: Optional[ReplayBuffer] = None
         self.replay_buffer_class = replay_buffer_class
         self.replay_buffer_kwargs = replay_buffer_kwargs or {}
         self._episode_storage = None
 
         # Save train freq parameter, will be converted later to TrainFreq object
         self.train_freq = train_freq
 
-        self.actor = None  # type: Optional[th.nn.Module]
-        self.replay_buffer: Optional[ReplayBuffer] = None
         # Update policy keyword arguments
         if sde_support:
             self.policy_kwargs["use_sde"] = self.use_sde
         # For gSDE only
         self.use_sde_at_warmup = use_sde_at_warmup
 
     def _convert_train_freq(self) -> None:
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/on_policy_algorithm.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/on_policy_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     :param seed: Seed for the pseudo random generators
     :param device: Device (cpu, cuda, ...) on which the code should be run.
         Setting it to auto, the code will be run on the GPU if possible.
     :param _init_setup_model: Whether or not to build the network at the creation of the instance
     :param supported_action_spaces: The action spaces supported by the algorithm.
     """
 
+    rollout_buffer: RolloutBuffer
+    policy: ActorCriticPolicy
+
     def __init__(
         self,
         policy: Union[str, Type[ActorCriticPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule],
         n_steps: int,
         gamma: float,
@@ -93,15 +96,14 @@
 
         self.n_steps = n_steps
         self.gamma = gamma
         self.gae_lambda = gae_lambda
         self.ent_coef = ent_coef
         self.vf_coef = vf_coef
         self.max_grad_norm = max_grad_norm
-        self.rollout_buffer = None
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         self._setup_lr_schedule()
         self.set_random_seed(self.seed)
@@ -113,21 +115,19 @@
             self.observation_space,
             self.action_space,
             device=self.device,
             gamma=self.gamma,
             gae_lambda=self.gae_lambda,
             n_envs=self.n_envs,
         )
-        self.policy = self.policy_class(  # pytype:disable=not-instantiable
-            self.observation_space,
-            self.action_space,
-            self.lr_schedule,
-            use_sde=self.use_sde,
-            **self.policy_kwargs  # pytype:disable=not-instantiable
+        # pytype:disable=not-instantiable
+        self.policy = self.policy_class(  # type: ignore[assignment]
+            self.observation_space, self.action_space, self.lr_schedule, use_sde=self.use_sde, **self.policy_kwargs
         )
+        # pytype:enable=not-instantiable
         self.policy = self.policy.to(self.device)
 
     def collect_rollouts(
         self,
         env: VecEnv,
         callback: BaseCallback,
         rollout_buffer: RolloutBuffer,
@@ -197,24 +197,31 @@
                 if (
                     done
                     and infos[idx].get("terminal_observation") is not None
                     and infos[idx].get("TimeLimit.truncated", False)
                 ):
                     terminal_obs = self.policy.obs_to_tensor(infos[idx]["terminal_observation"])[0]
                     with th.no_grad():
-                        terminal_value = self.policy.predict_values(terminal_obs)[0]
+                        terminal_value = self.policy.predict_values(terminal_obs)[0]  # type: ignore[arg-type]
                     rewards[idx] += self.gamma * terminal_value
 
-            rollout_buffer.add(self._last_obs, actions, rewards, self._last_episode_starts, values, log_probs)
-            self._last_obs = new_obs
+            rollout_buffer.add(
+                self._last_obs,  # type: ignore[arg-type]
+                actions,
+                rewards,
+                self._last_episode_starts,  # type: ignore[arg-type]
+                values,
+                log_probs,
+            )
+            self._last_obs = new_obs  # type: ignore[assignment]
             self._last_episode_starts = dones
 
         with th.no_grad():
             # Compute value for the last timestep
-            values = self.policy.predict_values(obs_as_tensor(new_obs, self.device))
+            values = self.policy.predict_values(obs_as_tensor(new_obs, self.device))  # type: ignore[arg-type]
 
         rollout_buffer.compute_returns_and_advantage(last_values=values, dones=dones)
 
         callback.on_rollout_end()
 
         return True
 
@@ -242,25 +249,28 @@
             reset_num_timesteps,
             tb_log_name,
             progress_bar,
         )
 
         callback.on_training_start(locals(), globals())
 
+        assert self.env is not None
+
         while self.num_timesteps < total_timesteps:
             continue_training = self.collect_rollouts(self.env, callback, self.rollout_buffer, n_rollout_steps=self.n_steps)
 
             if continue_training is False:
                 break
 
             iteration += 1
             self._update_current_progress_remaining(self.num_timesteps, total_timesteps)
 
             # Display training infos
             if log_interval is not None and iteration % log_interval == 0:
+                assert self.ep_info_buffer is not None
                 time_elapsed = max((time.time_ns() - self.start_time) / 1e9, sys.float_info.epsilon)
                 fps = int((self.num_timesteps - self._num_timesteps_at_start) / time_elapsed)
                 self.logger.record("time/iterations", iteration, exclude="tensorboard")
                 if len(self.ep_info_buffer) > 0 and len(self.ep_info_buffer[0]) > 0:
                     self.logger.record("rollout/ep_rew_mean", safe_mean([ep_info["r"] for ep_info in self.ep_info_buffer]))
                     self.logger.record("rollout/ep_len_mean", safe_mean([ep_info["l"] for ep_info in self.ep_info_buffer]))
                 self.logger.record("time/fps", fps)
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/policies.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
          dividing by 255.0 (True by default)
     :param optimizer_class: The optimizer to use,
         ``th.optim.Adam`` by default
     :param optimizer_kwargs: Additional keyword arguments,
         excluding the learning rate, to pass to the optimizer
     """
 
+    optimizer: th.optim.Optimizer
+
     def __init__(
         self,
         observation_space: spaces.Space,
         action_space: spaces.Space,
         features_extractor_class: Type[BaseFeaturesExtractor] = FlattenExtractor,
         features_extractor_kwargs: Optional[Dict[str, Any]] = None,
         features_extractor: Optional[BaseFeaturesExtractor] = None,
@@ -80,15 +82,14 @@
         self.observation_space = observation_space
         self.action_space = action_space
         self.features_extractor = features_extractor
         self.normalize_images = normalize_images
 
         self.optimizer_class = optimizer_class
         self.optimizer_kwargs = optimizer_kwargs
-        self.optimizer: th.optim.Optimizer
 
         self.features_extractor_class = features_extractor_class
         self.features_extractor_kwargs = features_extractor_kwargs
         # Automatically deactivate dtype and bounds checks
         if normalize_images is False and issubclass(features_extractor_class, (NatureCNN, CombinedExtractor)):
             self.features_extractor_kwargs.update(dict(normalized_image=True))
 
@@ -275,14 +276,16 @@
 
     :param args: positional arguments passed through to `BaseModel`.
     :param kwargs: keyword arguments passed through to `BaseModel`.
     :param squash_output: For continuous actions, whether the output is squashed
         or not using a ``tanh()`` function.
     """
 
+    features_extractor: BaseFeaturesExtractor
+
     def __init__(self, *args, squash_output: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
         self._squash_output = squash_output
 
     @staticmethod
     def _dummy_schedule(progress_remaining: float) -> float:
         """(float) Useful for pickling policy."""
@@ -333,19 +336,14 @@
         :param episode_start: The last masks (can be None, used in recurrent policies)
             this correspond to beginning of episodes,
             where the hidden states of the RNN must be reset.
         :param deterministic: Whether or not to return deterministic actions.
         :return: the model's action and the next hidden state
             (used in recurrent policies)
         """
-        # TODO (GH/1): add support for RNN policies
-        # if state is None:
-        #     state = self.initial_state
-        # if episode_start is None:
-        #     episode_start = [False for _ in range(self.n_envs)]
         # Switch to eval mode (this affects batch norm / dropout)
         self.set_training_mode(False)
 
         observation, vectorized_env = self.obs_to_tensor(observation)
 
         with th.no_grad():
             actions = self._predict(observation, deterministic=deterministic)
@@ -896,18 +894,20 @@
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     :param n_critics: Number of critic networks to create.
     :param share_features_extractor: Whether the features extractor is shared or not
         between the actor and the critic (this saves computation time)
     """
 
+    features_extractor: BaseFeaturesExtractor
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
         normalize_images: bool = True,
         n_critics: int = 2,
         share_features_extractor: bool = True,
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/preprocessing.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/results_plotter.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/results_plotter.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/running_mean_std.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/save_util.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/save_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
 def load_from_zip_file(
     load_path: Union[str, pathlib.Path, io.BufferedIOBase],
     load_data: bool = True,
     custom_objects: Optional[Dict[str, Any]] = None,
     device: Union[th.device, str] = "auto",
     verbose: int = 0,
     print_system_info: bool = False,
-) -> Tuple[Optional[Dict[str, Any]], Optional[TensorDict], Optional[TensorDict]]:
+) -> Tuple[Optional[Dict[str, Any]], TensorDict, Optional[TensorDict]]:
     """
     Load model data from a .zip archive
 
     :param load_path: Where to load the model from
     :param load_data: Whether we should load and return data
         (class parameters). Mainly used by 'load_parameters' to only load model parameters (weights)
     :param custom_objects: Dictionary of objects to replace
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/torch_layers.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/torch_layers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/type_aliases.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/type_aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 else:
     from typing_extensions import Protocol
 
 from stable_baselines3.common import callbacks, vec_env
 
 GymEnv = Union[gym.Env, vec_env.VecEnv]
 GymObs = Union[Tuple, Dict[str, Any], np.ndarray, int]
-Gym26ResetReturn = Tuple[GymObs, Dict]
+GymResetReturn = Tuple[GymObs, Dict]
 AtariResetReturn = Tuple[np.ndarray, Dict[str, Any]]
-GymStepReturn = Tuple[GymObs, float, bool, Dict]
-Gym26StepReturn = Tuple[GymObs, float, bool, bool, Dict]
+GymStepReturn = Tuple[GymObs, float, bool, bool, Dict]
 AtariStepReturn = Tuple[np.ndarray, SupportsFloat, bool, bool, Dict[str, Any]]
-TensorDict = Dict[Union[str, int], th.Tensor]
+TensorDict = Dict[str, th.Tensor]
 OptimizerStateDict = Dict[str, Any]
 MaybeCallback = Union[None, Callable, List[callbacks.BaseCallback], callbacks.BaseCallback]
 
 # A schedule takes the remaining progress as input
 # and ouputs a scalar (e.g. learning rate, clip range, ...)
 Schedule = Callable[[float], float]
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/utils.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,17 +467,15 @@
     with th.no_grad():
         # zip does not raise an exception if length of parameters does not match.
         for param, target_param in zip_strict(params, target_params):
             target_param.data.mul_(1 - tau)
             th.add(target_param.data, param.data, alpha=tau, out=target_param.data)
 
 
-def obs_as_tensor(
-    obs: Union[np.ndarray, Dict[Union[str, int], np.ndarray]], device: th.device
-) -> Union[th.Tensor, TensorDict]:
+def obs_as_tensor(obs: Union[np.ndarray, Dict[str, np.ndarray]], device: th.device) -> Union[th.Tensor, TensorDict]:
     """
     Moves the observation to the given device.
 
     :param obs:
     :param device: PyTorch device
     :return: PyTorch tensor of the observation on a desired device.
     """
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/__init__.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/base_vec_env.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/base_vec_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
             # to avoid a duplicate call to getattr_depth_check.
             attr = self.venv.getattr_recursive(name)
         else:  # attribute not present, child is an unwrapped VecEnv
             attr = getattr(self.venv, name)
 
         return attr
 
-    def getattr_depth_check(self, name: str, already_found: bool) -> str:
+    def getattr_depth_check(self, name: str, already_found: bool) -> Optional[str]:
         """See base class.
 
         :return: name of module whose attribute is being shadowed, if any.
         """
         all_attributes = self._get_all_attributes()
         if name in all_attributes and already_found:
             # this venv's attribute is being hidden because of a higher venv.
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/dummy_vec_env.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/patch_gym.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/patch_gym.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/stacked_observations.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/stacked_observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         For Dict space, channels_order can also be a dictionary.
     """
 
     def __init__(
         self,
         num_envs: int,
         n_stack: int,
-        observation_space: Union[spaces.Box, spaces.Dict],  # Replace by Space[TObs] in gym>=0.26
+        observation_space: Union[spaces.Box, spaces.Dict],
         channels_order: Optional[Union[str, Mapping[str, Optional[str]]]] = None,
     ) -> None:
         self.n_stack = n_stack
         self.observation_space = observation_space
         if isinstance(observation_space, spaces.Dict):
             if not isinstance(channels_order, Mapping):
                 channels_order = {key: channels_order for key in observation_space.spaces.keys()}
@@ -105,22 +105,24 @@
         """
         Reset the stacked_obs, add the reset observation to the stack, and return the stack.
 
         :param observation: Reset observation
         :return: The stacked reset observation
         """
         if isinstance(observation, dict):
-            return {key: self.sub_stacked_observations[key].reset(obs) for key, obs in observation.items()}
+            return {
+                key: self.sub_stacked_observations[key].reset(obs) for key, obs in observation.items()
+            }  # pytype: disable=bad-return-type
 
         self.stacked_obs[...] = 0
         if self.channels_first:
             self.stacked_obs[:, -observation.shape[self.stack_dimension] :, ...] = observation
         else:
             self.stacked_obs[..., -observation.shape[self.stack_dimension] :] = observation
-        return self.stacked_obs
+        return self.stacked_obs  # pytype: disable=bad-return-type
 
     def update(
         self,
         observations: TObs,
         dones: np.ndarray,
         infos: List[Dict[str, Any]],
     ) -> Tuple[TObs, List[Dict[str, Any]]]:
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/subproc_vec_env.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/util.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_check_nan.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_extract_dict_obs.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,12 @@
         super().__init__(venv=venv, observation_space=venv.observation_space.spaces[self.key])
 
     def reset(self) -> np.ndarray:
         obs = self.venv.reset()
         return obs[self.key]
 
     def step_wait(self) -> VecEnvStepReturn:
-        obs, reward, done, info = self.venv.step_wait()
-        return obs[self.key], reward, done, info
+        obs, reward, done, infos = self.venv.step_wait()
+        for info in infos:
+            if "terminal_observation" in info:
+                info["terminal_observation"] = info["terminal_observation"][self.key]
+        return obs[self.key], reward, done, infos
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_frame_stack.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_monitor.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_normalize.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_transpose.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_transpose.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/common/vec_env/vec_video_recorder.py` & `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/ddpg/ddpg.py` & `stable_baselines3-2.0.0a4/stable_baselines3/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/dqn/dqn.py` & `stable_baselines3-2.0.0a4/stable_baselines3/dqn/dqn.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torch.nn import functional as F
 
 from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 from stable_baselines3.common.utils import get_linear_fn, get_parameters_by_name, polyak_update
-from stable_baselines3.dqn.policies import CnnPolicy, DQNPolicy, MlpPolicy, MultiInputPolicy
+from stable_baselines3.dqn.policies import CnnPolicy, DQNPolicy, MlpPolicy, MultiInputPolicy, QNetwork
 
 SelfDQN = TypeVar("SelfDQN", bound="DQN")
 
 
 class DQN(OffPolicyAlgorithm):
     """
     Deep Q-Network (DQN)
@@ -63,14 +63,19 @@
     """
 
     policy_aliases: Dict[str, Type[BasePolicy]] = {
         "MlpPolicy": MlpPolicy,
         "CnnPolicy": CnnPolicy,
         "MultiInputPolicy": MultiInputPolicy,
     }
+    # Linear schedule will be defined in `_setup_model()`
+    exploration_schedule: Schedule
+    q_net: QNetwork
+    q_net_target: QNetwork
+    policy: DQNPolicy
 
     def __init__(
         self,
         policy: Union[str, Type[DQNPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 1e-4,
         buffer_size: int = 1_000_000,  # 1e6
@@ -127,18 +132,14 @@
         self.exploration_fraction = exploration_fraction
         self.target_update_interval = target_update_interval
         # For updating the target network with multiple envs:
         self._n_calls = 0
         self.max_grad_norm = max_grad_norm
         # "epsilon" for the epsilon-greedy exploration
         self.exploration_rate = 0.0
-        # Linear schedule will be defined in `_setup_model()`
-        self.exploration_schedule: Schedule
-        self.q_net: th.nn.Module
-        self.q_net_target: th.nn.Module
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
         self._create_aliases()
@@ -160,16 +161,14 @@
                     "therefore the target network will be updated after each call to env.step() "
                     f"which corresponds to {self.n_envs} steps."
                 )
 
             self.target_update_interval = max(self.target_update_interval // self.n_envs, 1)
 
     def _create_aliases(self) -> None:
-        # For type checker:
-        assert isinstance(self.policy, DQNPolicy)
         self.q_net = self.policy.q_net
         self.q_net_target = self.policy.q_net_target
 
     def _on_step(self) -> None:
         """
         Update the exploration rate and target network if needed.
         This method is called in ``collect_rollouts()`` after each step in the environment.
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/dqn/policies.py` & `stable_baselines3-2.0.0a4/stable_baselines3/dqn/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     :param action_space: Action space
     :param net_arch: The specification of the policy and value networks.
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
         net_arch: Optional[List[int]] = None,
@@ -46,28 +48,25 @@
 
         if net_arch is None:
             net_arch = [64, 64]
 
         self.net_arch = net_arch
         self.activation_fn = activation_fn
         self.features_dim = features_dim
-        assert isinstance(self.action_space, spaces.Discrete)
         action_dim = int(self.action_space.n)  # number of actions
         q_net = create_mlp(self.features_dim, action_dim, self.net_arch, self.activation_fn)
         self.q_net = nn.Sequential(*q_net)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         """
         Predict the q-values.
 
         :param obs: Observation
         :return: The estimated Q-Value for each action.
         """
-        # For type checker:
-        assert isinstance(self.features_extractor, BaseFeaturesExtractor)
         return self.q_net(self.extract_features(obs, self.features_extractor))
 
     def _predict(self, observation: th.Tensor, deterministic: bool = True) -> th.Tensor:
         q_values = self(observation)
         # Greedy action
         action = q_values.argmax(dim=1).reshape(-1)
         return action
@@ -102,14 +101,17 @@
          dividing by 255.0 (True by default)
     :param optimizer_class: The optimizer to use,
         ``th.optim.Adam`` by default
     :param optimizer_kwargs: Additional keyword arguments,
         excluding the learning rate, to pass to the optimizer
     """
 
+    q_net: QNetwork
+    q_net_target: QNetwork
+
     def __init__(
         self,
         observation_space: spaces.Space,
         action_space: spaces.Discrete,
         lr_schedule: Schedule,
         net_arch: Optional[List[int]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
@@ -142,16 +144,14 @@
             "observation_space": self.observation_space,
             "action_space": self.action_space,
             "net_arch": self.net_arch,
             "activation_fn": self.activation_fn,
             "normalize_images": normalize_images,
         }
 
-        self.q_net: QNetwork
-        self.q_net_target: QNetwork
         self._build(lr_schedule)
 
     def _build(self, lr_schedule: Schedule) -> None:
         """
         Create the network and the optimizer.
 
         Put the target network into evaluation mode.
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/her/goal_selection_strategy.py` & `stable_baselines3-2.0.0a4/stable_baselines3/her/goal_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/her/her_replay_buffer.py` & `stable_baselines3-2.0.0a4/stable_baselines3/her/her_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/ppo/ppo.py` & `stable_baselines3-2.0.0a4/stable_baselines3/ppo/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,18 @@
         Update policy using the currently gathered rollout buffer.
         """
         # Switch to train mode (this affects batch norm / dropout)
         self.policy.set_training_mode(True)
         # Update optimizer learning rate
         self._update_learning_rate(self.policy.optimizer)
         # Compute current clip range
-        clip_range = self.clip_range(self._current_progress_remaining)
+        clip_range = self.clip_range(self._current_progress_remaining)  # type: ignore[operator]
         # Optional: clip range for the value function
         if self.clip_range_vf is not None:
-            clip_range_vf = self.clip_range_vf(self._current_progress_remaining)
+            clip_range_vf = self.clip_range_vf(self._current_progress_remaining)  # type: ignore[operator]
 
         entropy_losses = []
         pg_losses, value_losses = [], []
         clip_fractions = []
 
         continue_training = True
         # train for n_epochs epochs
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/sac/policies.py` & `stable_baselines3-2.0.0a4/stable_baselines3/sac/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,20 @@
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
@@ -92,17 +94,17 @@
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
@@ -153,15 +155,15 @@
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
@@ -201,18 +203,22 @@
     :param optimizer_kwargs: Additional keyword arguments,
         excluding the learning rate, to pass to the optimizer
     :param n_critics: Number of critic networks to create.
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
+    actor: Actor
+    critic: ContinuousCritic
+    critic_target: ContinuousCritic
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
@@ -263,40 +269,46 @@
             {
                 "n_critics": n_critics,
                 "net_arch": critic_arch,
                 "share_features_extractor": share_features_extractor,
             }
         )
 
-        self.actor, self.actor_target = None, None
-        self.critic, self.critic_target = None, None
         self.share_features_extractor = share_features_extractor
 
         self._build(lr_schedule)
 
     def _build(self, lr_schedule: Schedule) -> None:
         self.actor = self.make_actor()
-        self.actor.optimizer = self.optimizer_class(self.actor.parameters(), lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.actor.optimizer = self.optimizer_class(
+            self.actor.parameters(),
+            lr=lr_schedule(1),  # type: ignore[call-arg]
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
 
         # Critic target should not share the features extractor with critic
         self.critic_target = self.make_critic(features_extractor=None)
         self.critic_target.load_state_dict(self.critic.state_dict())
 
-        self.critic.optimizer = self.optimizer_class(critic_parameters, lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.critic.optimizer = self.optimizer_class(
+            critic_parameters,
+            lr=lr_schedule(1),  # type: ignore[call-arg]
+            **self.optimizer_kwargs,
+        )
 
         # Target networks should always be in eval mode
         self.critic_target.set_training_mode(False)
 
     def _get_constructor_parameters(self) -> Dict[str, Any]:
         data = super()._get_constructor_parameters()
 
@@ -382,15 +394,15 @@
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
@@ -448,15 +460,15 @@
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

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/sac/sac.py` & `stable_baselines3-2.0.0a4/stable_baselines3/sac/sac.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import torch as th
 from gymnasium import spaces
 from torch.nn import functional as F
 
 from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
-from stable_baselines3.common.policies import BasePolicy
+from stable_baselines3.common.policies import BasePolicy, ContinuousCritic
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 from stable_baselines3.common.utils import get_parameters_by_name, polyak_update
-from stable_baselines3.sac.policies import CnnPolicy, MlpPolicy, MultiInputPolicy, SACPolicy
+from stable_baselines3.sac.policies import Actor, CnnPolicy, MlpPolicy, MultiInputPolicy, SACPolicy
 
 SelfSAC = TypeVar("SelfSAC", bound="SAC")
 
 
 class SAC(OffPolicyAlgorithm):
     """
     Soft Actor-Critic (SAC)
@@ -78,14 +78,18 @@
     """
 
     policy_aliases: Dict[str, Type[BasePolicy]] = {
         "MlpPolicy": MlpPolicy,
         "CnnPolicy": CnnPolicy,
         "MultiInputPolicy": MultiInputPolicy,
     }
+    policy: SACPolicy
+    actor: Actor
+    critic: ContinuousCritic
+    critic_target: ContinuousCritic
 
     def __init__(
         self,
         policy: Union[str, Type[SACPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 3e-4,
         buffer_size: int = 1_000_000,  # 1e6
@@ -133,39 +137,39 @@
             verbose=verbose,
             device=device,
             seed=seed,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             use_sde_at_warmup=use_sde_at_warmup,
             optimize_memory_usage=optimize_memory_usage,
-            supported_action_spaces=(spaces.Box),
+            supported_action_spaces=(spaces.Box,),
             support_multi_env=True,
         )
 
         self.target_entropy = target_entropy
         self.log_ent_coef = None  # type: Optional[th.Tensor]
         # Entropy coefficient / Entropy temperature
         # Inverse of the reward scale
         self.ent_coef = ent_coef
         self.target_update_interval = target_update_interval
-        self.ent_coef_optimizer = None
+        self.ent_coef_optimizer: Optional[th.optim.Adam] = None
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
         self._create_aliases()
         # Running mean and running var
         self.batch_norm_stats = get_parameters_by_name(self.critic, ["running_"])
         self.batch_norm_stats_target = get_parameters_by_name(self.critic_target, ["running_"])
         # Target entropy is used when learning the entropy coefficient
         if self.target_entropy == "auto":
             # automatically set target entropy if needed
-            self.target_entropy = -np.prod(self.env.action_space.shape).astype(np.float32)
+            self.target_entropy = float(-np.prod(self.env.action_space.shape).astype(np.float32))  # type: ignore
         else:
             # Force conversion
             # this will also throw an error for unexpected string
             self.target_entropy = float(self.target_entropy)
 
         # The entropy coefficient or entropy can be learned automatically
         # see Automating Entropy Adjustment for Maximum Entropy RL section
@@ -204,40 +208,40 @@
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
@@ -251,15 +255,16 @@
 
             # Get current Q-values estimates for each critic network
             # using action from the replay buffer
             current_q_values = self.critic(replay_data.observations, replay_data.actions)
 
             # Compute critic loss
             critic_loss = 0.5 * sum(F.mse_loss(current_q, target_q_values) for current_q in current_q_values)
-            critic_losses.append(critic_loss.item())
+            assert isinstance(critic_loss, th.Tensor)  # for type checker
+            critic_losses.append(critic_loss.item())  # type: ignore[union-attr]
 
             # Optimize the critic
             self.critic.optimizer.zero_grad()
             critic_loss.backward()
             self.critic.optimizer.step()
 
             # Compute actor loss
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/td3/policies.py` & `stable_baselines3-2.0.0a4/stable_baselines3/td3/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     """
 
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         net_arch: List[int],
         features_extractor: nn.Module,
         features_dim: int,
         activation_fn: Type[nn.Module] = nn.ReLU,
         normalize_images: bool = True,
     ):
         super().__init__(
@@ -102,18 +102,23 @@
     :param optimizer_kwargs: Additional keyword arguments,
         excluding the learning rate, to pass to the optimizer
     :param n_critics: Number of critic networks to create.
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
+    actor: Actor
+    actor_target: Actor
+    critic: ContinuousCritic
+    critic_target: ContinuousCritic
+
     def __init__(
         self,
         observation_space: spaces.Space,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
         features_extractor_class: Type[BaseFeaturesExtractor] = FlattenExtractor,
         features_extractor_kwargs: Optional[Dict[str, Any]] = None,
         normalize_images: bool = True,
         optimizer_class: Type[th.optim.Optimizer] = th.optim.Adam,
@@ -156,29 +161,31 @@
             {
                 "n_critics": n_critics,
                 "net_arch": critic_arch,
                 "share_features_extractor": share_features_extractor,
             }
         )
 
-        self.actor, self.actor_target = None, None
-        self.critic, self.critic_target = None, None
         self.share_features_extractor = share_features_extractor
 
         self._build(lr_schedule)
 
     def _build(self, lr_schedule: Schedule) -> None:
         # Create actor and target
         # the features extractor should not be shared
         self.actor = self.make_actor(features_extractor=None)
         self.actor_target = self.make_actor(features_extractor=None)
         # Initialize the target to have the same weights as the actor
         self.actor_target.load_state_dict(self.actor.state_dict())
 
-        self.actor.optimizer = self.optimizer_class(self.actor.parameters(), lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.actor.optimizer = self.optimizer_class(
+            self.actor.parameters(),
+            lr=lr_schedule(1),  # type: ignore[call-arg]
+            **self.optimizer_kwargs,
+        )
 
         if self.share_features_extractor:
             self.critic = self.make_critic(features_extractor=self.actor.features_extractor)
             # Critic target should not share the features extractor with critic
             # but it can share it with the actor target as actor and critic are sharing
             # the same features_extractor too
             # NOTE: as a result the effective poliak (soft-copy) coefficient for the features extractor
@@ -186,15 +193,19 @@
             self.critic_target = self.make_critic(features_extractor=self.actor_target.features_extractor)
         else:
             # Create new features extractor for each network
             self.critic = self.make_critic(features_extractor=None)
             self.critic_target = self.make_critic(features_extractor=None)
 
         self.critic_target.load_state_dict(self.critic.state_dict())
-        self.critic.optimizer = self.optimizer_class(self.critic.parameters(), lr=lr_schedule(1), **self.optimizer_kwargs)
+        self.critic.optimizer = self.optimizer_class(
+            self.critic.parameters(),
+            lr=lr_schedule(1),  # type: ignore[call-arg]
+            **self.optimizer_kwargs,
+        )
 
         # Target networks should always be in eval mode
         self.actor_target.set_training_mode(False)
         self.critic_target.set_training_mode(False)
 
     def _get_constructor_parameters(self) -> Dict[str, Any]:
         data = super()._get_constructor_parameters()
@@ -268,15 +279,15 @@
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
         features_extractor_class: Type[BaseFeaturesExtractor] = NatureCNN,
         features_extractor_kwargs: Optional[Dict[str, Any]] = None,
         normalize_images: bool = True,
         optimizer_class: Type[th.optim.Optimizer] = th.optim.Adam,
@@ -322,15 +333,15 @@
     :param share_features_extractor: Whether to share or not the features extractor
         between the actor and the critic (this saves computation time)
     """
 
     def __init__(
         self,
         observation_space: spaces.Dict,
-        action_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         activation_fn: Type[nn.Module] = nn.ReLU,
         features_extractor_class: Type[BaseFeaturesExtractor] = CombinedExtractor,
         features_extractor_kwargs: Optional[Dict[str, Any]] = None,
         normalize_images: bool = True,
         optimizer_class: Type[th.optim.Optimizer] = th.optim.Adam,
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3/td3/td3.py` & `stable_baselines3-2.0.0a4/stable_baselines3/td3/td3.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import torch as th
 from gymnasium import spaces
 from torch.nn import functional as F
 
 from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
-from stable_baselines3.common.policies import BasePolicy
+from stable_baselines3.common.policies import BasePolicy, ContinuousCritic
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 from stable_baselines3.common.utils import get_parameters_by_name, polyak_update
-from stable_baselines3.td3.policies import CnnPolicy, MlpPolicy, MultiInputPolicy, TD3Policy
+from stable_baselines3.td3.policies import Actor, CnnPolicy, MlpPolicy, MultiInputPolicy, TD3Policy
 
 SelfTD3 = TypeVar("SelfTD3", bound="TD3")
 
 
 class TD3(OffPolicyAlgorithm):
     """
     Twin Delayed DDPG (TD3)
@@ -66,14 +66,19 @@
     """
 
     policy_aliases: Dict[str, Type[BasePolicy]] = {
         "MlpPolicy": MlpPolicy,
         "CnnPolicy": CnnPolicy,
         "MultiInputPolicy": MultiInputPolicy,
     }
+    policy: TD3Policy
+    actor: Actor
+    actor_target: Actor
+    critic: ContinuousCritic
+    critic_target: ContinuousCritic
 
     def __init__(
         self,
         policy: Union[str, Type[TD3Policy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 1e-3,
         buffer_size: int = 1_000_000,  # 1e6
@@ -116,15 +121,15 @@
             stats_window_size=stats_window_size,
             tensorboard_log=tensorboard_log,
             verbose=verbose,
             device=device,
             seed=seed,
             sde_support=False,
             optimize_memory_usage=optimize_memory_usage,
-            supported_action_spaces=(spaces.Box),
+            supported_action_spaces=(spaces.Box,),
             support_multi_env=True,
         )
 
         self.policy_delay = policy_delay
         self.target_noise_clip = target_noise_clip
         self.target_policy_noise = target_policy_noise
 
@@ -153,15 +158,15 @@
         # Update learning rate according to lr schedule
         self._update_learning_rate([self.actor.optimizer, self.critic.optimizer])
 
         actor_losses, critic_losses = [], []
         for _ in range(gradient_steps):
             self._n_updates += 1
             # Sample replay buffer
-            replay_data = self.replay_buffer.sample(batch_size, env=self._vec_normalize_env)
+            replay_data = self.replay_buffer.sample(batch_size, env=self._vec_normalize_env)  # type: ignore[union-attr]
 
             with th.no_grad():
                 # Select action according to policy and add clipped noise
                 noise = replay_data.actions.clone().data.normal_(0, self.target_policy_noise)
                 noise = noise.clamp(-self.target_noise_clip, self.target_noise_clip)
                 next_actions = (self.actor_target(replay_data.next_observations) + noise).clamp(-1, 1)
 
@@ -171,14 +176,15 @@
                 target_q_values = replay_data.rewards + (1 - replay_data.dones) * self.gamma * next_q_values
 
             # Get current Q-values estimates for each critic network
             current_q_values = self.critic(replay_data.observations, replay_data.actions)
 
             # Compute critic loss
             critic_loss = sum(F.mse_loss(current_q, target_q_values) for current_q in current_q_values)
+            assert isinstance(critic_loss, th.Tensor)
             critic_losses.append(critic_loss.item())
 
             # Optimize the critics
             self.critic.optimizer.zero_grad()
             critic_loss.backward()
             self.critic.optimizer.step()
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3.egg-info/PKG-INFO` & `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-baselines3
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3.egg-info/SOURCES.txt` & `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/stable_baselines3.egg-info/requires.txt` & `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_buffers.py` & `stable_baselines3-2.0.0a4/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_callbacks.py` & `stable_baselines3-2.0.0a4/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_cnn.py` & `stable_baselines3-2.0.0a4/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_custom_policy.py` & `stable_baselines3-2.0.0a4/tests/test_custom_policy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_deterministic.py` & `stable_baselines3-2.0.0a4/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_dict_env.py` & `stable_baselines3-2.0.0a4/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_distributions.py` & `stable_baselines3-2.0.0a4/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_env_checker.py` & `stable_baselines3-2.0.0a4/tests/test_env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_envs.py` & `stable_baselines3-2.0.0a4/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_gae.py` & `stable_baselines3-2.0.0a4/tests/test_gae.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_her.py` & `stable_baselines3-2.0.0a4/tests/test_her.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_identity.py` & `stable_baselines3-2.0.0a4/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_logger.py` & `stable_baselines3-2.0.0a4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_monitor.py` & `stable_baselines3-2.0.0a4/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_predict.py` & `stable_baselines3-2.0.0a4/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_preprocessing.py` & `stable_baselines3-2.0.0a4/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_run.py` & `stable_baselines3-2.0.0a4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_save_load.py` & `stable_baselines3-2.0.0a4/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_sde.py` & `stable_baselines3-2.0.0a4/tests/test_sde.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_spaces.py` & `stable_baselines3-2.0.0a4/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_tensorboard.py` & `stable_baselines3-2.0.0a4/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_train_eval_mode.py` & `stable_baselines3-2.0.0a4/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_utils.py` & `stable_baselines3-2.0.0a4/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,18 @@
 @pytest.mark.parametrize("direct_policy", [False, True])
 def test_evaluate_policy(direct_policy: bool):
     model = A2C("MlpPolicy", "Pendulum-v1", seed=0)
     n_steps_per_episode, n_eval_episodes = 200, 2
 
     def dummy_callback(locals_, _globals):
         locals_["model"].n_callback_calls += 1
+        assert "observations" in locals_
+        assert "new_observations" in locals_
+        assert locals_["new_observations"] is not locals_["observations"]
+        assert not np.allclose(locals_["new_observations"], locals_["observations"])
 
     assert model.policy is not None
     policy = model.policy if direct_policy else model
 
     policy.n_callback_calls = 0  # type: ignore[assignment, attr-defined]
     _, episode_lengths = evaluate_policy(
         policy,  # type: ignore[arg-type]
```

### Comparing `stable_baselines3-2.0.0a2/tests/test_vec_check_nan.py` & `stable_baselines3-2.0.0a4/tests/test_vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_vec_envs.py` & `stable_baselines3-2.0.0a4/tests/test_vec_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_vec_monitor.py` & `stable_baselines3-2.0.0a4/tests/test_vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_vec_normalize.py` & `stable_baselines3-2.0.0a4/tests/test_vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a2/tests/test_vec_stacked_obs.py` & `stable_baselines3-2.0.0a4/tests/test_vec_stacked_obs.py`

 * *Files identical despite different names*

