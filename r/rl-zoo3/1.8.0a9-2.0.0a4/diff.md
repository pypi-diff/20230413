# Comparing `tmp/rl_zoo3-1.8.0a9.tar.gz` & `tmp/rl_zoo3-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rl_zoo3-1.8.0a9.tar", last modified: Sun Mar 12 19:19:03 2023, max compression
+gzip compressed data, was "rl_zoo3-2.0.0a4.tar", last modified: Thu Apr 13 14:54:20 2023, max compression
```

## Comparing `rl_zoo3-1.8.0a9.tar` & `rl_zoo3-2.0.0a4.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1071 2019-10-14 19:05:46.000000 rl_zoo3-1.8.0a9/LICENSE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      907 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14777 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1138 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      553 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6563 2023-01-03 10:43:05.000000 rl_zoo3-1.8.0a9/rl_zoo3/benchmark.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8688 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      668 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/cli.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10701 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/enjoy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    35639 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/exp_manager.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3594 2022-09-26 13:08:47.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/a2c.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4549 2022-09-19 19:35:53.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ars.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3039 2022-09-19 19:35:53.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ddpg.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1902 2022-12-11 16:01:58.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/dqn.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3680 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/her.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11668 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ppo.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11593 2023-03-12 18:55:26.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ppo_lstm.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1809 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/qrdqn.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5905 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/sac.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3248 2022-09-19 19:35:53.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/td3.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6090 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/tqc.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3850 2023-01-05 13:20:22.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/trpo.yml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20960 2023-03-12 18:55:26.000000 rl_zoo3-1.8.0a9/rl_zoo3/hyperparams_opt.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1453 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/import_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4606 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/load_from_hub.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      222 2023-01-25 22:48:07.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10804 2023-02-13 13:49:57.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/all_plots.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18815 2023-02-13 13:49:57.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/plot_from_file.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3485 2022-12-18 18:36:38.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/plot_train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2777 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/plots/score_normalization.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15239 2023-02-13 13:49:57.000000 rl_zoo3-1.8.0a9/rl_zoo3/push_to_hub.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/rl_zoo3/py.typed
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7044 2023-01-03 10:43:05.000000 rl_zoo3-1.8.0a9/rl_zoo3/record_training.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6142 2023-03-12 19:18:52.000000 rl_zoo3-1.8.0a9/rl_zoo3/record_video.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11407 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17117 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/version.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10479 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/rl_zoo3/wrappers.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      907 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1156 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       45 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/entry_points.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      138 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/rl_zoo3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/scripts/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       90 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/scripts/all_plots.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      105 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/scripts/plot_from_file.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       93 2022-10-31 13:58:40.000000 rl_zoo3-1.8.0a9/scripts/plot_train.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-03-12 19:19:03.000000 rl_zoo3-1.8.0a9/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2141 2023-03-12 19:18:55.000000 rl_zoo3-1.8.0a9/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1071 2019-10-14 19:05:46.000000 rl_zoo3-2.0.0a4/LICENSE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15989 2023-04-12 16:11:03.000000 rl_zoo3-2.0.0a4/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1477 2023-04-12 16:21:41.000000 rl_zoo3-2.0.0a4/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.784656 rl_zoo3-2.0.0a4/rl_zoo3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      672 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7346 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/benchmark.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8726 2023-04-13 14:26:15.000000 rl_zoo3-2.0.0a4/rl_zoo3/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      668 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/cli.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10854 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/enjoy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    36245 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/exp_manager.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3516 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/gym_patches.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3594 2022-09-26 13:08:47.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/a2c.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4549 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ars.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3039 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ddpg.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1902 2022-12-11 16:01:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/dqn.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3685 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/her.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12265 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11593 2023-03-12 18:55:26.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo_lstm.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1809 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/qrdqn.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5879 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/sac.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3248 2022-09-19 19:35:53.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/td3.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5772 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/tqc.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3850 2023-01-05 13:20:22.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/trpo.yml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20864 2023-03-20 14:17:58.000000 rl_zoo3-2.0.0a4/rl_zoo3/hyperparams_opt.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1657 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/import_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4606 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/load_from_hub.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/rl_zoo3/plots/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      222 2023-01-25 22:48:07.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10790 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/all_plots.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18815 2023-02-13 13:49:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_from_file.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3485 2022-12-18 18:36:38.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2777 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/plots/score_normalization.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15321 2023-04-12 12:35:57.000000 rl_zoo3-2.0.0a4/rl_zoo3/push_to_hub.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/rl_zoo3/py.typed
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7030 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/rl_zoo3/record_training.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6562 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/record_video.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11132 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17652 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/rl_zoo3/utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 14:14:10.000000 rl_zoo3-2.0.0a4/rl_zoo3/version.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12272 2023-04-13 13:47:23.000000 rl_zoo3-2.0.0a4/rl_zoo3/wrappers.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.784656 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1296 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       45 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/entry_points.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      150 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 14:54:20.000000 rl_zoo3-2.0.0a4/rl_zoo3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.780656 rl_zoo3-2.0.0a4/scripts/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       90 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/all_plots.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      105 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/plot_from_file.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       93 2022-10-31 13:58:40.000000 rl_zoo3-2.0.0a4/scripts/plot_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2174 2023-04-13 14:52:51.000000 rl_zoo3-2.0.0a4/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:54:20.788656 rl_zoo3-2.0.0a4/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      490 2023-03-20 14:11:48.000000 rl_zoo3-2.0.0a4/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4499 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_enjoy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4817 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_hyperparams_opt.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4407 2023-04-12 16:18:57.000000 rl_zoo3-2.0.0a4/tests/test_train.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1697 2023-04-12 14:32:14.000000 rl_zoo3-2.0.0a4/tests/test_wrappers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rl_zoo3-1.8.0a9/LICENSE` & `rl_zoo3-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/PKG-INFO` & `rl_zoo3-2.0.0a4/rl_zoo3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: rl_zoo3
-Version: 1.8.0a9
+Name: rl-zoo3
+Version: 2.0.0a4
 Summary: A Training Framework for Stable Baselines3 Reinforcement Learning Agents
 Home-page: https://github.com/DLR-RM/rl-baselines3-zoo
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
-Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines sb3 toolbox python data-science
+Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym gymnasium openai stable baselines sb3 toolbox python data-science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `rl_zoo3-1.8.0a9/README.md` & `rl_zoo3-2.0.0a4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 Please the see [dedicated section](https://rl-baselines3-zoo.readthedocs.io/en/master/guide/tuning.html) of the documentation.
 
 ## Custom Configuration
 
 Please the see [dedicated section](https://rl-baselines3-zoo.readthedocs.io/en/master/guide/config.html) of the documentation.
 
-## Current Collection: 195+ Trained Agents!
+## Current Collection: 200+ Trained Agents!
 
 Final performance of the trained agents can be found in [`benchmark.md`](./benchmark.md). To compute them, simply run `python -m rl_zoo3.benchmark`.
 
 List and videos of trained agents can be found on our Huggingface page: https://huggingface.co/sb3
 
 *NOTE: this is not a quantitative benchmark as it corresponds to only one run (cf [issue #38](https://github.com/araffin/rl-baselines-zoo/issues/38)). This benchmark is meant to check algorithm (maximal) performance, find potential bugs and also allow users to have access to pretrained agents.*
 
@@ -231,44 +231,31 @@
 |  RL Algo |  PandaReach | PandaPickAndPlace | PandaPush | PandaSlide | PandaStack |
 |----------|-------------|-------------------|-----------|------------|------------|
 | HER+TQC | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 
 
 ### MiniGrid Envs
 
-See https://github.com/maximecb/gym-minigrid
+See https://github.com/Farama-Foundation/Minigrid.
 A simple, lightweight and fast Gym environments implementation of the famous gridworld.
 
-|  RL Algo | Empty | FourRooms | DoorKey | MultiRoom | Fetch |
-|----------|-------|-----------|---------|-----------|-------|
-| A2C      | | | | | |
-| PPO      | |  |  | | |
-| DDPG     | | | | | |
-| SAC      | | | | | |
-| TRPO     | | | | | |
-
-There are 19 environment groups (variations for each) in total.
-
-Note that you need to specify `--gym-packages gym_minigrid` with `enjoy.py` and `train.py` as it is not a standard Gym environment, as well as installing the custom Gym package module or putting it in python path.
-
-```
-pip install gym-minigrid==1.0.3
-python train.py --algo ppo --env MiniGrid-DoorKey-5x5-v0 --gym-packages gym_minigrid
-```
+| RL Algo | Empty-Random-5x5   | FourRooms          | DoorKey-5x5        | MultiRoom-N4-S5    | Fetch-5x5-N2       | GoToDoor-5x5       | PutNear-6x6-N2     | RedBlueDoors-6x6   | LockedRoom         | KeyCorridorS3R1    | Unlock             | ObstructedMaze-2Dlh |
+| ------- | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | ------------------- |
+| A2C     |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                     |
+| PPO     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark:  |
+| DQN     |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                     |
+| QR-DQN  |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                     |
+| TRPO    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                     |
 
-This does the same thing as:
-
-```python
-import gym_minigrid
-```
+There are 22 environment groups (variations for each) in total.
 
 
 ## Colab Notebook: Try it Online!
 
-You can train agents online using [colab notebook](https://colab.research.google.com/github/Stable-Baselines-Team/rl-colab-notebooks/blob/sb3/rl-baselines-zoo.ipynb).
+You can train agents online using [Colab notebook](https://colab.research.google.com/github/Stable-Baselines-Team/rl-colab-notebooks/blob/sb3/rl-baselines-zoo.ipynb).
 
 ### Passing arguments in an interactive session
 
 The zoo is not meant to be executed from an interactive session (e.g: Jupyter Notebooks, IPython), however, it can be done by modifying `sys.argv` and adding the desired arguments.
 
 *Example*
 ```python
```

### Comparing `rl_zoo3-1.8.0a9/pyproject.toml` & `rl_zoo3-2.0.0a4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.ruff]
 # Same as Black.
 line-length = 127
 # Assume Python 3.7
 target-version = "py37"
-# TODO(antonin): activate "RUF" https://beta.ruff.rs/docs/rules/#ruff-specific-rules-ruf
-select = ["E", "F", "B", "UP", "C90"]
-ignore = []
+# See https://beta.ruff.rs/docs/rules/
+select = ["E", "F", "B", "UP", "C90", "RUF"]
+# Ignore explicit stacklevel`
+ignore = ["B028"]
 
 [tool.ruff.per-file-ignores]
 # "./rl_zoo3/plots/all_plots.py"= ["E501"]
 # "./rl_zoo3/plots/plot_train.py"= ["E501"]
 
 
 [tool.ruff.mccabe]
@@ -22,23 +23,25 @@
 [tool.isort]
 profile = "black"
 line_length = 127
 src_paths = ["stable_baselines3", "rl_zoo3"]
 
 [tool.pytype]
 inputs = ["."]
+exclude = ["tests/dummy_env"]
 # disable = []
 
 [tool.mypy]
 ignore_missing_imports = true
 follow_imports = "silent"
 show_error_codes = true
 exclude = """(?x)(
     rl_zoo3/hyperparams_opt.py$
     | rl_zoo3/exp_manager.py$
+    | tests/dummy_env/*$
   )"""
 
 [tool.pytest.ini_options]
 # Deterministic ordering for tests; useful for pytest-xdist.
 env = [
 	"PYTHONHASHSEED=0"
 ]
@@ -48,7 +51,21 @@
     "ignore::DeprecationWarning:tensorboard",
     # Gym warnings
     "ignore::UserWarning:gym",
 ]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')"
 ]
+
+[tool.coverage.run]
+disable_warnings = ["couldnt-parse"]
+branch = false
+omit = [
+	"tests/*",
+	"setup.py",
+	"rl_zoo3/plots/*",
+	"rl_zoo3/push_to_hub.py",
+	"scripts/*",
+]
+
+[tool.coverage.report]
+exclude_lines = [ "pragma: no cover", "raise NotImplementedError()", "if typing.TYPE_CHECKING:"]
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/benchmark.py` & `rl_zoo3-2.0.0a4/rl_zoo3/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import shutil
 import subprocess
 from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 import pytablewriter
+from huggingface_sb3 import EnvironmentName
 from stable_baselines3.common.results_plotter import load_results, ts2xy
 
+from rl_zoo3.load_from_hub import download_from_hub
 from rl_zoo3.utils import get_hf_trained_models, get_latest_run_id, get_saved_hyperparams, get_trained_models
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--log-dir", help="Root log folder", default="rl-trained-agents/", type=str)
 parser.add_argument("--benchmark-dir", help="Benchmark log folder", default="logs/benchmark/", type=str)
 parser.add_argument("-n", "--n-timesteps", help="number of timesteps", default=150000, type=int)
 parser.add_argument("--n-envs", help="number of environments", default=1, type=int)
@@ -37,15 +39,15 @@
     "mean_reward": [],
     "std_reward": [],
     "n_timesteps": [],
     "eval_timesteps": [],
     "eval_episodes": [],
 }
 
-for idx, trained_model in enumerate(trained_models.keys()):  # noqa: C901
+for idx, trained_model in enumerate(trained_models.keys()):
     algo, env_id = trained_models[trained_model]
     n_envs = args.n_envs
     n_timesteps = args.n_timesteps
 
     # HER is now a replay buffer class
     if algo == "her":
         continue
@@ -94,25 +96,43 @@
         print(f"Skipping mujoco env: {env_id}")
         if not skip_eval:
             continue
 
     if skip_eval:
         print("Skipping eval...")
     else:
-        return_code = subprocess.call(["python", "enjoy.py"] + arguments)
+        return_code = subprocess.call(["python", "enjoy.py", *arguments])
         if return_code != 0:
             print("Error during evaluation, skipping...")
             continue
         x, y = ts2xy(load_results(reward_log), "timesteps")
 
     if len(x) > 0:
         # Retrieve training timesteps from config
         exp_id = get_latest_run_id(os.path.join(args.log_dir, algo), env_id)
         log_path = os.path.join(args.log_dir, algo, f"{env_id}_{exp_id}", env_id)
         hyperparams, _ = get_saved_hyperparams(log_path)
+        # Model not downloaded
+        if len(hyperparams) == 0:
+            print("Pretrained model not found, trying to download it from sb3 Huggingface hub: https://huggingface.co/sb3")
+            exp_id = 1
+            log_path = os.path.join(args.log_dir, algo, f"{env_id}_{exp_id}", env_id)
+            # Auto-download
+            download_from_hub(
+                algo=algo,
+                env_name=EnvironmentName(env_id),
+                exp_id=exp_id,
+                folder=args.log_dir,
+                organization="sb3",
+                repo_name=None,
+                force=False,
+            )
+            # Try again
+            hyperparams, _ = get_saved_hyperparams(log_path)
+
         # Hack to format it properly
         if hyperparams["n_timesteps"] < 1e6:
             n_training_timesteps = f"{int(hyperparams['n_timesteps'] / 1e3)}k"
         else:
             n_training_timesteps = f"{int(hyperparams['n_timesteps'] / 1e6)}M"
 
         mean_reward = np.mean(y)
@@ -147,15 +167,15 @@
 writer = pytablewriter.MarkdownTableWriter(max_precision=3)
 writer.from_dataframe(results_df)
 
 header = """
 ## Performance of trained agents
 
 Final performance of the trained agents can be found in the table below.
-This was computed by running `python -m utils.benchmark`:
+This was computed by running `python -m rl_zoo3.benchmark`:
 it runs the trained agent (trained on `n_timesteps`) for `eval_timesteps` and then reports the mean episode reward
 during this evaluation.
 
 It uses the deterministic policy except for Atari games.
 
 You can view each model card (it includes video and hyperparameters)
 on our Huggingface page: https://huggingface.co/sb3
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/callbacks.py` & `rl_zoo3-2.0.0a4/rl_zoo3/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,16 @@
 
     def _on_rollout_end(self) -> None:
         # Make mypy happy
         assert isinstance(self.model, (SAC, TQC))
 
         if self._model_ready:
             self._model.replay_buffer = deepcopy(self.model.replay_buffer)
-            self.model.set_parameters(deepcopy(self._model.get_parameters()))
-            self.model.actor = self.model.policy.actor  # type: ignore[union-attr, attr-defined]
+            self.model.set_parameters(deepcopy(self._model.get_parameters()))  # type: ignore[arg-type]
+            self.model.actor = self.model.policy.actor  # type: ignore[union-attr, attr-defined, assignment]
             if self.num_timesteps >= self._model.learning_starts:
                 self.train()
             # Do not wait for the training loop to finish
             # self.process.join()
 
     def _on_training_end(self) -> None:
         # Wait for the thread to terminate
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/cli.py` & `rl_zoo3-2.0.0a4/rl_zoo3/cli.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/enjoy.py` & `rl_zoo3-2.0.0a4/rl_zoo3/enjoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     parser.add_argument("--seed", help="Random generator seed", type=int, default=0)
     parser.add_argument("--reward-log", help="Where to log reward", default="", type=str)
     parser.add_argument(
         "--gym-packages",
         type=str,
         nargs="+",
         default=[],
-        help="Additional external Gym environment package modules to import (e.g. gym_minigrid)",
+        help="Additional external Gym environment package modules to import",
     )
     parser.add_argument(
         "--env-kwargs", type=str, nargs="+", action=StoreDict, help="Optional keyword argument to pass to the env constructor"
     )
     parser.add_argument(
         "--custom-objects", action="store_true", default=False, help="Use custom objects to solve loading issues"
     )
@@ -133,14 +133,15 @@
 
     if args.num_threads > 0:
         if args.verbose > 1:
             print(f"Setting torch.num_threads to {args.num_threads}")
         th.set_num_threads(args.num_threads)
 
     is_atari = ExperimentManager.is_atari(env_name.gym_id)
+    is_minigrid = ExperimentManager.is_minigrid(env_name.gym_id)
 
     stats_path = os.path.join(log_path, env_name)
     hyperparams, maybe_stats_path = get_saved_hyperparams(stats_path, norm_reward=args.norm_reward, test_mode=True)
 
     # load env_kwargs if existing
     env_kwargs = {}
     args_path = os.path.join(log_path, env_name, "args.yml")
@@ -184,20 +185,22 @@
     if newer_python_version or args.custom_objects:
         custom_objects = {
             "learning_rate": 0.0,
             "lr_schedule": lambda _: 0.0,
             "clip_range": lambda _: 0.0,
         }
 
-    model = ALGOS[algo].load(model_path, env=env, custom_objects=custom_objects, device=args.device, **kwargs)
+    if "HerReplayBuffer" in hyperparams.get("replay_buffer_class", ""):
+        kwargs["env"] = env
 
+    model = ALGOS[algo].load(model_path, custom_objects=custom_objects, device=args.device, **kwargs)
     obs = env.reset()
 
     # Deterministic by default except for atari games
-    stochastic = args.stochastic or is_atari and not args.deterministic
+    stochastic = args.stochastic or (is_atari or is_minigrid) and not args.deterministic
     deterministic = not stochastic
 
     episode_reward = 0.0
     episode_rewards, episode_lengths = [], []
     ep_len = 0
     # For HER, monitor success rate
     successes = []
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/exp_manager.py` & `rl_zoo3-2.0.0a4/rl_zoo3/exp_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 import time
 import warnings
 from collections import OrderedDict
 from pathlib import Path
 from pprint import pprint
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-import gym
+import gym as gym26
+import gymnasium as gym
 import numpy as np
 import optuna
 import torch as th
 import yaml
-from gym import spaces
+from gymnasium import spaces
 from huggingface_sb3 import EnvironmentName
 from optuna.pruners import BasePruner, MedianPruner, NopPruner, SuccessiveHalvingPruner
 from optuna.samplers import BaseSampler, RandomSampler, TPESampler
 from optuna.study import MaxTrialsCallback
 from optuna.trial import TrialState
 from optuna.visualization import plot_optimization_history, plot_param_importances
 from sb3_contrib.common.vec_env import AsyncEval
 
 # For using HER with GoalEnv
-from stable_baselines3 import HerReplayBuffer  # noqa: F401
+from stable_baselines3 import HerReplayBuffer
 from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.callbacks import BaseCallback, CheckpointCallback, EvalCallback, ProgressBarCallback
 from stable_baselines3.common.env_util import make_vec_env
 from stable_baselines3.common.noise import NormalActionNoise, OrnsteinUhlenbeckActionNoise
 from stable_baselines3.common.preprocessing import is_image_space, is_image_space_channels_first
 from stable_baselines3.common.sb2_compat.rmsprop_tf_like import RMSpropTFLike  # noqa: F401
 from stable_baselines3.common.utils import constant_fn
@@ -39,15 +40,15 @@
     VecFrameStack,
     VecNormalize,
     VecTransposeImage,
     is_vecenv_wrapped,
 )
 
 # For custom activation fn
-from torch import nn as nn  # noqa: F401
+from torch import nn as nn
 
 # Register custom envs
 import rl_zoo3.import_envs  # noqa: F401 pytype: disable=import-error
 from rl_zoo3.callbacks import SaveVecNormalizeCallback, TrialEvalCallback
 from rl_zoo3.hyperparams_opt import HYPERPARAMS_SAMPLER
 from rl_zoo3.utils import ALGOS, get_callback_list, get_class_by_name, get_latest_run_id, get_wrapper_class, linear_schedule
 
@@ -154,15 +155,15 @@
         self.max_total_trials = max_total_trials
         # number of parallel jobs when doing hyperparameter search
         self.n_jobs = n_jobs
         self.sampler = sampler
         self.pruner = pruner
         self.n_startup_trials = n_startup_trials
         self.n_evaluations = n_evaluations
-        self.deterministic_eval = not self.is_atari(env_id)
+        self.deterministic_eval = not (self.is_atari(env_id) or self.is_minigrid(env_id))
         self.device = device
 
         # Logging
         self.log_folder = log_folder
         self.tensorboard_log = None if tensorboard_log == "" else os.path.join(tensorboard_log, self.env_name)
         self.verbose = verbose
         self.args = args
@@ -357,15 +358,15 @@
             # Use the same discount factor as for the algorithm
             if "gamma" in hyperparams:
                 self.normalize_kwargs["gamma"] = hyperparams["gamma"]
 
             del hyperparams["normalize"]
         return hyperparams
 
-    def _preprocess_hyperparams(
+    def _preprocess_hyperparams(  # noqa: C901
         self, hyperparams: Dict[str, Any]
     ) -> Tuple[Dict[str, Any], Optional[Callable], List[BaseCallback], Optional[Callable]]:
         self.n_envs = hyperparams.get("n_envs", 1)
 
         if self.verbose > 0:
             print(f"Using {self.n_envs} environments")
 
@@ -508,32 +509,41 @@
                 eval_freq=self.eval_freq,
                 deterministic=self.deterministic_eval,
             )
 
             self.callbacks.append(eval_callback)
 
     @staticmethod
+    def entry_point(env_id: str) -> str:
+        try:
+            return str(gym.envs.registry[env_id].entry_point)  # pytype: disable=module-attr
+        except KeyError:
+            return str(gym26.envs.registry[env_id].entry_point)  # pytype: disable=module-attr
+
+    @staticmethod
     def is_atari(env_id: str) -> bool:
-        entry_point = gym.envs.registry.env_specs[env_id].entry_point  # pytype: disable=module-attr
-        return "AtariEnv" in str(entry_point)
+        return "AtariEnv" in ExperimentManager.entry_point(env_id)
+
+    @staticmethod
+    def is_minigrid(env_id: str) -> bool:
+        return "minigrid" in ExperimentManager.entry_point(env_id)
 
     @staticmethod
     def is_bullet(env_id: str) -> bool:
-        entry_point = gym.envs.registry.env_specs[env_id].entry_point  # pytype: disable=module-attr
-        return "pybullet_envs" in str(entry_point)
+        return "pybullet_envs" in ExperimentManager.entry_point(env_id)
 
     @staticmethod
     def is_robotics_env(env_id: str) -> bool:
-        entry_point = gym.envs.registry.env_specs[env_id].entry_point  # pytype: disable=module-attr
-        return "gym.envs.robotics" in str(entry_point) or "panda_gym.envs" in str(entry_point)
+        return "gym.envs.robotics" in ExperimentManager.entry_point(
+            env_id
+        ) or "panda_gym.envs" in ExperimentManager.entry_point(env_id)
 
     @staticmethod
     def is_panda_gym(env_id: str) -> bool:
-        entry_point = gym.envs.registry.env_specs[env_id].entry_point  # pytype: disable=module-attr
-        return "panda_gym.envs" in str(entry_point)
+        return "panda_gym.envs" in ExperimentManager.entry_point(env_id)
 
     def _maybe_normalize(self, env: VecEnv, eval_env: bool) -> VecEnv:
         """
         Wrap the env into a VecNormalize wrapper if needed
         and load saved statistics when present.
 
         :param env:
@@ -586,18 +596,27 @@
             "Neck" in self.env_name.gym_id
             or self.is_robotics_env(self.env_name.gym_id)
             or "parking-v0" in self.env_name.gym_id
             and len(self.monitor_kwargs) == 0  # do not overwrite custom kwargs
         ):
             self.monitor_kwargs = dict(info_keywords=("is_success",))
 
-        # Define make_env here so it works with subprocesses
-        # when the registry was modified with `--gym-packages`
-        # See https://github.com/HumanCompatibleAI/imitation/pull/160
-        spec = gym.spec(self.env_name.gym_id)
+        # Make Pybullet compatible with gym 0.26
+        if self.is_bullet(self.env_name.gym_id):
+            spec = gym26.spec(self.env_name.gym_id)
+            self.env_kwargs.update(dict(apply_api_compatibility=True))
+        else:
+            # Define make_env here so it works with subprocesses
+            # when the registry was modified with `--gym-packages`
+            # See https://github.com/HumanCompatibleAI/imitation/pull/160
+            try:
+                spec = gym.spec(self.env_name.gym_id)
+            except gym.error.NameNotFound:
+                # Registered with gym 0.26
+                spec = gym26.spec(self.env_name.gym_id)
 
         def make_env(**kwargs) -> gym.Env:
             env = spec.make(**kwargs)
             return env
 
         # On most env, SubprocVecEnv does not help and is quite memory hungry
         # therefore we use DummyVecEnv by default
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/a2c.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/a2c.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ars.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ars.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ddpg.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ddpg.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/dqn.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/dqn.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/her.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/her.yml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   policy_kwargs: "dict(n_critics=2, net_arch=[512, 512, 512])"
   online_sampling: True
 
 
 FetchPickAndPlace-v1:
   env_wrapper:
     - sb3_contrib.common.wrappers.TimeFeatureWrapper
-    # - rl_zoo3.wrappers.DoneOnSuccessWrapper:
+    # - rl_zoo3.wrappers.TruncatedOnSuccessWrapper:
     #     reward_offset: 0
     #     n_successes: 4
     # - stable_baselines3.common.monitor.Monitor
   n_timesteps: !!float 1e6
   policy: 'MlpPolicy'
   model_class: 'tqc'
   n_sampled_goal: 4
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ppo.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo.yml`

 * *Files 6% similar despite different names*

```diff
@@ -280,48 +280,78 @@
   gae_lambda: 0.95
   gamma: 0.99
   n_epochs: 10
   ent_coef: 0.0
   learning_rate: 2.5e-4
   clip_range: 0.2
 
+
 # Following https://github.com/lcswillems/rl-starter-files
-# requires --gym-packages gym_minigrid
-MiniGrid-DoorKey-5x5-v0:
-  # Dict Observations are now supported
-  # env_wrapper: gym_minigrid.wrappers.FlatObsWrapper
+MiniGrid-Empty-Random-5x5-v0: &minigrid-defaults
+  env_wrapper: minigrid.wrappers.FlatObsWrapper # See GH/1320#issuecomment-1421108191
   normalize: true
   n_envs: 8 # number of environment copies running in parallel
   n_timesteps: !!float 1e5
-  policy: 'MultiInputPolicy'
+  policy: 'MlpPolicy'
   n_steps: 128 # batch size is n_steps * n_env
   batch_size: 64 # Number of training minibatches per update
   gae_lambda: 0.95 #  Factor for trade-off of bias vs variance for Generalized Advantage Estimator
   gamma: 0.99
   n_epochs: 10 #  Number of epoch when optimizing the surrogate
   ent_coef: 0.0 # Entropy coefficient for the loss caculation
   learning_rate: 2.5e-4 # The learning rate, it can be a function
   clip_range: 0.2 # Clipping parameter, it can be a function
 
-# requires --gym-packages gym_minigrid
 MiniGrid-FourRooms-v0:
-  normalize: true
-  n_envs: 8
-  n_timesteps: !!float 4e6
-  policy: 'MultiInputPolicy'
+  <<: *minigrid-defaults
+  n_timesteps: !!float 5e6
   n_steps: 512
-  batch_size: 64
-  gae_lambda: 0.95
-  gamma: 0.99
-  n_epochs: 10
-  ent_coef: 0.0
-  learning_rate: 2.5e-4
-  clip_range: 0.2
 
-CarRacing-v0:
+MiniGrid-DoorKey-5x5-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e5
+
+MiniGrid-MultiRoom-N4-S5-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e7 # Unsolved
+
+MiniGrid-Fetch-5x5-N2-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 5e6
+
+MiniGrid-GoToDoor-5x5-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 5e6
+
+MiniGrid-PutNear-6x6-N2-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e7
+
+MiniGrid-RedBlueDoors-6x6-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e6
+  n_steps: 512
+
+MiniGrid-LockedRoom-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e7 # Unsolved
+
+MiniGrid-KeyCorridorS3R1-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 5e5
+
+MiniGrid-Unlock-v0:
+  <<: *minigrid-defaults
+
+MiniGrid-ObstructedMaze-2Dlh-v0:
+  <<: *minigrid-defaults
+  n_timesteps: !!float 1e7 # Unsolved
+
+
+CarRacing-v1:
   env_wrapper:
     - rl_zoo3.wrappers.FrameSkip:
         skip: 2
     - gym.wrappers.resize_observation.ResizeObservation:
         shape: 64
     - gym.wrappers.gray_scale_observation.GrayScaleObservation:
         keep_dim: true
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/ppo_lstm.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/ppo_lstm.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/qrdqn.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/qrdqn.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/sac.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/sac.yml`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
   batch_size: 256
   ent_coef: 'auto'
   train_freq: 1
   gradient_steps: 1
   learning_starts: 10000
 
 # To be tuned
-CarRacing-v0:
+CarRacing-v1:
   env_wrapper:
     - rl_zoo3.wrappers.FrameSkip:
         skip: 2
     # wrapper from https://github.com/araffin/aae-train-donkeycar
     - ae.wrapper.AutoencoderWrapper:
         ae_path: "logs/car_racing_rgb_160.pkl"
     - rl_zoo3.wrappers.HistoryWrapper:
@@ -221,15 +221,14 @@
   batch_size: 256
   gamma: 0.95
   learning_rate: 0.001
   learning_starts: 1000
   normalize: True
   replay_buffer_class: HerReplayBuffer
   replay_buffer_kwargs: "dict(
-    online_sampling=True,
     goal_selection_strategy='future',
     n_sampled_goal=4
   )"
   policy_kwargs: "dict(net_arch=[64, 64])"
 
 
 # ==== Custom Envs ===
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/td3.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/td3.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/tqc.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/tqc.yml`

 * *Files 6% similar despite different names*

```diff
@@ -161,70 +161,64 @@
 
 Swimmer-v3:
   <<: *mujoco-defaults
   gamma: 0.9999
 
 # === HER Robotics GoalEnvs ===
 FetchReach-v1:
-  env_wrapper: sb3_contrib.common.wrappers.TimeFeatureWrapper
   n_timesteps: !!float 20000
   policy: 'MultiInputPolicy'
   buffer_size: 1000000
   ent_coef: 'auto'
   batch_size: 256
   gamma: 0.95
   learning_rate: 0.001
   learning_starts: 1000
   normalize: True
   replay_buffer_class: HerReplayBuffer
   replay_buffer_kwargs: "dict(
-    online_sampling=True,
     goal_selection_strategy='future',
     n_sampled_goal=4
   )"
   policy_kwargs: "dict(net_arch=[64, 64], n_critics=1)"
 
 FetchPush-v1: &her-defaults
-  env_wrapper: sb3_contrib.common.wrappers.TimeFeatureWrapper
   n_timesteps: !!float 1e6
   policy: 'MultiInputPolicy'
   buffer_size: 1000000
   batch_size: 2048
   gamma: 0.95
   learning_rate: !!float 1e-3
   tau: 0.05
   replay_buffer_class: HerReplayBuffer
   replay_buffer_kwargs: "dict(
-    online_sampling=True,
     goal_selection_strategy='future',
     n_sampled_goal=4,
   )"
   policy_kwargs: "dict(net_arch=[512, 512, 512], n_critics=2)"
 
 FetchSlide-v1:
   <<: *her-defaults
   n_timesteps: !!float 3e6
 
 FetchPickAndPlace-v1:
   <<: *her-defaults
 
 PandaReach-v1:
-  env_wrapper: sb3_contrib.common.wrappers.TimeFeatureWrapper
   n_timesteps: !!float 20000
   policy: 'MultiInputPolicy'
   buffer_size: 1000000
   ent_coef: 'auto'
   batch_size: 256
   gamma: 0.95
   learning_rate: 0.001
   learning_starts: 1000
   normalize: True
   replay_buffer_class: HerReplayBuffer
   replay_buffer_kwargs: "dict(
-    online_sampling=True,
     goal_selection_strategy='future',
     n_sampled_goal=4
   )"
   policy_kwargs: "dict(net_arch=[64, 64], n_critics=1)"
 
 PandaPush-v1:
   <<: *her-defaults
@@ -245,18 +239,16 @@
   buffer_size: 1000000
   batch_size: 512
   gamma: 0.98
   learning_rate: !!float 1.5e-3
   tau: 0.005
   replay_buffer_class: HerReplayBuffer
   replay_buffer_kwargs: "dict(
-    online_sampling=False,
     goal_selection_strategy='episode',
     n_sampled_goal=4,
-    max_episode_length=100
   )"
 
 # Tuned
 CarRacing-v0:
   env_wrapper:
     - rl_zoo3.wrappers.FrameSkip:
         skip: 2
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams/trpo.yml` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams/trpo.yml`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/hyperparams_opt.py` & `rl_zoo3-2.0.0a4/rl_zoo3/hyperparams_opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,14 @@
     :return:
     """
     her_kwargs = trial.her_kwargs.copy()
     her_kwargs["n_sampled_goal"] = trial.suggest_int("n_sampled_goal", 1, 5)
     her_kwargs["goal_selection_strategy"] = trial.suggest_categorical(
         "goal_selection_strategy", ["final", "episode", "future"]
     )
-    her_kwargs["online_sampling"] = trial.suggest_categorical("online_sampling", [True, False])
     hyperparams["replay_buffer_kwargs"] = her_kwargs
     return hyperparams
 
 
 def sample_tqc_params(trial: optuna.Trial) -> Dict[str, Any]:
     """
     Sampler for TQC hyperparams.
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/import_envs.py` & `rl_zoo3-2.0.0a4/rl_zoo3/import_envs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import gym
-from gym.envs.registration import register
+from typing import Optional
+
+import gymnasium as gym
+from gymnasium.envs.registration import register
 
 from rl_zoo3.wrappers import MaskVelocityWrapper
 
 try:
     import pybullet_envs  # pytype: disable=import-error
 except ImportError:
     pybullet_envs = None
@@ -44,19 +46,24 @@
     panda_gym = None
 
 try:
     import rocket_lander_gym  # pytype: disable=import-error
 except ImportError:
     rocket_lander_gym = None
 
+try:
+    import minigrid  # pytype: disable=import-error
+except ImportError:
+    minigrid = None
+
 
 # Register no vel envs
 def create_no_vel_env(env_id: str):
-    def make_env():
-        env = gym.make(env_id)
+    def make_env(render_mode: Optional[str] = None):
+        env = gym.make(env_id, render_mode=render_mode)
         env = MaskVelocityWrapper(env)
         return env
 
     return make_env
 
 
 for env_id in MaskVelocityWrapper.velocity_indices.keys():
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/load_from_hub.py` & `rl_zoo3-2.0.0a4/rl_zoo3/load_from_hub.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/plots/all_plots.py` & `rl_zoo3-2.0.0a4/rl_zoo3/plots/all_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     post_processed_results = {}
 
     args.algos = [algo.upper() for algo in args.algos]
 
     if args.labels is None:
         args.labels = args.exp_folders
 
-    for env in args.env:  # noqa: C901
+    for env in args.env:
         plt.figure(f"Results {env}")
         plt.title(f"{env}", fontsize=14)
 
         x_label_suffix = "" if args.no_million else "(in Million)"
         plt.xlabel(f"Timesteps {x_label_suffix}", fontsize=14)
         plt.ylabel("Score", fontsize=14)
         results[env] = {}
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/plots/plot_from_file.py` & `rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_from_file.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/plots/plot_train.py` & `rl_zoo3-2.0.0a4/rl_zoo3/plots/plot_train.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/plots/score_normalization.py` & `rl_zoo3-2.0.0a4/rl_zoo3/plots/score_normalization.py`

 * *Files identical despite different names*

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/push_to_hub.py` & `rl_zoo3-2.0.0a4/rl_zoo3/push_to_hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
 
     if args.num_threads > 0:
         if args.verbose > 1:
             print(f"Setting torch.num_threads to {args.num_threads}")
         th.set_num_threads(args.num_threads)
 
     is_atari = ExperimentManager.is_atari(env_name.gym_id)
+    is_minigrid = ExperimentManager.is_minigrid(env_name.gym_id)
 
     stats_path = os.path.join(log_path, env_name)
     hyperparams, maybe_stats_path = get_saved_hyperparams(stats_path, test_mode=True)
 
     # load env_kwargs if existing
     env_kwargs = {}
     args_path = os.path.join(log_path, env_name, "args.yml")
@@ -378,15 +379,15 @@
 
     # Note: we assume that we push models using the same machine (same python version)
     # that trained them, if not, we would need to pass custom object as in enjoy.py
     custom_objects: Dict[str, Any] = {}
     model = ALGOS[algo].load(model_path, env=eval_env, custom_objects=custom_objects, device=args.device, **kwargs)
 
     # Deterministic by default except for atari games
-    stochastic = args.stochastic or is_atari and not args.deterministic
+    stochastic = args.stochastic or (is_atari or is_minigrid) and not args.deterministic
     deterministic = not stochastic
 
     # Default model name, the model will be saved under "{algo}-{env_name}.zip"
     model_name = ModelName(algo, env_name)
 
     if args.repo_name is None:
         args.repo_name = model_name
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/record_training.py` & `rl_zoo3-2.0.0a4/rl_zoo3/record_training.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 from copy import deepcopy
 
 from huggingface_sb3 import EnvironmentName
 
 from rl_zoo3.utils import ALGOS, get_latest_run_id
 
-if __name__ == "__main__":  # noqa: C901
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--env", help="environment ID", type=EnvironmentName, default="CartPole-v1")
     parser.add_argument("-f", "--folder", help="Log folder", type=str, default="rl-trained-agents")
     parser.add_argument("-o", "--output-folder", help="Output folder", type=str)
     parser.add_argument("--algo", help="RL Algorithm", default="ppo", type=str, required=False, choices=list(ALGOS.keys()))
     parser.add_argument("-n", "--n-timesteps", help="number of timesteps", default=1000, type=int)
     parser.add_argument("--n-envs", help="number of environments", default=1, type=int)
@@ -75,27 +75,27 @@
         # Disable rendering to generate videos faster
         "--no-render",
     ]
     if deterministic is not None:
         args_final_model.append("--deterministic")
 
     if os.path.exists(os.path.join(log_path, f"{env_name}.zip")):
-        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video"] + args_final_model)
+        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video", *args_final_model])
         assert return_code == 0, "Failed to record the final model"
 
     if os.path.exists(os.path.join(log_path, "best_model.zip")):
-        args_best_model = args_final_model + ["--load-best"]
-        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video"] + args_best_model)
+        args_best_model = [*args_final_model, "--load-best"]
+        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video", *args_best_model])
         assert return_code == 0, "Failed to record the best model"
 
-    args_checkpoint = args_final_model + ["--load-checkpoint"]
+    args_checkpoint = [*args_final_model, "--load-checkpoint"]
     args_checkpoint.append("0")
     for checkpoint in checkpoints:
         args_checkpoint[-1] = str(checkpoint)
-        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video"] + args_checkpoint)
+        return_code = subprocess.call(["python", "-m", "rl_zoo3.record_video", *args_checkpoint])
         assert return_code == 0, f"Failed to record the {checkpoint} checkpoint model"
 
     # add text to each video
     episode_videos_names = [dir_ent.name for dir_ent in os.scandir(video_folder) if dir_ent.name.endswith(".mp4")]
 
     checkpoints_videos_names = list(filter(lambda x: x.startswith("checkpoint"), episode_videos_names))
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/record_video.py` & `rl_zoo3-2.0.0a4/rl_zoo3/record_video.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from huggingface_sb3 import EnvironmentName
 from stable_baselines3.common.utils import set_random_seed
 from stable_baselines3.common.vec_env import VecVideoRecorder
 
 from rl_zoo3.exp_manager import ExperimentManager
 from rl_zoo3.utils import ALGOS, StoreDict, create_test_env, get_model_path, get_saved_hyperparams
 
-if __name__ == "__main__":  # noqa: C901
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--env", help="environment ID", type=EnvironmentName, default="CartPole-v1")
     parser.add_argument("-f", "--folder", help="Log folder", type=str, default="rl-trained-agents")
     parser.add_argument("-o", "--output-folder", help="Output folder", type=str)
     parser.add_argument("--algo", help="RL Algorithm", default="ppo", type=str, required=False, choices=list(ALGOS.keys()))
     parser.add_argument("-n", "--n-timesteps", help="number of timesteps", default=1000, type=int)
     parser.add_argument("--n-envs", help="number of environments", default=1, type=int)
@@ -69,14 +69,15 @@
 
     print(f"Loading {model_path}")
     off_policy_algos = ["qrdqn", "dqn", "ddpg", "sac", "her", "td3", "tqc"]
 
     set_random_seed(args.seed)
 
     is_atari = ExperimentManager.is_atari(env_name.gym_id)
+    is_minigrid = ExperimentManager.is_minigrid(env_name.gym_id)
 
     stats_path = os.path.join(log_path, env_name)
     hyperparams, maybe_stats_path = get_saved_hyperparams(stats_path)
 
     # load env_kwargs if existing
     env_kwargs = {}
     args_path = os.path.join(log_path, env_name, "args.yml")
@@ -85,14 +86,17 @@
             loaded_args = yaml.load(f, Loader=yaml.UnsafeLoader)  # pytype: disable=module-attr
             if loaded_args["env_kwargs"] is not None:
                 env_kwargs = loaded_args["env_kwargs"]
     # overwrite with command line arguments
     if args.env_kwargs is not None:
         env_kwargs.update(args.env_kwargs)
 
+    # Force rgb_array rendering (gym 0.26+)
+    env_kwargs.update(render_mode="rgb_array")
+
     env = create_test_env(
         env_name.gym_id,
         n_envs=n_envs,
         stats_path=maybe_stats_path,
         seed=seed,
         log_dir=None,
         should_render=not args.no_render,
@@ -123,20 +127,26 @@
         }
 
     print(f"Loading {model_path}")
 
     model = ALGOS[algo].load(model_path, env=env, custom_objects=custom_objects, **kwargs)
 
     # Deterministic by default except for atari games
-    stochastic = args.stochastic or is_atari and not args.deterministic
+    stochastic = args.stochastic or (is_atari or is_minigrid) and not args.deterministic
     deterministic = not stochastic
 
     if video_folder is None:
         video_folder = os.path.join(log_path, "videos")
 
+    if is_atari:
+        # Patch Atari for rendering
+        # see https://github.com/mgbellemare/Arcade-Learning-Environment/issues/473
+        env.unwrapped.render_mode = env_kwargs.get("render_mode")
+        env.render_mode = env_kwargs.get("render_mode")
+
     # Note: apparently it renders by default
     env = VecVideoRecorder(
         env,
         video_folder,
         record_video_trigger=lambda x: x == 0,
         video_length=video_length,
         name_prefix=name_prefix,
@@ -149,15 +159,15 @@
         for _ in range(video_length + 1):
             action, lstm_states = model.predict(
                 obs,  # type: ignore[arg-type]
                 state=lstm_states,
                 episode_start=episode_starts,
                 deterministic=deterministic,
             )
-            obs, _, dones, _ = env.step(action)  # type: ignore[assignment]
-            episode_starts = dones
             if not args.no_render:
                 env.render()
+            obs, _, dones, _ = env.step(action)  # type: ignore[assignment]
+            episode_starts = dones
     except KeyboardInterrupt:
         pass
 
     env.close()
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/train.py` & `rl_zoo3-2.0.0a4/rl_zoo3/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 import difflib
 import importlib
 import os
 import time
 import uuid
 
-import gym
+import gym as gym26
+import gymnasium as gym
 import numpy as np
 import stable_baselines3 as sb3
 import torch as th
 from stable_baselines3.common.utils import set_random_seed
 
 # Register custom envs
 import rl_zoo3.import_envs  # noqa: F401 pytype: disable=import-error
@@ -105,15 +106,15 @@
     parser.add_argument("--study-name", help="Study name for distributed optimization", type=str, default=None)
     parser.add_argument("--verbose", help="Verbose mode (0: no output, 1: INFO)", default=1, type=int)
     parser.add_argument(
         "--gym-packages",
         type=str,
         nargs="+",
         default=[],
-        help="Additional external Gym environment package modules to import (e.g. gym_minigrid)",
+        help="Additional external Gym environment package modules to import",
     )
     parser.add_argument(
         "--env-kwargs", type=str, nargs="+", action=StoreDict, help="Optional keyword argument to pass to the env constructor"
     )
     parser.add_argument(
         "-params",
         "--hyperparams",
@@ -126,21 +127,14 @@
         "-conf",
         "--conf-file",
         type=str,
         default=None,
         help="Custom yaml file or python package from which the hyperparameters will be loaded."
         "We expect that python packages contain a dictionary called 'hyperparams' which contains a key for each environment.",
     )
-    parser.add_argument(
-        "-yaml",
-        "--yaml-file",
-        type=str,
-        default=None,
-        help="This parameter is deprecated, please use `--conf-file` instead",
-    )
     parser.add_argument("-uuid", "--uuid", action="store_true", default=False, help="Ensure that the run has a unique ID")
     parser.add_argument(
         "--track",
         action="store_true",
         default=False,
         help="if toggled, this experiment will be tracked with Weights and Biases",
     )
@@ -160,20 +154,17 @@
     args = parser.parse_args()
 
     # Going through custom gym packages to let them register in the global registory
     for env_module in args.gym_packages:
         importlib.import_module(env_module)
 
     env_id = args.env
-    registered_envs = set(gym.envs.registry.env_specs.keys())  # pytype: disable=module-attr
-
-    if args.yaml_file is not None:
-        raise ValueError(
-            "The`--yaml-file` parameter is deprecated and will be removed in RL Zoo3 v1.8, please use `--conf-file` instead",
-        )
+    registered_envs = set(gym.envs.registry.keys())  # pytype: disable=module-attr
+    # Add gym 0.26 envs
+    registered_envs.update(gym26.envs.registry.keys())  # pytype: disable=module-attr
 
     # If the environment is not found, suggest the closest match
     if env_id not in registered_envs:
         try:
             closest_match = difflib.get_close_matches(env_id, registered_envs, n=1)[0]
         except IndexError:
             closest_match = "'no close match found...'"
@@ -206,15 +197,15 @@
             import wandb
         except ImportError as e:
             raise ImportError(
                 "if you want to use Weights & Biases to track experiment, please install W&B via `pip install wandb`"
             ) from e
 
         run_name = f"{args.env}__{args.algo}__{args.seed}__{int(time.time())}"
-        tags = args.wandb_tags + [f"v{sb3.__version__}"]
+        tags = [*args.wandb_tags, f"v{sb3.__version__}"]
         run = wandb.init(
             name=run_name,
             project=args.wandb_project_name,
             entity=args.wandb_entity,
             tags=tags,
             config=vars(args),
             sync_tensorboard=True,  # auto-upload sb3's tensorboard metrics
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/utils.py` & `rl_zoo3-2.0.0a4/rl_zoo3/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import argparse
 import glob
 import importlib
 import os
+from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
-import gym
+import gym as gym26
+import gymnasium as gym
 import stable_baselines3 as sb3  # noqa: F401
 import torch as th  # noqa: F401
 import yaml
-from gym import spaces
+from gymnasium import spaces
 from huggingface_hub import HfApi
 from huggingface_sb3 import EnvironmentName, ModelName
 from sb3_contrib import ARS, QRDQN, TQC, TRPO, RecurrentPPO
 from stable_baselines3 import A2C, DDPG, DQN, PPO, SAC, TD3
 from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.callbacks import BaseCallback
 from stable_baselines3.common.env_util import make_vec_env
 from stable_baselines3.common.sb2_compat.rmsprop_tf_like import RMSpropTFLike  # noqa: F401
 from stable_baselines3.common.vec_env import DummyVecEnv, SubprocVecEnv, VecEnv, VecFrameStack, VecNormalize
 
 # For custom activation fn
-from torch import nn as nn  # noqa: F401 pylint: disable=unused-import
+from torch import nn as nn
 
 ALGOS: Dict[str, Type[BaseAlgorithm]] = {
     "a2c": A2C,
     "ddpg": DDPG,
     "dqn": DQN,
     "ppo": PPO,
     "sac": SAC,
@@ -36,19 +38,15 @@
     "trpo": TRPO,
     "ppo_lstm": RecurrentPPO,
 }
 
 
 def flatten_dict_observations(env: gym.Env) -> gym.Env:
     assert isinstance(env.observation_space, spaces.Dict)
-    try:
-        return gym.wrappers.FlattenObservation(env)
-    except AttributeError:
-        keys = env.observation_space.spaces.keys()
-        return gym.wrappers.FlattenDictWrapper(env, dict_keys=list(keys))
+    return gym.wrappers.FlattenObservation(env)
 
 
 def get_wrapper_class(hyperparams: Dict[str, Any], key: str = "env_wrapper") -> Optional[Callable[[gym.Env], gym.Env]]:
     """
     Get one or more Gym environment wrapper class specified as a hyper parameter
     "env_wrapper".
     Works also for VecEnvWrapper with the key "vec_env_wrapper".
@@ -230,36 +228,53 @@
     vec_env_cls = DummyVecEnv
     if n_envs > 1 or (ExperimentManager.is_bullet(env_id) and should_render):
         # HACK: force SubprocVecEnv for Bullet env
         # as Pybullet envs does not follow gym.render() interface
         vec_env_cls = SubprocVecEnv  # type: ignore[assignment]
         # start_method = 'spawn' for thread safe
 
-    # panda-gym is based on pybullet, whose rendering requires to be configure at initialization
-    if ExperimentManager.is_panda_gym(env_id) and should_render:
-        if env_kwargs is None:
-            env_kwargs = {"render": True}
-        else:
-            env_kwargs["render"] = True
+    # Fix for gym 0.26, to keep old behavior
+    env_kwargs = env_kwargs or {}
+    env_kwargs = deepcopy(env_kwargs)
+    if "render_mode" not in env_kwargs and should_render:
+        env_kwargs.update(render_mode="human")
+
+    # Make Pybullet compatible with gym 0.26
+    if ExperimentManager.is_bullet(env_id):
+        spec = gym26.spec(env_id)
+        env_kwargs.update(dict(apply_api_compatibility=True))
+    else:
+        # Define make_env here so it works with subprocesses
+        # when the registry was modified with `--gym-packages`
+        # See https://github.com/HumanCompatibleAI/imitation/pull/160
+        try:
+            spec = gym.spec(env_id)  # type: ignore[assignment]
+        except gym.error.NameNotFound:
+            # Registered with gym 0.26
+            spec = gym26.spec(env_id)
+
+    def make_env(**kwargs) -> gym.Env:
+        env = spec.make(**kwargs)
+        return env  # type: ignore[return-value]
 
     env = make_vec_env(
-        env_id,
+        make_env,
         n_envs=n_envs,
         monitor_dir=log_dir,
         seed=seed,
         wrapper_class=env_wrapper,
         env_kwargs=env_kwargs,
         vec_env_cls=vec_env_cls,
         vec_env_kwargs=vec_env_kwargs,
     )
 
     if "vec_env_wrapper" in hyperparams.keys():
         vec_env_wrapper = get_wrapper_class(hyperparams, "vec_env_wrapper")
         assert vec_env_wrapper is not None
-        env = vec_env_wrapper(env)
+        env = vec_env_wrapper(env)  # type: ignore[assignment, arg-type]
         del hyperparams["vec_env_wrapper"]
 
     # Load saved stats for normalizing input and rewards
     # And optionally stack frames
     if stats_path is not None:
         if hyperparams["normalize"]:
             print("Loading running average")
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3/wrappers.py` & `rl_zoo3-2.0.0a4/rl_zoo3/wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,67 @@
-import gym
+from typing import Any, Dict, Optional, SupportsFloat, Tuple
+
+import gymnasium as gym
 import numpy as np
-from gym import spaces
+from gymnasium import spaces
+from gymnasium.core import ObsType
 from sb3_contrib.common.wrappers import TimeFeatureWrapper  # noqa: F401 (backward compatibility)
+from stable_baselines3.common.type_aliases import GymResetReturn, GymStepReturn
 
 
-class DoneOnSuccessWrapper(gym.Wrapper):
+class TruncatedOnSuccessWrapper(gym.Wrapper):
     """
     Reset on success and offsets the reward.
     Useful for GoalEnv.
     """
 
     def __init__(self, env: gym.Env, reward_offset: float = 0.0, n_successes: int = 1):
         super().__init__(env)
         self.reward_offset = reward_offset
         self.n_successes = n_successes
         self.current_successes = 0
 
-    def reset(self):
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None) -> GymResetReturn:
         self.current_successes = 0
-        return self.env.reset()
+        assert options is None, "Options not supported for now"
+        return self.env.reset(seed=seed)
 
-    def step(self, action):
-        obs, reward, done, info = self.env.step(action)
+    def step(self, action) -> GymStepReturn:
+        obs, reward, terminated, truncated, info = self.env.step(action)
         if info.get("is_success", False):
             self.current_successes += 1
         else:
             self.current_successes = 0
         # number of successes in a row
-        done = done or self.current_successes >= self.n_successes
-        reward += self.reward_offset
-        return obs, reward, done, info
+        truncated = truncated or self.current_successes >= self.n_successes
+        reward = float(reward) + self.reward_offset
+        return obs, reward, terminated, truncated, info
 
     def compute_reward(self, achieved_goal, desired_goal, info):
         reward = self.env.compute_reward(achieved_goal, desired_goal, info)
         return reward + self.reward_offset
 
 
-class ActionNoiseWrapper(gym.Wrapper):
+class ActionNoiseWrapper(gym.Wrapper[ObsType, np.ndarray, ObsType, np.ndarray]):
     """
     Add gaussian noise to the action (without telling the agent),
     to test the robustness of the control.
 
     :param env:
     :param noise_std: Standard deviation of the noise
     """
 
     def __init__(self, env: gym.Env, noise_std: float = 0.1):
         super().__init__(env)
         self.noise_std = noise_std
 
-    def step(self, action):
+    def step(self, action: np.ndarray) -> Tuple[ObsType, SupportsFloat, bool, bool, Dict[str, Any]]:
+        assert isinstance(self.action_space, spaces.Box)
         noise = np.random.normal(np.zeros_like(action), np.ones_like(action) * self.noise_std)
-        noisy_action = action + noise
+        noisy_action = np.clip(action + noise, self.action_space.low, self.action_space.high)
         return self.env.step(noisy_action)
 
 
 class ActionSmoothingWrapper(gym.Wrapper):
     """
     Smooth the action using exponential moving average.
 
@@ -68,21 +74,23 @@
         self.smoothing_coef = smoothing_coef
         self.smoothed_action = None
         # from https://github.com/rail-berkeley/softlearning/issues/3
         # for smoothing latent space
         # self.alpha = self.smoothing_coef
         # self.beta = np.sqrt(1 - self.alpha ** 2) / (1 - self.alpha)
 
-    def reset(self):
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None) -> GymResetReturn:
         self.smoothed_action = None
-        return self.env.reset()
+        assert options is None, "Options not supported for now"
+        return self.env.reset(seed=seed)
 
-    def step(self, action):
+    def step(self, action) -> GymStepReturn:
         if self.smoothed_action is None:
             self.smoothed_action = np.zeros_like(action)
+        assert self.smoothed_action is not None
         self.smoothed_action = self.smoothing_coef * self.smoothed_action + (1 - self.smoothing_coef) * action
         return self.env.step(self.smoothed_action)
 
 
 class DelayedRewardWrapper(gym.Wrapper):
     """
     Delay the reward by `delay` steps, it makes the task harder but more realistic.
@@ -94,191 +102,195 @@
 
     def __init__(self, env: gym.Env, delay: int = 10):
         super().__init__(env)
         self.delay = delay
         self.current_step = 0
         self.accumulated_reward = 0.0
 
-    def reset(self):
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None) -> GymResetReturn:
         self.current_step = 0
         self.accumulated_reward = 0.0
-        return self.env.reset()
+        assert options is None, "Options not supported for now"
+        return self.env.reset(seed=seed)
 
-    def step(self, action):
-        obs, reward, done, info = self.env.step(action)
+    def step(self, action) -> GymStepReturn:
+        obs, reward, terminated, truncated, info = self.env.step(action)
 
-        self.accumulated_reward += reward
+        self.accumulated_reward += float(reward)
         self.current_step += 1
 
-        if self.current_step % self.delay == 0 or done:
+        if self.current_step % self.delay == 0 or terminated or truncated:
             reward = self.accumulated_reward
             self.accumulated_reward = 0.0
         else:
             reward = 0.0
-        return obs, reward, done, info
+        return obs, reward, terminated, truncated, info
 
 
-class HistoryWrapper(gym.Wrapper):
+class HistoryWrapper(gym.Wrapper[np.ndarray, np.ndarray, np.ndarray, np.ndarray]):
     """
     Stack past observations and actions to give an history to the agent.
 
     :param env:
     :param horizon:Number of steps to keep in the history.
     """
 
     def __init__(self, env: gym.Env, horizon: int = 2):
         assert isinstance(env.observation_space, spaces.Box)
+        assert isinstance(env.action_space, spaces.Box)
 
         wrapped_obs_space = env.observation_space
         wrapped_action_space = env.action_space
 
-        # TODO: double check, it seems wrong when we have different low and highs
-        low_obs = np.repeat(wrapped_obs_space.low, horizon, axis=-1)
-        high_obs = np.repeat(wrapped_obs_space.high, horizon, axis=-1)
+        low_obs = np.tile(wrapped_obs_space.low, horizon)
+        high_obs = np.tile(wrapped_obs_space.high, horizon)
 
-        low_action = np.repeat(wrapped_action_space.low, horizon, axis=-1)
-        high_action = np.repeat(wrapped_action_space.high, horizon, axis=-1)
+        low_action = np.tile(wrapped_action_space.low, horizon)
+        high_action = np.tile(wrapped_action_space.high, horizon)
 
         low = np.concatenate((low_obs, low_action))
         high = np.concatenate((high_obs, high_action))
 
         # Overwrite the observation space
-        env.observation_space = spaces.Box(low=low, high=high, dtype=wrapped_obs_space.dtype)
+        env.observation_space = spaces.Box(low=low, high=high, dtype=wrapped_obs_space.dtype)  # type: ignore[arg-type]
 
         super().__init__(env)
 
         self.horizon = horizon
         self.low_action, self.high_action = low_action, high_action
         self.low_obs, self.high_obs = low_obs, high_obs
         self.low, self.high = low, high
         self.obs_history = np.zeros(low_obs.shape, low_obs.dtype)
         self.action_history = np.zeros(low_action.shape, low_action.dtype)
 
-    def _create_obs_from_history(self):
+    def _create_obs_from_history(self) -> np.ndarray:
         return np.concatenate((self.obs_history, self.action_history))
 
-    def reset(self):
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None) -> Tuple[np.ndarray, Dict]:
         # Flush the history
         self.obs_history[...] = 0
         self.action_history[...] = 0
-        obs = self.env.reset()
+        assert options is None, "Options not supported for now"
+        obs, info = self.env.reset(seed=seed)
         self.obs_history[..., -obs.shape[-1] :] = obs
-        return self._create_obs_from_history()
+        return self._create_obs_from_history(), info
 
-    def step(self, action):
-        obs, reward, done, info = self.env.step(action)
+    def step(self, action) -> Tuple[np.ndarray, SupportsFloat, bool, bool, Dict]:
+        obs, reward, terminated, truncated, info = self.env.step(action)
         last_ax_size = obs.shape[-1]
 
         self.obs_history = np.roll(self.obs_history, shift=-last_ax_size, axis=-1)
         self.obs_history[..., -obs.shape[-1] :] = obs
 
         self.action_history = np.roll(self.action_history, shift=-action.shape[-1], axis=-1)
         self.action_history[..., -action.shape[-1] :] = action
-        return self._create_obs_from_history(), reward, done, info
+        return self._create_obs_from_history(), reward, terminated, truncated, info
 
 
 class HistoryWrapperObsDict(gym.Wrapper):
     """
     History Wrapper for dict observation.
 
     :param env:
     :param horizon: Number of steps to keep in the history.
     """
 
     def __init__(self, env: gym.Env, horizon: int = 2):
+        assert isinstance(env.observation_space, spaces.Dict)
         assert isinstance(env.observation_space.spaces["observation"], spaces.Box)
+        assert isinstance(env.action_space, spaces.Box)
 
         wrapped_obs_space = env.observation_space.spaces["observation"]
         wrapped_action_space = env.action_space
 
-        # TODO: double check, it seems wrong when we have different low and highs
-        low_obs = np.repeat(wrapped_obs_space.low, horizon, axis=-1)
-        high_obs = np.repeat(wrapped_obs_space.high, horizon, axis=-1)
+        low_obs = np.tile(wrapped_obs_space.low, horizon)
+        high_obs = np.tile(wrapped_obs_space.high, horizon)
 
-        low_action = np.repeat(wrapped_action_space.low, horizon, axis=-1)
-        high_action = np.repeat(wrapped_action_space.high, horizon, axis=-1)
+        low_action = np.tile(wrapped_action_space.low, horizon)
+        high_action = np.tile(wrapped_action_space.high, horizon)
 
         low = np.concatenate((low_obs, low_action))
         high = np.concatenate((high_obs, high_action))
 
         # Overwrite the observation space
-        env.observation_space.spaces["observation"] = spaces.Box(low=low, high=high, dtype=wrapped_obs_space.dtype)
+        env.observation_space.spaces["observation"] = spaces.Box(
+            low=low,
+            high=high,
+            dtype=wrapped_obs_space.dtype,  # type: ignore[arg-type]
+        )
 
         super().__init__(env)
 
         self.horizon = horizon
         self.low_action, self.high_action = low_action, high_action
         self.low_obs, self.high_obs = low_obs, high_obs
         self.low, self.high = low, high
         self.obs_history = np.zeros(low_obs.shape, low_obs.dtype)
         self.action_history = np.zeros(low_action.shape, low_action.dtype)
 
-    def _create_obs_from_history(self):
+    def _create_obs_from_history(self) -> np.ndarray:
         return np.concatenate((self.obs_history, self.action_history))
 
-    def reset(self):
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None) -> Tuple[Dict[str, np.ndarray], Dict]:
         # Flush the history
         self.obs_history[...] = 0
         self.action_history[...] = 0
-        obs_dict = self.env.reset()
+        assert options is None, "Options not supported for now"
+        obs_dict, info = self.env.reset(seed=seed)
         obs = obs_dict["observation"]
         self.obs_history[..., -obs.shape[-1] :] = obs
 
         obs_dict["observation"] = self._create_obs_from_history()
 
-        return obs_dict
+        return obs_dict, info
 
-    def step(self, action):
-        obs_dict, reward, done, info = self.env.step(action)
+    def step(self, action) -> Tuple[Dict[str, np.ndarray], SupportsFloat, bool, bool, Dict]:
+        obs_dict, reward, terminated, truncated, info = self.env.step(action)
         obs = obs_dict["observation"]
         last_ax_size = obs.shape[-1]
 
         self.obs_history = np.roll(self.obs_history, shift=-last_ax_size, axis=-1)
         self.obs_history[..., -obs.shape[-1] :] = obs
 
         self.action_history = np.roll(self.action_history, shift=-action.shape[-1], axis=-1)
         self.action_history[..., -action.shape[-1] :] = action
 
         obs_dict["observation"] = self._create_obs_from_history()
 
-        return obs_dict, reward, done, info
+        return obs_dict, reward, terminated, truncated, info
 
 
 class FrameSkip(gym.Wrapper):
     """
     Return only every ``skip``-th frame (frameskipping)
 
     :param env: the environment
     :param skip: number of ``skip``-th frame
     """
 
     def __init__(self, env: gym.Env, skip: int = 4):
         super().__init__(env)
         self._skip = skip
 
-    def step(self, action: np.ndarray):
+    def step(self, action) -> GymStepReturn:
         """
         Step the environment with the given action
         Repeat action, sum reward.
 
         :param action: the action
-        :return: observation, reward, done, information
+        :return: observation, reward, terminated, truncated, information
         """
         total_reward = 0.0
-        done = None
         for _ in range(self._skip):
-            obs, reward, done, info = self.env.step(action)
-            total_reward += reward
-            if done:
+            obs, reward, terminated, truncated, info = self.env.step(action)
+            total_reward += float(reward)
+            if terminated or truncated:
                 break
 
-        return obs, total_reward, done, info
-
-    def reset(self):
-        return self.env.reset()
+        return obs, total_reward, terminated, truncated, info
 
 
 class MaskVelocityWrapper(gym.ObservationWrapper):
     """
     Gym environment observation wrapper used to mask velocity terms in
     observations. The intention is the make the MDP partially observable.
     Adapted from https://github.com/LiuWenlin595/FinalProject.
@@ -295,14 +307,15 @@
         "LunarLander-v2": np.array([2, 3, 5]),
         "LunarLanderContinuous-v2": np.array([2, 3, 5]),
     }
 
     def __init__(self, env: gym.Env):
         super().__init__(env)
 
+        assert env.unwrapped.spec is not None
         env_id: str = env.unwrapped.spec.id
         # By default no masking
         self.mask = np.ones_like(env.observation_space.sample())
         try:
             # Mask velocity
             self.mask[self.velocity_indices[env_id]] = 0.0
         except KeyError as e:
```

### Comparing `rl_zoo3-1.8.0a9/rl_zoo3.egg-info/PKG-INFO` & `rl_zoo3-2.0.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: rl-zoo3
-Version: 1.8.0a9
+Name: rl_zoo3
+Version: 2.0.0a4
 Summary: A Training Framework for Stable Baselines3 Reinforcement Learning Agents
 Home-page: https://github.com/DLR-RM/rl-baselines3-zoo
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
-Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines sb3 toolbox python data-science
+Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym gymnasium openai stable baselines sb3 toolbox python data-science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `rl_zoo3-1.8.0a9/setup.py` & `rl_zoo3-2.0.0a4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,16 @@
             "py.typed",
             "version.txt",
             "hyperparams/*.yml",
         ]
     },
     entry_points={"console_scripts": ["rl_zoo3=rl_zoo3.cli:main"]},
     install_requires=[
-        "sb3-contrib>=1.8.0a9",
+        "sb3_contrib>=2.0.0a4",
+        "gym==0.26.2",
         "huggingface_sb3>=2.2.1",
         "tqdm",
         "rich",
         "optuna",
         "pyyaml>=5.1",
         "pytablewriter~=0.64",
         # TODO: add test dependencies
@@ -40,15 +41,15 @@
         "plots": ["seaborn", "rliable>=1.0.5", "scipy~=1.7.3"],
     },
     description="A Training Framework for Stable Baselines3 Reinforcement Learning Agents",
     author="Antonin Raffin",
     url="https://github.com/DLR-RM/rl-baselines3-zoo",
     author_email="antonin.raffin@dlr.de",
     keywords="reinforcement-learning-algorithms reinforcement-learning machine-learning "
-    "gym openai stable baselines sb3 toolbox python data-science",
+    "gym gymnasium openai stable baselines sb3 toolbox python data-science",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=__version__,
     python_requires=">=3.7",
     # PyPI package information.
     classifiers=[
```

