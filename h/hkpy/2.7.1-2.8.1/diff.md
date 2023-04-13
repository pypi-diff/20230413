# Comparing `tmp/hkpy-2.7.1.tar.gz` & `tmp/hkpy-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkpy-2.7.1.tar", last modified: Mon Jan 16 18:24:45 2023, max compression
+gzip compressed data, was "hkpy-2.8.1.tar", last modified: Thu Apr 13 19:22:34 2023, max compression
```

## Comparing `hkpy-2.7.1.tar` & `hkpy-2.8.1.tar`

### file list

```diff
@@ -1,77 +1,92 @@
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.972123 hkpy-2.7.1/
--rw-r--r--   0 srfiorini   (501) staff       (20)     1088 2022-12-06 19:32:26.000000 hkpy-2.7.1/LICENSE
--rw-r--r--   0 srfiorini   (501) staff       (20)       23 2023-01-16 13:40:23.000000 hkpy-2.7.1/MANIFEST.in
--rw-r--r--   0 srfiorini   (501) staff       (20)      851 2023-01-16 18:24:45.971988 hkpy-2.7.1/PKG-INFO
--rw-r--r--   0 srfiorini   (501) staff       (20)     2538 2022-12-06 19:32:26.000000 hkpy-2.7.1/README.md
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.961741 hkpy-2.7.1/hkpy/
--rw-r--r--   0 srfiorini   (501) staff       (20)      218 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/__init__.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.962801 hkpy-2.7.1/hkpy/common/
--rw-r--r--   0 srfiorini   (501) staff       (20)      109 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/common/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2163 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/common/result_set.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.964223 hkpy-2.7.1/hkpy/hkbase/
--rw-r--r--   0 srfiorini   (501) staff       (20)      309 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     6600 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/hkbase.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     6160 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/hkobserverfactory.py
--rw-r--r--   0 srfiorini   (501) staff       (20)    23183 2022-12-08 13:20:27.000000 hkpy-2.7.1/hkpy/hkbase/hkrepository.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1169 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/hktransaction.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.964576 hkpy-2.7.1/hkpy/hkbase/observer/
--rw-r--r--   0 srfiorini   (501) staff       (20)      162 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/__init__.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.965444 hkpy-2.7.1/hkpy/hkbase/observer/clients/
--rw-r--r--   0 srfiorini   (501) staff       (20)      331 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/clients/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     5210 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/clients/configurableobserverclient.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1691 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/clients/observerclient.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     6873 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     7990 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/clients/restobserverclient.py
--rw-r--r--   0 srfiorini   (501) staff       (20)      599 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/observer/notification.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1859 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/query.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1600 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkbase/query_management.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.967148 hkpy-2.7.1/hkpy/hklib/
--rw-r--r--   0 srfiorini   (501) staff       (20)     2726 2022-12-07 19:56:04.000000 hkpy-2.7.1/hkpy/hklib/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1790 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hklib/anchor.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2123 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hklib/connector.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     3321 2022-12-12 13:38:25.000000 hkpy-2.7.1/hkpy/hklib/entity.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.968462 hkpy-2.7.1/hkpy/hklib/fi/
--rw-r--r--   0 srfiorini   (501) staff       (20)      250 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2410 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/fi.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1431 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/fianchor.py
--rw-r--r--   0 srfiorini   (501) staff       (20)      193 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/fioperator.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     3910 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/fiparser.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1477 2023-01-16 14:34:44.000000 hkpy-2.7.1/hkpy/hklib/fi/grammar.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     6927 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hklib/graph.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     3516 2022-12-07 19:56:04.000000 hkpy-2.7.1/hkpy/hklib/graphbuilder.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     3738 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hklib/link.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     9768 2023-01-03 17:36:05.000000 hkpy-2.7.1/hkpy/hklib/node.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.968637 hkpy-2.7.1/hkpy/hkpyo/
--rw-r--r--   0 srfiorini   (501) staff       (20)      177 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/__init__.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.969542 hkpy-2.7.1/hkpy/hkpyo/converters/
--rw-r--r--   0 srfiorini   (501) staff       (20)    16080 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/converters/HKOReaderHKG.py
--rw-r--r--   0 srfiorini   (501) staff       (20)    19047 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/converters/HKOWriterHKG.py
--rw-r--r--   0 srfiorini   (501) staff       (20)      197 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/converters/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)      493 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/converters/constants.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1533 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/converters/utils.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.970054 hkpy-2.7.1/hkpy/hkpyo/hkb/
--rw-r--r--   0 srfiorini   (501) staff       (20)      158 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/hkb/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2694 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/hkb/hkbo.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2290 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/hkb/hkbo_simple.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.970408 hkpy-2.7.1/hkpy/hkpyo/model/
--rw-r--r--   0 srfiorini   (501) staff       (20)      135 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/model/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)    16316 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/model/hko_model.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.970764 hkpy-2.7.1/hkpy/hkpyo/reasoners/
--rw-r--r--   0 srfiorini   (501) staff       (20)      141 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/reasoners/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     4855 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/hkpyo/reasoners/simple_reasoner.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.971113 hkpy-2.7.1/hkpy/oops/
--rw-r--r--   0 srfiorini   (501) staff       (20)      185 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/oops/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)      775 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/oops/oops.py
--rw-r--r--   0 srfiorini   (501) staff       (20)        0 2023-01-16 13:40:23.000000 hkpy-2.7.1/hkpy/py.typed
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.971716 hkpy-2.7.1/hkpy/utils/
--rw-r--r--   0 srfiorini   (501) staff       (20)      155 2022-12-06 19:32:26.000000 hkpy-2.7.1/hkpy/utils/__init__.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     1379 2022-12-07 19:56:04.000000 hkpy-2.7.1/hkpy/utils/constants.py
--rw-r--r--   0 srfiorini   (501) staff       (20)     2234 2022-12-07 19:56:04.000000 hkpy-2.7.1/hkpy/utils/misc.py
-drwxr-xr-x   0 srfiorini   (501) staff       (20)        0 2023-01-16 18:24:45.962439 hkpy-2.7.1/hkpy.egg-info/
--rw-r--r--   0 srfiorini   (501) staff       (20)      851 2023-01-16 18:24:45.000000 hkpy-2.7.1/hkpy.egg-info/PKG-INFO
--rw-r--r--   0 srfiorini   (501) staff       (20)     1612 2023-01-16 18:24:45.000000 hkpy-2.7.1/hkpy.egg-info/SOURCES.txt
--rw-r--r--   0 srfiorini   (501) staff       (20)        1 2023-01-16 18:24:45.000000 hkpy-2.7.1/hkpy.egg-info/dependency_links.txt
--rw-r--r--   0 srfiorini   (501) staff       (20)       71 2023-01-16 18:24:45.000000 hkpy-2.7.1/hkpy.egg-info/requires.txt
--rw-r--r--   0 srfiorini   (501) staff       (20)        5 2023-01-16 18:24:45.000000 hkpy-2.7.1/hkpy.egg-info/top_level.txt
--rw-r--r--   0 srfiorini   (501) staff       (20)       38 2023-01-16 18:24:45.972168 hkpy-2.7.1/setup.cfg
--rw-r--r--   0 srfiorini   (501) staff       (20)     1974 2023-01-11 13:00:43.000000 hkpy-2.7.1/setup.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:34.051376 hkpy-2.8.1/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.758390 hkpy-2.8.1/.venv/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.766920 hkpy-2.8.1/.venv/lib/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.775477 hkpy-2.8.1/.venv/lib/python3.10/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.824112 hkpy-2.8.1/.venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.532160 hkpy-2.8.1/.venv/lib/python3.10/site-packages/hkpy/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 18:41:08.000000 hkpy-2.8.1/.venv/lib/python3.10/site-packages/hkpy/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.636512 hkpy-2.8.1/.venv/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      286 2023-04-13 18:34:18.000000 hkpy-2.8.1/.venv/lib/python3.10/site-packages/pip/py.typed
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1088 2023-04-13 14:26:29.000000 hkpy-2.8.1/LICENSE
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       45 2023-04-13 19:17:08.000000 hkpy-2.8.1/MANIFEST.in
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-04-13 19:22:34.044856 hkpy-2.8.1/PKG-INFO
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2538 2023-04-13 14:26:29.000000 hkpy-2.8.1/README.md
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.745329 hkpy-2.8.1/hkpy/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      218 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.137560 hkpy-2.8.1/hkpy/common/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      109 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/common/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2163 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/common/result_set.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.663862 hkpy-2.8.1/hkpy/hkbase/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      309 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6600 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkbase.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6160 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkobserverfactory.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    23414 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkrepository.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1169 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hktransaction.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.818390 hkpy-2.8.1/hkpy/hkbase/observer/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      162 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:31.281090 hkpy-2.8.1/hkpy/hkbase/observer/clients/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      331 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     5210 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/configurableobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1691 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/observerclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6873 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     7990 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/restobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      599 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/notification.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1859 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/query.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1600 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/query_management.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:31.891013 hkpy-2.8.1/hkpy/hklib/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2726 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1790 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/anchor.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2123 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/connector.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3321 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/entity.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.334190 hkpy-2.8.1/hkpy/hklib/fi/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      250 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2410 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/fi.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1875 2023-04-13 15:31:05.000000 hkpy-2.8.1/hkpy/hklib/fi/fianchor.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      193 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/fioperator.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4098 2023-04-13 15:31:05.000000 hkpy-2.8.1/hkpy/hklib/fi/fiparser.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1477 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/grammar.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6927 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/graph.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3516 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/graphbuilder.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3738 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hklib/link.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     9768 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hklib/node.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.408228 hkpy-2.8.1/hkpy/hkpyo/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      177 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.818380 hkpy-2.8.1/hkpy/hkpyo/converters/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16080 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/HKOReaderHKG.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    19047 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/HKOWriterHKG.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      197 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      493 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/constants.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1533 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/utils.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.067527 hkpy-2.8.1/hkpy/hkpyo/hkb/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      158 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2694 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2290 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo_simple.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.223279 hkpy-2.8.1/hkpy/hkpyo/model/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      135 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/model/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16316 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/model/hko_model.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.382840 hkpy-2.8.1/hkpy/hkpyo/reasoners/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      141 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/reasoners/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4855 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/reasoners/simple_reasoner.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.518031 hkpy-2.8.1/hkpy/oops/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      185 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/oops/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      775 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/oops/oops.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.726486 hkpy-2.8.1/hkpy/utils/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      155 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1379 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/constants.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2234 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/misc.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.003978 hkpy-2.8.1/hkpy.egg-info/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/PKG-INFO
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1828 2023-04-13 19:22:28.000000 hkpy-2.8.1/hkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        1 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       71 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/requires.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/top_level.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       38 2023-04-13 19:22:34.054394 hkpy-2.8.1/setup.cfg
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1976 2023-04-13 19:18:58.000000 hkpy-2.8.1/setup.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.988545 hkpy-2.8.1/tests/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4004 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3454 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_context.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2092 2023-04-13 15:31:05.000000 hkpy-2.8.1/tests/test_fi.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      903 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_literal.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3764 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_simple_reasoner.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-04-13 19:20:59.000000 hkpy-2.8.1/version.txt
```

### Comparing `hkpy-2.7.1/LICENSE` & `hkpy-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/PKG-INFO` & `hkpy-2.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: hkpy
-Version: 2.7.1
+Version: 2.8.1
 Summary: A Python module to create software abstraction for accessing hyperknowledge graphs
 Home-page: https://github.com/ibm-hyperknowledge/hkpy
 Author: IBM Research Brazil
 Author-email: mmoreno@br.ibm.com
 License: MIT
 Keywords: Hyperknowlede,Knowledge Engineering
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python module to create software abstraction for accessing hyperknowledge graphs
-
```

### Comparing `hkpy-2.7.1/README.md` & `hkpy-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/common/result_set.py` & `hkpy-2.8.1/hkpy/common/result_set.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/hkbase.py` & `hkpy-2.8.1/hkpy/hkbase/hkbase.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/hkobserverfactory.py` & `hkpy-2.8.1/hkpy/hkbase/hkobserverfactory.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/hkrepository.py` & `hkpy-2.8.1/hkpy/hkbase/hkrepository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###
 # Copyright (c) 2019-present, IBM Research
 # Licensed under The MIT License [see LICENSE for details]
 ###
-
-from typing import TypeVar, List, Dict, Union, Optional, Any, cast
+import urllib
+from typing import TypeVar, List, Dict, Union, Optional, Any, cast, Tuple
 
 import os
 import copy
 import json
 import requests
 from urllib.parse import quote
 from io import TextIOWrapper, BufferedReader, BufferedIOBase, BytesIO
@@ -439,15 +439,15 @@
                    id_: Optional[str] = None) -> str:
         """
         """
 
         url = f'{self.base._repository_uri}/{self.name}/storage/object'
 
         if id_ is not None:
-            url = f'{url}/{id_}'
+            url = f'{url}/{urllib.parse.quote_plus(id_)}'
 
         if isinstance(object_, (TextIOWrapper, BufferedReader, BufferedIOBase)):
             object_ = object_.read()
         elif isinstance(object_, str) and os.path.isfile(object_):
             with open(object_ ,'rb') as f:
                 object_ = f.read()
         elif isinstance(object_, str):
@@ -465,24 +465,24 @@
 
         return data['objectId'] if 'objectId' in data else data
 
     def delete_object(self, id_: str) -> None:
         """
         """
 
-        url = f'{self.base._repository_uri}/{self.name}/storage/object/{id_}'
+        url = f'{self.base._repository_uri}/{self.name}/storage/object/{urllib.parse.quote_plus(id_)}'
 
         response = requests.delete(url=url, headers=self._headers)
         response_validator(response=response)
 
     def get_object(self, id_: str) -> bytes:
         """
         """
 
-        url = f'{self.base._repository_uri}/{self.name}/storage/object/{id_}'
+        url = f'{self.base._repository_uri}/{self.name}/storage/object/{urllib.parse.quote_plus(id_)}'
 
         response = requests.get(url=url, headers=self._headers)
         _, data = response_validator(response=response, content='.')
 
         return data
 
     def get_all_stored_queries(self, transaction_id: Optional[str] = None) -> List[HKStoredQuery]:
@@ -603,30 +603,33 @@
         if 'head' in data and 'boolean' in data:
             return data['boolean']
         # validate if data is of the correct format
         if not ('results' in data and 'bindings' in data['results'] and 'head' in data):
             raise HKpyError(f'The given data is not of the expected format')
         return SPARQLResultSet(data)
 
-    def resolve_fi(self, fi: FI, raw = False) -> Union[bytes, List[HKEntity]] :
+    def resolve_fi(self, fi: FI, raw: bool = False, output_mimetype: bool = False) -> Union[HKEntity, Tuple[Any, str]]:
         """
         Resolve a full FI. Set raw to True in order to get raw output. Otherwise the function will try to
         interpret the response (i.e. into hk objects)
         """
         quoted_fi = quote(fi.__str__(), safe="");
         url = f'{self.base._repository_uri}/{self.name}/fi/{quoted_fi}'
 
         response = requests.get(url=url, headers=self._headers)
         _, data = response_validator(response=response, content='.')
 
+        content_type = response.headers['Content-Type']
         if raw:
-            return data
+            if output_mimetype:
+                return data, content_type
+            else:
+                return data
 
         # some extra response data converter
-        content_type = response.headers['Content-Type']
         if content_type.startswith('hyperknowledge/graph'):
             return hkfy(response.json())
         elif content_type.startswith('hyperknowledge/node'):
             return hkfy(response.json())
         elif content_type.startswith('text'):
             return response.content.decode()
         else:
```

### Comparing `hkpy-2.7.1/hkpy/hkbase/hktransaction.py` & `hkpy-2.8.1/hkpy/hkbase/hktransaction.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/observer/clients/configurableobserverclient.py` & `hkpy-2.8.1/hkpy/hkbase/observer/clients/configurableobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/observer/clients/observerclient.py` & `hkpy-2.8.1/hkpy/hkbase/observer/clients/observerclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py` & `hkpy-2.8.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/observer/clients/restobserverclient.py` & `hkpy-2.8.1/hkpy/hkbase/observer/clients/restobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/observer/notification.py` & `hkpy-2.8.1/hkpy/hkbase/observer/notification.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/query.py` & `hkpy-2.8.1/hkpy/hkbase/query.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkbase/query_management.py` & `hkpy-2.8.1/hkpy/hkbase/query_management.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/__init__.py` & `hkpy-2.8.1/hkpy/hklib/__init__.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/anchor.py` & `hkpy-2.8.1/hkpy/hklib/anchor.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/connector.py` & `hkpy-2.8.1/hkpy/hklib/connector.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/entity.py` & `hkpy-2.8.1/hkpy/hklib/entity.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/fi/fi.py` & `hkpy-2.8.1/hkpy/hklib/fi/fi.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/fi/fianchor.py` & `hkpy-2.8.1/hkpy/hklib/fi/fianchor.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,11 +34,20 @@
                 strAnchor = f"""{strAnchor}({self.token.__str__()})"""
             elif isinstance(self.token, dict) and len(self.token) > 0:
                 args = []
                 for param, value in self.token.items():
                     args.append(f"""{param}: {value}""")
                 strArguments = ','.join(args)
                 strAnchor = f"""{strAnchor}({{{strArguments}}})"""
+            elif isinstance(self.token, list) and len(self.token) > 0:
+                elements = []
+                for value in self.token:
+                    if isinstance(value, str):
+                        elements.append(f'''"{value}"''')
+                    else:
+                        elements.append(f'''{value}''')
+                str_elements = ','.join(elements)
+                strAnchor = f"""{strAnchor}([{str_elements}])"""
             else:
                 strAnchor = f"""{strAnchor}({self.token.__str__()})"""
 
         return f"""{strAnchor}"""
```

### Comparing `hkpy-2.7.1/hkpy/hklib/fi/fiparser.py` & `hkpy-2.8.1/hkpy/hklib/fi/fiparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,23 +86,30 @@
 def processJsonPlus(ast):
     ast = ast.children[0]
     if isinstance(ast, Token):
         if ast.type == 'FALSE': return False
         if ast.type == 'NULL': return None
         if ast.type == 'TRUE': return True
         if ast.type == 'NUMBER': return astlib.literal_eval(ast)
-        if ast.type == 'STRING': return ast
+        if ast.type == 'STRING': return astlib.literal_eval(ast)
     else:
         if ast.data == 'fijs': return processFijs(ast)
         if ast.data == 'object': return processObject(ast)
         if ast.data == 'array': return processArray(ast)
 
 
 def processArray(ast):
-    raise Exception('Not supported!')
+    array = []
+    if len(ast.children) > 0:
+        members = ast.children
+        for member in members:
+            element = processJsonPlus(member)
+            array.append(element)
+    return array
+
 
 def processObject(ast):
     object = {}
     if len(ast.children) > 0:
         members = ast.children
         for member in members:
             pair = processMember(member)
```

### Comparing `hkpy-2.7.1/hkpy/hklib/fi/grammar.py` & `hkpy-2.8.1/hkpy/hklib/fi/grammar.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/graph.py` & `hkpy-2.8.1/hkpy/hklib/graph.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/graphbuilder.py` & `hkpy-2.8.1/hkpy/hklib/graphbuilder.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/link.py` & `hkpy-2.8.1/hkpy/hklib/link.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hklib/node.py` & `hkpy-2.8.1/hkpy/hklib/node.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/converters/HKOReaderHKG.py` & `hkpy-2.8.1/hkpy/hkpyo/converters/HKOReaderHKG.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/converters/HKOWriterHKG.py` & `hkpy-2.8.1/hkpy/hkpyo/converters/HKOWriterHKG.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/converters/utils.py` & `hkpy-2.8.1/hkpy/hkpyo/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/hkb/hkbo.py` & `hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/hkb/hkbo_simple.py` & `hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo_simple.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/model/hko_model.py` & `hkpy-2.8.1/hkpy/hkpyo/model/hko_model.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/hkpyo/reasoners/simple_reasoner.py` & `hkpy-2.8.1/hkpy/hkpyo/reasoners/simple_reasoner.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/oops/oops.py` & `hkpy-2.8.1/hkpy/oops/oops.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/utils/constants.py` & `hkpy-2.8.1/hkpy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy/utils/misc.py` & `hkpy-2.8.1/hkpy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.7.1/hkpy.egg-info/PKG-INFO` & `hkpy-2.8.1/hkpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: hkpy
-Version: 2.7.1
+Version: 2.8.1
 Summary: A Python module to create software abstraction for accessing hyperknowledge graphs
 Home-page: https://github.com/ibm-hyperknowledge/hkpy
 Author: IBM Research Brazil
 Author-email: mmoreno@br.ibm.com
 License: MIT
 Keywords: Hyperknowlede,Knowledge Engineering
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python module to create software abstraction for accessing hyperknowledge graphs
-
```

### Comparing `hkpy-2.7.1/hkpy.egg-info/SOURCES.txt` & `hkpy-2.8.1/hkpy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+./version.txt
+.venv/lib/python3.10/site-packages/hkpy/py.typed
+.venv/lib/python3.10/site-packages/pip/py.typed
 hkpy/__init__.py
 hkpy/py.typed
 hkpy.egg-info/PKG-INFO
 hkpy.egg-info/SOURCES.txt
 hkpy.egg-info/dependency_links.txt
 hkpy.egg-info/requires.txt
 hkpy.egg-info/top_level.txt
@@ -52,8 +55,13 @@
 hkpy/hkpyo/model/hko_model.py
 hkpy/hkpyo/reasoners/__init__.py
 hkpy/hkpyo/reasoners/simple_reasoner.py
 hkpy/oops/__init__.py
 hkpy/oops/oops.py
 hkpy/utils/__init__.py
 hkpy/utils/constants.py
-hkpy/utils/misc.py
+hkpy/utils/misc.py
+tests/test.py
+tests/test_context.py
+tests/test_fi.py
+tests/test_literal.py
+tests/test_simple_reasoner.py
```

### Comparing `hkpy-2.7.1/setup.py` & `hkpy-2.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for dir_ in dirs:
         dirs += find_recursive_packages(dir_)
     
     return [dir_.replace('/', '.') for dir_ in dirs]
 
 
 NAME = 'hkpy'
-VERSION = open('version.txt', 'r').read().strip()
+VERSION = open('./version.txt', 'r').read().strip()
 URL = 'https://github.com/ibm-hyperknowledge/hkpy'
 DESCRIPTION = 'A Python module to create software abstraction for accessing hyperknowledge graphs'
 LONG_DESCRIPTION = None
 AUTHOR = 'IBM Research Brazil'
 AUTHOR_EMAIL = 'mmoreno@br.ibm.com'
 KEYWORDS = 'Hyperknowlede, Knowledge Engineering'
 REQUIRES_PYTHON = '>=3.6'
```

