# Comparing `tmp/codefast-23.4.7.8.tar.gz` & `tmp/codefast-23.4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefast-23.4.7.8.tar", last modified: Fri Apr  7 08:59:14 2023, max compression
+gzip compressed data, was "codefast-23.4.8.2.tar", last modified: Sat Apr  8 02:19:48 2023, max compression
```

## Comparing `codefast-23.4.7.8.tar` & `codefast-23.4.8.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-07 08:59:00.000000 codefast-23.4.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-07 08:59:14.638387 codefast-23.4.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-07 08:59:00.000000 codefast-23.4.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.634387 codefast-23.4.7.8/codefast/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.634387 codefast-23.4.7.8/codefast/asyncio/
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/asyncio/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/asyncio/asynclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.634387 codefast-23.4.7.8/codefast/axe/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/axe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/axe/axe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/axe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.634387 codefast-23.4.7.8/codefast/base/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/base/format_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/betterargs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/betterargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/betterargs/abstractclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/concurrent/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/concurrent/fastapi_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/concurrent/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/decorators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/decorators/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/experimental/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/experimental/nsq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/fio/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/fio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/fio/ffpb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/functools/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/functools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/functools/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/functools/subroutine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/io/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/dblite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/osdb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/network/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/network/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/network/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/network/richdownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/network/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/factory_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/responsibility_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/patterns/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/supercell/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/supercell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.638387 codefast-23.4.7.8/codefast/types/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-04-07 08:59:00.000000 codefast-23.4.7.8/codefast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 08:59:14.634387 codefast-23.4.7.8/codefast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-07 08:59:14.000000 codefast-23.4.7.8/codefast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-07 08:59:14.000000 codefast-23.4.7.8/codefast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 08:59:14.000000 codefast-23.4.7.8/codefast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 08:59:14.000000 codefast-23.4.7.8/codefast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 08:59:14.000000 codefast-23.4.7.8/codefast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 08:59:14.638387 codefast-23.4.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-07 08:59:00.000000 codefast-23.4.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-08 02:19:36.000000 codefast-23.4.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-08 02:19:48.427110 codefast-23.4.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-08 02:19:36.000000 codefast-23.4.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast/asyncio/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/asyncio/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/asyncio/asynclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/axe/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe/axe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/base/format_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/betterargs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/betterargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/betterargs/abstractclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/fastapi_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/experimental/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/experimental/nsq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/fio/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/fio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/fio/ffpb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/functools/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/subroutine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/dblite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/osdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/richdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/factory_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/responsibility_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/supercell/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/supercell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:19:48.427110 codefast-23.4.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-08 02:19:36.000000 codefast-23.4.8.2/setup.py
```

### Comparing `codefast-23.4.7.8/LICENSE` & `codefast-23.4.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/PKG-INFO` & `codefast-23.4.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.4.7.8
+Version: 23.4.8.2
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 License: UNKNOWN
 Description: A package encapsulating a few frequently used functions for faster Python programming.
```

### Comparing `codefast-23.4.7.8/README.md` & `codefast-23.4.8.2/README.md`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/__init__.py` & `codefast-23.4.8.2/codefast/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,40 @@
 from codefast.network import Network as net
 from codefast.network import urljoin
 from codefast.utils import (b64decode, b64encode, cipher, decipher, retry,
                             shell, syscall, uuid, md5sum)
 
 # ----------------------------
 
+
 def date_file(prefix: str, file_ext: str) -> str:
     import datetime
     return f"{prefix}_{datetime.datetime.now().strftime('%Y%m%d%H%M')}.{file_ext}"
 
 
 def eval(s: str):
     try:
         import json
         return json.loads(s)
     except json.decoder.JSONDecodeError as e:
         warning(e)
         return ast.literal_eval(s)
 
+
 def generate_version():
     """ Generate package version based on date
     """
     import datetime
     return datetime.datetime.now().strftime('%y.%m.%d.%H')
 
+def blocking():
+    # block main thread from exiting
+    import time
+    while True:
+        time.sleep(1<<10)
 
 csv = utils.CSVIO
 dic = fpdict
 j = fpjson
 js = FastJson()
 lis = fplist
 l = fplist
```

### Comparing `codefast-23.4.7.8/codefast/argparser.py` & `codefast-23.4.8.2/codefast/argparser.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/asyncio/asynclient.py` & `codefast-23.4.8.2/codefast/asyncio/asynclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/axe/axe.py` & `codefast-23.4.8.2/codefast/axe/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/axe.py` & `codefast-23.4.8.2/codefast/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/base/format_print.py` & `codefast-23.4.8.2/codefast/base/format_print.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/betterargs/abstractclient.py` & `codefast-23.4.8.2/codefast/betterargs/abstractclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/cn.py` & `codefast-23.4.8.2/codefast/cn.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/concurrency.py` & `codefast-23.4.8.2/codefast/concurrency.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/concurrent/fastapi_demo.py` & `codefast-23.4.8.2/codefast/concurrent/fastapi_demo.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/concurrent/scheduler.py` & `codefast-23.4.8.2/codefast/concurrent/scheduler.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/constants.py` & `codefast-23.4.8.2/codefast/constants.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/core.py` & `codefast-23.4.8.2/codefast/core.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/decorators/__init__.py` & `codefast-23.4.8.2/codefast/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/decorators/retry.py` & `codefast-23.4.8.2/codefast/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/ds.py` & `codefast-23.4.8.2/codefast/ds.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/experimental/nsq.py` & `codefast-23.4.8.2/codefast/experimental/nsq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/fio/ffpb.py` & `codefast-23.4.8.2/codefast/fio/ffpb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/frameworks/__init__.py` & `codefast-23.4.8.2/codefast/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/functools/subroutine.py` & `codefast-23.4.8.2/codefast/functools/subroutine.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/io/_json.py` & `codefast-23.4.8.2/codefast/io/_json.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/io/dblite.py` & `codefast-23.4.8.2/codefast/io/dblite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/io/file.py` & `codefast-23.4.8.2/codefast/io/file.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/io/osdb.py` & `codefast-23.4.8.2/codefast/io/osdb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/io/sqlite.py` & `codefast-23.4.8.2/codefast/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/logger.py` & `codefast-23.4.8.2/codefast/logger.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/math.py` & `codefast-23.4.8.2/codefast/math.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/network/curl.py` & `codefast-23.4.8.2/codefast/network/curl.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/network/factory.py` & `codefast-23.4.8.2/codefast/network/factory.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/network/richdownloader.py` & `codefast-23.4.8.2/codefast/network/richdownloader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/network/tools.py` & `codefast-23.4.8.2/codefast/network/tools.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/patterns/factory_method.py` & `codefast-23.4.8.2/codefast/patterns/factory_method.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/patterns/observer.py` & `codefast-23.4.8.2/codefast/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/patterns/pipeline.py` & `codefast-23.4.8.2/codefast/patterns/pipeline.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/patterns/responsibility_chain.py` & `codefast-23.4.8.2/codefast/patterns/responsibility_chain.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/reader.py` & `codefast-23.4.8.2/codefast/reader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/types/__init__.py` & `codefast-23.4.8.2/codefast/types/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast/utils.py` & `codefast-23.4.8.2/codefast/utils.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/codefast.egg-info/PKG-INFO` & `codefast-23.4.8.2/codefast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.4.7.8
+Version: 23.4.8.2
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 License: UNKNOWN
 Description: A package encapsulating a few frequently used functions for faster Python programming.
```

### Comparing `codefast-23.4.7.8/codefast.egg-info/SOURCES.txt` & `codefast-23.4.8.2/codefast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codefast-23.4.7.8/setup.py` & `codefast-23.4.8.2/setup.py`

 * *Files identical despite different names*

