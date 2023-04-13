# Comparing `tmp/deploifai-0.4.2.tar.gz` & `tmp/deploifai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cli/cli/dist/.tmp-bg1qbj3c/deploifai-0.4.2.tar", last modified: Thu Mar 16 09:38:28 2023, max compression
+gzip compressed data, was "/home/runner/work/cli/cli/dist/.tmp-6o0keaae/deploifai-0.4.3.tar", last modified: Thu Apr 13 20:08:37 2023, max compression
```

## Comparing `deploifai-0.4.2.tar` & `deploifai-0.4.3.tar`

### file list

```diff
@@ -1,142 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-16 09:37:46.000000 deploifai-0.4.2/.github/workflows/dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-16 09:37:46.000000 deploifai-0.4.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-16 09:37:46.000000 deploifai-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 09:37:46.000000 deploifai-0.4.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-16 09:37:46.000000 deploifai-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-16 09:38:28.000000 deploifai-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-16 09:37:46.000000 deploifai-0.4.2/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)    20076 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/application/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/application/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/cloud_profile/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/cloud_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/cloud_profile/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/cloud_profile/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/aws/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/aws/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/aws/data_storage/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/azure/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/azure/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/azure/data_storage/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/gcp/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/gcp/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/gcp/data_storage/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/clouds/utilities/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/utilities/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/clouds/utilities/data_storage/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/core/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/core/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/core/data_storage/data_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/dataset/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/experiment/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/mlflow/get_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/project/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/browse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/project/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/server/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/server/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/server/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/server/start.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/server/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/cloud_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/utilities/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/config/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/config/find_config_filepath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/config/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/frontend_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/python_supported.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/server_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/utilities/version_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/workspace/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-16 09:37:46.000000 deploifai-0.4.2/deploifai/cli/workspace/set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-16 09:38:28.000000 deploifai-0.4.2/deploifai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 09:37:46.000000 deploifai-0.4.2/dev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/application.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/auth.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/cloud-profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/mlflow.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/project.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/server.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 09:37:46.000000 deploifai-0.4.2/docs/workspace.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-16 09:37:46.000000 deploifai-0.4.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-16 09:37:46.000000 deploifai-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-16 09:37:46.000000 deploifai-0.4.2/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/release/homebrew/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 09:37:46.000000 deploifai-0.4.2/release/homebrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-16 09:37:46.000000 deploifai-0.4.2/release/homebrew/deploifai.placeholder.rb
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-03-16 09:37:46.000000 deploifai-0.4.2/release/homebrew/deploifai.rb
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-16 09:37:46.000000 deploifai-0.4.2/release/homebrew/homebrew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 09:38:28.000000 deploifai-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-16 09:37:46.000000 deploifai-0.4.2/requirements/cli.txt
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-16 09:37:46.000000 deploifai-0.4.2/requirements/deploifai.txt
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-16 09:37:46.000000 deploifai-0.4.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-16 09:37:46.000000 deploifai-0.4.2/requirements/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-16 09:37:46.000000 deploifai-0.4.2/sample.env
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 09:38:28.000000 deploifai-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-16 09:37:46.000000 deploifai-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 20:07:59.000000 deploifai-0.4.3/.github/workflows/dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-13 20:07:59.000000 deploifai-0.4.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-13 20:07:59.000000 deploifai-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 20:07:59.000000 deploifai-0.4.3/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:07:59.000000 deploifai-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 20:08:37.000000 deploifai-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-13 20:07:59.000000 deploifai-0.4.3/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/application/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/application/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/cloud_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/cloud_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/cloud_profile/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/cloud_profile/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/aws/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/aws/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/aws/data_storage/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/azure/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/azure/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/azure/data_storage/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/gcp/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/gcp/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/gcp/data_storage/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/clouds/utilities/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/utilities/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/clouds/utilities/data_storage/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/core/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/core/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/core/data_storage/data_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/dataset/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/experiment/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/mlflow/get_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/browse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/project/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/server/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/server/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/server/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/server/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/cloud_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/utilities/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/config/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/config/find_config_filepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/config/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/frontend_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/python_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/server_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/utilities/version_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/workspace/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-13 20:07:59.000000 deploifai-0.4.3/deploifai/cli/workspace/set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:08:37.000000 deploifai-0.4.3/deploifai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 20:07:59.000000 deploifai-0.4.3/dev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/application.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/cloud-profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/mlflow.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/project.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/server.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 20:07:59.000000 deploifai-0.4.3/docs/workspace.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 20:07:59.000000 deploifai-0.4.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 20:07:59.000000 deploifai-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 20:07:59.000000 deploifai-0.4.3/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/release/homebrew/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:07:59.000000 deploifai-0.4.3/release/homebrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 20:07:59.000000 deploifai-0.4.3/release/homebrew/deploifai.placeholder.rb
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-13 20:07:59.000000 deploifai-0.4.3/release/homebrew/deploifai.rb
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-13 20:07:59.000000 deploifai-0.4.3/release/homebrew/homebrew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:08:37.000000 deploifai-0.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 20:07:59.000000 deploifai-0.4.3/requirements/cli.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-13 20:07:59.000000 deploifai-0.4.3/requirements/deploifai.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 20:07:59.000000 deploifai-0.4.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-13 20:07:59.000000 deploifai-0.4.3/requirements/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 20:07:59.000000 deploifai-0.4.3/sample.env
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:08:37.000000 deploifai-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-13 20:07:59.000000 deploifai-0.4.3/setup.py
```

### Comparing `deploifai-0.4.2/.github/workflows/dev.yml` & `deploifai-0.4.3/.github/workflows/dev.yml`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/.github/workflows/release.yml` & `deploifai-0.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/PKG-INFO` & `deploifai-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploifai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deploifai CLI
 Home-page: https://github.com/deploifai/cli
 Author: Deploifai Limited
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deploifai-0.4.2/contribute.md` & `deploifai-0.4.3/contribute.md`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/api/__init__.py` & `deploifai-0.4.3/deploifai/cli/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -656,7 +656,261 @@
             create_mutation_data = r.json()
 
             return create_mutation_data["data"]["stopTraining"]
         except TypeError:
             raise DeploifaiAPIError("Could not stop Training Server. Please try again.")
         except KeyError:
             raise DeploifaiAPIError("Could not stop Training Server. Please try again.")
+
+    def get_container_registries(self, username: str, cloud_profile_id: str):
+        query = """
+        query ($whereAccount: AccountWhereUniqueInput! $whereContainerRegistry: ContainerRegistryWhereInput){
+            containerRegistries(whereAccount: $whereAccount whereContainerRegistry: $whereContainerRegistry){
+                id
+                name
+            }
+        }
+        """
+
+        variables = {
+            "whereAccount": {"username": username},
+            "whereContainerRegistry": {"cloudProfileId": {"equals": cloud_profile_id}},
+        }
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": query, "variables": variables},
+                headers=self.headers,
+            )
+
+            container_registries = r.json()
+            return container_registries["data"]["containerRegistries"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not get Container Registries. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not get Container Registries. Please try again.")
+
+    def get_container_registry(self, registry_id: str):
+        query = """
+        query ($where: ContainerRegistryWhereUniqueInput!){
+            containerRegistry(where: $where){
+                id
+                name
+                info {
+                    loginServer
+                    username
+                    password
+                    imageUri
+                }
+            }
+        }
+        """
+
+        variables = {"where": {"id": registry_id}}
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": query, "variables": variables},
+                headers=self.headers,
+            )
+
+            container_registry = r.json()
+            return container_registry["data"]["containerRegistry"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not get Container Registry. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not get Container Registry. Please try again.")
+
+    def create_container_registry(self, project_id: str, name: str, cloud_profile_id: str):
+        mutation = """
+        mutation($whereProject: ProjectWhereUniqueInput! $data: CreateContainerRegistryInput!){
+            createContainerRegistry(whereProject: $whereProject data: $data){
+                id
+                name
+                sluggedName
+                info {
+                    loginServer
+                    username
+                    password
+                    imageUri
+                }
+            }
+        }
+        """
+
+        variables = {
+            "whereProject": {"id": project_id},
+            "data": {
+                "name": name,
+                "cloudProfileId": cloud_profile_id,
+                "cloudProviderContainerRegistryConfig": {},
+            }
+        }
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": mutation, "variables": variables},
+                headers=self.headers,
+            )
+
+            create_mutation_data = r.json()
+
+            return create_mutation_data["data"]["createContainerRegistry"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not create Container Registry. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not create Container Registry. Please try again.")
+
+    def get_application_infrastructure_plans(self, cloud_provider: str):
+        query = """
+        query ($provider: CloudProvider) {
+            applicationInfrastructurePlans(provider: $provider) {
+                plan
+                config {
+                    ... on AWSAppDefaultConfig{
+                    ec2InstanceType
+                    }
+                    ... on AzureAppDefaultConfig{
+                    cgCpu
+                    }
+                    ... on GCPAppDefaultConfig{
+                    containerCpu
+                    }
+                }
+            }
+        }
+        """
+
+        variables = {
+            "provider": cloud_provider,
+        }
+
+        app_configs = []
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": query, "variables": variables},
+                headers=self.headers,
+            )
+            app_info = r.json()
+
+            if "errors" in app_info:
+                raise DeploifaiAPIError(app_info['errors'][0]['message'])
+
+            app_configs = app_info["data"]["applicationInfrastructurePlans"]
+        except Exception:
+            pass
+        finally:
+            return app_configs
+
+    def get_applications(self, workspace: str, where_application: dict = None):
+        query = """
+        query ($whereAccount: AccountWhereUniqueInput! $whereApplication: ApplicationWhereInput){
+            applications(whereAccount: $whereAccount whereApplication: $whereApplication){
+                id
+                name
+                status
+            }
+        }
+        """
+
+        variables = {
+            "whereAccount": {"username": workspace},
+            "whereApplication": where_application,
+        }
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": query, "variables": variables},
+                headers=self.headers,
+            )
+            app_info = r.json()
+
+            if "errors" in app_info:
+                raise DeploifaiAPIError(app_info['errors'][0]['message'])
+
+            app_details = app_info["data"]["applications"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not find Applications. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not find Applications. Please try again.")
+
+        return app_details
+
+    def get_application(self, application_id: str):
+        query = """
+        query ($where: ApplicationWhereUniqueInput!){
+            application(where: $where){
+                id
+                name
+                status
+                hostname
+            }
+        }
+        """
+
+        variables = {"where": {"id": application_id}}
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": query, "variables": variables},
+                headers=self.headers,
+            )
+            app_info = r.json()
+
+            if "errors" in app_info:
+                raise DeploifaiAPIError(app_info['errors'][0]['message'])
+
+            app_details = app_info["data"]["application"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not find Application. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not find Application. Please try again.")
+
+        return app_details
+
+    def create_application(self, project_id: str, name: str, cloud_profile_id: str, config: dict, image_uri: str, port: int, environment_variables: list):
+        mutation = """
+        mutation($whereProject: ProjectWhereUniqueInput! $data: CreateApplicationInput!){
+            createApplication(whereProject: $whereProject data: $data){
+                id
+                name
+            }
+        }
+        """
+
+        variables = {
+            "whereProject": {"id": project_id},
+            "data": {
+                "name": name,
+                "cloudProfileId": cloud_profile_id,
+                "cloudProviderAppConfig": config,
+                "container": {
+                    "image": image_uri,
+                    "port": port,
+                },
+                "environmentVariables": environment_variables,
+            }
+        }
+
+        try:
+            r = requests.post(
+                self.uri,
+                json={"query": mutation, "variables": variables},
+                headers=self.headers,
+            )
+
+            create_mutation_data = r.json()
+
+            return create_mutation_data["data"]["createApplication"]
+        except TypeError:
+            raise DeploifaiAPIError("Could not create Application. Please try again.")
+        except KeyError:
+            raise DeploifaiAPIError("Could not create Application. Please try again.")
+
+    def update_application(self):
+        ...
```

### Comparing `deploifai-0.4.2/deploifai/cli/application/init.py` & `deploifai-0.4.3/deploifai/cli/application/init.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/auth/login.py` & `deploifai-0.4.3/deploifai/cli/auth/login.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/auth/logout.py` & `deploifai-0.4.3/deploifai/cli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/cli.py` & `deploifai-0.4.3/deploifai/cli/cli.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/cloud_profile/list.py` & `deploifai-0.4.3/deploifai/cli/cloud_profile/list.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/clouds/aws/data_storage/handler.py` & `deploifai-0.4.3/deploifai/cli/clouds/aws/data_storage/handler.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/clouds/azure/data_storage/handler.py` & `deploifai-0.4.3/deploifai/cli/clouds/azure/data_storage/handler.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/clouds/gcp/data_storage/handler.py` & `deploifai-0.4.3/deploifai/cli/clouds/gcp/data_storage/handler.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/clouds/utilities/data_storage/handler.py` & `deploifai-0.4.3/deploifai/cli/clouds/utilities/data_storage/handler.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/context.py` & `deploifai-0.4.3/deploifai/cli/context.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/core/data_storage/data_storage.py` & `deploifai-0.4.3/deploifai/cli/core/data_storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/__init__.py` & `deploifai-0.4.3/deploifai/cli/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/create.py` & `deploifai-0.4.3/deploifai/cli/dataset/create.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/info.py` & `deploifai-0.4.3/deploifai/cli/dataset/info.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/init.py` & `deploifai-0.4.3/deploifai/cli/dataset/init.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/list.py` & `deploifai-0.4.3/deploifai/cli/dataset/list.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/pull.py` & `deploifai-0.4.3/deploifai/cli/dataset/pull.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/dataset/push.py` & `deploifai-0.4.3/deploifai/cli/dataset/push.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/mlflow/get_setup.py` & `deploifai-0.4.3/deploifai/cli/mlflow/get_setup.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/project/browse.py` & `deploifai-0.4.3/deploifai/cli/project/browse.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/project/create.py` & `deploifai-0.4.3/deploifai/cli/project/create.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/project/info.py` & `deploifai-0.4.3/deploifai/cli/project/info.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/project/init.py` & `deploifai-0.4.3/deploifai/cli/project/init.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/project/list.py` & `deploifai-0.4.3/deploifai/cli/project/list.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/server/create.py` & `deploifai-0.4.3/deploifai/cli/server/create.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/server/list.py` & `deploifai-0.4.3/deploifai/cli/server/list.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/utilities/config/dataset_config.py` & `deploifai-0.4.3/deploifai/cli/utilities/config/dataset_config.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/utilities/config/find_config_filepath.py` & `deploifai-0.4.3/deploifai/cli/utilities/config/find_config_filepath.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/utilities/config/local_config.py` & `deploifai-0.4.3/deploifai/cli/utilities/config/local_config.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/utilities/server_state.py` & `deploifai-0.4.3/deploifai/cli/utilities/server_state.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/utilities/version_comparison.py` & `deploifai-0.4.3/deploifai/cli/utilities/version_comparison.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/workspace/list.py` & `deploifai-0.4.3/deploifai/cli/workspace/list.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai/cli/workspace/set.py` & `deploifai-0.4.3/deploifai/cli/workspace/set.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/deploifai.egg-info/PKG-INFO` & `deploifai-0.4.3/deploifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploifai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deploifai CLI
 Home-page: https://github.com/deploifai/cli
 Author: Deploifai Limited
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deploifai-0.4.2/deploifai.egg-info/SOURCES.txt` & `deploifai-0.4.3/deploifai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 deploifai.egg-info/top_level.txt
 deploifai/cli/__init__.py
 deploifai/cli/cli.py
 deploifai/cli/context.py
 deploifai/cli/api/__init__.py
 deploifai/cli/api/errors.py
 deploifai/cli/application/__init__.py
+deploifai/cli/application/create.py
 deploifai/cli/application/init.py
 deploifai/cli/auth/__init__.py
 deploifai/cli/auth/login.py
 deploifai/cli/auth/logout.py
 deploifai/cli/auth/status.py
 deploifai/cli/cloud_profile/__init__.py
 deploifai/cli/cloud_profile/create.py
```

### Comparing `deploifai-0.4.2/readme.md` & `deploifai-0.4.3/readme.md`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/release/homebrew/deploifai.placeholder.rb` & `deploifai-0.4.3/release/homebrew/deploifai.placeholder.rb`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/release/homebrew/deploifai.rb` & `deploifai-0.4.3/release/homebrew/deploifai.rb`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/release/homebrew/homebrew.py` & `deploifai-0.4.3/release/homebrew/homebrew.py`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/requirements/deploifai.txt` & `deploifai-0.4.3/requirements/deploifai.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 boto3==1.26.78
 botocore==1.29.78
 cachetools==5.3.0
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==3.0.1
 cryptography==39.0.1
+docker==6.0.1
 google-api-core==2.11.0
 google-auth==2.16.1
 google-cloud-core==2.3.2
 google-cloud-storage==2.7.0
 google-crc32c==1.5.0
 google-resumable-media==2.4.1
 googleapis-common-protos==1.58.0
 idna==3.4
 isodate==0.6.1
 jmespath==1.0.1
 msal==1.21.0
 msal-extensions==1.0.0
+packaging==23.0
 portalocker==2.7.0
 protobuf==4.22.0
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycparser==2.21
 PyJWT==2.6.0
 python-dateutil==2.8.2
 requests==2.28.2
 rsa==4.9
 s3transfer==0.6.0
 semver==2.13.0
 six==1.16.0
 typing_extensions==4.5.0
 urllib3==1.26.14
+websocket-client==1.5.1
```

### Comparing `deploifai-0.4.2/requirements/dev.txt` & `deploifai-0.4.3/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `deploifai-0.4.2/requirements/readme.md` & `deploifai-0.4.3/requirements/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 azure-identity
 azure-storage-blob
 boto3
 google-auth
 google-cloud-storage
 semver
 cryptography
+docker
 ```
 
 ### CLI dependencies
 
 `cli` module dependencies for the CLI tool
 
 ```text
```

### Comparing `deploifai-0.4.2/setup.py` & `deploifai-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         "click-spinner",
         "tqdm",
         "azure-identity",
         "azure-storage-blob",
         "boto3",
         "google-auth",
         "google-cloud-storage",
+        "docker",
         "InquirerPy",
         "pyperclip",
         "semver",
         "cryptography",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.7",
```

