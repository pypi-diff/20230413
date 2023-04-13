# Comparing `tmp/rapyuta-io-cli-1.0.0.tar.gz` & `tmp/rapyuta-io-cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-1.0.0.tar", last modified: Tue Feb  7 11:52:41 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-2.0.0.tar", last modified: Thu Apr 13 16:22:15 2023, max compression
```

## Comparing `rapyuta-io-cli-1.0.0.tar` & `rapyuta-io-cli-2.0.0.tar`

### file list

```diff
@@ -1,202 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    15249 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    39586 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12936 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    88023 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    22851 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    12046 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3977 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    11814 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/marketplace/
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4450 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    21111 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9327 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/util.py
--rw-r--r--   0 runner    (1001) docker     (122)   159487 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    18238 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2822 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    32016 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/usergroup/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3342 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.149480 rapyuta-io-cli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-13 16:22:15.149480 rapyuta-io-cli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.121477 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4570 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-13 16:22:14.000000 rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.121477 rapyuta-io-cli-2.0.0/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.121477 rapyuta-io-cli-2.0.0/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15225 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.121477 rapyuta-io-cli-2.0.0/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.125478 rapyuta-io-cli-2.0.0/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39586 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/build/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.125478 rapyuta-io-cli-2.0.0/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.125478 rapyuta-io-cli-2.0.0/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.125478 rapyuta-io-cli-2.0.0/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.129478 rapyuta-io-cli-2.0.0/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14531 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    88023 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.129478 rapyuta-io-cli-2.0.0/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.133478 rapyuta-io-cli-2.0.0/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22851 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/device/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.133478 rapyuta-io-cli-2.0.0/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12046 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/disk/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.133478 rapyuta-io-cli-2.0.0/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.133478 rapyuta-io-cli-2.0.0/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3977 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11814 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/managedservice/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.137479 rapyuta-io-cli-2.0.0/riocli/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/marketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/marketplace/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/marketplace/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/marketplace/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/marketplace/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.137479 rapyuta-io-cli-2.0.0/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.137479 rapyuta-io-cli-2.0.0/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21111 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/network/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.137479 rapyuta-io-cli-2.0.0/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9327 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)   159487 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/package/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.141479 rapyuta-io-cli-2.0.0/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.141479 rapyuta-io-cli-2.0.0/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18238 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/project/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.141479 rapyuta-io-cli-2.0.0/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.145480 rapyuta-io-cli-2.0.0/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2822 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32016 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/secret/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.145480 rapyuta-io-cli-2.0.0/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.145480 rapyuta-io-cli-2.0.0/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/static_route/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.149480 rapyuta-io-cli-2.0.0/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/usergroup/list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:22:15.149480 rapyuta-io-cli-2.0.0/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3342 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/riocli/utils/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 16:22:15.149480 rapyuta-io-cli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-13 16:22:02.000000 rapyuta-io-cli-2.0.0/setup.py
```

### Comparing `rapyuta-io-cli-1.0.0/PKG-INFO` & `rapyuta-io-cli-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 1.0.0
+Version: 2.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-1.0.0/README.md` & `rapyuta-io-cli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 1.0.0
+Version: 2.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-2.0.0/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 riocli/chart/search.py
 riocli/chart/util.py
 riocli/completion/__init__.py
 riocli/config/__init__.py
 riocli/config/config.py
 riocli/deployment/__init__.py
 riocli/deployment/delete.py
+riocli/deployment/errors.py
 riocli/deployment/inspect.py
 riocli/deployment/list.py
 riocli/deployment/logs.py
 riocli/deployment/model.py
 riocli/deployment/run.py
 riocli/deployment/ssh.py
 riocli/deployment/status.py
@@ -122,14 +123,15 @@
 riocli/package/util.py
 riocli/package/validation.py
 riocli/parameter/__init__.py
 riocli/parameter/apply.py
 riocli/parameter/delete.py
 riocli/parameter/diff.py
 riocli/parameter/download.py
+riocli/parameter/list.py
 riocli/parameter/upload.py
 riocli/parameter/utils.py
 riocli/project/__init__.py
 riocli/project/create.py
 riocli/project/delete.py
 riocli/project/inspect.py
 riocli/project/list.py
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/__main__.py` & `rapyuta-io-cli-2.0.0/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/apply/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     click.secho("----- Files Processed ----", fg="yellow")
     for file in glob_files:
         click.secho(file, fg="yellow")
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies()
 
-    if not silent:
+    if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
     rc.apply(dryrun=dryrun, workers=workers)
 
 
 @click.command(
     'delete',
@@ -86,11 +86,11 @@
     if len(glob_files) == 0:
         click.secho('no files specified', fg='red')
         raise SystemExit(1)
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies(check_missing=False, delete=True)
 
-    if not silent:
+    if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
     rc.delete(dryrun=dryrun)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/explain.py` & `rapyuta-io-cli-2.0.0/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/parse.py` & `rapyuta-io-cli-2.0.0/riocli/apply/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,46 +85,48 @@
                                 or self.DEFAULT_MAX_WORKERS)
         if kwargs['workers'] == 1:
             return self.apply_sync(*args, **kwargs)
 
         return self.apply_async(*args, **kwargs)
 
     def apply_async(self, *args, **kwargs):
-        WORKERS = int(kwargs.get('workers') or self.DEFAULT_MAX_WORKERS)
+        workers = int(kwargs.get('workers') or self.DEFAULT_MAX_WORKERS)
         task_queue = queue.Queue()
         done_queue = queue.Queue()
 
         def worker():
             while True:
-                obj = task_queue.get()
-                if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
-                    # click.secho("obj {} is being aplied".format(obj))
+                o = task_queue.get()
+                if o in self.resolved_objects and 'manifest' in self.resolved_objects[o]:
                     try:
-                        self._apply_manifest(obj, *args, **kwargs)
+                        self._apply_manifest(o, *args, **kwargs)
                     except Exception as ex:
                         click.secho(
-                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(obj, str(ex)))
-                        raise ex
+                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(o, str(ex)))
+                        done_queue.put(ex)
+                        continue
 
                 task_queue.task_done()
-                done_queue.put(obj)
+                done_queue.put(o)
 
         worker_list = []
-        for worker_id in range(0, WORKERS):
+        for worker_id in range(workers):
             worker_list.append(threading.Thread(target=worker, daemon=True))
             worker_list[worker_id].start()
 
         self.graph.prepare()
         while self.graph.is_active():
             for obj in self.graph.get_ready():
-                # if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
                 task_queue.put(obj)
 
             done_obj = done_queue.get()
-            self.graph.done(done_obj)
+            if not isinstance(done_obj, Exception):
+                self.graph.done(done_obj)
+            else:
+                raise Exception(done_obj)
 
         task_queue.join()
 
     def apply_sync(self, *args, **kwargs):
         self.graph.prepare()
         while self.graph.is_active():
             for obj in self.graph.get_ready():
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/resolver.py` & `rapyuta-io-cli-2.0.0/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/template.py` & `rapyuta-io-cli-2.0.0/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/util.py` & `rapyuta-io-cli-2.0.0/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/login.py` & `rapyuta-io-cli-2.0.0/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/logout.py` & `rapyuta-io-cli-2.0.0/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/refresh_token.py` & `rapyuta-io-cli-2.0.0/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/staging.py` & `rapyuta-io-cli-2.0.0/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/status.py` & `rapyuta-io-cli-2.0.0/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/token.py` & `rapyuta-io-cli-2.0.0/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/util.py` & `rapyuta-io-cli-2.0.0/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/bootstrap.py` & `rapyuta-io-cli-2.0.0/riocli/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.0"
+__version__ = "2.0.0"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/create.py` & `rapyuta-io-cli-2.0.0/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/delete.py` & `rapyuta-io-cli-2.0.0/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/import_build.py` & `rapyuta-io-cli-2.0.0/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/list.py` & `rapyuta-io-cli-2.0.0/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/logs.py` & `rapyuta-io-cli-2.0.0/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/model.py` & `rapyuta-io-cli-2.0.0/riocli/build/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/trigger.py` & `rapyuta-io-cli-2.0.0/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/util.py` & `rapyuta-io-cli-2.0.0/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/validation.py` & `rapyuta-io-cli-2.0.0/riocli/build/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/apply.py` & `rapyuta-io-cli-2.0.0/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/chart.py` & `rapyuta-io-cli-2.0.0/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/delete.py` & `rapyuta-io-cli-2.0.0/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/search.py` & `rapyuta-io-cli-2.0.0/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/util.py` & `rapyuta-io-cli-2.0.0/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/completion/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/config/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/config/config.py` & `rapyuta-io-cli-2.0.0/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/delete.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/list.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/logs.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/model.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
+import sys
 import typing
 
 import click
 from rapyuta_io import Client
 from rapyuta_io.clients.catalog_client import Package
+from rapyuta_io.clients.deployment import DeploymentNotRunningException
 from rapyuta_io.clients.native_network import NativeNetwork
 from rapyuta_io.clients.package import ProvisionConfiguration, RestartPolicy, ExecutableMount
 from rapyuta_io.clients.rosbag import ROSBagJob, ROSBagOptions, ROSBagCompression, UploadOptions, \
     ROSBagOnDemandUploadOptions, ROSBagTimeRange, ROSBagUploadTypes, OverrideOptions, TopicOverrideInfo
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
+from riocli.deployment.errors import ERRORS
 from riocli.deployment.util import add_mount_volume_provision_config
 from riocli.deployment.validation import validate
 from riocli.model import Model
 from riocli.package.util import find_package_guid
 from riocli.static_route.util import find_static_route_guid
 
 
@@ -136,15 +139,15 @@
                     })
                 provision_config.context["managedServices"] = managed_services
 
         if self.spec.runtime == 'device':
             device_guid, device = self.rc.find_depends(self.spec.device.depends)
             if device is None and device_guid:
                 device = client.get_device(device_guid)
-            provision_config.add_device(__componentName, device=device)
+            provision_config.add_device(__componentName, device=device, set_component_alias=False)
 
             if 'restart' in self.spec:
                 provision_config.add_restart_policy(__componentName, self.RESTART_POLICY[self.spec.restart.lower()])
 
             # Add Network
             # if self.spec.rosNetworks:
             # for network in self.spec.rosNetworks:
@@ -155,18 +158,27 @@
             if 'volumes' in self.spec:
                 for vol in self.spec.volumes:
                     exec_mounts.append(ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
             if len(exec_mounts) > 0:
                 provision_config = add_mount_volume_provision_config(provision_config, __componentName, device,
                                                                      exec_mounts)
 
+        provision_config.set_component_alias(__componentName, self.metadata.name)
+
         if os.environ.get('DEBUG'):
             print(provision_config)
         deployment = pkg.provision(self.metadata.name, provision_config)
-        deployment.poll_deployment_till_ready()
+
+        try:
+            deployment.poll_deployment_till_ready()
+        except DeploymentNotRunningException as e:
+            raise Exception(process_deployment_errors(e)) from e
+        except Exception as e:
+            raise e
+
         deployment.get_status()
         return deployment
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         if 'depends' in self.spec:
             pass
         pass
@@ -299,7 +311,38 @@
 
             override_options_kw_args['topic_override_info'] = override_infos
 
         if 'excludeTopics' in override_options:
             override_options_kw_args['exclude_topics'] = override_options.excludeTopics
 
         return OverrideOptions(**override_options_kw_args)
+
+
+def process_deployment_errors(e: DeploymentNotRunningException):
+    errors = e.deployment_status.errors
+    err_fmt = "[{}] {}\nAction: {}"
+    support_action = ('Report the issue together with the relevant'
+                      ' details to the support team')
+
+    action, description = "", ""
+    msgs = []
+    for code in errors:
+        if code in ERRORS:
+            description = ERRORS[code]['description']
+            action = ERRORS[code]['action']
+        elif code.startswith('DEP_E2'):
+            description = 'Internal rapyuta.io error in the components deployed on cloud'
+            action = support_action
+        elif code.startswith('DEP_E3'):
+            description = 'Internal rapyuta.io error in the components deployed on a device'
+            action = support_action
+        elif code.startswith('DEP_E4'):
+            description = 'Internal rapyuta.io error'
+            action = support_action
+
+        code = click.style(code, fg='yellow')
+        description = click.style(description, fg='red')
+        action = click.style(action, fg='green')
+
+        msgs.append(err_fmt.format(code, description, action))
+
+    return "\n".join(msgs)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/run.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/run.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/ssh.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/status.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/util.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/validation.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/wait.py` & `rapyuta-io-cli-2.0.0/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/config.py` & `rapyuta-io-cli-2.0.0/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/create.py` & `rapyuta-io-cli-2.0.0/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/delete.py` & `rapyuta-io-cli-2.0.0/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/deployment.py` & `rapyuta-io-cli-2.0.0/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/execute.py` & `rapyuta-io-cli-2.0.0/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/files.py` & `rapyuta-io-cli-2.0.0/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/label.py` & `rapyuta-io-cli-2.0.0/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/list.py` & `rapyuta-io-cli-2.0.0/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/metric.py` & `rapyuta-io-cli-2.0.0/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/model.py` & `rapyuta-io-cli-2.0.0/riocli/device/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/onboard.py` & `rapyuta-io-cli-2.0.0/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/device_init.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/forward.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/scp.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/service.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/ssh.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/util.py` & `rapyuta-io-cli-2.0.0/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/topic.py` & `rapyuta-io-cli-2.0.0/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/util.py` & `rapyuta-io-cli-2.0.0/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/validation.py` & `rapyuta-io-cli-2.0.0/riocli/device/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/create.py` & `rapyuta-io-cli-2.0.0/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/delete.py` & `rapyuta-io-cli-2.0.0/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/list.py` & `rapyuta-io-cli-2.0.0/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/model.py` & `rapyuta-io-cli-2.0.0/riocli/disk/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/util.py` & `rapyuta-io-cli-2.0.0/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/validation.py` & `rapyuta-io-cli-2.0.0/riocli/disk/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/exceptions/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/list.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/model.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/util.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/validation.py` & `rapyuta-io-cli-2.0.0/riocli/managedservice/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/marketplace/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/install.py` & `rapyuta-io-cli-2.0.0/riocli/marketplace/install.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/list.py` & `rapyuta-io-cli-2.0.0/riocli/marketplace/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/util.py` & `rapyuta-io-cli-2.0.0/riocli/marketplace/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/model/base.py` & `rapyuta-io-cli-2.0.0/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/create.py` & `rapyuta-io-cli-2.0.0/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/delete.py` & `rapyuta-io-cli-2.0.0/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/list.py` & `rapyuta-io-cli-2.0.0/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/logs.py` & `rapyuta-io-cli-2.0.0/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/model.py` & `rapyuta-io-cli-2.0.0/riocli/network/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,20 @@
             network, _ = find_network_name(client, self.metadata.name, self.spec.type, is_resolve_conflict=False)
             return network
         except NetworkNotFound:
             return False
 
     def create_object(self, client: Client) -> Union[NativeNetwork, RoutedNetwork]:
         if self.spec.type == 'routed':
-            return self._create_routed_network(client)
+            network = self._create_routed_network(client)
+            network.poll_routed_network_till_ready()
+            return network
 
         network = client.create_native_network(self.to_v1(client))
+        network.poll_native_network_till_ready()
         return network
 
     def update_object(self, client: Client, obj: Union[RoutedNetwork, NativeNetwork]) -> Any:
         # try:
         #     obj.delete()
         #     self.create_object(client)
         # except Exception as e:
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/native_network.py` & `rapyuta-io-cli-2.0.0/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/routed_network.py` & `rapyuta-io-cli-2.0.0/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/util.py` & `rapyuta-io-cli-2.0.0/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/validation.py` & `rapyuta-io-cli-2.0.0/riocli/network/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/create.py` & `rapyuta-io-cli-2.0.0/riocli/package/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/delete.py` & `rapyuta-io-cli-2.0.0/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/deployment.py` & `rapyuta-io-cli-2.0.0/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/list.py` & `rapyuta-io-cli-2.0.0/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/model.py` & `rapyuta-io-cli-2.0.0/riocli/package/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/util.py` & `rapyuta-io-cli-2.0.0/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/validation.py` & `rapyuta-io-cli-2.0.0/riocli/package/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/parameter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-# Copyright 2021 Rapyuta Robotics
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import click
-from click_help_colors import HelpColorsGroup
-
-from riocli.parameter.apply import apply_configurations
-from riocli.parameter.diff import diff_configurations
-from riocli.parameter.download import download_configurations
-from riocli.parameter.upload import upload_configurations
-
-
-# from riocli.parameter.diff import diff_configurations
-# from riocli.parameter.download import download_configurations
-
-
-@click.group(
-    invoke_without_command=False,
-    cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
-)
-def parameter() -> None:
-    """
-    Define groups of executables to deploy together
-    """
-    pass
-
-
-parameter.add_command(upload_configurations)
-parameter.add_command(download_configurations)
-parameter.add_command(diff_configurations)
-parameter.add_command(apply_configurations)
+# Copyright 2023 Rapyuta Robotics
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import click
+from click_help_colors import HelpColorsGroup
+
+from riocli.parameter.apply import apply_configurations
+from riocli.parameter.delete import delete_configurations
+from riocli.parameter.diff import diff_configurations
+from riocli.parameter.download import download_configurations
+from riocli.parameter.list import list_configuration_trees
+from riocli.parameter.upload import upload_configurations
+
+
+# from riocli.parameter.diff import diff_configurations
+# from riocli.parameter.download import download_configurations
+
+
+@click.group(
+    invoke_without_command=False,
+    cls=HelpColorsGroup,
+    help_headers_color='yellow',
+    help_options_color='green',
+)
+def parameter() -> None:
+    """
+    Define groups of executables to deploy together
+    """
+    pass
+
+
+parameter.add_command(upload_configurations)
+parameter.add_command(download_configurations)
+parameter.add_command(diff_configurations)
+parameter.add_command(apply_configurations)
+parameter.add_command(list_configuration_trees)
+parameter.add_command(delete_configurations)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/apply.py` & `rapyuta-io-cli-2.0.0/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/delete.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/create.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import click
+from click_spinner import spinner
 
 from riocli.config import new_client
 
 
-@click.command('delete')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
-              help='Directory names to upload')
-def delete_configurations(tree_names: str = None) -> None:
+@click.command('create')
+@click.argument('prefix', type=str)
+def create_static_route(prefix: str) -> None:
     """
-    Upload a set of configurations to IO.
-
-    Compile the IO configurations from the paths provided. Output to a temporary directory. Upload the directory.
+    Creates a new instance of static route
     """
     try:
         client = new_client()
-        pass
-    except IOError as e:
-        click.secho(str(e.__traceback__), fg='red')
+        with spinner():
+            route = client.create_static_route(prefix)
+        click.secho("Static Route created successfully for URL {}".format(route.urlString), fg='green')
+    except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/download.py` & `rapyuta-io-cli-2.0.0/riocli/parameter/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-# Copyright 2021 Rapyuta Robotics
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-# -----------------------------------------------------------------------------
-#
-# Configurations
-# Args
-#    path,  tree_names,  delete_existing=True|False
-# -----------------------------------------------------------------------------
-
-from tempfile import mkdtemp
-from typing import Tuple
-from xmlrpc.client import Boolean
-
-import click
-from rapyuta_io.utils.error import APIError, InternalServerError
-
-from riocli.config import new_client
-
-
-@click.command('download')
-@click.option('--path', type=click.Path(dir_okay=True, file_okay=False, writable=True, exists=True, resolve_path=True),
-              default=["."],
-              help='Root Path for the Parameters to be download')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
-              help='Tree names to fetch')
-@click.option('--delete-existing', is_flag=True,
-              help='Overwrite existing parameter tree')
-def download_configurations(path: click.Path, tree_names: Tuple = None, delete_existing: Boolean = False) -> None:
-    """
-    Download the configurations
-    """
-    if path is None:
-        path = mkdtemp()  # Temporary directory to hold the configurations
-
-    tree_names = list(tree_names)
-
-    try:
-        client = new_client()
-
-        client.download_configurations(str(path), tree_names=tree_names, delete_existing_trees=delete_existing)
-
-    except (APIError, InternalServerError) as e:
-        click.secho(f"failed API request {str(e)}", fg='red')
-        raise SystemExit(1)
-    except (IOError, OSError) as e:
-        click.secho(f"failed file/directory creation {str(e)}", fg='red')
-        raise SystemExit(1)
-
-    click.secho("Downloaded IO configurations to '{}'".format(path), fg='green')
-    return path
+# Copyright 2023 Rapyuta Robotics
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import typing
+from tempfile import mkdtemp
+from xmlrpc.client import Boolean
+
+import click
+from click_spinner import spinner
+
+from riocli.config import new_client
+from riocli.parameter.utils import display_trees
+
+
+# -----------------------------------------------------------------------------
+#
+# Configurations
+# Args
+#    path,  tree_names,  delete_existing=True|False
+# -----------------------------------------------------------------------------
+
+
+@click.command('download')
+@click.option('--tree-names', type=click.STRING, multiple=True, default=None, help='Tree names to fetch')
+@click.option('--overwrite', '--delete-existing', 'delete_existing', is_flag=True,
+              help='Overwrite existing parameter tree')
+@click.argument('path', type=click.Path(exists=True), required=False)
+def download_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: Boolean = False) -> None:
+    """
+    Download the Configuration Parameter trees.
+    """
+    if path is None:
+        # Not using the Context Manager because we need to persist the Temporary directory.
+        path = mkdtemp()
+
+    click.secho('Downloading at {}'.format(path))
+
+    try:
+        client = new_client()
+
+        with spinner():
+            client.download_configurations(path, tree_names=list(tree_names),
+                                           delete_existing_trees=delete_existing)
+
+        click.secho('✅ Configuration Parameters downloaded successfully', fg='green')
+    except Exception as e:
+        click.secho(e, fg='red')
+        raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/create.py` & `rapyuta-io-cli-2.0.0/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/delete.py` & `rapyuta-io-cli-2.0.0/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/list.py` & `rapyuta-io-cli-2.0.0/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/model.py` & `rapyuta-io-cli-2.0.0/riocli/project/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/select.py` & `rapyuta-io-cli-2.0.0/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/util.py` & `rapyuta-io-cli-2.0.0/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/validation.py` & `rapyuta-io-cli-2.0.0/riocli/project/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/blob.py` & `rapyuta-io-cli-2.0.0/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/job.py` & `rapyuta-io-cli-2.0.0/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/create.py` & `rapyuta-io-cli-2.0.0/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/delete.py` & `rapyuta-io-cli-2.0.0/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/docker_secret.py` & `rapyuta-io-cli-2.0.0/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/import_secret.py` & `rapyuta-io-cli-2.0.0/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/list.py` & `rapyuta-io-cli-2.0.0/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/model.py` & `rapyuta-io-cli-2.0.0/riocli/secret/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/source_secret.py` & `rapyuta-io-cli-2.0.0/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/util.py` & `rapyuta-io-cli-2.0.0/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/validation.py` & `rapyuta-io-cli-2.0.0/riocli/secret/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/shell/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/shell/prompt.py` & `rapyuta-io-cli-2.0.0/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/create.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/open.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from click_spinner import spinner
 
 from riocli.config import new_client
+from riocli.static_route.util import name_to_guid
 
 
-@click.command('create')
-@click.argument('prefix', type=str)
-def create_static_route(prefix: str) -> None:
+@click.command('open')
+@click.argument('static-route', type=str)
+@name_to_guid
+def open_static_route(static_route, static_route_guid) -> None:
     """
-    Creates a new instance of static route
+    Opens the static route in the default browser
     """
     try:
         client = new_client()
-        with spinner():
-            route = client.create_static_route(prefix)
-        click.secho("Static Route created successfully for URL {}".format(route.urlString), fg='green')
+        route = client.get_static_route(static_route_guid)
+        click.launch(url='https://{}'.format(route.urlString), wait=False)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/delete.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/inspect.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/list.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/model.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/open.py` & `rapyuta-io-cli-2.0.0/riocli/parameter/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
+from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.config import new_client
-from riocli.static_route.util import name_to_guid
+from riocli.parameter.utils import _api_call
+from riocli.utils import tabulate_data
 
 
-@click.command('open')
-@click.argument('static-route', type=str)
-@name_to_guid
-def open_static_route(static_route, static_route_guid) -> None:
+@click.command('list')
+def list_configuration_trees() -> None:
     """
-    Opens the static route in the default browser
+    List the Configuration Parameter Trees.
     """
     try:
-        client = new_client()
-        route = client.get_static_route(static_route_guid)
-        click.launch(url='https://{}'.format(route.urlString), wait=False)
+        data = _api_call(HttpMethod.GET)
+        if 'data' not in data:
+            raise Exception('Something went wrong!')
+
+        trees = [[tree] for tree in data['data']]
+
+        tabulate_data(trees, headers=['Tree Name'])
+
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/util.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/validation.py` & `rapyuta-io-cli-2.0.0/riocli/static_route/validation.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/__init__.py` & `rapyuta-io-cli-2.0.0/riocli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/context.py` & `rapyuta-io-cli-2.0.0/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/execute.py` & `rapyuta-io-cli-2.0.0/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/mermaid.py` & `rapyuta-io-cli-2.0.0/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/selector.py` & `rapyuta-io-cli-2.0.0/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-2.0.0/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/setup.py` & `rapyuta-io-cli-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
-
 """setup.py: setuptools control."""
 
-
 import re
-from setuptools import setup, find_packages
 
+from setuptools import setup, find_packages
 
 version = re.search(
     '^__version__\s*=\s*"(.*)"', open("riocli/bootstrap.py").read(), re.M
 ).group(1)
 
 
 with open("README.md", "rb") as f:
@@ -53,11 +51,12 @@
         "pyyaml>=5.4.1",
         "rapyuta-io>=1.8.0",
         "requests>=2.20.0",
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
-        "pyrfc3339>=1.1"
+        "pyrfc3339>=1.1",
+        "directory-tree>=0.0.3.1"
     ],
     setup_requires=["flake8"],
 )
```

