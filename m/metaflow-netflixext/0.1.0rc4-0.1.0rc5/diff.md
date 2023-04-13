# Comparing `tmp/metaflow-netflixext-0.1.0rc4.tar.gz` & `tmp/metaflow-netflixext-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.1.0rc4.tar", last modified: Tue Apr  4 10:03:17 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.1.0rc5.tar", last modified: Thu Apr 13 08:36:25 2023, max compression
```

## Comparing `metaflow-netflixext-0.1.0rc4.tar` & `metaflow-netflixext-0.1.0rc5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.951521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31265 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.955521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126840 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42598 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.951521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-04 10:03:17.000000 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-04 10:03:17.000000 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:03:17.000000 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-04 10:03:17.000000 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 10:03:17.000000 metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:03:17.959521 metaflow-netflixext-0.1.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-04 10:03:02.000000 metaflow-netflixext-0.1.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32856 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148709 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44143 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/setup.py
```

### Comparing `metaflow-netflixext-0.1.0rc4/LICENSE` & `metaflow-netflixext-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/PKG-INFO` & `metaflow-netflixext-0.1.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.1.0rc4/README.md` & `metaflow-netflixext-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,20 @@
         # We need to install ipykernel into the resolved environment
         obj.echo("    Resolving an environment compatible with Jupyter ...", nl=False)
         # We don't pin to avoid issues with python versions -- it will take the
         # best one it can.
         env = cast(Conda, obj.conda).add_to_resolved_env(
             env,
             using_steps=["ipykernel"],
-            deps=[TStr(category="conda", value="ipykernel")],
+            deps=[
+                TStr(
+                    category="pip" if env.env_type == EnvType.PIP_ONLY else "conda",
+                    value="ipykernel",
+                )
+            ],
             sources=[],
             architecture=arch_id(),
         )
         # Cache this information for the next time around
         cast(Conda, obj.conda).cache_environments([env])
         cast(Conda, obj.conda).add_environments([env])
         cast(Conda, obj.conda).set_default_environment(env.env_id)
@@ -462,27 +467,29 @@
             "Cannot specify a Python version if using --using-pathspec or --using",
         )
     resolver = EnvsResolver(obj.conda)
 
     new_conda_deps = {}  # type: Dict[str, str]
     new_pip_deps = {}  # type: Dict[str, str]
     new_sources = []  # type: List[TStr]
+    new_extras = []  # type: List[TStr]
 
     using_str = None  # type: Optional[str]
     if using:
         using_str = using
     if using_pathspec:
         using_str = "step:%s" % using_pathspec
 
     archs = list(arch) if arch else [arch_id()]
     base_env_id = None
     base_env_conda_deps = {}  # type: Dict[str, str]
     base_env_pip_deps = {}  # type: Dict[str, str]
     base_env_conda_channels = []  # type: List[str]
     base_env_pip_sources = []  # type: List[str]
+    base_env_extras = []  # type: List[TStr]
     base_env_python = python
     base_env = None  # type: Optional[ResolvedEnvironment]
     if using_str:
         base_env_id = cast(Conda, obj.conda).env_id_from_alias(using_str, local_only)
         if base_env_id is None:
             raise CommandException("No known environment for '%s'" % using_str)
 
@@ -521,19 +528,22 @@
         base_env_conda_channels.extend(
             [s.value for s in all_sources if s.category == "conda"]
         )
         base_env_pip_sources.extend(
             [s.value for s in all_sources if s.category == "pip"]
         )
 
+        # Finally the extras
+        base_env_extras = base_env.extras
+
     # Parse yaml first to put conda sources first to be consistent with step decorator
     if yml_file:
-        _parse_yml_file(yml_file, new_sources, new_conda_deps, new_pip_deps)
+        _parse_yml_file(yml_file, new_extras, new_sources, new_conda_deps, new_pip_deps)
     if req_file:
-        _parse_req_file(req_file, new_sources, new_pip_deps)
+        _parse_req_file(req_file, new_extras, new_sources, new_pip_deps)
 
     if base_env_python is None:
         base_env_python = platform.python_version()
 
     # Compute the deps
     if len(new_conda_deps) == 0 and (
         not base_env or base_env.env_type == EnvType.PIP_ONLY
@@ -570,15 +580,17 @@
             (
                 TStr("pip", "%s==%s" % (name, ver) if ver else name)
                 for name, ver in pip_deps.items()
             ),
         )
     )
 
-    requested_req_id = ResolvedEnvironment.get_req_id(deps, sources)
+    extras = base_env_extras + new_extras
+
+    requested_req_id = ResolvedEnvironment.get_req_id(deps, sources, extras)
 
     for cur_arch in archs:
         if base_env_id:
             base_env = cast(Conda, obj.conda).environment(
                 EnvID(
                     req_id=base_env_id.req_id,
                     full_id=base_env_id.full_id,
@@ -591,14 +603,15 @@
                     "Environment for '%s' is not available on architecture '%s'"
                     % (using_str, cur_arch)
                 )
         resolver.add_environment(
             EnvID(requested_req_id, "_default", cur_arch),
             deps,
             sources,
+            extras,
             base_env,
             local_only=local_only,
             force=force,
             force_co_resolve=len(archs) > 1,
         )
 
     has_something = False
@@ -794,40 +807,68 @@
     if obj.quiet:
         obj.echo_always(env.quiet_print(existing_envs))
     else:
         obj.echo(env.pretty_print(existing_envs))
     cast(Conda, obj.conda).write_out_environments()
 
 
-def _parse_req_file(file_name: str, sources: List[TStr], deps: Dict[str, str]):
+def _parse_req_file(
+    file_name: str, extra_args: List[TStr], sources: List[TStr], deps: Dict[str, str]
+):
     with open(file_name, mode="r", encoding="utf-8") as f:
         for line in f:
             line = line.strip()
             if not line:
                 continue
-            elif line.startswith("-i") or line.startswith("--index-url"):
-                sources.append(
-                    TStr(category="pip", value=line.split(" ", 1)[1].strip())
+            splits = line.split(maxsplit=1)
+            first_word = splits[0]
+            if len(splits) > 1:
+                rem = splits[1]
+            else:
+                rem = None
+            if first_word in ("-i", "--index-url"):
+                raise InvalidEnvironmentException(
+                    "To specify a base PIP index, set `METAFLOW_CONDA_DEFAULT_PIP_SOURCE; "
+                    "you can specify additional indices using --extra-index-url"
+                )
+            elif first_word == "--extra-index-url" and rem:
+                sources.append(TStr(category="pip", value=rem))
+            elif first_word in ("-f", "--find-links", "--trusted-host") and rem:
+                extra_args.append(
+                    TStr(category="pip", value=" ".join([first_word, rem]))
                 )
-            elif line.startswith("#"):
+            elif first_word in ("--pre", "--no-index"):
+                extra_args.append(TStr(category="pip", value=first_word))
+            elif first_word.startswith("#"):
                 continue
-            elif line.startswith("-"):
+            elif first_word.startswith("-"):
                 raise InvalidEnvironmentException(
                     "'%s' is not a supported line in a requirements.txt" % line
                 )
+            elif (
+                first_word.startswith("git+")
+                or first_word.startswith("hg+")
+                or first_word.startswith("bzr+")
+                or first_word.startswith("svn+")
+                or (rem and rem[0] == "@")
+            ):
+                if rem and rem[0] == "@":
+                    first_word = rem[1:].strip()
+                deps[first_word] = ""
             else:
                 splits = line.split("=", 1)
                 if len(splits) == 1:
                     deps[line.strip()] = ""
                 else:
                     deps[splits[0].strip()] = splits[1].lstrip(" =").rstrip()
 
 
 def _parse_yml_file(
     file_name: str,
+    _: List[TStr],
     sources: List[TStr],
     conda_deps: Dict[str, str],
     pip_deps: Dict[str, str],
 ):
     with open(file_name, mode="r", encoding="utf-8") as f:
         # Very poor man's yaml parsing
         mode = None
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,12 +85,12 @@
 # Preferred Format for Conda packages
 CONDA_PREFERRED_FORMAT = from_conf(
     "CONDA_PREFERRED_FORMAT",
     None,
     get_validate_choice_fn([".tar.bz2", ".conda"]),
 )
 
-CONDA_DEFAULT_PIP_SOURCES = from_conf("CONDA_DEFAULT_PIP_SOURCES", [])
+CONDA_DEFAULT_PIP_SOURCE = from_conf("CONDA_DEFAULT_PIP_SOURCE", None)
 
 CONDA_REMOTE_COMMANDS = ("batch", "kubernetes")
 
 DEBUG_OPTIONS = ["conda"]
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 import tarfile
 import tempfile
 import time
 
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import closing
 from distutils.version import LooseVersion
-from itertools import chain
+from itertools import chain, product
 from typing import (
     Any,
     Callable,
     Dict,
+    FrozenSet,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     OrderedDict,
     Sequence,
@@ -51,41 +52,45 @@
     CONDA_LOCAL_PATH,
     CONDA_LOCK_TIMEOUT,
     CONDA_PACKAGES_DIRNAME,
     CONDA_ENVS_DIRNAME,
     CONDA_PREFERRED_FORMAT,
     CONDA_REMOTE_INSTALLER,
     CONDA_REMOTE_INSTALLER_DIRNAME,
-    CONDA_DEFAULT_PIP_SOURCES,
+    CONDA_DEFAULT_PIP_SOURCE,
 )
 from metaflow.metaflow_environment import InvalidEnvironmentException
 
+from metaflow_extensions.netflix_ext.vendor.packaging.tags import Tag
+from metaflow_extensions.netflix_ext.vendor.packaging.utils import parse_wheel_filename
 
 from .utils import (
     CONDA_FORMATS,
     TRANSMUT_PATHCOMPONENT,
     AliasType,
     CondaException,
     CondaStepException,
     arch_id,
     convert_filepath,
     get_conda_root,
     is_alias_mutable,
     parse_explicit_url_conda,
     parse_explicit_url_pip,
-    pip_platform_args,
+    parse_explicit_path_pip,
+    pip_tags_from_arch,
     plural_marker,
     resolve_env_alias,
 )
 
 from .env_descr import (
     CondaPackageSpecification,
     EnvID,
     EnvType,
     PackageSpecification,
+    PipCachePackage,
     PipPackageSpecification,
     ResolvedEnvironment,
     TStr,
     read_conda_manifest,
     write_to_conda_manifest,
 )
 
@@ -101,27 +106,29 @@
 
 class Conda(object):
     _cached_info = None
 
     def __init__(
         self, echo: Callable[..., None], datastore_type: str, mode: str = "local"
     ):
-        from metaflow.cli import logger
+        from metaflow.cli import logger, echo_dev_null
 
         if id(echo) != id(logger):
 
             def _modified_logger(*args: Any, **kwargs: Any):
                 if "timestamp" in kwargs:
                     del kwargs["timestamp"]
                 echo(*args, **kwargs)
 
             self._echo = _modified_logger
         else:
             self._echo = echo
 
+        self._no_echo = echo_dev_null
+
         self._datastore_type = datastore_type
         self._mode = mode
         self._bins = None  # type: Optional[Dict[str, Optional[str]]]
         self._conda_executable_type = None  # type: Optional[str]
 
         # For remote mode, make sure we are not going to try to check too much
         # We don't need much at all in remote mode.
@@ -183,14 +190,15 @@
         return None
 
     def resolve(
         self,
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
+        extras: Sequence[TStr],
         architecture: str,
         env_type: Optional[EnvType] = None,
     ) -> ResolvedEnvironment:
         if self._mode != "local":
             # TODO: Maybe relax this later but for now assume that the remote environment
             # is a "lighter" conda.
             raise CondaException("Cannot resolve environments in a remote environment")
@@ -223,14 +231,19 @@
             )
         if self._bins and self._bins.get(resolver_bin) is None:
             raise InvalidEnvironmentException(
                 "Resolver '%s' for %s mode is not installed"
                 % (resolver_bin, env_type.value)
             )
 
+        if extras and env_type != EnvType.PIP_ONLY:
+            raise InvalidEnvironmentException(
+                "Passing extra arguments is only supported for pip-only environments, "
+                "found '%s' but environment type is %s" % (str(extras), env_type.value)
+            )
         try:
             if env_type == EnvType.CONDA_ONLY:
                 packages = self._resolve_env_with_conda(deps, sources, architecture)
             elif env_type == EnvType.MIXED:
                 if resolver_bin == "conda-lock":
                     packages = self._resolve_env_with_conda_lock(
                         deps, sources, architecture
@@ -240,59 +253,71 @@
                     # add other mixed resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
             else:
                 # Pip only mode
                 packages = self._resolve_env_with_conda(deps, sources, architecture)
+                conda_only_deps = [d for d in deps if d.category == "conda"]
+                conda_only_sources = [s for s in sources if s.category == "conda"]
+                builder_resolved_env = ResolvedEnvironment(
+                    conda_only_deps,
+                    conda_only_sources,
+                    None,
+                    architecture,
+                    all_packages=packages,
+                    env_type=EnvType.CONDA_ONLY,
+                )
                 if resolver_bin == "pip":
                     # We need to get the python package to get the version
                     python_version = None  # type: Optional[str]
                     for p in packages:
                         if p.filename.startswith("python-"):
                             python_version = p.package_version
                             break
                     if python_version is None:
                         raise CondaException(
                             "Could not determine version of Python from conda packages"
                         )
-                    else:
-                        if (
-                            architecture == arch_id()
-                            and python_version == platform.python_version()
-                        ):
-                            python_version = None
-                        packages.extend(
-                            self._resolve_env_with_pip(
-                                python_version, deps, sources, architecture
-                            )
+
+                    packages.extend(
+                        self._resolve_env_with_pip(
+                            python_version,
+                            deps,
+                            sources,
+                            extras,
+                            architecture,
+                            builder_resolved_env,
                         )
+                    )
                 else:
                     # Should also never happen and be caught earlier but being clean
                     # add other pip resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
 
             return ResolvedEnvironment(
                 deps,
                 sources,
+                extras,
                 architecture,
                 all_packages=packages,
                 env_type=env_type,
             )
         except CondaException as e:
             raise CondaStepException(e, using_steps)
 
     def add_to_resolved_env(
         self,
         cur_env: ResolvedEnvironment,
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
+        extras: Sequence[TStr],
         architecture: str,
         inputs_are_addl: bool = True,
         cur_is_accurate: bool = True,
     ) -> ResolvedEnvironment:
         if self._mode != "local":
             # TODO: Maybe relax this later but for now assume that the remote environment
             # is a "lighter" conda.
@@ -306,30 +331,35 @@
                 "Mismatched architecture when extending an environment"
             )
         # We form the new list of dependencies based on the ones we have in cur_env
         # and the new ones.
         if inputs_are_addl:
             sources = list(chain(cur_env.sources, sources))
             user_deps = list(chain(cur_env.deps, deps))
+            extras = list(chain(cur_env.extras, extras))
         else:
             sources = sources
             user_deps = deps
+            extras = extras
         deps = list(
             chain(
                 [
                     TStr(p.TYPE, "%s==%s" % (p.package_name, p.package_version))
                     for p in cur_env.packages
                 ],
                 user_deps,
             )
         )
+
         # We check if we already resolved this environment and bypass resolving for
         # if it we already have solved for it.
         new_env_id = EnvID(
-            ResolvedEnvironment.get_req_id(user_deps, sources), "_default", architecture
+            ResolvedEnvironment.get_req_id(user_deps, sources, extras),
+            "_default",
+            architecture,
         )
         new_resolved_env = self.environment(new_env_id)
         if new_resolved_env:
             return new_resolved_env
 
         # Figure out the env_type
         new_env_type = cur_env.env_type
@@ -348,14 +378,15 @@
                 % (EnvType.CONDA_ONLY, EnvType.MIXED)
             )
 
         new_resolved_env = self.resolve(
             using_steps,
             deps,
             sources,
+            extras,
             architecture,
             env_type=new_env_type,
         )
 
         # We now try to copy as much information as possible from the current environment
         # which includes information about cached packages
         cur_packages = {p.filename: p.to_dict() for p in cur_env.packages}
@@ -365,14 +396,15 @@
             if existing_info:
                 merged_packages.append(PackageSpecification.from_dict(existing_info))
             else:
                 merged_packages.append(p)
         return ResolvedEnvironment(
             user_deps,
             sources,
+            extras,
             architecture,
             all_packages=merged_packages,
             env_type=new_resolved_env.env_type,
             accurate_source=cur_is_accurate,
         )
 
     def create_for_step(
@@ -1583,15 +1615,15 @@
                     "%s#%s" % (lnk["url"], lnk["md5"])
                 )
                 result.append(
                     CondaPackageSpecification(
                         filename=parse_result.filename,
                         url=parse_result.url,
                         url_format=parse_result.url_format,
-                        hashes={parse_result.url_format: parse_result.hash},
+                        hashes={parse_result.url_format: cast(str, parse_result.hash)},
                     )
                 )
         else:
 
             def _pkg_key(
                 name: str, platform: str, build_string: str, build_number: str
             ) -> str:
@@ -1619,56 +1651,85 @@
                     )
                 parse_result = parse_explicit_url_conda("%s#%s" % (url, md5_hash))
                 result.append(
                     CondaPackageSpecification(
                         filename=parse_result.filename,
                         url=parse_result.url,
                         url_format=parse_result.url_format,
-                        hashes={parse_result.url_format: parse_result.hash},
+                        hashes={parse_result.url_format: cast(str, parse_result.hash)},
                     )
                 )
         return result
 
     def _resolve_env_with_pip(
         self,
-        python_version: Optional[str],
+        python_version: str,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
+        extras: Sequence[TStr],
         architecture: str,
+        builder_env: ResolvedEnvironment,
     ) -> List[PackageSpecification]:
 
         deps = [d for d in deps if d.category == "pip"]
 
+        # Some args may be two actual arguments like "-f <something>" thus the map
+        extra_args = list(
+            chain.from_iterable(
+                map(
+                    lambda x: x.split(maxsplit=1),
+                    (e.value for e in extras if e.category == "pip"),
+                )
+            )
+        )
         result = []
         with tempfile.TemporaryDirectory() as pip_dir:
             args = [
+                "--isolated",
                 "install",
                 "--ignore-installed",
                 "--dry-run",
                 "--target",
                 pip_dir,
                 "--report",
                 os.path.join(pip_dir, "out.json"),
             ]
+            args.extend(extra_args)
+            if CONDA_DEFAULT_PIP_SOURCE:
+                args.extend(["-i", CONDA_DEFAULT_PIP_SOURCE])
             for c in chain(
-                CONDA_DEFAULT_PIP_SOURCES or [],
                 (s.value for s in sources if s.category == "pip"),
             ):
-                args.extend(["-i", c])
+                args.extend(["--extra-index-url", c])
 
-            if python_version is not None:
-                # If architecture != arch_id(), we will always have python_version
-                # specified
-
-                # Just take the first two -- it seems to work better that way
+            supported_tags = pip_tags_from_arch(python_version, architecture)
+            if python_version != platform.python_version() or architecture != arch_id():
                 clean_version = ".".join(python_version.split(".")[:2])
                 args.extend(["--only-binary=:all:", "--python-version", clean_version])
 
-                if architecture != arch_id():
-                    args.extend(pip_platform_args(python_version, architecture))
+            if architecture != arch_id():
+                implementations = []  # type: List[str]
+                abis = []  # type: List[str]
+                platforms = []  # type: List[str]
+                for tag in supported_tags:
+                    implementations.append(tag.interpreter)
+                    abis.append(tag.abi)
+                    platforms.append(tag.platform)
+                implementations = [x.interpreter for x in supported_tags]
+                extra_args = (
+                    *(
+                        chain.from_iterable(
+                            product(["--implementation"], implementations)
+                        )
+                    ),
+                    *(chain.from_iterable(product(["--abi"], abis))),
+                    *(chain.from_iterable(product(["--platform"], platforms))),
+                )
+
+                args.extend(extra_args)
 
             # Unfortunately, pip doesn't like things like ==<= so we need to strip
             # the ==
             for d in deps:
                 splits = d.value.split("==")
                 if len(splits) == 1:
                     args.append(d.value)
@@ -1684,30 +1745,384 @@
 
             # We should now have a json blob in out.json
             result = []  # type: List[PackageSpecification]
             with open(
                 os.path.join(pip_dir, "out.json"), mode="r", encoding="utf-8"
             ) as f:
                 desc = json.load(f)
+            packages_to_build = []  # type: List[Dict[str, Any]]
             for package_desc in desc["install"]:
-                parse_result = parse_explicit_url_pip(
-                    "%s#%s"
-                    % (
-                        package_desc["download_info"]["url"],
-                        package_desc["download_info"]["archive_info"]["hash"],
-                    )
+                # We can either have a direct URL (in which case we have an "archive_info"
+                # blob), a directory (in which case we have a "dir_info" blob) or
+                # a repo (in which case we have a "vcs_info" blob).
+                # The first case is easy.
+                # For the second case, if we are in editable mode, we error out (it
+                # shouldn't get to here). If not, we add the file directly
+                # For the third case, we will build the package (only if the same
+                # arch) and then add it.
+                # The spec is given here:
+                # https://packaging.python.org/en/latest/specifications/direct-url-data-structure/
+                dl_info = package_desc["download_info"]
+                url = dl_info["url"]
+                if "dir_info" in dl_info or url.startswith("file://"):
+                    if dl_info["dir_info"].get("editable", False):
+                        raise CondaException(
+                            "Cannot include an editable PIP package: '%s'" % url
+                        )
+                    if os.path.isdir(url[7:]):
+                        packages_to_build.append(dl_info)
+                    else:
+                        parse_result = parse_explicit_path_pip(url)
+                        if parse_result.url_format != ".whl":
+                            # This is a source package so we need to build it
+                            packages_to_build.append(dl_info)
+                        else:
+                            package_spec = PipPackageSpecification(
+                                parse_result.filename,
+                                parse_result.url,
+                                parse_result.url_format,
+                                None,
+                            )
+                            # Use url to not have the `file://` and not use the canonical
+                            # file://local-file/ path
+                            package_spec.add_local_file(parse_result.url_format, url)
+                            result.append(package_spec)
+                elif "vcs_info" in dl_info:
+                    packages_to_build.append(dl_info)
+                else:
+                    if "hashes" in dl_info["archive_info"]:
+                        hashes = dl_info["archive_info"]["hashes"]
+                        for fmt, val in hashes.items():
+                            if fmt == PipPackageSpecification.base_hash_name():
+                                hash = "%s=%s" % (fmt, val)
+                                break
+                        else:
+                            raise CondaException(
+                                "Cannot find hash '%s' for package at '%s'"
+                                % (
+                                    PipPackageSpecification.base_hash_name(),
+                                    url,
+                                )
+                            )
+                    else:
+                        # Fallback on older "hash" field
+                        hash = dl_info["archive_info"]["hash"]
+
+                    parse_result = parse_explicit_url_pip("%s#%s" % (url, hash))
+                    if parse_result.url_format != ".whl":
+                        packages_to_build.append(dl_info)
+                    else:
+                        result.append(
+                            PipPackageSpecification(
+                                parse_result.filename,
+                                parse_result.url,
+                                parse_result.url_format,
+                                {parse_result.url_format: parse_result.hash}
+                                if parse_result.hash
+                                else None,
+                            )
+                        )
+            if packages_to_build:
+                # Will contain:
+                #  - build_url: url to use to build with pip wheel
+                #  - cache_url: url in the cache
+                #  - pkg_filename: name of the package
+                #  - pkg_spec: PackageSpecification for the package
+                # Keyed by the cannonical URL we assign for it
+                to_build_pkg_info = (
+                    {}
+                )  # type: Dict[str, Dict[str, Union[str, PackageSpecification, List[Tuple[FrozenSet[Tag], str]]]]]
+                for package_desc in packages_to_build:
+                    if "vcs_info" in package_desc:
+                        base_build_url = "%s+%s@%s" % (
+                            package_desc["vcs_info"]["vcs"],
+                            package_desc["url"],
+                            package_desc["vcs_info"]["commit_id"],
+                        )
+                        # We form a "fake" URL which will give us a unique key so we can
+                        # look up the package build in the cache. Given we have the
+                        # commit_id, we assume that for a combination of repo, commit_id
+                        # and subdirectory, we have a uniquely built package. This will
+                        # give users some consistency as well in the sense that an
+                        # environment that uses the same git package reference will
+                        # actually use the same package
+                        base_pkg_url = "%s/%s" % (
+                            package_desc["url"],
+                            package_desc["vcs_info"]["commit_id"],
+                        )
+                        if "subdirectory" in package_desc:
+                            base_build_url += (
+                                "#subdirectory=%s" % package_desc["subdirectory"]
+                            )
+                            base_pkg_url += "/%s" % package_desc["subdirectory"]
+                        to_build_pkg_info[base_pkg_url] = {
+                            "build_url": base_build_url,
+                            "cache_url": PipCachePackage.make_partial_cache_url(
+                                base_pkg_url
+                            ),
+                        }
+                    elif "dir_info" in package_desc:
+                        local_path = package_desc["url"][7:]
+                        if os.path.isdir(local_path):
+                            # For now support only setup.py packages.
+                            if not os.path.isfile(os.path.join(local_path, "setup.py")):
+                                raise InvalidEnvironmentException(
+                                    "Local directory '%s' is not supported as it is "
+                                    "missing a 'setup.py'" % local_path
+                                )
+                            package_name, package_version = (
+                                self._call_binary(
+                                    [
+                                        os.path.join(local_path, "setup.py"),
+                                        "-q",
+                                        "--name",
+                                        "--version",
+                                    ],
+                                    binary=sys.executable,
+                                )
+                                .decode(encoding="utf-8")
+                                .splitlines()
+                            )
+                            local_path = os.path.join(
+                                package_desc["url"],
+                                "%s-%s.whl" % (package_name, package_version),
+                            )
+                        parse_result = parse_explicit_path_pip(local_path)
+                        to_build_pkg_info[parse_result.url] = {
+                            "build_url": package_desc["url"],
+                            "cache_url": PipCachePackage.make_partial_cache_url(
+                                parse_result.url
+                            ),
+                        }
+                    else:
+                        # Just a regular .tar.gz package
+                        if package_desc["url"].endswith(".tar.gz"):
+                            cache_url = package_desc["url"][:-7] + ".whl"
+                        else:
+                            raise InvalidEnvironmentException(
+                                "Expected a '.tar.gz' package: '%s'"
+                                % package_desc["url"]
+                            )
+                        to_build_pkg_info[cache_url] = {
+                            "build_url": package_desc["url"],
+                            "cache_url": PipCachePackage.make_partial_cache_url(
+                                cache_url
+                            ),
+                        }
+
+                # We check in the cache -- we don't actually have the filename or
+                # hash so we check things starting with the partial URL
+                debug.conda_exec(
+                    "Checking for pre-built packages: %s" % str(to_build_pkg_info)
                 )
-                result.append(
-                    PipPackageSpecification(
-                        parse_result.filename,
-                        parse_result.url,
-                        parse_result.url_format,
-                        {parse_result.url_format: parse_result.hash},
+                found_files = self._storage.list_content(
+                    (x["cache_url"] for x in to_build_pkg_info.values())
+                )
+                keys_to_check = []  # type: List[str]
+                for cache_path, is_file in found_files:
+                    cache_path = cast(str, cache_path)
+                    is_file = cast(bool, is_file)
+                    if is_file:
+                        raise CondaException(
+                            "Invalid cache content at '%s'" % cache_path
+                        )
+
+                    debug.conda_exec(
+                        "Found potential pre-built package at '%s'" % cache_path
+                    )
+                    for k, v in to_build_pkg_info.items():
+                        if cache_path.startswith(cast(str, v["cache_url"])):
+                            keys_to_check.append(k)
+                            # We now have a potential filename for the package. We
+                            # note it so that we can later match it based on the
+                            # supported tags for this platform
+                            filename = os.path.split(cache_path.rstrip("/"))[1]
+                            cast(
+                                List[Tuple[FrozenSet[Tag], str]],
+                                v.setdefault("pkg_filenames", []),
+                            ).append((parse_wheel_filename(filename)[3], cache_path))
+                            if "pkg_filename" in v:
+                                raise CondaException(
+                                    "File at '%s' is a duplicate of '%s'"
+                                    % (cache_path, v["cache_url"])
+                                )
+                # We now check all the keys_to_check (basically where we found potential
+                # matches) for files that have the right tag for the platform we are
+                # building for
+                for k in keys_to_check:
+                    potentials = cast(
+                        List[Tuple[FrozenSet[Tag], str]],
+                        to_build_pkg_info[k]["pkg_filenames"],
+                    )
+                    for t in supported_tags:
+                        # Tags are ordered from most-preferred to least preferred
+                        for p in potentials:
+                            # Potentials are in no particular order but we will
+                            # effectively get a package with the most preferred tag
+                            # if one exists
+                            if t in p[0]:
+                                to_build_pkg_info[k]["cache_url"] = p[1]
+                                to_build_pkg_info[k]["pkg_filename"] = os.path.split(
+                                    p[1].rstrip("/")
+                                )[1]
+                                debug.conda_exec(
+                                    "For '%s', found matching package at %s" % (k, p[1])
+                                )
+                                break
+                        else:
+                            # If we don't find a match, continue to next tag (and
+                            # skip break of outer loop on next line)
+                            continue
+                        break
+
+                # We now check for hashes for those packages we did find (it's the
+                # next level down in the cache)
+                found_files = self._storage.list_content(
+                    (
+                        x["cache_url"]
+                        for x in to_build_pkg_info.values()
+                        if "pkg_filename" in x
                     )
                 )
+                for cache_path, is_file in found_files:
+                    cache_path = cast(str, cache_path)
+                    is_file = cast(bool, is_file)
+                    if is_file:
+                        raise CondaException(
+                            "Invalid cache content at '%s'" % cache_path
+                        )
+
+                    debug.conda_exec("Found package with hash at '%s'" % cache_path)
+                    for k, v in to_build_pkg_info.items():
+                        if cache_path.startswith(cast(str, v["cache_url"])):
+                            # We now have the hash for the package
+                            pkg_hash = os.path.split(cache_path.rstrip("/"))[1]
+                            pkg_url = os.path.join(k, cast(str, v["pkg_filename"]))
+                            v["cache_url"] = PipCachePackage.make_cache_url(
+                                pkg_url, pkg_hash
+                            )
+                            v["pkg_spec"] = PipPackageSpecification(
+                                cast(str, v["pkg_filename"])[:-4],
+                                pkg_url,
+                                ".whl",
+                                {".whl": pkg_hash},
+                                {".whl": PipCachePackage(v["cache_url"])},
+                            )
+                            break
+                    else:
+                        raise CondaException(
+                            "Found unexpected content at '%s'" % cache_path
+                        )
+
+                if any("pkg_spec" not in v for v in to_build_pkg_info.values()):
+                    self._echo(" (building PIP packages from repositories)", nl=False)
+                    # We need to build packages -- we only allow this if the architecture
+                    # is the same to avoid potential cross-building. We could relax this to
+                    # noarch packages but playing it safe for now
+                    if arch_id() != architecture:
+                        raise CondaException(
+                            "Specifying PIP packages from repositories requires "
+                            "building the wheels and this is only allowed if the target "
+                            "architecture is the same as this one"
+                        )
+                    debug.conda_exec(
+                        "Creating builder environment to build PIP packages"
+                    )
+
+                    target_directory = os.path.join(self._package_dirs[0], "pip")
+                    os.makedirs(target_directory, exist_ok=True)
+
+                    techo = self._echo
+                    self._echo = self._no_echo
+                    self.create_for_name(
+                        self._env_builder_directory_from_envid(builder_env.env_id),
+                        builder_env,
+                    )
+                    self._echo = techo
+
+                    builder_python = cast(
+                        str,
+                        self.python(
+                            self._env_builder_directory_from_envid(builder_env.env_id)
+                        ),
+                    )
+
+                    def _build_with_pip(identifier: int, key: str, url: str):
+                        dest_path = os.path.join(pip_dir, "build_%d" % identifier)
+                        debug.conda_exec(
+                            "Building package '%s'  for '%s' in '%s'"
+                            % (url, key, dest_path)
+                        )
+                        self._call_binary(
+                            [
+                                "-m",
+                                "pip",
+                                "--isolated",
+                                "wheel",
+                                "--no-deps",
+                                "--progress-bar",
+                                "off",
+                                "-w",
+                                dest_path,
+                                url,
+                            ],
+                            binary=builder_python,
+                        )
+                        return key, dest_path
+
+                    with ThreadPoolExecutor() as executor:
+                        build_result = [
+                            executor.submit(
+                                _build_with_pip, idx, key, cast(str, v["build_url"])
+                            )
+                            for idx, (key, v) in enumerate(to_build_pkg_info.items())
+                            if not "pkg_filename" in v
+                        ]
+                        for f in as_completed(build_result):
+                            key, build_dir = f.result()
+                            wheel_files = [
+                                f
+                                for f in os.listdir(build_dir)
+                                if os.path.isfile(os.path.join(build_dir, f))
+                                and f.endswith(".whl")
+                            ]
+                            if len(wheel_files) != 1:
+                                raise CondaException(
+                                    "Could not build '%s' -- found built packages: %s"
+                                    % (key, wheel_files)
+                                )
+
+                            wheel_file = os.path.join(build_dir, wheel_files[0])
+                            # Move the built wheel to a less temporary location
+                            wheel_file = shutil.copy(wheel_file, target_directory)
+                            debug.conda_exec(
+                                "Package for '%s' built in '%s'" % (key, wheel_file)
+                            )
+
+                            parse_result = parse_explicit_path_pip(
+                                "file://%s" % wheel_file
+                            )
+                            package_spec = PipPackageSpecification(
+                                parse_result.filename,
+                                os.path.join(key, "%s.whl" % parse_result.filename),
+                                parse_result.url_format,
+                                None,
+                            )
+                            package_spec.add_local_file(
+                                parse_result.url_format, wheel_file
+                            )
+
+                            to_build_pkg_info[key][
+                                "pkg_filename"
+                            ] = parse_result.filename
+                            to_build_pkg_info[key]["pkg_spec"] = package_spec
+
+                for v in to_build_pkg_info.values():
+                    result.append(cast(PackageSpecification, v["pkg_spec"]))
+
         return result
 
     def _resolve_env_with_conda_lock(
         self,
         deps: Sequence[TStr],
         channels: Sequence[TStr],
         architecture: str,
@@ -1753,15 +2168,15 @@
                 raise CondaException(
                     "Could not manage poetry's dependency using '{cmd}' -- got error"
                     "code {code}'; see pretty-printed error above".format(
                         cmd=e.cmd, code=e.returncode
                     )
                 )
 
-        pip_channels = (CONDA_DEFAULT_PIP_SOURCES or []) + [
+        pip_channels = ([CONDA_DEFAULT_PIP_SOURCE] if CONDA_DEFAULT_PIP_SOURCE else []) + [
             c.value for c in channels if c.category == "pip"
         ]  # type: List[str]
         try:
             # We resolve the environment using conda-lock
 
             # Write out the requirement yml file. It's easy enough so don't use a YAML
             # library to avoid adding another dep
@@ -1897,25 +2312,33 @@
                                 )
                             parse_result = parse_explicit_url_pip(components[4])
                             result.append(
                                 PipPackageSpecification(
                                     parse_result.filename,
                                     parse_result.url,
                                     parse_result.url_format,
-                                    {parse_result.url_format: parse_result.hash},
+                                    {
+                                        parse_result.url_format: cast(
+                                            str, parse_result.hash
+                                        )
+                                    },
                                 )
                             )
                         else:
                             parse_result = parse_explicit_url_conda(l.strip())
                             result.append(
                                 CondaPackageSpecification(
                                     parse_result.filename,
                                     parse_result.url,
                                     parse_result.url_format,
-                                    {parse_result.url_format: parse_result.hash},
+                                    {
+                                        parse_result.url_format: cast(
+                                            str, parse_result.hash
+                                        )
+                                    },
                                 )
                             )
                     if not emit and l.strip() == "@EXPLICIT":
                         emit = True
             return result
         finally:
             if outfile_name and os.path.isfile(outfile_name):
@@ -2653,14 +3076,18 @@
             return "https://" + "/".join(components[2:-2])
 
     @staticmethod
     def _env_directory_from_envid(env_id: EnvID) -> str:
         return "metaflow_%s_%s" % (env_id.req_id, env_id.full_id)
 
     @staticmethod
+    def _env_builder_directory_from_envid(env_id: EnvID) -> str:
+        return "metaflow_builder_%s_%s" % (env_id.req_id, env_id.full_id)
+
+    @staticmethod
     def _lnk_path_for_pkg(pkg: PackageSpecification, pkg_fmt: str) -> str:
         cached_base_version = pkg.cached_version(pkg.url_format)
         if cached_base_version:
             base_url = os.path.split(cached_base_version.url)[0]
         else:
             base_url = os.path.split(
                 pkg.cache_pkg_type().make_cache_url(
@@ -2767,22 +3194,24 @@
         args: List[str],
         binary: str,
         addl_env: Optional[Mapping[str, str]] = None,
         pretty_print_exception: bool = True,
     ) -> bytes:
         if binary in _CONDA_DEP_RESOLVERS:
             return self._call_conda(args, binary, addl_env, pretty_print_exception)
-        if self._bins is None or self._bins[binary] is None:
+        if self._bins and self._bins.get(binary) is not None:
+            binary = cast(str, self._bins[binary])
+        elif not os.path.isfile(binary) or not os.access(binary, os.X_OK):
             raise InvalidEnvironmentException("Binary '%s' unknown" % binary)
         if addl_env is None:
             addl_env = {}
         try:
-            debug.conda_exec("Binary call: %s" % str([self._bins[binary]] + args))
+            debug.conda_exec("Binary call: %s" % str([binary] + args))
             return subprocess.check_output(
-                [self._bins[binary]] + args,
+                [binary] + args,
                 stderr=subprocess.PIPE,
                 env=dict(os.environ, **addl_env),
             ).strip()
         except subprocess.CalledProcessError as e:
             print(
                 "Pretty-printed STDOUT:\n%s" % e.output.decode("utf-8")
                 if e.output
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,27 @@
     def _ensure_class_per_type():
         if CachePackage._class_per_type is None:
             CachePackage._class_per_type = {
                 c.TYPE: c for c in CachePackage.__subclasses__()
             }
 
     @classmethod
+    def make_partial_cache_url(cls, base_url: str):
+        if cls.TYPE != "pip":
+            raise ValueError("make_partial_cache_url only for pip packages")
+        cls._ensure_class_per_type()
+        url = urlparse(base_url)
+        return os.path.join(
+            cast(str, CONDA_PACKAGES_DIRNAME),
+            cls.TYPE,
+            url.netloc,
+            url.path.lstrip("/"),
+        )
+
+    @classmethod
     def make_cache_url(
         cls,
         base_url: str,
         file_hash: str,
         file_format: Optional[str] = None,
         is_transmuted: bool = False,
     ) -> str:
@@ -205,15 +218,15 @@
 
     _class_per_type = None  # type: Optional[Dict[str, Type[PackageSpecification]]]
 
     def __init__(
         self,
         filename: str,
         url: str,
-        url_format: str,
+        url_format: Optional[str] = None,
         hashes: Optional[Dict[str, str]] = None,
         cache_info: Optional[Dict[str, CachePackage]] = None,
     ):
         # if "/" in filename and not filename.startswith(self.TYPE):
         #     raise ValueError(
         #         "Attempting to create a package of type %s with filename %s"
         #         % (self.TYPE, filename)
@@ -553,35 +566,37 @@
 
 
 class ResolvedEnvironment:
     def __init__(
         self,
         user_dependencies: Sequence[TStr],
         user_sources: Optional[Sequence[TStr]],
+        user_extra_args: Optional[Sequence[TStr]],
         arch: Optional[str] = None,
         env_id: Optional[EnvID] = None,
         all_packages: Optional[Sequence[PackageSpecification]] = None,
         resolved_on: Optional[datetime] = None,
         resolved_by: Optional[str] = None,
         co_resolved: Optional[List[str]] = None,
         env_type: EnvType = EnvType.MIXED,
         accurate_source: bool = True,
     ):
         self._env_type = env_type
         self._user_dependencies = list(user_dependencies)
         self._user_sources = list(user_sources) if user_sources else []
+        self._user_extra_args = list(user_extra_args) if user_extra_args else []
         if all_packages is not None:
             # It should already be sorted but being very safe
             all_packages = sorted(all_packages, key=lambda p: p.filename)
 
         self._accurate_source = accurate_source
 
         if not env_id:
             env_req_id = ResolvedEnvironment.get_req_id(
-                self._user_dependencies, self._user_sources
+                self._user_dependencies, self._user_sources, self._user_extra_args
             )
             env_full_id = "_unresolved"
             if all_packages is not None:
                 env_full_id = self._compute_hash(
                     [
                         "%s#%s" % (p.filename, p.pkg_hash(p.url_format))
                         for p in all_packages
@@ -600,27 +615,33 @@
         self._parent = None  # type: Optional["CachedEnvironmentInfo"]
         self._dirty = False
 
     @staticmethod
     def get_req_id(
         deps: Sequence[TStr],
         sources: Optional[Sequence[TStr]] = None,
+        extra_args: Optional[Sequence[TStr]] = None,
     ) -> str:
         # Extract per category so we can sort independently for each category
         deps_by_category = {}  # type: Dict[str, List[str]]
         sources_by_category = {}  # type: Dict[str, List[str]]
+        extras_by_category = {}  # type: Dict[str, List[str]]
         for d in deps:
             deps_by_category.setdefault(d.category, []).append(d.value)
         if sources:
             for s in sources:
                 sources_by_category.setdefault(s.category, []).append(s.value)
+        if extra_args:
+            for e in extra_args:
+                extras_by_category.setdefault(e.category, []).append(e.value)
         return ResolvedEnvironment._compute_hash(
             chain(
                 *(sorted(deps_by_category[c]) for c in sorted(deps_by_category)),
-                *(sorted(sources_by_category[c]) for c in sorted(sources_by_category))
+                *(sorted(sources_by_category[c]) for c in sorted(sources_by_category)),
+                *(sorted(extras_by_category[c]) for c in sorted(extras_by_category))
             )
         )
 
     @staticmethod
     def set_coresolved_full_id(envs: Sequence["ResolvedEnvironment"]) -> None:
         envs = sorted(envs, key=lambda x: x.env_id.arch)
         to_hash = []  # type: List[str]
@@ -644,14 +665,18 @@
         return self._user_dependencies
 
     @property
     def sources(self) -> List[TStr]:
         return self._user_sources
 
     @property
+    def extras(self) -> List[TStr]:
+        return self._user_extra_args
+
+    @property
     def env_id(self) -> EnvID:
         if self._env_id.full_id in ("_default", "_unresolved") and self._all_packages:
             self._all_packages.sort(key=lambda p: p.filename)
             env_full_id = self._compute_hash(
                 [p.filename for p in self._all_packages]
                 + [self._env_id.arch or arch_id()]
             )
@@ -764,22 +789,31 @@
                 "*Resolved by* %s" % self.resolved_by,
                 "",
             ]
         )
         if local_instances:
             lines.extend(["*Locally present as* %s" % ", ".join(local_instances), ""])
 
+        # The `replace` is because the echo function uses "*" to split in bold/not bold
+        # It is quite likely to have a package spec like "3.8.*" so we replace it with
+        # the similar looking "3.8.x"
         lines.append(
-            "*User-requested packages* %s" % ", ".join([str(d) for d in self.deps])
+            "*User-requested packages* %s"
+            % ", ".join([str(d).replace("*", "x") for d in self.deps])
         )
 
         if self.sources:
             lines.append(
                 "*User sources* %s" % ", ".join([str(s) for s in self.sources])
             )
+
+        if self.extras:
+            lines.append(
+                "*Extra resolution flags* %s" % ", ".join([str(s) for s in self.extras])
+            )
         lines.append("")
 
         if conda_packages:
             lines.append(
                 "*Conda Packages installed* %s"
                 % ", ".join(
                     [
@@ -853,14 +887,15 @@
     def is_cached(self, formats: Dict[str, List[str]]) -> bool:
         return all([pkg.is_cached(formats.get(pkg.TYPE, [])) for pkg in self.packages])
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "deps": [str(x) for x in self._user_dependencies],
             "sources": [str(x) for x in self._user_sources],
+            "extras": [str(x) for x in self._user_extra_args],
             "packages": [p.to_dict() for p in self.packages],
             "resolved_on": self._resolved_on.isoformat(),
             "resolved_by": self._resolved_by,
             "resolved_archs": self._co_resolved,
             "env_type": self._env_type.value,
             "accurate_source": self._accurate_source,
         }
@@ -871,14 +906,15 @@
         env_id: EnvID,
         d: Mapping[str, Any],
     ):
         all_packages = [PackageSpecification.from_dict(pd) for pd in d["packages"]]
         return cls(
             user_dependencies=[TStr.from_str(x) for x in d["deps"]],
             user_sources=[TStr.from_str(x) for x in d["sources"]],
+            user_extra_args=[TStr.from_str(x) for x in d.get("extras", [])],
             env_id=env_id,
             all_packages=all_packages,
             resolved_on=datetime.fromisoformat(d["resolved_on"]),
             resolved_by=d["resolved_by"],
             co_resolved=d["resolved_archs"],
             env_type=EnvType(d.get("env_type", EnvType.MIXED.value)),
             accurate_source=d.get("accurate_source", True),
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self._co_resolved_force_resolve = set()  # type: Set[str]
 
     def add_environment(
         self,
         env_id: EnvID,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
+        extras: Sequence[TStr],
         base_env: Optional[ResolvedEnvironment] = None,
         base_from_full_id: bool = False,
         local_only: bool = False,
         force: bool = False,
         force_co_resolve: bool = False,
     ):
         self._non_step_envs = True
@@ -73,14 +74,15 @@
                     resolved_env = None
 
             self._requested_envs[env_id] = {
                 "id": env_id,
                 "steps": ["ad-hoc"],
                 "deps": deps,
                 "sources": sources,
+                "extras": extras,
                 "conda_format": [CONDA_PREFERRED_FORMAT]
                 if CONDA_PREFERRED_FORMAT
                 else ["_any"],
                 "base": base_env,
                 "base_accurate": base_env
                 and base_env.is_info_accurate
                 and not base_from_full_id,
@@ -118,14 +120,15 @@
             resolved_env = self._conda.environment(env_id) if not force else None
             if env_id not in self._requested_envs:
                 self._requested_envs[env_id] = {
                     "id": env_id,
                     "steps": [step_name],
                     "deps": decorator.step_deps,
                     "sources": decorator.source_deps,
+                    "extras": [],
                     "conda_format": [CONDA_PREFERRED_FORMAT]
                     if CONDA_PREFERRED_FORMAT
                     else ["_any"],
                     "base": from_env,
                     "base_accurate": from_env
                     and from_env.is_info_accurate
                     and resolve_env_alias(cast(str, decorator.from_env_name))[0]
@@ -240,25 +243,27 @@
                 return (
                     env_id,
                     self._conda.add_to_resolved_env(
                         env_desc["base"],
                         env_desc["steps"],
                         env_desc["deps"],
                         env_desc["sources"],
+                        env_desc["extras"],
                         env_id.arch,
                         inputs_are_addl=False,
                         cur_is_accurate=env_desc["base_accurate"],
                     ),
                 )
             return (
                 env_id,
                 self._conda.resolve(
                     env_desc["steps"],
                     env_desc["deps"],
                     env_desc["sources"],
+                    env_desc["extras"],
                     env_id.arch,
                 ),
             )
 
         # NOTE: Co-resolved environments allow you to resolve a bunch of "equivalent"
         # environments for different platforms. This is great as it can allow you to
         # run code on Linux and then instantiate an environment to look at it on Mac.
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 
 import os
 import platform
 import re
 
 from enum import Enum
 from itertools import chain, product
-from typing import NamedTuple, Optional, Sequence, Tuple, Union
-from urllib.parse import urlparse
+from typing import List, NamedTuple, Optional, Sequence, Tuple, Union
+from urllib.parse import urlparse, unquote
 
-from metaflow_extensions.netflix_ext.vendor.packaging.tags import cpython_tags
+from metaflow_extensions.netflix_ext.vendor.packaging.tags import (
+    compatible_tags,
+    _cpython_abis,
+    cpython_tags,
+    Tag,
+)
 
 from metaflow.debug import debug
 from metaflow.exception import MetaflowException
 import metaflow.metaflow_config as mf_config
 from metaflow.metaflow_config import (
     CONDA_MAGIC_FILE_V2,  # type: ignore
     CONDA_PREFERRED_FORMAT,  # type: ignore
@@ -22,15 +27,15 @@
 from metaflow.metaflow_environment import InvalidEnvironmentException
 
 # NOTA: Most of the code does not assume that there are only two formats BUT the
 # transmute code does (since you can only specify the infile -- the outformat and file
 # are inferred)
 _ALL_CONDA_FORMATS = (".tar.bz2", ".conda")
 _VALID_IMAGE_NAME = "[^a-z0-9_/]"
-_VALID_TAG_NAME = "[^a-z0-9]"
+_VALID_TAG_NAME = "[^a-z0-9_]"
 
 
 class AliasType(Enum):
     PATHSPEC = "pathspec"
     FULL_ID = "full-id"
     REQ_FULL_ID = "both-id"
     GENERIC = "generic"
@@ -110,58 +115,56 @@
     else:
         raise InvalidEnvironmentException(
             "The *@conda* decorator is not supported "
             "outside of Linux and Darwin platforms"
         )
 
 
-def pip_platform_args(python_version: str, arch: str) -> Sequence[str]:
-    # Converts a Conda architecture to the arguments we pass to pip
-    # to get packages for that platform
-    py_version = tuple(map(int, python_version.split(".")))
+def pip_tags_from_arch(python_version: str, arch: str) -> List[Tag]:
+    # Converts a Conda architecture to a tuple containing (implementation, platforms, abis)
+    # This function will assume a CPython implementation
+
+    # This is inspired by what pip does:
+    # https://github.com/pypa/pip/blob/0442875a68f19b0118b0b88c747bdaf6b24853ba/src/pip/_internal/utils/compatibility_tags.py
+    py_version = tuple(map(int, python_version.split(".")[:2]))
     if arch.startswith("linux-"):
         detail = arch.split("-")[-1]
         if detail == "64":
             detail = "x86_64"
         platforms = [
             "manylinux%s_%s" % (tag, arch) for tag in ["_2_17", "2014", "2010", "1"]
         ]
-        platforms.append("linux_%s" % arch)
+        platforms.append("linux_%s" % detail)
     elif arch == "osx-64":
         platforms = [
             "macosx_10_9_x86_64",
             *("macosx_10_%s_universal2" % v for v in range(16, 3, -1)),
             *("macosx_10_%s_universal" % v for v in range(16, 3, -1)),
         ]
     elif arch == "osx-arm64":
         platforms = [
             "macosx_11_0_arm64",
             *("macosx_10_%s_universal2" % v for v in range(16, 3, -1)),
         ]
     else:
         raise InvalidEnvironmentException("Unsupported platform: %s" % arch)
 
-    platforms = []
-    # We now have all the platforms, we also need the abis for CPython.
-    abis = [
-        x
-        for x in map(lambda x: x.abi, cpython_tags(py_version, platforms=["_"]))
-        if x not in ["none", "abi3"]
-    ]
-    return [
-        "--implementation",
-        "cp",
-        *(chain.from_iterable(product(["--platform"], platforms))),
-        *(chain.from_iterable(product(["--abi"], abis))),
-    ]
+    interpreter = "cp%s" % ("".join(map(str, py_version)))
+
+    abis = _cpython_abis(py_version)
+
+    supported = []  # type: List[Tag]
+    supported.extend(cpython_tags(py_version, abis, platforms))
+    supported.extend(compatible_tags(py_version, interpreter, platforms))
+    return supported
 
 
 ParseExplicitResult = NamedTuple(
     "ParseExplicitResult",
-    [("filename", str), ("url", str), ("url_format", str), ("hash", str)],
+    [("filename", str), ("url", str), ("url_format", str), ("hash", Optional[str])],
 )
 
 
 def parse_explicit_url_conda(url: str) -> ParseExplicitResult:
     # Takes a URL in the form url#hash and returns:
     #  - the filename
     #  - the URL (without the hash)
@@ -172,25 +175,53 @@
 
     url_clean, url_hash = url.rsplit("#", 1)
 
     filename = os.path.split(urlparse(url_clean).path)[1]
     for f in _ALL_CONDA_FORMATS:
         if filename.endswith(f):
             url_format = f
-            filename = filename[: -len(f)]
+            filename = unquote(filename[: -len(f)])
             break
     else:
         raise CondaException(
             "URL '%s' is not a supported format (%s)" % (url, CONDA_FORMATS)
         )
     return ParseExplicitResult(
         filename=filename, url=url_clean, url_format=url_format, hash=url_hash
     )
 
 
+def parse_explicit_path_pip(path: str) -> ParseExplicitResult:
+    # Takes a filename in the form file://<path> and returns:
+    #  - the filename
+    #  - the URL (always file://local/<filename> so caching works across systems)
+    #  - the format of the URL
+    #  - the hash will be set to None
+    if not path.startswith("file://"):
+        raise CondaException("Local path '%s' does not start with file://" % path)
+    path = path[7:]
+    orig_filename = os.path.basename(path)
+    for f in [".whl", ".tar.gz"]:
+        if orig_filename.endswith(f):
+            url_format = f
+            filename = unquote(orig_filename[: -len(f)])
+            break
+    else:
+        raise CondaException(
+            "Path '%s' is not a supported format (%s)"
+            % (path, str([".whl", ".tar.gz"]))
+        )
+    return ParseExplicitResult(
+        filename=filename,
+        url="file://local-file/%s" % orig_filename,
+        url_format=url_format,
+        hash=None,
+    )
+
+
 def parse_explicit_url_pip(url: str) -> ParseExplicitResult:
     # Takes a URL in the form url#hash and returns:
     #  - the filename
     #  - the URL (without the hash)
     #  - the format for the URL
     #  - the hash
     filename = None
@@ -201,15 +232,15 @@
         raise CondaException("URL '%s' has a SHA type which is not supported" % url)
     url_hash = url_hash[7:]
 
     filename = os.path.split(urlparse(url_clean).path)[1]
     for f in [".whl", ".tar.gz"]:
         if filename.endswith(f):
             url_format = f
-            filename = filename[: -len(f)]
+            filename = unquote(filename[: -len(f)])
             break
     else:
         raise CondaException(
             "URL '%s' is not a supported format (%s)" % (url, str([".whl", ".tar.gz"]))
         )
     return ParseExplicitResult(
         filename=filename, url=url_clean, url_format=url_format, hash=url_hash
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.1.0rc4/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc4/setup.py` & `metaflow-netflixext-0.1.0rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.1.0rc4"
+version = "0.1.0rc5"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

