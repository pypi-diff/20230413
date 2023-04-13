# Comparing `tmp/ndex2-3.5.1.tar.gz` & `tmp/ndex2-3.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ndex2-3.5.1.tar", last modified: Thu Apr 13 01:17:08 2023, max compression
+gzip compressed data, was "dist/ndex2-3.5.1a1.tar", last modified: Tue Apr 11 22:48:15 2023, max compression
```

## Comparing `ndex2-3.5.1.tar` & `ndex2-3.5.1a1.tar`

### file list

```diff
@@ -1,78 +1,70 @@
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/
--rw-r--r--   0 churas     (501) staff       (20)     9488 2023-04-13 01:16:47.000000 ndex2-3.5.1/HISTORY.rst
--rw-r--r--   0 churas     (501) staff       (20)     1526 2023-04-13 01:09:43.000000 ndex2-3.5.1/LICENSE.txt
--rw-r--r--   0 churas     (501) staff       (20)      237 2021-09-18 05:39:58.000000 ndex2-3.5.1/MANIFEST.in
--rw-r--r--   0 churas     (501) staff       (20)     2477 2021-09-18 05:39:58.000000 ndex2-3.5.1/Makefile
--rw-r--r--   0 churas     (501) staff       (20)    15298 2023-04-13 01:17:08.000000 ndex2-3.5.1/PKG-INFO
--rw-r--r--   0 churas     (501) staff       (20)     2507 2023-04-13 01:09:43.000000 ndex2-3.5.1/README.rst
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/docs/
--rw-r--r--   0 churas     (501) staff       (20)      606 2019-05-25 04:18:25.000000 ndex2-3.5.1/docs/Makefile
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/docs/_build/
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/docs/_build/html/
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/docs/_build/html/_static/
--rw-r--r--   0 churas     (501) staff       (20)      673 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 churas     (501) staff       (20)      756 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 churas     (501) staff       (20)      829 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 churas     (501) staff       (20)      641 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/comment.png
--rw-r--r--   0 churas     (501) staff       (20)      222 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 churas     (501) staff       (20)      202 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/down.png
--rw-r--r--   0 churas     (501) staff       (20)      286 2019-03-09 14:07:37.000000 ndex2-3.5.1/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (501) staff       (20)       90 2019-03-09 14:07:37.000000 ndex2-3.5.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (501) staff       (20)       90 2019-03-09 14:07:37.000000 ndex2-3.5.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (501) staff       (20)      214 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 churas     (501) staff       (20)      203 2019-03-10 07:47:02.000000 ndex2-3.5.1/docs/_build/html/_static/up.png
--rw-r--r--   0 churas     (501) staff       (20)     9473 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/conf.py
--rw-r--r--   0 churas     (501) staff       (20)     1067 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/convertnicecx.rst
--rw-r--r--   0 churas     (501) staff       (20)      520 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/createnicecx.rst
--rw-r--r--   0 churas     (501) staff       (20)       28 2019-05-25 04:18:25.000000 ndex2-3.5.1/docs/history.rst
--rw-r--r--   0 churas     (501) staff       (20)      241 2021-09-18 05:39:58.000000 ndex2-3.5.1/docs/index.rst
--rw-r--r--   0 churas     (501) staff       (20)     1062 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/installation.rst
--rw-r--r--   0 churas     (501) staff       (20)       46 2019-05-25 04:18:25.000000 ndex2-3.5.1/docs/license.rst
--rw-r--r--   0 churas     (501) staff       (20)      581 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/miscref.rst
--rw-r--r--   0 churas     (501) staff       (20)      545 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/modules.rst
--rw-r--r--   0 churas     (501) staff       (20)     2769 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/ndex2.rst
--rw-r--r--   0 churas     (501) staff       (20)     2357 2019-01-03 05:56:49.000000 ndex2-3.5.1/docs/ndex2.tests.rst
--rw-r--r--   0 churas     (501) staff       (20)     1949 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/ndex2client.rst
--rw-r--r--   0 churas     (501) staff       (20)     7395 2023-04-13 01:09:43.000000 ndex2-3.5.1/docs/quicktutorial.rst
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2/
--rw-r--r--   0 churas     (501) staff       (20)    28035 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2/__init__.py
--rw-r--r--   0 churas     (501) staff       (20)    88026 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2/client.py
--rw-r--r--   0 churas     (501) staff       (20)     2635 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2/constants.py
--rw-r--r--   0 churas     (501) staff       (20)      955 2021-09-18 05:39:58.000000 ndex2-3.5.1/ndex2/exceptions.py
--rw-r--r--   0 churas     (501) staff       (20)    20507 2021-09-18 05:39:58.000000 ndex2-3.5.1/ndex2/niceCxInterface.py
--rw-r--r--   0 churas     (501) staff       (20)   106528 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2/nice_cx_network.py
--rw-r--r--   0 churas     (501) staff       (20)     6120 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2/util.py
--rw-r--r--   0 churas     (501) staff       (20)       22 2023-04-13 01:10:16.000000 ndex2-3.5.1/ndex2/version.py
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/
--rw-r--r--   0 churas     (501) staff       (20)    15298 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/PKG-INFO
--rw-r--r--   0 churas     (501) staff       (20)     1743 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (501) staff       (20)        1 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (501) staff       (20)      167 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/requires.txt
--rw-r--r--   0 churas     (501) staff       (20)       14 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/ndex2cx/
--rw-r--r--   0 churas     (501) staff       (20)      697 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2cx/__init__.py
--rw-r--r--   0 churas     (501) staff       (20)    18128 2023-04-13 01:09:43.000000 ndex2-3.5.1/ndex2cx/nice_cx_builder.py
--rw-r--r--   0 churas     (501) staff       (20)      255 2021-09-18 05:39:58.000000 ndex2-3.5.1/ndex2cx/parallelCX.py
--rw-r--r--   0 churas     (501) staff       (20)      295 2023-04-13 01:17:08.000000 ndex2-3.5.1/setup.cfg
--rw-r--r--   0 churas     (501) staff       (20)     3578 2023-04-13 01:09:43.000000 ndex2-3.5.1/setup.py
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/tests/
--rw-r--r--   0 churas     (501) staff       (20)       60 2018-12-31 21:28:20.000000 ndex2-3.5.1/tests/__init__.py
-drwxr-xr-x   0 churas     (501) staff       (20)        0 2023-04-13 01:17:08.000000 ndex2-3.5.1/tests/data/
--rw-r--r--   0 churas     (501) staff       (20)   108653 2019-05-25 04:18:25.000000 ndex2-3.5.1/tests/data/darkthemefinal.cx
--rw-r--r--   0 churas     (501) staff       (20)   218291 2019-05-25 04:18:25.000000 ndex2-3.5.1/tests/data/darkthemefinalwithnodevis.cx
--rw-r--r--   0 churas     (501) staff       (20)    10185 2019-05-25 04:18:25.000000 ndex2-3.5.1/tests/data/glypican2.cx
--rw-r--r--   0 churas     (501) staff       (20)    10436 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/data/glypican2.cx2
--rw-r--r--   0 churas     (501) staff       (20)    73563 2019-05-25 04:18:25.000000 ndex2-3.5.1/tests/data/wntsignaling.cx
--rw-r--r--   0 churas     (501) staff       (20)     1074 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test__init__.py
--rw-r--r--   0 churas     (501) staff       (20)    95333 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_client.py
--rw-r--r--   0 churas     (501) staff       (20)    12063 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_create_nice_cx_from_networkx.py
--rw-r--r--   0 churas     (501) staff       (20)     7496 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_create_nice_cx_from_pandas.py
--rw-r--r--   0 churas     (501) staff       (20)     2999 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_create_nice_cx_from_raw_cx.py
--rw-r--r--   0 churas     (501) staff       (20)    25010 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_defaultnetworkxfactory.py
--rw-r--r--   0 churas     (501) staff       (20)     2625 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_integration__init__.py
--rw-r--r--   0 churas     (501) staff       (20)    13161 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_integration_nice_cx_network.py
--rw-r--r--   0 churas     (501) staff       (20)    41979 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_integration_test_of_client.py
--rw-r--r--   0 churas     (501) staff       (20)     9488 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_legacynetworkxversiontwoplusfactory.py
--rw-r--r--   0 churas     (501) staff       (20)    13715 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_nice_cx_builder.py
--rw-r--r--   0 churas     (501) staff       (20)    41667 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_nice_cx_network.py
--rw-r--r--   0 churas     (501) staff       (20)     7828 2023-04-13 01:09:43.000000 ndex2-3.5.1/tests/test_pandasdataconverter.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/
+-rw-r--r--   0 churas     (504) staff       (20)     9490 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1526 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/LICENSE.txt
+-rw-r--r--   0 churas     (504) staff       (20)      237 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     2477 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/Makefile
+-rw-r--r--   0 churas     (504) staff       (20)    15318 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2507 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      606 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 ndex2-3.5.1a1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)     9473 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)     1067 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/convertnicecx.rst
+-rw-r--r--   0 churas     (504) staff       (20)      520 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/createnicecx.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      241 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1062 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)       46 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/docs/license.rst
+-rw-r--r--   0 churas     (504) staff       (20)      581 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/miscref.rst
+-rw-r--r--   0 churas     (504) staff       (20)      545 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     2769 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/ndex2.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1949 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/ndex2client.rst
+-rw-r--r--   0 churas     (504) staff       (20)     7395 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/docs/quicktutorial.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2/
+-rw-r--r--   0 churas     (504) staff       (20)    28035 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    88026 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2/client.py
+-rw-r--r--   0 churas     (504) staff       (20)     2635 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      955 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    20507 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2/niceCxInterface.py
+-rw-r--r--   0 churas     (504) staff       (20)   106528 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)     6120 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2/util.py
+-rw-r--r--   0 churas     (504) staff       (20)       24 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2/version.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)    15318 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1425 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)      167 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       14 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/ndex2cx/
+-rw-r--r--   0 churas     (504) staff       (20)      697 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/ndex2cx/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    18128 2023-04-11 22:45:25.000000 ndex2-3.5.1a1/ndex2cx/nice_cx_builder.py
+-rw-r--r--   0 churas     (504) staff       (20)      255 2021-04-01 21:50:41.000000 ndex2-3.5.1a1/ndex2cx/parallelCX.py
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     3578 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/tests/
+-rw-r--r--   0 churas     (504) staff       (20)     6148 2022-06-14 21:58:22.000000 ndex2-3.5.1a1/tests/.DS_Store
+-rw-r--r--   0 churas     (504) staff       (20)       60 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-04-11 22:48:15.000000 ndex2-3.5.1a1/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)   108653 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/darkthemefinal.cx
+-rw-r--r--   0 churas     (504) staff       (20)   218291 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/darkthemefinalwithnodevis.cx
+-rw-r--r--   0 churas     (504) staff       (20)    10185 2021-03-31 01:22:47.000000 ndex2-3.5.1a1/tests/data/glypican2.cx
+-rw-r--r--   0 churas     (504) staff       (20)    10436 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/data/glypican2.cx2
+-rw-r--r--   0 churas     (504) staff       (20)    73563 2021-04-01 00:54:02.000000 ndex2-3.5.1a1/tests/data/wntsignaling.cx
+-rw-r--r--   0 churas     (504) staff       (20)     1074 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    95333 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_client.py
+-rw-r--r--   0 churas     (504) staff       (20)    12063 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_networkx.py
+-rw-r--r--   0 churas     (504) staff       (20)     7496 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_pandas.py
+-rw-r--r--   0 churas     (504) staff       (20)     2999 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_create_nice_cx_from_raw_cx.py
+-rw-r--r--   0 churas     (504) staff       (20)    25010 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_defaultnetworkxfactory.py
+-rw-r--r--   0 churas     (504) staff       (20)     2625 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    13161 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration_nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)    41979 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_integration_test_of_client.py
+-rw-r--r--   0 churas     (504) staff       (20)     9488 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_legacynetworkxversiontwoplusfactory.py
+-rw-r--r--   0 churas     (504) staff       (20)    13715 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_nice_cx_builder.py
+-rw-r--r--   0 churas     (504) staff       (20)    41667 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_nice_cx_network.py
+-rw-r--r--   0 churas     (504) staff       (20)     7828 2023-04-11 19:16:56.000000 ndex2-3.5.1a1/tests/test_pandasdataconverter.py
```

### Comparing `ndex2-3.5.1/HISTORY.rst` & `ndex2-3.5.1a1/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 History
 =======
 
 3.5.1 (2023-04-11)
 -------------------
 
 * Bug fixes
+
     * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
       `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+
     * Updated post and put calls in ``client.py`` to only pass credentials if they are
       set. This change is to accommodate changes in upcoming version 3 of requests library
 
 3.5.0 (2022-06-28)
 -------------------
 
 * Enhancements
```

### Comparing `ndex2-3.5.1/LICENSE.txt` & `ndex2-3.5.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/Makefile` & `ndex2-3.5.1a1/Makefile`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/PKG-INFO` & `ndex2-3.5.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ndex2
-Version: 3.5.1
+Version: 3.5.1a1
 Summary: Nice CX Python includes a client and a data model.
 Home-page: https://github.com/ndexbio/ndex2-client
 Author: The NDEx Project
 Author-email: contact@ndexbio.org
 License: BSD
 Description: **NDEx2 Python Client**
         =========================
@@ -93,16 +93,18 @@
         History
         =======
         
         3.5.1 (2023-04-11)
         -------------------
         
         * Bug fixes
+        
             * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
               `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+        
             * Updated post and put calls in ``client.py`` to only pass credentials if they are
               set. This change is to accommodate changes in upcoming version 3 of requests library
         
         3.5.0 (2022-06-28)
         -------------------
         
         * Enhancements
```

### Comparing `ndex2-3.5.1/README.rst` & `ndex2-3.5.1a1/README.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/Makefile` & `ndex2-3.5.1a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/conf.py` & `ndex2-3.5.1a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/convertnicecx.rst` & `ndex2-3.5.1a1/docs/convertnicecx.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/createnicecx.rst` & `ndex2-3.5.1a1/docs/createnicecx.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/installation.rst` & `ndex2-3.5.1a1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/miscref.rst` & `ndex2-3.5.1a1/docs/miscref.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/modules.rst` & `ndex2-3.5.1a1/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/ndex2.rst` & `ndex2-3.5.1a1/docs/ndex2.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/ndex2client.rst` & `ndex2-3.5.1a1/docs/ndex2client.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/docs/quicktutorial.rst` & `ndex2-3.5.1a1/docs/quicktutorial.rst`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/__init__.py` & `ndex2-3.5.1a1/ndex2/__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/client.py` & `ndex2-3.5.1a1/ndex2/client.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/constants.py` & `ndex2-3.5.1a1/ndex2/constants.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/exceptions.py` & `ndex2-3.5.1a1/ndex2/exceptions.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/niceCxInterface.py` & `ndex2-3.5.1a1/ndex2/niceCxInterface.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/nice_cx_network.py` & `ndex2-3.5.1a1/ndex2/nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2/util.py` & `ndex2-3.5.1a1/ndex2/util.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2.egg-info/PKG-INFO` & `ndex2-3.5.1a1/ndex2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ndex2
-Version: 3.5.1
+Version: 3.5.1a1
 Summary: Nice CX Python includes a client and a data model.
 Home-page: https://github.com/ndexbio/ndex2-client
 Author: The NDEx Project
 Author-email: contact@ndexbio.org
 License: BSD
 Description: **NDEx2 Python Client**
         =========================
@@ -93,16 +93,18 @@
         History
         =======
         
         3.5.1 (2023-04-11)
         -------------------
         
         * Bug fixes
+        
             * Fixed bug where ``ndex2.create_nice_cx_from_networkx()`` fails with numpy version 1.24
               `Issue #96 <https://github.com/ndexbio/ndex2-client/issues/96>`__
+        
             * Updated post and put calls in ``client.py`` to only pass credentials if they are
               set. This change is to accommodate changes in upcoming version 3 of requests library
         
         3.5.0 (2022-06-28)
         -------------------
         
         * Enhancements
```

### Comparing `ndex2-3.5.1/ndex2cx/__init__.py` & `ndex2-3.5.1a1/ndex2cx/__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/ndex2cx/nice_cx_builder.py` & `ndex2-3.5.1a1/ndex2cx/nice_cx_builder.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/setup.py` & `ndex2-3.5.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/data/darkthemefinal.cx` & `ndex2-3.5.1a1/tests/data/darkthemefinal.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/data/darkthemefinalwithnodevis.cx` & `ndex2-3.5.1a1/tests/data/darkthemefinalwithnodevis.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/data/glypican2.cx` & `ndex2-3.5.1a1/tests/data/glypican2.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/data/glypican2.cx2` & `ndex2-3.5.1a1/tests/data/glypican2.cx2`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/data/wntsignaling.cx` & `ndex2-3.5.1a1/tests/data/wntsignaling.cx`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test__init__.py` & `ndex2-3.5.1a1/tests/test__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_client.py` & `ndex2-3.5.1a1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_create_nice_cx_from_networkx.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_networkx.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_create_nice_cx_from_pandas.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_create_nice_cx_from_raw_cx.py` & `ndex2-3.5.1a1/tests/test_create_nice_cx_from_raw_cx.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_defaultnetworkxfactory.py` & `ndex2-3.5.1a1/tests/test_defaultnetworkxfactory.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_integration__init__.py` & `ndex2-3.5.1a1/tests/test_integration__init__.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_integration_nice_cx_network.py` & `ndex2-3.5.1a1/tests/test_integration_nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_integration_test_of_client.py` & `ndex2-3.5.1a1/tests/test_integration_test_of_client.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_legacynetworkxversiontwoplusfactory.py` & `ndex2-3.5.1a1/tests/test_legacynetworkxversiontwoplusfactory.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_nice_cx_builder.py` & `ndex2-3.5.1a1/tests/test_nice_cx_builder.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_nice_cx_network.py` & `ndex2-3.5.1a1/tests/test_nice_cx_network.py`

 * *Files identical despite different names*

### Comparing `ndex2-3.5.1/tests/test_pandasdataconverter.py` & `ndex2-3.5.1a1/tests/test_pandasdataconverter.py`

 * *Files identical despite different names*

