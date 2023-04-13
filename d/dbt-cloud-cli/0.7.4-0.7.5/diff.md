# Comparing `tmp/dbt-cloud-cli-0.7.4.tar.gz` & `tmp/dbt-cloud-cli-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-cloud-cli-0.7.4.tar", last modified: Thu Feb  9 11:58:47 2023, max compression
+gzip compressed data, was "dbt-cloud-cli-0.7.5.tar", last modified: Thu Apr 13 05:30:38 2023, max compression
```

## Comparing `dbt-cloud-cli-0.7.4.tar` & `dbt-cloud-cli-0.7.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/
--rw-r--r--   0 simo      (1000) simo      (1000)    11342 2021-12-07 10:27:17.000000 dbt-cloud-cli-0.7.4/LICENSE
--rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/PKG-INFO
--rw-r--r--   0 simo      (1000) simo      (1000)    50430 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.4/README.md
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/
--rw-r--r--   0 simo      (1000) simo      (1000)       39 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.4/dbt_cloud/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)    12765 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.4/dbt_cloud/cli.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/
--rw-r--r--   0 simo      (1000) simo      (1000)      715 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/__init__.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/account/
--rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:09:18.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/account/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      336 2022-07-14 08:25:40.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/account/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      407 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/account/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/audit_log/
--rw-r--r--   0 simo      (1000) simo      (1000)       44 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/audit_log/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1250 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/audit_log/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)     3923 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/command.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/environment/
--rw-r--r--   0 simo      (1000) simo      (1000)       49 2022-03-25 16:24:22.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/environment/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      632 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/environment/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/
--rw-r--r--   0 simo      (1000) simo      (1000)      209 2022-01-27 08:25:48.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     3157 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/create.py
--rw-r--r--   0 simo      (1000) simo      (1000)      547 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/delete.py
--rw-r--r--   0 simo      (1000) simo      (1000)      782 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      795 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/list.py
--rw-r--r--   0 simo      (1000) simo      (1000)     2169 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/job/run.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/metadata/
--rw-r--r--   0 simo      (1000) simo      (1000)       48 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/metadata/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      700 2022-05-17 07:10:38.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/metadata/query.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/project/
--rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/project/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      529 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/project/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      429 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/project/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/
--rw-r--r--   0 simo      (1000) simo      (1000)      260 2022-03-14 13:54:59.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      661 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/cancel.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1049 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1112 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/get_artifact.py
--rw-r--r--   0 simo      (1000) simo      (1000)     2344 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/list.py
--rw-r--r--   0 simo      (1000) simo      (1000)      859 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.4/dbt_cloud/command/run/list_artifacts.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud/demo/
--rw-r--r--   0 simo      (1000) simo      (1000)       34 2022-02-09 20:32:20.000000 dbt-cloud-cli-0.7.4/dbt_cloud/demo/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     4886 2022-02-13 13:33:26.000000 dbt-cloud-cli-0.7.4/dbt_cloud/demo/catalog.py
--rw-r--r--   0 simo      (1000) simo      (1000)       45 2021-12-07 10:42:57.000000 dbt-cloud-cli-0.7.4/dbt_cloud/exc.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1814 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.4/dbt_cloud/field.py
--rw-r--r--   0 simo      (1000) simo      (1000)      160 2021-12-25 10:54:57.000000 dbt-cloud-cli-0.7.4/dbt_cloud/serde.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/
--rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 simo      (1000) simo      (1000)     1376 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 simo      (1000) simo      (1000)        1 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       55 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 simo      (1000) simo      (1000)      124 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       10 2023-02-09 11:58:46.000000 dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/top_level.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       90 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.4/pyproject.toml
--rw-r--r--   0 simo      (1000) simo      (1000)       38 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/setup.cfg
--rw-r--r--   0 simo      (1000) simo      (1000)     1062 2023-02-09 11:58:36.000000 dbt-cloud-cli-0.7.4/setup.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-02-09 11:58:47.072015 dbt-cloud-cli-0.7.4/tests/
--rw-r--r--   0 simo      (1000) simo      (1000)        0 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.4/tests/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     6282 2023-02-09 11:53:22.000000 dbt-cloud-cli-0.7.4/tests/conftest.py
--rw-r--r--   0 simo      (1000) simo      (1000)      896 2022-01-12 16:57:47.000000 dbt-cloud-cli-0.7.4/tests/test_command.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1229 2022-03-25 17:06:38.000000 dbt-cloud-cli-0.7.4/tests/test_job.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/
+-rw-r--r--   0 simo      (1000) simo      (1000)    11342 2021-12-07 10:27:17.000000 dbt-cloud-cli-0.7.5/LICENSE
+-rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/PKG-INFO
+-rw-r--r--   0 simo      (1000) simo      (1000)    50430 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.5/README.md
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/
+-rw-r--r--   0 simo      (1000) simo      (1000)       39 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.5/dbt_cloud/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)    12820 2023-04-13 05:30:17.000000 dbt-cloud-cli-0.7.5/dbt_cloud/cli.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/
+-rw-r--r--   0 simo      (1000) simo      (1000)      715 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/__init__.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/account/
+-rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:09:18.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/account/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      336 2022-07-14 08:25:40.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/account/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      407 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/account/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/audit_log/
+-rw-r--r--   0 simo      (1000) simo      (1000)       44 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/audit_log/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1250 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/audit_log/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     3923 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/command.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/environment/
+-rw-r--r--   0 simo      (1000) simo      (1000)       49 2022-03-25 16:24:22.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/environment/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      632 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/environment/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/
+-rw-r--r--   0 simo      (1000) simo      (1000)      209 2022-01-27 08:25:48.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     3157 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/create.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      547 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/delete.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      782 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      795 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/list.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     2169 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/job/run.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/metadata/
+-rw-r--r--   0 simo      (1000) simo      (1000)       48 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/metadata/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      700 2022-05-17 07:10:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/metadata/query.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.414997 dbt-cloud-cli-0.7.5/dbt_cloud/command/project/
+-rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/project/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      529 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/project/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      429 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/project/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/
+-rw-r--r--   0 simo      (1000) simo      (1000)      260 2022-03-14 13:54:59.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      661 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/cancel.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1049 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1112 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/get_artifact.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     2344 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/list.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      859 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.5/dbt_cloud/command/run/list_artifacts.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/dbt_cloud/demo/
+-rw-r--r--   0 simo      (1000) simo      (1000)       34 2022-02-09 20:32:20.000000 dbt-cloud-cli-0.7.5/dbt_cloud/demo/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     4886 2022-02-13 13:33:26.000000 dbt-cloud-cli-0.7.5/dbt_cloud/demo/catalog.py
+-rw-r--r--   0 simo      (1000) simo      (1000)       45 2021-12-07 10:42:57.000000 dbt-cloud-cli-0.7.5/dbt_cloud/exc.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1814 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.5/dbt_cloud/field.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      160 2021-12-25 10:54:57.000000 dbt-cloud-cli-0.7.5/dbt_cloud/serde.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/
+-rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 simo      (1000) simo      (1000)     1376 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)        1 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       55 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)      124 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       10 2023-04-13 05:30:38.000000 dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       90 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.5/pyproject.toml
+-rw-r--r--   0 simo      (1000) simo      (1000)       38 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/setup.cfg
+-rw-r--r--   0 simo      (1000) simo      (1000)     1062 2023-04-13 05:30:25.000000 dbt-cloud-cli-0.7.5/setup.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-04-13 05:30:38.424997 dbt-cloud-cli-0.7.5/tests/
+-rw-r--r--   0 simo      (1000) simo      (1000)        0 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.5/tests/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     6282 2023-02-09 11:53:22.000000 dbt-cloud-cli-0.7.5/tests/conftest.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      896 2022-01-12 16:57:47.000000 dbt-cloud-cli-0.7.5/tests/test_command.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1229 2022-03-25 17:06:38.000000 dbt-cloud-cli-0.7.5/tests/test_job.py
```

### Comparing `dbt-cloud-cli-0.7.4/LICENSE` & `dbt-cloud-cli-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/PKG-INFO` & `dbt-cloud-cli-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-cloud-cli
-Version: 0.7.4
+Version: 0.7.5
 Summary: dbt Cloud command line interface (CLI)
 Home-page: https://github.com/data-mie/dbt-cloud-cli
 Author: Simo Tumelius
 Author-email: simo@datamie.fi
 License: Apache Software License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-cloud-cli-0.7.4/README.md` & `dbt-cloud-cli-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/cli.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
     if wait:
         run_id = response.json()["data"]["id"]
         while True:
             run_get_command = DbtCloudRunGetCommand(
                 api_token=command.api_token,
                 account_id=command.account_id,
+                dbt_cloud_host=command.dbt_cloud_host,
                 run_id=run_id,
             )
             response = run_get_command.execute()
             status = DbtCloudRunStatus(response.json()["data"]["status"])
             click.echo(f"Job {command.job_id} run {run_id}: {status.name} ...")
             if status == DbtCloudRunStatus.SUCCESS:
                 break
```

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/__init__.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/audit_log/get.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/audit_log/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/command.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/command.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/environment/list.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/environment/list.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/job/create.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/job/create.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/job/delete.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/job/delete.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/job/get.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/job/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/job/list.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/job/list.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/job/run.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/job/run.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/metadata/query.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/metadata/query.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/project/get.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/project/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/run/cancel.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/run/cancel.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/run/get.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/run/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/run/get_artifact.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/run/get_artifact.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/run/list.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/run/list.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/command/run/list_artifacts.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/command/run/list_artifacts.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/demo/catalog.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/demo/catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud/field.py` & `dbt-cloud-cli-0.7.5/dbt_cloud/field.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/PKG-INFO` & `dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-cloud-cli
-Version: 0.7.4
+Version: 0.7.5
 Summary: dbt Cloud command line interface (CLI)
 Home-page: https://github.com/data-mie/dbt-cloud-cli
 Author: Simo Tumelius
 Author-email: simo@datamie.fi
 License: Apache Software License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt-cloud-cli-0.7.4/dbt_cloud_cli.egg-info/SOURCES.txt` & `dbt-cloud-cli-0.7.5/dbt_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/setup.py` & `dbt-cloud-cli-0.7.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 README = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="dbt-cloud-cli",
-    version="0.7.4",
+    version="0.7.5",
     description="dbt Cloud command line interface (CLI)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/data-mie/dbt-cloud-cli",
     author="Simo Tumelius",
     author_email="simo@datamie.fi",
     license="Apache Software License",
```

### Comparing `dbt-cloud-cli-0.7.4/tests/conftest.py` & `dbt-cloud-cli-0.7.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/tests/test_command.py` & `dbt-cloud-cli-0.7.5/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.4/tests/test_job.py` & `dbt-cloud-cli-0.7.5/tests/test_job.py`

 * *Files identical despite different names*

