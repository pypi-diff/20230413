# Comparing `tmp/autumn8-1.0.2rc3.tar.gz` & `tmp/autumn8-1.0.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.2rc3.tar", last modified: Wed Apr 12 20:42:23 2023, max compression
+gzip compressed data, was "autumn8-1.0.2rc4.tar", last modified: Thu Apr 13 19:01:04 2023, max compression
```

## Comparing `autumn8-1.0.2rc3.tar` & `autumn8-1.0.2rc4.tar`

### file list

```diff
@@ -1,59 +1,65 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-12 20:01:39.000000 autumn8-1.0.2rc3/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.2rc3/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4109 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    15368 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1795 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5148 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.2rc3/autumn8/cli/pending_uploads.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-04-12 20:41:46.000000 autumn8-1.0.2rc3/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-12 19:59:12.000000 autumn8-1.0.2rc3/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65037 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.2rc3/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3637 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10396 2023-04-12 20:32:46.000000 autumn8-1.0.2rc3/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc3/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.2rc3/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.2rc3/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc3/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-12 20:01:39.000000 autumn8-1.0.2rc3/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.196385 autumn8-1.0.2rc3/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-12 20:42:23.000000 autumn8-1.0.2rc3/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-04-12 20:41:35.000000 autumn8-1.0.2rc3/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:42:23.206385 autumn8-1.0.2rc3/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc3/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.670702 autumn8-1.0.2rc4/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-13 19:01:04.670702 autumn8-1.0.2rc4/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.630702 autumn8-1.0.2rc4/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.640702 autumn8-1.0.2rc4/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-12 20:01:39.000000 autumn8-1.0.2rc4/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.2rc4/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.640702 autumn8-1.0.2rc4/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4109 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16909 2023-04-13 19:00:22.000000 autumn8-1.0.2rc4/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1795 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-04-13 18:59:31.000000 autumn8-1.0.2rc4/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.2rc4/autumn8/cli/pending_uploads.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.640702 autumn8-1.0.2rc4/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-04-13 18:59:40.000000 autumn8-1.0.2rc4/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.650702 autumn8-1.0.2rc4/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-04-13 17:44:29.000000 autumn8-1.0.2rc4/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-13 18:59:53.000000 autumn8-1.0.2rc4/autumn8/common/config/s3.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65037 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.650702 autumn8-1.0.2rc4/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.2rc4/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.2rc4/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.2rc4/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.2rc4/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.2rc4/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.660702 autumn8-1.0.2rc4/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.660702 autumn8-1.0.2rc4/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.2rc4/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.670702 autumn8-1.0.2rc4/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3637 2023-04-12 20:32:46.000000 autumn8-1.0.2rc4/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11126 2023-04-13 18:59:31.000000 autumn8-1.0.2rc4/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc4/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.2rc4/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.2rc4/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc4/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-12 20:01:39.000000 autumn8-1.0.2rc4/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.630702 autumn8-1.0.2rc4/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1371 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-13 19:01:04.000000 autumn8-1.0.2rc4/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-04-12 20:59:17.000000 autumn8-1.0.2rc4/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-13 19:01:04.670702 autumn8-1.0.2rc4/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-13 19:01:04.670702 autumn8-1.0.2rc4/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc4/tests/test_settings.py
```

### Comparing `autumn8-1.0.2rc3/PKG-INFO` & `autumn8-1.0.2rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc3
+Version: 1.0.2rc4
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc3/README.md` & `autumn8-1.0.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/analyze.py` & `autumn8-1.0.2rc4/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/cli_environment.py` & `autumn8-1.0.2rc4/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/commands/cloud.py` & `autumn8-1.0.2rc4/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/commands/models.py` & `autumn8-1.0.2rc4/autumn8/cli/commands/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -249,30 +249,23 @@
         ),
         click.option(
             "--input_file",
             type=str,
             help="The model input filepath.",
         ),
         click.option(
-            "-y",
-            "--yes",
-            "auto_confirm",
-            type=bool,
-            is_flag=True,
-            help="Skip all confirmation input from the user.",
-        ),
-        click.option(
             "--skip_inputs",
             "should_skip_inputs",
             type=bool,
             is_flag=True,
             help="Don't ask about inputs, let AutoDL try to infer them.",
         ),
         options.use_organization_id,
         options.use_quiet_mode,
+        options.use_auto_confirm,
         click.option(
             "-g",
             "--group_id",
             type=str,
             help="The ID of the model group to add the model to.",
         ),
     ]
@@ -347,14 +340,15 @@
         "framework": framework,
         "quantization": quantization,
         "inputs": input_dims,
         "group_id": group_id,
     }
 
     if not auto_confirm:
+        logger.info("")
         logger.info("The details for your model are as follows:")
         click.echo(f"{json.dumps(model_config, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
@@ -403,16 +397,16 @@
     should_skip_inputs: bool,
     input_dims,
     input_file,
     group_id,
     max_upload_workers,
     **kwargs,
 ):
-    """submit checkpoint to AutoDL"""
-    environment = kwargs["environment"]
+    """Submit checkpoint to AutoDL"""
+    environment: CliEnvironment = kwargs["environment"]
 
     if model_type is None:
         model_type_user_choice = questionary.select(
             "Choose one of the supported models for the checkpoint data",
             choices=list(supported_models_by_human_readable_label.keys()),
             use_shortcuts=True,
         ).unsafe_ask()
@@ -446,14 +440,15 @@
         "quantization": quantization,
         "inputs": input_dims,
         "group_id": group_id,
         "model_type": model_type,
     }
 
     if not auto_confirm:
+        logger.info("")
         logger.info("The details for your model are as follows:")
         click.echo(f"{json.dumps(model_config, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
@@ -487,14 +482,88 @@
         model_type=model_type,
         max_upload_workers=max_upload_workers,
     )
 
     announce_model_upload_response(model_upload_response)
 
 
+@model_commands_group.command()
+@options.use_environment
+@options.use_organization_id
+@options.use_quiet_mode
+@click.option(
+    "-i",
+    "--model_id",
+    type=int,
+    help=f"Model ID to delete",
+    prompt="Model ID to delete",
+)
+def get_model(
+    organization_id: int,
+    model_id: int,
+    quiet: bool,
+    **kwargs,
+):
+    """Get model data from AutoDL"""
+    environment: CliEnvironment = kwargs["environment"]
+
+    model_info = lab.get_model(
+        environment,
+        organization_id,
+        model_id,
+    )
+    announce_model_upload_response(model_info)
+
+
+@model_commands_group.command()
+@options.use_environment
+@options.use_organization_id
+@options.use_quiet_mode
+@options.use_auto_confirm
+@click.option(
+    "-i",
+    "--model_id",
+    type=int,
+    help=f"Model ID to delete",
+    prompt="Model ID to delete",
+)
+def delete_model(
+    organization_id: int,
+    model_id: int,
+    auto_confirm: bool,
+    quiet: bool,
+    **kwargs,
+):
+    """Delete model from AutoDL"""
+    environment: CliEnvironment = kwargs["environment"]
+
+    if not auto_confirm:
+        model_info = lab.get_model(
+            environment,
+            organization_id,
+            model_id,
+        )
+
+        logger.info("")
+        logger.info("The details for your model are as follows:")
+        click.echo(f"{json.dumps(model_info, indent=4)}")
+        click.confirm(
+            text="\n" + "Do you want to delete it?",
+            abort=True,
+            default=True,
+        )
+
+    model_delete_response = lab.delete_model(
+        environment,
+        organization_id,
+        model_id,
+    )
+    announce_model_upload_response(model_delete_response)
+
+
 def zip_checkpoint_dir(checkpoint_filepath_or_url: str, model_name: str) -> str:
     zipped_model_file = zipfile.ZipFile(
         os.path.join(".", model_name + ".zip"),
         "w",
         compresslevel=0,
     )
```

### Comparing `autumn8-1.0.2rc3/autumn8/cli/examples.py` & `autumn8-1.0.2rc4/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/interactive.py` & `autumn8-1.0.2rc4/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/main.py` & `autumn8-1.0.2rc4/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/cli/options.py` & `autumn8-1.0.2rc4/autumn8/cli/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,23 @@
     "--organization_id",
     "--org_id",
     type=int,
     callback=pick_or_verify_organization,
     help="The ID of the Organization to use",
 )
 
+use_auto_confirm = click.option(
+    "-y",
+    "--yes",
+    "auto_confirm",
+    type=bool,
+    is_flag=True,
+    help="Skip all confirmation input from the user.",
+)
+
 use_quiet_mode = click.option(
     "-q",
     "--quiet",
     is_flag=True,
     callback=lambda ctx, param, value: logging.set_max_log_verbosity(
         logging.ERROR
     )
```

### Comparing `autumn8-1.0.2rc3/autumn8/cli/pending_uploads.py` & `autumn8-1.0.2rc4/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/common/config/cloud_info.py` & `autumn8-1.0.2rc4/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/common/config/s3.py` & `autumn8-1.0.2rc4/autumn8/common/config/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         aws_secret_access_key=secret,
     )
 
 
 def init_s3(s3_host) -> S3ServiceResource:
     # TODO - we need to somehow include these in CLI without hardcoding
 
-    # AWS_ACCESS_KEY_ID = os.environ["NEXT_PUBLIC_AWS_ACCESS_KEY_ID"]
-    # AWS_SECRET_ACCESS_KEY = os.environ["NEXT_PUBLIC_AWS_SECRET_KEY"]
+    # AWS_ACCESS_KEY_ID = autumn8.env.cli().NEXT_PUBLIC_AWS_ACCESS_KEY_ID
+    # AWS_SECRET_ACCESS_KEY = autumn8.env.cli().NEXT_PUBLIC_AWS_SECRET_KEY
     AWS_ACCESS_KEY_ID = "AKIASO72NKUYW7ONNRFO"
     AWS_SECRET_ACCESS_KEY = "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"
 
     # is_using_localstack = "localhost" in s3_host
 
     # if not is_using_localstack:
     #     # TODO: clean up the whole codebase, so that we don't provide the s3_endpoint, unless we want to use localstack
@@ -47,15 +47,14 @@
 
     return boto3.resource(
         "s3",
         region_name=AUTODL_S3_REGION,
         endpoint_url=s3_host,
         aws_access_key_id=AWS_ACCESS_KEY_ID,
         aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
-        # config=Config(s3={"use_accelerate_endpoint": not is_using_localstack}),
     )
 
 
 def init_s3_client(s3_host) -> S3Client:
     return init_s3(s3_host).meta.client
```

### Comparing `autumn8-1.0.2rc3/autumn8/common/config/settings.py` & `autumn8-1.0.2rc4/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/common/config/supported_instances.py` & `autumn8-1.0.2rc4/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/common/types.py` & `autumn8-1.0.2rc4/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/examples/mnist.py` & `autumn8-1.0.2rc4/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/examples/model.py` & `autumn8-1.0.2rc4/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.2rc4/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.2rc4/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/__init__.py` & `autumn8-1.0.2rc4/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/api/cloud.py` & `autumn8-1.0.2rc4/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/api/lab.py` & `autumn8-1.0.2rc4/autumn8/lib/api/lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,46 +71,69 @@
         auth=HTTPBasicAuth(user_id, api_key),
     )
 
     require_ok_response(response)
     return json.loads(response.text)["user"]
 
 
-def post_model(
+def get_model(environment: CliEnvironment, organization_id: int, model_id: int):
+    autodl_host = environment.value.app_host
+    api_route = f"{autodl_host}/api/lab/model/stub"
+    logger.info("Fetching model with id=%s", model_id)
+    response = requests.get(
+        url_with_params(
+            api_route,
+            {"organization_id": organization_id, "model_id": model_id},
+        ),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+    )
+
+    require_ok_response(response)
+    return response.json()
+
+
+def delete_model(
     environment: CliEnvironment,
     organization_id: int,
-    model_config: Dict[str, Any],
+    model_id: int,
 ):
     autodl_host = environment.value.app_host
     api_route = f"{autodl_host}/api/lab/model"
-    logger.info("Submitting model to %s", api_route)
-    response = requests.post(
-        url_with_params(api_route, {"organization_id": organization_id}),
+    logger.info("Deleting model with id=%s", model_id)
+    response = requests.delete(
+        url_with_params(
+            api_route,
+            {"organization_id": organization_id, "model_id": model_id},
+        ),
         headers={"Content-Type": "application/json"},
-        data=json.dumps(model_config),
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
 
     require_ok_response(response)
     return response.json()
 
 
-def delete_model(
-    environment: CliEnvironment, organization_id: int, model_id: int
+def post_model(
+    environment: CliEnvironment,
+    organization_id: int,
+    model_config: Dict[str, Any],
 ):
     autodl_host = environment.value.app_host
-    new_url = url_with_params(
-        f"{autodl_host}/api/lab/model",
-        {"model_id": model_id, "organization_id": organization_id},
-    )
-    response = requests.delete(
-        new_url,
+    api_route = f"{autodl_host}/api/lab/model"
+    logger.info("Submitting model to %s", api_route)
+    response = requests.post(
+        url_with_params(api_route, {"organization_id": organization_id}),
+        headers={"Content-Type": "application/json"},
+        data=json.dumps(model_config),
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
+
     require_ok_response(response)
+    return response.json()
 
 
 def normal_or_multipart_upload(
     environment,
     s3_file_url,
     f,
     resume_args,
```

### Comparing `autumn8-1.0.2rc3/autumn8/lib/api_creds.py` & `autumn8-1.0.2rc4/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/logging.py` & `autumn8-1.0.2rc4/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/logging.yaml` & `autumn8-1.0.2rc4/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/package_resolver.py` & `autumn8-1.0.2rc4/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8/lib/service.py` & `autumn8-1.0.2rc4/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.2rc4/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc3
+Version: 1.0.2rc4
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc3/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.2rc4/autumn8.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 autumn8/common/_version.py
 autumn8/common/types.py
 autumn8/common/config/__init__.py
 autumn8/common/config/cloud_info.py
 autumn8/common/config/s3.py
 autumn8/common/config/settings.py
 autumn8/common/config/supported_instances.py
+autumn8/env/__init__.py
+autumn8/env/app.py
+autumn8/env/cli.py
+autumn8/env/predictor.py
+autumn8/env/worker.py
 autumn8/examples/convblock.py
 autumn8/examples/loadMnist.py
 autumn8/examples/mnist.py
 autumn8/examples/model.py
 autumn8/examples/sbert-alpha.py
 autumn8/examples/tensorflow_custom_layers.py
 autumn8/lib/__init__.py
```

### Comparing `autumn8-1.0.2rc3/pyproject.toml` & `autumn8-1.0.2rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.2rc4/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc3/tests/test_settings.py` & `autumn8-1.0.2rc4/tests/test_settings.py`

 * *Files identical despite different names*

