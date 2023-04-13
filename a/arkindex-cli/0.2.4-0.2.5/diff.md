# Comparing `tmp/arkindex-cli-0.2.4.tar.gz` & `tmp/arkindex-cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-cli-0.2.4.tar", last modified: Mon Feb 27 15:43:39 2023, max compression
+gzip compressed data, was "arkindex-cli-0.2.5.tar", last modified: Thu Apr 13 08:33:32 2023, max compression
```

## Comparing `arkindex-cli-0.2.4.tar` & `arkindex-cli-0.2.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1342 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.910019 arkindex-cli-0.2.4/arkindex_cli/
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/argtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     4208 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2369 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.910019 arkindex-cli-0.2.4/arkindex_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/elements/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8629 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/list.py
--rw-rw-rw-   0 root         (0) root         (0)    13082 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/ml_splits.py
--rw-rw-rw-   0 root         (0) root         (0)     4654 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/page_copy.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/reject_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/unlink.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/elements/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/export/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18108 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/alto.py
--rw-rw-rw-   0 root         (0) root         (0)     9285 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    30744 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/db.py
--rw-rw-rw-   0 root         (0) root         (0)     2592 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/entities.py
--rw-rw-rw-   0 root         (0) root         (0)    11589 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/export/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/models/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/models/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     8297 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/process/
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6684 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/process/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/process/recover.py
--rw-rw-rw-   0 root         (0) root         (0)     3049 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/process/report.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/upload/
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/arkindex_cli/commands/upload/alto/
--rw-rw-rw-   0 root         (0) root         (0)    20020 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/alto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6647 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/alto/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     9303 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/iiif.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/minio_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8060 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/commands/upload/page_xml_import.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/arkindex_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:43:39.910019 arkindex-cli-0.2.4/arkindex_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1751 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-27 15:43:39.000000 arkindex-cli-0.2.4/arkindex_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/requirements-export.txt
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/requirements-tests.txt
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 15:43:39.914019 arkindex-cli-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-02-27 15:42:47.000000 arkindex-cli-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-13 08:30:48.000000 arkindex-cli-0.2.5/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.656972 arkindex-cli-0.2.5/arkindex_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/argtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4208 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2369 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.656972 arkindex-cli-0.2.5/arkindex_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.656972 arkindex-cli-0.2.5/arkindex_cli/commands/elements/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8629 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    13082 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/ml_splits.py
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/page_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/reject_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/unlink.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/elements/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/arkindex_cli/commands/export/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18108 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/alto.py
+-rw-rw-rw-   0 root         (0) root         (0)     9285 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    30744 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     2592 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/export/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/arkindex_cli/commands/models/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4060 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/models/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/arkindex_cli/commands/process/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/process/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/process/recover.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/process/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/arkindex_cli/commands/upload/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/arkindex_cli/commands/upload/alto/
+-rw-rw-rw-   0 root         (0) root         (0)    24164 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/alto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16784 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/alto/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9303 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/iiif.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/minio_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8060 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/commands/upload/page_xml_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/arkindex_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:33:32.656972 arkindex-cli-0.2.5/arkindex_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 08:33:32.000000 arkindex-cli-0.2.5/arkindex_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/requirements-export.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/requirements-tests.txt
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-13 08:26:58.000000 arkindex-cli-0.2.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 08:33:32.660972 arkindex-cli-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-04-13 08:01:03.000000 arkindex-cli-0.2.5/setup.py
```

### Comparing `arkindex-cli-0.2.4/PKG-INFO` & `arkindex-cli-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: export
 
 # Arkindex CLI
 
 Documentation for users is available in the [docs](./docs) folder, and online as [cli.arkindex.org](https://cli.arkindex.org).
```

### Comparing `arkindex-cli-0.2.4/README.md` & `arkindex-cli-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/argtypes.py` & `arkindex-cli-0.2.5/arkindex_cli/argtypes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/auth.py` & `arkindex-cli-0.2.5/arkindex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/cli.py` & `arkindex-cli-0.2.5/arkindex_cli/cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/benchmark.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/benchmark.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/classes.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/classes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/link.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/link.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/list.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/list.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/ml_splits.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/ml_splits.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/page_copy.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/page_copy.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/reject_classifications.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/reject_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/unlink.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/unlink.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/elements/utils.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/elements/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/alto.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/alto.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/csv.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/csv.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/db.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/db.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/entities.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/pdf.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     **kwargs,
 ) -> None:
     """
     Gets the database path, argument from cli, path to the generated pdf and the
     temporary directory where to find downloaded images
     """
 
-    assert DEPS_AVAILABLE, "Missing PDF export dependencies"
+    assert (
+        DEPS_AVAILABLE
+    ), "Missing PDF export dependencies. Run `pip install arkindex-cli[export]` to install them."
 
     # creating temporary directory
     temp_dir = Path(tempfile.mkdtemp())
     logger.info(f"created temporary directory: {temp_dir}")
 
     # chooses color depending on debug option
     selected_color = colors.transparent
```

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/export/utils.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/export/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/login.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/models/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/models/publish.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/models/publish.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             size=size,
             hash=hash,
             archive_hash=archive_hash,
         )
 
     if valid_version["id"] != model_version["id"]:
         logger.warning(
-            f"Model version {model_version['id']} has been marked as erroneous and left aside."
+            f"Model version {model_version['id']} has been marked as erroneous and left aside. "
             f"Using existing model version {valid_version['id']}"
         )
 
 
 def run(
     use_parent_folder: bool = False,
     rename: Optional[str] = None,
@@ -118,12 +118,13 @@
             publish_model(
                 client,
                 worker_name,
                 worker_configuration,
                 use_parent_folder=use_parent_folder,
                 rename=rename,
             )
-        except Exception:
-            logger.exception(f"{worker_name} publishing has failed with error")
+        except Exception as e:
+            msg = getattr(e, "content", repr(e))
+            logger.exception(f"{worker_name} publishing has failed with error: {msg}")
             logger.error("Skipping this model.")
 
     logger.info("All done.")
```

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/models/utils.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,10 +244,28 @@
             id=model_version_id,
             body={"size": size, "hash": hash, "archive_hash": archive_hash},
         )
     except ErrorResponse as e:
         msg = getattr(e, "content", repr(e))
         if e.status_code == 409:
             logger.warning(f"An available model version exists with hash {hash}")
+            # Do not keep empty model versions, it won't be used anyways
+            destroy_model_version(client=client, model_version_id=model_version_id)
             return e.content
         logger.error(f"Failed to update model version: {msg}")
         raise e
+
+
+def destroy_model_version(
+    client: ArkindexClient,
+    model_version_id: Union[str, UUID],
+) -> None:
+    logger.info("Deleting the model version...")
+    try:
+        client.request(
+            "DestroyModelVersion",
+            id=model_version_id,
+        )
+    except ErrorResponse as e:
+        msg = getattr(e, "content", repr(e))
+        logger.error(f"Failed to delete model version: {msg}")
+        raise e
```

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/process/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/process/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/process/base.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/process/base.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/process/recover.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/process/recover.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/process/report.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/process/report.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/secrets.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/upload/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/upload/alto/__init__.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/upload/alto/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 import csv
 import errno
 import json
 import logging
 import re
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 from uuid import UUID
-from xmlrpc.client import Boolean
 
 from apistar.exceptions import ErrorResponse
 from arkindex import ArkindexClient
 from lxml import etree as ET
 from lxml import objectify
 from rich.progress import Progress, track
 
 from arkindex_cli.argtypes import URLArgument
 from arkindex_cli.auth import Profiles
-from arkindex_cli.commands.upload.alto.parser import AltoElement, RootAltoElement
+from arkindex_cli.commands.upload.alto.parser import (
+    AltoElement,
+    MetsProcessingError,
+    RootAltoElement,
+    RootMetsElement,
+)
 
 REGEX_IMAGE_ID = re.compile(r"0+(\d+)")
 
 logger = logging.getLogger(__name__)
 
 
 def add_alto_parser(subcommands):
@@ -72,14 +76,15 @@
     )
     types.add_argument(
         "--existing-types",
         help='Specify correspondences between element types in the Arkindex corpus and in the ALTO files. Format: --existing-types="alto_type:arkindex_type alto_type_2:arkindex_type_2"',
         type=str,
     )
     gallica.set_defaults(func=run_gallica)
+
     alto = subcommands.add_parser(
         "alto",
         description="Upload ALTO XML documents to Arkindex.",
         help="Upload ALTO XML documents to Arkindex.",
     )
     alto.add_argument(
         "--alto-namespace",
@@ -102,14 +107,26 @@
     alto.add_argument(
         "--parent-id",
         help="UUID of a parent folder under which page elements will be created.",
         type=UUID,
         required=True,
     )
     alto.add_argument(
+        "--dpi-x",
+        help="Horizontal resolution of the image, in dots per inch, to be used for ALTO files using coordinates in tenths of millimeters.\n"
+        "Strictly positive integer. Ignored for files using coordinates in pixels.",
+        type=int,
+    )
+    alto.add_argument(
+        "--dpi-y",
+        help="Vertical resolution of the image, in dots per inch, to be used for ALTO files using coordinates in tenths of millimeters.\n"
+        "Strictly positive integer. Ignored for files using coordinates in pixels.",
+        type=int,
+    )
+    alto.add_argument(
         "--json-summary",
         help="Build a JSON file creation report for each parsed ALTO file.",
         action="store_true",
     )
     types = alto.add_mutually_exclusive_group(required=True)
     types.add_argument(
         "--create-types",
@@ -119,14 +136,37 @@
     types.add_argument(
         "--existing-types",
         help='Specify correspondences between element types in the Arkindex corpus and in the ALTO files. Format: --existing-types="alto_type:arkindex_type alto_type_2:arkindex_type_2"',
         type=str,
     )
     alto.set_defaults(func=run)
 
+    mets = subcommands.add_parser(
+        "mets",
+        description="Upload METS XML documents to Arkindex.",
+        help="Upload METS XML documents to Arkindex.",
+    )
+    mets.add_argument(
+        "path",
+        help="Path to a METS file.",
+        type=Path,
+    )
+    mets.add_argument(
+        "corpus_id",
+        help="ID of the Arkindex corpus.",
+        type=UUID,
+    )
+    mets.add_argument(
+        "--element-id",
+        help="ID of the Arkindex element.",
+        type=UUID,
+        required=True,
+    )
+    mets.set_defaults(func=run_mets)
+
 
 def check_element_type(corpus: dict, type_slug: str) -> None:
     types = {type["slug"] for type in corpus["types"]}
     if type_slug not in types:
         raise ValueError(f"Type {type_slug} not found.")
     return True
 
@@ -143,15 +183,15 @@
 
 
 def get_element_type(
     client: ArkindexClient,
     corpus_id: UUID,
     node_name: str,
     types_dict: Optional[dict],
-    create_types: Boolean = False,
+    create_types: bool = False,
 ):
     """
     Retrieve or create an alto node's corresponding Arkindex element type.
     """
     arkindex_corpus_types = [
         item["slug"] for item in client.request("RetrieveCorpus", id=corpus_id)["types"]
     ]
@@ -185,32 +225,35 @@
             logger.info(
                 f"Element type {node_name} exists in target corpus {corpus_id}."
             )
         return node_name
 
 
 def create_elements(
-    client, item, image_id, element_name, corpus, parent_id, types_dict, create_types
+    client: ArkindexClient,
+    item: Union[AltoElement, dict],
+    image_id: str,
+    element_name: str,
+    corpus: dict,
+    parent_id: UUID,
+    types_dict: Optional[dict],
+    create_types: bool,
 ):
     # Specific handling of the Page node, which is the "base" element created from the
     # image on Arkindex, and which is parent to all other elements.
     if type(item) == AltoElement and item.node_name == "page":
         page_node = item
         # For page nodes, a polygon can be defined by WIDTH, HEIGHT, V_POS and H_POS
         # like other nodes, or from WIDTH and HEIGHT only.
         if page_node.polygon:
             page_polygon = page_node.polygon
         else:
-            page_polygon = [
-                [0, 0],
-                [0, page_node.height],
-                [page_node.width, page_node.height],
-                [page_node.width, 0],
-                [0, 0],
-            ]
+            page_polygon = page_node.ark_polygon(
+                {"x": 0, "y": 0, "width": page_node.width, "height": page_node.height}
+            )
         logger.info(f"Creating page {element_name}…")
         page = client.request(
             "CreateElement",
             body={
                 "corpus": corpus["id"],
                 "parent": str(parent_id),
                 "type": get_element_type(
@@ -358,26 +401,30 @@
 def upload_alto_file(
     path: Path,
     client: ArkindexClient,
     iiif_base_url: str,
     corpus: dict,
     parent_id: UUID,
     types_dict: Optional[dict],
-    create_types: Boolean,
+    create_types: bool,
+    dpi_x: Optional[int] = None,
+    dpi_y: Optional[int] = None,
     gallica: bool = False,
     folders_ark_id_dict: dict = None,
     alto_namespace: str = None,
     json_summary: bool = False,
 ) -> None:
     with open(path) as file:
         # This ensures that comments in the XML files do not cause the
         # "no Alto namespace found" exception.
         parser = ET.XMLParser(remove_comments=True)
         tree = objectify.parse(file, parser=parser)
-        root = RootAltoElement(tree.getroot(), alto_namespace=alto_namespace)
+        root = RootAltoElement(
+            tree.getroot(), alto_namespace=alto_namespace, dpi_x=dpi_x, dpi_y=dpi_y
+        )
 
     # Skip empty files immediately
     if not len(root.content):
         logger.warning(f"No content found in file {path}")
         return
 
     page_nodes = root.content.findall(".//{*}Page", namespaces=root.namespaces)
@@ -388,30 +435,42 @@
         # urljoin or path.join would erase that identifier prefix.
         if gallica:
             url = format_url(path, iiif_base_url, folders_ark_id_dict)
             image_id = create_iiif_image(client, url)
         else:
             image_id = create_iiif_image(client, iiif_base_url + root.filename)
         page_name = root.filename
-        page_node = AltoElement(page_nodes[0], alto_namespace=alto_namespace)
+        page_node = AltoElement(
+            page_nodes[0],
+            alto_namespace=alto_namespace,
+            unit=root.unit,
+            dpi_x=dpi_x,
+            dpi_y=dpi_y,
+        )
         page_node.parse_children()
         elements = create_elements(
             client,
             page_node,
             image_id,
             page_name,
             corpus,
             parent_id,
             types_dict,
             create_types,
         )
     elif len(page_nodes) > 1:
         elements = {}
         for page_node in page_nodes:
-            page_node = AltoElement(page_node, alto_namespace=alto_namespace)
+            page_node = AltoElement(
+                page_node,
+                alto_namespace=alto_namespace,
+                unit=root.unit,
+                dpi_x=dpi_x,
+                dpi_y=dpi_y,
+            )
             if page_node.page_image_id is None:
                 logger.warning(
                     "Attribute PHYSICAL_IMG_NR was not set for this Page node. Skipping…"
                 )
                 return
             image_id = create_iiif_image(
                 client, iiif_base_url + page_node.page_image_id
@@ -447,16 +506,16 @@
             )
 
 
 def run_gallica(
     path: Path,
     iiif_base_url: str,
     parent_id: UUID,
-    create_types: Boolean,
-    existing_types: Boolean,
+    create_types: bool = False,
+    existing_types: Optional[str] = None,
     metadata_file: Path = None,
     json_summary: bool = False,
     profile_slug: Optional[str] = None,
     alto_namespace: str = None,
 ):
     # If this is a Gallica import, load the metadata CSV file
     folders_ark_id_dict = dict()
@@ -478,34 +537,48 @@
     )
 
 
 def run(
     path: Path,
     iiif_base_url: str,
     parent_id: UUID,
-    create_types: Boolean,
-    existing_types: Boolean,
+    dpi_x: Optional[int] = None,
+    dpi_y: Optional[int] = None,
+    create_types: bool = False,
+    existing_types: Optional[str] = None,
     folders_ark_id_dict: dict = None,
     profile_slug: Optional[str] = None,
     gallica: bool = False,
     alto_namespace: str = None,
     json_summary: bool = False,
 ) -> int:
-
-    with Progress(transient=True) as progress:
-        progress.add_task(start=False, description="Loading API client")
-        client = Profiles().get_api_client_or_exit(profile_slug)
+    if (dpi_x is None) ^ (dpi_y is None):
+        logger.error("--dpi-x and --dpi-y must be either both set or both unset.")
+        return errno.EINVAL
+
+    if dpi_x is not None and dpi_x <= 0:
+        logger.error("--dpi-x must be a strictly positive integer.")
+        return errno.EINVAL
+
+    if dpi_y is not None and dpi_y <= 0:
+        logger.error("--dpi-y must be a strictly positive integer.")
+        return errno.EINVAL
 
     if not path.is_dir():
         logger.error(f"{path} is not a directory.")
         return errno.ENOTDIR
 
     file_paths = list(path.rglob("*.xml"))
     if not file_paths:
         logger.error(f"No XML files found in {path}.")
+        return errno.ENOENT
+
+    with Progress(transient=True) as progress:
+        progress.add_task(start=False, description="Loading API client")
+        client = Profiles().get_api_client_or_exit(profile_slug)
 
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Fetching parent element")
         try:
             parent = client.request("RetrieveElement", id=parent_id)
         except ErrorResponse as e:
             logger.error(
@@ -535,32 +608,88 @@
             try:
                 check_element_type(corpus, arkindex_type)
             except ValueError as e:
                 logger.error(str(e))
                 return errno.EINVAL
 
     failed = 0
+
     for file_path in track(file_paths, description="Uploading"):
         try:
             upload_alto_file(
                 gallica=gallica,
                 folders_ark_id_dict=folders_ark_id_dict,
                 path=file_path,
                 client=client,
                 iiif_base_url=iiif_base_url,
                 corpus=corpus,
                 parent_id=parent_id,
                 types_dict=types_dict,
                 create_types=create_types,
+                dpi_x=dpi_x,
+                dpi_y=dpi_y,
                 alto_namespace=alto_namespace,
                 json_summary=json_summary,
             )
         except ErrorResponse as e:
             logger.error(
                 f"Upload failed for file {file_path}: HTTP {e.status_code} - {e.content}"
             )
             failed += 1
         except Exception as e:
             logger.error(f"Upload failed for file {file_path}: {e}")
             failed += 1
     # Return a non-zero error code when all files have failed
     return failed >= len(file_paths)
+
+
+def run_mets(
+    path: Path,
+    corpus_id: UUID,
+    element_id: UUID,
+    profile_slug: Optional[str] = None,
+):
+    with Progress(transient=True) as progress:
+        progress.add_task(start=False, description="Loading API client")
+        client = Profiles().get_api_client_or_exit(profile_slug)
+
+    # Parse TOC
+    assert path.exists(), f"Cannot find METS at {path}"
+
+    with path.open() as file:
+        # This ensures that comments in the XML files do not cause the
+        # "no Alto namespace found" exception.
+        parser = ET.XMLParser(remove_comments=True)
+        tree = objectify.parse(file, parser=parser)
+
+        root = RootMetsElement(path, tree.getroot())
+
+    with Progress(transient=True) as progress:
+        progress.add_task(start=False, description="Fetching corpus")
+        try:
+            corpus = client.request("RetrieveCorpus", id=corpus_id)
+        except ErrorResponse as e:
+            logger.error(
+                f"Could not retrieve corpus {corpus_id}: HTTP {e.status_code} - {e.content}"
+            )
+            return errno.EREMOTEIO
+
+    # Check that every type used by the tree is available on the corpus
+    for type_slug in root.parse_object_types():
+        check_element_type(corpus, type_slug=type_slug)
+
+    # Check the existence of the top element
+    with Progress(transient=True) as progress:
+        progress.add_task(start=False, description="Fetching parent element")
+        try:
+            client.request("RetrieveElement", id=element_id)
+        except ErrorResponse as e:
+            logger.error(
+                f"Could not retrieve parent element {element_id}: HTTP {e.status_code} - {e.content}"
+            )
+            return errno.EREMOTEIO
+
+    try:
+        root.publish(arkindex_client=client, parent_id=element_id, corpus_id=corpus_id)
+    except MetsProcessingError:
+        logger.error(f"Failed to publish METS file @ {path}")
+        return errno.EREMOTEIO
```

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/upload/iiif.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/upload/iiif.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/upload/minio_client.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/upload/minio_client.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/commands/upload/page_xml_import.py` & `arkindex-cli-0.2.5/arkindex_cli/commands/upload/page_xml_import.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli/utils.py` & `arkindex-cli-0.2.5/arkindex_cli/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/arkindex_cli.egg-info/PKG-INFO` & `arkindex-cli-0.2.5/arkindex_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: export
 
 # Arkindex CLI
 
 Documentation for users is available in the [docs](./docs) folder, and online as [cli.arkindex.org](https://cli.arkindex.org).
```

### Comparing `arkindex-cli-0.2.4/arkindex_cli.egg-info/SOURCES.txt` & `arkindex-cli-0.2.5/arkindex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.4/setup.py` & `arkindex-cli-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     version=VERSION,
     description="Arkindex CLI client easy and sexy to use",
     author="Teklia",
     author_email="contact@teklia.com",
     url="https://arkindex.teklia.com",
     long_description=README,
     long_description_content_type="text/markdown",
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     install_requires=install_requires,
     tests_require=[],
     extras_require={"export": requirements("requirements-export.txt")},
     packages=find_packages(),
     entry_points={"console_scripts": ["arkindex = arkindex_cli.cli:main"]},
 )
```

