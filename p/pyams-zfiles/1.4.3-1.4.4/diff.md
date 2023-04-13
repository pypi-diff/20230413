# Comparing `tmp/pyams_zfiles-1.4.3.tar.gz` & `tmp/pyams_zfiles-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_zfiles-1.4.3.tar", last modified: Tue Feb 21 10:39:30 2023, max compression
+gzip compressed data, was "dist/pyams_zfiles-1.4.4.tar", last modified: Thu Apr 13 13:46:36 2023, max compression
```

## Comparing `pyams_zfiles-1.4.3.tar` & `pyams_zfiles-1.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3629 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1658 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    93884 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/docs/graphql-api.json
--rw-rw-rw-   0 root         (0) root         (0)    40137 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/docs/rest-api.json
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2940 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/api/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12553 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/api/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    18813 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/api/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    11258 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/api/rpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    14479 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/document.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/folder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4315 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     7217 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/include.py
--rw-rw-rw-   0 root         (0) root         (0)    15212 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16465 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo
--rw-rw-rw-   0 root         (0) root         (0)    26086 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po
--rw-rw-rw-   0 root         (0) root         (0)    20175 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/locales/pyams_zfiles.pot
--rw-rw-rw-   0 root         (0) root         (0)     7939 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/skin/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/skin/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/skin/file.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/synchronizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/tests/
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    12744 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/utility.py
--rw-rw-rw-   0 root         (0) root         (0)    11105 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4877 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4807 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11289 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/synchronizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/templates/properties-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     4461 2023-02-21 10:39:05.000000 pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3629 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1545 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      463 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-21 10:39:30.000000 pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1772 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    93884 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/docs/graphql-api.json
+-rw-rw-rw-   0 root         (0) root         (0)    64214 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/docs/rest-api.json
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2940 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/api/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12553 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/api/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    27996 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/api/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11249 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/api/rpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    11997 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14649 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/folder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     7218 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    15645 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15088 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo
+-rw-rw-rw-   0 root         (0) root         (0)    24071 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po
+-rw-rw-rw-   0 root         (0) root         (0)    17093 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/locales/pyams_zfiles.pot
+-rw-rw-rw-   0 root         (0) root         (0)     8043 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/skin/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/skin/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/synchronizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12735 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)    10714 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4807 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/synchronizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/templates/properties-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2023-04-13 13:46:15.000000 pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      463 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 13:46:36.000000 pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/top_level.txt
```

### Comparing `pyams_zfiles-1.4.3/LICENSE` & `pyams_zfiles-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/PKG-INFO` & `pyams_zfiles-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_zfiles
-Version: 1.4.3
+Version: 1.4.4
 Summary: PyAMS files storage manager
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,19 @@
 ZFiles is just a storage manager for these documents; the lifecycle management is delegated to
 the applications which use it as storage backend.
 
 
 Changelog
 =========
 
+1.4.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+ - added enums for workflow states
+
 1.4.3
 -----
  - updated translations
 
 1.4.2
 -----
  - updated workflow delete view
```

### Comparing `pyams_zfiles-1.4.3/docs/HISTORY.rst` & `pyams_zfiles-1.4.4/docs/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+1.4.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+ - added enums for workflow states
+
 1.4.3
 -----
  - updated translations
 
 1.4.2
 -----
  - updated workflow delete view
```

### Comparing `pyams_zfiles-1.4.3/docs/README.rst` & `pyams_zfiles-1.4.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/docs/graphql-api.json` & `pyams_zfiles-1.4.4/docs/graphql-api.json`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/setup.py` & `pyams_zfiles-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.4.3'
+version = '1.4.4'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_form',
     'pyams_pagelet',
     'pyams_skin',
     'pyams_table',
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/api/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/api/graph.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/api/graph.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/api/rpc.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/api/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 from pyramid_rpc.xmlrpc import xmlrpc_method
 
 from pyams_file.interfaces.thumbnail import IThumbnails
 from pyams_utils.registry import get_utility
 from pyams_utils.rpc import RPC_FORBIDDEN, RPC_OBJECT_NOT_FOUND, RPC_SERVICE_UNAVAILABLE, \
     raise_rpc_exception
 from pyams_workflow.interfaces import IWorkflowState, IWorkflowVersions
-from pyams_zfiles.interfaces import ARCHIVED_STATE, CREATE_DOCUMENT_PERMISSION, \
-    CREATE_DOCUMENT_WITH_OWNER_PERMISSION, DEFAULT_CONFIGURATION_NAME, IDocumentContainer, \
-    IDocumentSynchronizer, JSONRPC_ENDPOINT, MANAGE_DOCUMENT_PERMISSION, READ_DOCUMENT_PERMISSION, \
-    SYNCHRONIZE_PERMISSION, XMLRPC_ENDPOINT
+from pyams_zfiles.interfaces import CREATE_DOCUMENT_PERMISSION, CREATE_DOCUMENT_WITH_OWNER_PERMISSION, \
+    DEFAULT_CONFIGURATION_NAME, IDocumentContainer, IDocumentSynchronizer, JSONRPC_ENDPOINT, MANAGE_DOCUMENT_PERMISSION, \
+    READ_DOCUMENT_PERMISSION, STATE, SYNCHRONIZE_PERMISSION, XMLRPC_ENDPOINT
 
 
 __docformat__ = 'restructuredtext'
 
 
 @jsonrpc_method(endpoint=JSONRPC_ENDPOINT,
                 method='findFiles',
@@ -244,15 +243,15 @@
 @xmlrpc_method(endpoint=XMLRPC_ENDPOINT,
                method='archiveFile',
                require_csrf=False)
 def archive_file(request, oid, version=None):
     """Archive document"""
     document = get_document(request, oid, version, MANAGE_DOCUMENT_PERMISSION)
     document.update_status({
-        'status': ARCHIVED_STATE
+        'status': STATE.ARCHIVED.value
     })
 
 
 @jsonrpc_method(endpoint=JSONRPC_ENDPOINT,
                 method='removeFile',
                 require_csrf=False)
 @xmlrpc_method(endpoint=XMLRPC_ENDPOINT,
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/doctests/README.rst` & `pyams_zfiles-1.4.4/src/pyams_zfiles/doctests/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     >>> include_zodbconn(config)
     >>> from pyramid_rpc.xmlrpc import includeme as include_xmlrpc
     >>> include_xmlrpc(config)
     >>> from pyramid_rpc.jsonrpc import includeme as include_jsonrpc
     >>> include_jsonrpc(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
+    >>> from cornice_swagger import includeme as include_swagger
+    >>> include_swagger(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_site import includeme as include_site
     >>> include_site(config)
     >>> from pyams_i18n import includeme as include_i18n
     >>> include_i18n(config)
     >>> from pyams_catalog import includeme as include_catalog
@@ -134,21 +136,21 @@
 
     >>> pprint(document.to_json(fields=['content_type', 'creator', 'status']))
     {'content_type': 'text/plain',
      'creator': 'system:admin',
      'status': 'draft'}
 
     >>> from pyams_workflow.interfaces import IWorkflow, IWorkflowStateLabel
-    >>> from pyams_zfiles.workflow import DRAFT_STATE
+    >>> from pyams_zfiles.interfaces import STATE
 
     >>> wf = config.registry.getAdapter(document, IWorkflow)
     >>> wf
     <pyams_zfiles.workflow.DocumentWorkflow object at 0x...>
 
-    >>> label = config.registry.queryAdapter(wf, IWorkflowStateLabel, name=DRAFT_STATE)
+    >>> label = config.registry.queryAdapter(wf, IWorkflowStateLabel, name=STATE.DRAFT.value)
     >>> label.get_label(document)
     'draft created on .../.../... at ...:...'
 
 
     >>> from pyams_utils.traversing import get_parent
     >>> from pyams_zfiles.interfaces import IDocumentFolder
     >>> folder = get_parent(document, IDocumentFolder)
@@ -238,15 +240,15 @@
      'tags': ['Tag 1', 'Tag 2'],
      'title': 'Test document',
      'update_mode': 'private',
      'updated_time': None,
      'updater': 'system:admin',
      'version': 2}
 
-    >>> label = config.registry.queryAdapter(wf, IWorkflowStateLabel, name=DRAFT_STATE)
+    >>> label = config.registry.queryAdapter(wf, IWorkflowStateLabel, name=STATE.DRAFT.value)
     >>> label.get_label(document)
     'new version created on .../.../... at ...:...'
 
 
 Getting document
 ----------------
 
@@ -258,15 +260,15 @@
 
 But you can specify a specific version or a specific workflow status:
 
     >>> document = utility.get_document(oid, version=1)
     >>> document.to_json().get('version')
     1
 
-    >>> document = utility.get_document(oid, status='published')
+    >>> document = utility.get_document(oid, status=STATE.PUBLISHED.value)
     >>> document.to_json().get('version')
     1
 
 
 Searching documents
 -------------------
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/document.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 from pyams_utils.interfaces.form import NOT_CHANGED
 from pyams_utils.registry import get_utility
 from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_utils.vocabulary import vocabulary_config
 from pyams_workflow.interfaces import IWorkflowInfo, IWorkflowState
-from pyams_zfiles.interfaces import ACCESS_MODE_IDS, DocumentContainerError, IDocument, \
+from pyams_zfiles.interfaces import ACCESS_MODE, ACCESS_MODE_NAMES, DocumentContainerError, IDocument, \
     IDocumentContainer, IDocumentRoles, IDocumentVersion, MANAGE_APPLICATION_PERMISSION, \
-    MANAGE_DOCUMENT_PERMISSION, PRIVATE_MODE, PUBLIC_MODE, \
+    MANAGE_DOCUMENT_PERMISSION, \
     PYAMS_ZFILES_APPLICATIONS_VOCABULARY, READ_DOCUMENT_PERMISSION, ZFILES_WORKFLOW_NAME
 from pyams_zfiles.workflow import ZFILES_WORKFLOW
 
 
 __docformat__ = 'restructuredtext'
 
 
@@ -200,35 +200,41 @@
 
     def update_security_policy(self, properties, request=None):  # pylint: disable=unused-argument
         """Document policy security updater"""
         roles = IDocumentRoles(self)
         protection = IRoleProtectedObject(self)
         granted = protection.authenticated_granted or set()
         if (not self.access_mode) or ('access_mode' in properties):
-            access_mode = properties.pop('access_mode', PRIVATE_MODE)
-            if access_mode in ACCESS_MODE_IDS:
-                access_mode = ACCESS_MODE_IDS.index(access_mode)
-            self.access_mode = access_mode
-            if access_mode == PUBLIC_MODE:
-                granted |= {READ_DOCUMENT_PERMISSION}
+            mode = properties.pop('access_mode', ACCESS_MODE.PRIVATE.value)
+            try:
+                access_mode = ACCESS_MODE(mode).value
+            except ValueError:
+                pass
             else:
-                granted -= {READ_DOCUMENT_PERMISSION}
-                if access_mode == PRIVATE_MODE:
-                    roles.readers = set()
+                self.access_mode = access_mode
+                if access_mode == ACCESS_MODE.PUBLIC.value:
+                    granted |= {READ_DOCUMENT_PERMISSION}
+                else:
+                    granted -= {READ_DOCUMENT_PERMISSION}
+                    if access_mode == ACCESS_MODE.PRIVATE.value:
+                        roles.readers = set()
         if (not self.update_mode) or ('update_mode' in properties):
-            update_mode = properties.pop('update_mode', PRIVATE_MODE)
-            if update_mode in ACCESS_MODE_IDS:
-                update_mode = ACCESS_MODE_IDS.index(update_mode)
-            self.update_mode = update_mode
-            if update_mode == PUBLIC_MODE:
-                granted |= {MANAGE_DOCUMENT_PERMISSION}
+            mode = properties.pop('update_mode', ACCESS_MODE.PRIVATE.value)
+            try:
+                update_mode = ACCESS_MODE(mode).value
+            except ValueError:
+                pass
             else:
-                granted -= {MANAGE_DOCUMENT_PERMISSION}
-                if update_mode == PRIVATE_MODE:
-                    roles.managers = set()
+                self.update_mode = update_mode
+                if update_mode == ACCESS_MODE.PUBLIC.value:
+                    granted |= {MANAGE_DOCUMENT_PERMISSION}
+                else:
+                    granted -= {MANAGE_DOCUMENT_PERMISSION}
+                    if update_mode == ACCESS_MODE.PRIVATE.value:
+                        roles.managers = set()
         protection.authenticated_granted = granted or None
 
     def update_status(self, properties, request=None):
         """Workflow status updater"""
         if 'status' in properties:
             info = IWorkflowInfo(self)
             info.fire_transition_toward(properties.pop('status'), request=request)
@@ -279,17 +285,17 @@
             'creator': list(roles.creator)[0],
             'created_time': dc.created.isoformat() if dc.created else None,  # pylint: disable=no-member
             'owner': list(roles.owner)[0],
             'updater': self.updater,
             'updated_time': dc.modified.isoformat() if dc.modified else None,  # pylint: disable=no-member
             'status_updater': state.state_principal,
             'status_update_time': state.state_date.isoformat(),  # pylint: disable=no-member
-            'access_mode': ACCESS_MODE_IDS[self.access_mode],
+            'access_mode': ACCESS_MODE_NAMES[self.access_mode],
             'readers': list(roles.readers or ()),
-            'update_mode': ACCESS_MODE_IDS[self.update_mode],
+            'update_mode': ACCESS_MODE_NAMES[self.update_mode],
             'managers': list(roles.managers or ())
         }
         if fields:
             for key in tuple(result.keys()):
                 if key not in fields:
                     del result[key]
         return result
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/folder.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/generations/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/generations/evolve1.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/include.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/include.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     })
 
     # register new REST API routes
     config.add_route(REST_CONTAINER_ROUTE,
                      config.registry.settings.get('pyams.zfiles.rest_container_route',
                                                   '/api/zfiles/rest'))
     config.add_route(REST_SYNCHRONIZER_ROUTE,
-                     config.registry.settings.get('pyams.zfiles.rest_synchronize_roue',
+                     config.registry.settings.get('pyams.zfiles.rest_synchronize_route',
                                                   '/api/zfiles/rest/synchronize'))
     config.add_route(REST_DOCUMENT_ROUTE,
                      config.registry.settings.get('pyams.zfiles.rest_document_route',
                                                   '/api/zfiles/rest/{oid}*version'))
 
     # register new GraphQL API route
     config.add_route(GRAPHQL_API_ROUTE,
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/interfaces.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 from zope.schema import Bool, Choice, Dict, List, Password, TextLine
 from zope.schema.interfaces import IDict
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_file.schema import FileField
 from pyams_security.interfaces import IContentRoles
 from pyams_security.schema import PrincipalField, PrincipalsSetField
-from pyams_workflow.interfaces import IWorkflow, IWorkflowManagedContent, \
-    IWorkflowPublicationSupport
+from pyams_workflow.interfaces import IWorkflow, IWorkflowManagedContent, IWorkflowPublicationSupport
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_zfiles import _
 
 
@@ -114,53 +113,71 @@
 ZFILES_WORKFLOW_NAME = 'pyams_zfiles.workflow'
 
 
 class IDocumentWorkflow(IWorkflow):
     """Document workflow marker interface"""
 
 
-DRAFT_STATE = 'draft'
-PUBLISHED_STATE = 'published'
-ARCHIVED_STATE = 'archived'
-DELETED_STATE = 'deleted'
+class STATE(Enum):
+    """State modes"""
+    DRAFT = 'draft'
+    PUBLISHED = 'published'
+    ARCHIVED = 'archived'
+    DELETED = 'deleted'
+
+
+STATES_VALUES = tuple(map(lambda x: x.value, STATE))
+
 
 STATE_LABELS = {
-    DRAFT_STATE: _("Draft"),
-    PUBLISHED_STATE: _("Published"),
-    ARCHIVED_STATE: _("Archived"),
-    DELETED_STATE: _("Deleted")
+    STATE.DRAFT.value: _("Draft"),
+    STATE.PUBLISHED.value: _("Published"),
+    STATE.ARCHIVED.value: _("Archived"),
+    STATE.DELETED.value: _("Deleted")
 }
 
+STATES_HEADERS = {
+    STATE.DRAFT.value: _("draft created"),
+    STATE.PUBLISHED.value: _("published"),
+    STATE.ARCHIVED.value: _("archived")
+}
+
+STATES_VOCABULARY = SimpleVocabulary([
+    SimpleTerm(i, title=t)
+    for i, t in STATE_LABELS.items()
+])
+
 
-class AccessMode(IntEnum):
-    """Access modes"""
-    private = 0  # pylint: disable=invalid-name
-    protected = 1  # pylint: disable=invalid-name
-    public = 2  # pylint: disable=invalid-name
-
-
-PRIVATE_MODE = AccessMode.private
-PROTECTED_MODE = AccessMode.protected
-PUBLIC_MODE = AccessMode.public
-
-ACCESS_MODE_IDS = [
-    'private',
-    'protected',
-    'public'
-]
-
-ACCESS_MODE_LABELS = (
-    _("Private"),
-    _("Protected"),
-    _("Public")
-)
+class ACCESS_MODE(IntEnum):
+    """Security policy access modes"""
+    PRIVATE = 0
+    PROTECTED = 1
+    PUBLIC = 2
+
+
+# Keep for compatibility reason
+AccessMode = ACCESS_MODE
+
+
+ACCESS_MODE_NAMES = {
+    ACCESS_MODE.PRIVATE.value: 'private',
+    ACCESS_MODE.PROTECTED.value: 'protected',
+    ACCESS_MODE.PUBLIC.value: 'public'
+}
+
+ACCESS_MODE_LABELS = {
+    ACCESS_MODE.PRIVATE.value: _("Private"),
+    ACCESS_MODE.PROTECTED.value: _("Protected"),
+    ACCESS_MODE.PUBLIC.value: _("Public")
+}
 
 
 ACCESS_MODE_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(i, t, t) for i, t in enumerate(ACCESS_MODE_LABELS)
+    SimpleTerm(i, title=t)
+    for i, t in ACCESS_MODE_LABELS.items()
 ])
 
 
 class IPropertiesField(IDict):
     """Properties schema field interface"""
 
 
@@ -198,21 +215,21 @@
                     description=_("This unique signature is built using SHA512 algorithm"),
                     required=True)
 
     access_mode = Choice(title=_("Access mode"),
                          description=_("Access mode on this document"),
                          required=True,
                          vocabulary=ACCESS_MODE_VOCABULARY,
-                         default=PRIVATE_MODE)
+                         default=ACCESS_MODE.PRIVATE.value)
 
     update_mode = Choice(title=_("Update mode"),
                          description=_("Update mode on this document"),
                          required=True,
                          vocabulary=ACCESS_MODE_VOCABULARY,
-                         default=PRIVATE_MODE)
+                         default=ACCESS_MODE.PRIVATE.value)
 
     properties = PropertiesField(title=_("Properties"),
                                  description=_("List of free additional properties which can be "
                                                "applied to the document; these properties can't "
                                                "be used for searching"),
                                  required=False)
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/layer.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo` & `pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -128,17 +128,14 @@
 
 msgid "Document content type"
 msgstr "Type de contenu"
 
 msgid "Document content update"
 msgstr "Mise à jour du contenu du document"
 
-msgid "Document created"
-msgstr "Document créé"
-
 msgid "Document creation date"
 msgstr "Date de création"
 
 msgid "Document creation dates range"
 msgstr "Dates de création"
 
 msgid "Document creation timestamp"
@@ -161,59 +158,47 @@
 
 msgid "Document data hash"
 msgstr "Hash"
 
 msgid "Document data in Base64 encoding"
 msgstr "Contenu du document encodé en Base64"
 
-msgid "Document data; may be provided in Base64 when using JSON"
-msgstr "Contenu du document, encodé en Base64 en JSON"
-
 msgid "Document file hash"
 msgstr "Hash du document au format SHA512"
 
 msgid "Document file name"
 msgstr "Nom du fichier"
 
 msgid "Document file size"
 msgstr "Taille du fichier"
 
 msgid "Document last modification dates range"
 msgstr "Dates de dernière modification du document"
 
-msgid "Document last update dates range"
-msgstr "Dates de mise à jour"
-
 msgid "Document last workflow update dates range"
 msgstr "Dates de dernière modification du statut du document"
 
 msgid "Document manager (role)"
 msgstr "Gestionnaire de document (rôle)"
 
 msgid "Document managers"
 msgstr "Contributeurs"
 
 msgid "Document managers IDs"
 msgstr "Liste des gestionnaires du document"
 
-msgid "Document not found"
-msgstr "Document non trouvé"
-
 msgid "Document owner"
 msgstr "Propriétaire"
 
 msgid "Document owner (role)"
 msgstr "Propriétaire de document (rôle)"
 
 msgid "Document properties"
 msgstr "Propriétés du document"
 
-msgid "Document properties, provided as a mapping"
-msgstr "Propriétés du document"
-
 msgid ""
 "Document properties; you can set properties names and values using URL "
 "encoding, like in \"property_name=value1&another_prop=value2\"; if you set "
 "the same property several times, the property values will be combined with "
 "an \"or\""
 msgstr ""
 "Propriétés du document ; vous pouvez indiquer les propriétés et leur valeur "
@@ -239,26 +224,20 @@
 msgstr ""
 "Vous pouvez sélectionner plusieurs tags en les séparant avec des points-"
 "virgules"
 
 msgid "Document tags"
 msgstr "Tags"
 
-msgid "Document tags, separated with semicolons"
-msgstr "Liste des tags du document"
-
 msgid "Document title"
 msgstr "Libellé du document"
 
 msgid "Document unique identifier"
 msgstr "Identifiant unique du document"
 
-msgid "Document unique identifiers"
-msgstr "Identifiants uniques de documents"
-
 msgid "Document update mode"
 msgstr "Mode de mise à jour du document"
 
 msgid "Document version"
 msgstr "Version du document"
 
 msgid "Document workflow state"
@@ -305,17 +284,14 @@
 
 msgid "File hash"
 msgstr "Hash"
 
 msgid "File name"
 msgstr "Nom de fichier"
 
-msgid "Forbidden access"
-msgstr "Accès interdit"
-
 msgid "If 'no', this configuration will not be usable for synchronization"
 msgstr ""
 "Si 'non', cette configuration sera désactivée et ne pourra pas être utilisée "
 "pour effectuer une synchronisation de documents"
 
 msgid ""
 "If 'yes', a menu will be displayed to get access to documents container from "
@@ -338,29 +314,17 @@
 
 msgid "Last document updater"
 msgstr "Mise à jour"
 
 msgid "Last document updater principal ID"
 msgstr "ID du dernier mandataire ayant modifié le document"
 
-msgid "Last workflow status update dates range"
-msgstr "Dates de changement de statut"
-
 msgid "Last workflow status updater principal ID"
 msgstr "ID du dernier mandataire ayant modifié le statut du document"
 
-msgid "List of document tags"
-msgstr "Tags du document"
-
-msgid "List of documents to import in remote documents container"
-msgstr "Liste des documents à importer dans la GED distante"
-
-msgid "List of documents to remove from remote documents container"
-msgstr "Liste des documents à supprimer de la GED distante"
-
 msgid ""
 "List of free additional properties which can be applied to the document; "
 "these properties can't be used for searching"
 msgstr ""
 "Liste de propriétés additionnelles appliquées au document ; ces propriétés "
 "sont libres mais ne sont pas indexées et donc non utilisables pour effectuer "
 "des recherches"
@@ -368,29 +332,20 @@
 msgid ""
 "List of free additional tags which can be applied to the document; these "
 "tags can be used for searching"
 msgstr ""
 "Liste de tags appliqués au document ; ces tags peuvent être appliqués pour "
 "effectuer des recherches"
 
-msgid "List of requested field names"
-msgstr "Liste des champs sélectionnés"
-
-msgid "List of requested fields names"
-msgstr "Liste des champs sélectionnés"
-
 msgid "Manage ZFiles application"
 msgstr "Gérer l'application ZFiles"
 
 msgid "Manage document"
 msgstr "Gérer les documents"
 
-msgid "Missing arguments"
-msgstr "Arguments manquants"
-
 msgid "Modification dates"
 msgstr "Dates de modification"
 
 msgid "Name"
 msgstr "Nom de la configuration"
 
 msgid "Name of principals allowed to read the document"
@@ -491,17 +446,14 @@
 
 msgid "Search document"
 msgstr "Rechercher un document"
 
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
-msgid "Selected configuration name"
-msgstr "Nom de la configuration sélectionnée"
-
 msgid "Source application"
 msgstr "Application source"
 
 msgid "Source application name"
 msgstr "Application source"
 
 msgid "State"
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po` & `pyams_zfiles-1.4.4/src/pyams_zfiles/locales/fr/LC_MESSAGES/pyams_zfiles.po`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyAMS files storage manager
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS zfiles 1.0.0\n"
-"POT-Creation-Date: 2023-02-20 11:41+0100\n"
+"POT-Creation-Date: 2023-04-12 16:16+0200\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
@@ -68,369 +68,366 @@
 msgid "Document reader (role)"
 msgstr "Lecteur de document (rôle)"
 
 #: src/pyams_zfiles/layer.py:36
 msgid "PyAMS ZFiles skin"
 msgstr "Thème PyAMS ZFiles"
 
-#: src/pyams_zfiles/interfaces.py:127 src/pyams_zfiles/workflow.py:51
+#: src/pyams_zfiles/interfaces.py:132
 msgid "Draft"
 msgstr "Brouillon"
 
-#: src/pyams_zfiles/interfaces.py:128 src/pyams_zfiles/workflow.py:52
+#: src/pyams_zfiles/interfaces.py:133
 msgid "Published"
 msgstr "Publié"
 
-#: src/pyams_zfiles/interfaces.py:129 src/pyams_zfiles/workflow.py:53
+#: src/pyams_zfiles/interfaces.py:134
 msgid "Archived"
 msgstr "Archivé"
 
-#: src/pyams_zfiles/interfaces.py:130 src/pyams_zfiles/workflow.py:54
+#: src/pyams_zfiles/interfaces.py:135
 msgid "Deleted"
 msgstr "Supprimé"
 
-#: src/pyams_zfiles/interfaces.py:152
+#: src/pyams_zfiles/interfaces.py:139
+msgid "draft created"
+msgstr "brouillon créé"
+
+#: src/pyams_zfiles/interfaces.py:140
+msgid "published"
+msgstr "publié"
+
+#: src/pyams_zfiles/interfaces.py:141
+msgid "archived"
+msgstr "archivé"
+
+#: src/pyams_zfiles/interfaces.py:168
 msgid "Private"
 msgstr "Privé"
 
-#: src/pyams_zfiles/interfaces.py:153
+#: src/pyams_zfiles/interfaces.py:169
 msgid "Protected"
 msgstr "Protégé"
 
-#: src/pyams_zfiles/interfaces.py:154
+#: src/pyams_zfiles/interfaces.py:170
 msgid "Public"
 msgstr "Public"
 
-#: src/pyams_zfiles/interfaces.py:181 src/pyams_zfiles/interfaces.py:273
-#: src/pyams_zfiles/zmi/search.py:66 src/pyams_zfiles/api/rest.py:128
-#: src/pyams_zfiles/api/graph.py:71 src/pyams_zfiles/api/graph.py:129
-#: src/pyams_zfiles/api/graph.py:147 src/pyams_zfiles/api/graph.py:207
+#: src/pyams_zfiles/interfaces.py:198 src/pyams_zfiles/interfaces.py:290
+#: src/pyams_zfiles/zmi/search.py:66 src/pyams_zfiles/api/graph.py:71
+#: src/pyams_zfiles/api/graph.py:129 src/pyams_zfiles/api/graph.py:147
+#: src/pyams_zfiles/api/graph.py:207
 msgid "Document unique identifier"
 msgstr "Identifiant unique du document"
 
 #.
 #. read-write attributes
-#: src/pyams_zfiles/interfaces.py:184 src/pyams_zfiles/zmi/search.py:72
-#: src/pyams_zfiles/api/rest.py:57 src/pyams_zfiles/api/rest.py:108
-#: src/pyams_zfiles/api/rest.py:151 src/pyams_zfiles/api/graph.py:58
-#: src/pyams_zfiles/api/graph.py:173 src/pyams_zfiles/api/graph.py:209
+#: src/pyams_zfiles/interfaces.py:201 src/pyams_zfiles/zmi/search.py:72
+#: src/pyams_zfiles/api/graph.py:58 src/pyams_zfiles/api/graph.py:173
+#: src/pyams_zfiles/api/graph.py:209
 msgid "Document title"
 msgstr "Libellé du document"
 
-#: src/pyams_zfiles/interfaces.py:185 src/pyams_zfiles/zmi/search.py:73
+#: src/pyams_zfiles/interfaces.py:202 src/pyams_zfiles/zmi/search.py:73
 msgid "User friendly name of the document"
 msgstr "Libellé utilisateur associé au document"
 
-#: src/pyams_zfiles/interfaces.py:188 src/pyams_zfiles/api/rest.py:60
-#: src/pyams_zfiles/api/rest.py:110 src/pyams_zfiles/api/rest.py:154
-#: src/pyams_zfiles/api/graph.py:59
+#: src/pyams_zfiles/interfaces.py:205 src/pyams_zfiles/api/graph.py:59
 msgid "Source application name"
 msgstr "Application source"
 
-#: src/pyams_zfiles/interfaces.py:189 src/pyams_zfiles/zmi/search.py:77
+#: src/pyams_zfiles/interfaces.py:206 src/pyams_zfiles/zmi/search.py:77
 msgid "Name of the application which submitted the document"
 msgstr "Nom de l'application ayant soumis le document"
 
-#: src/pyams_zfiles/interfaces.py:193
+#: src/pyams_zfiles/interfaces.py:210
 msgid "Document data"
 msgstr "Contenu du document"
 
-#: src/pyams_zfiles/interfaces.py:194
+#: src/pyams_zfiles/interfaces.py:211
 msgid "This is where document content is stored"
 msgstr "Contenu utile du document"
 
-#: src/pyams_zfiles/interfaces.py:197
+#: src/pyams_zfiles/interfaces.py:214
 msgid "Document data hash"
 msgstr "Hash"
 
-#: src/pyams_zfiles/interfaces.py:198
+#: src/pyams_zfiles/interfaces.py:215
 msgid "This unique signature is built using SHA512 algorithm"
 msgstr "Signature du contenu du fichier basé sur l'algorithme SHA512"
 
-#: src/pyams_zfiles/interfaces.py:201 src/pyams_zfiles/api/rest.py:80
+#: src/pyams_zfiles/interfaces.py:218
 msgid "Access mode"
 msgstr "Mode d'accès"
 
-#: src/pyams_zfiles/interfaces.py:202
+#: src/pyams_zfiles/interfaces.py:219
 msgid "Access mode on this document"
 msgstr "Mode d'accès au document en lecture"
 
-#: src/pyams_zfiles/interfaces.py:207 src/pyams_zfiles/api/rest.py:87
+#: src/pyams_zfiles/interfaces.py:224
 msgid "Update mode"
 msgstr "Mode de mise à jour"
 
-#: src/pyams_zfiles/interfaces.py:208
+#: src/pyams_zfiles/interfaces.py:225
 msgid "Update mode on this document"
 msgstr "Mode d'accès au document en modification"
 
-#: src/pyams_zfiles/interfaces.py:213 src/pyams_zfiles/zmi/search.py:86
+#: src/pyams_zfiles/interfaces.py:230 src/pyams_zfiles/zmi/search.py:86
 #: src/pyams_zfiles/zmi/document.py:76
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_zfiles/interfaces.py:214
+#: src/pyams_zfiles/interfaces.py:231
 msgid ""
 "List of free additional properties which can be applied to the document; "
 "these properties can't be used for searching"
 msgstr ""
 "Liste de propriétés additionnelles appliquées au document ; ces propriétés "
 "sont libres mais ne sont pas indexées et donc non utilisables pour effectuer "
 "des recherches"
 
-#: src/pyams_zfiles/interfaces.py:221 src/pyams_zfiles/api/graph.py:62
+#: src/pyams_zfiles/interfaces.py:238 src/pyams_zfiles/api/graph.py:62
 msgid "Document tags"
 msgstr "Tags"
 
-#: src/pyams_zfiles/interfaces.py:222
+#: src/pyams_zfiles/interfaces.py:239
 msgid ""
 "List of free additional tags which can be applied to the document; these "
 "tags can be used for searching"
 msgstr ""
 "Liste de tags appliqués au document ; ces tags peuvent être appliqués pour "
 "effectuer des recherches"
 
-#: src/pyams_zfiles/interfaces.py:227
+#: src/pyams_zfiles/interfaces.py:244
 msgid "Last document updater"
 msgstr "Mise à jour"
 
-#: src/pyams_zfiles/interfaces.py:228
+#: src/pyams_zfiles/interfaces.py:245
 msgid "Name of the last principal which updated the document"
 msgstr "Nom du dernier mandataire ayant mis à jour le document"
 
-#: src/pyams_zfiles/interfaces.py:245
+#: src/pyams_zfiles/interfaces.py:262
 msgid "Document creator"
 msgstr "Créateur"
 
-#: src/pyams_zfiles/interfaces.py:246 src/pyams_zfiles/zmi/search.py:105
+#: src/pyams_zfiles/interfaces.py:263 src/pyams_zfiles/zmi/search.py:105
 msgid "Name of the principal which created the document"
 msgstr "Nom du mandataire ayant créé le document"
 
-#: src/pyams_zfiles/interfaces.py:250
+#: src/pyams_zfiles/interfaces.py:267
 msgid "Document owner"
 msgstr "Propriétaire"
 
-#: src/pyams_zfiles/interfaces.py:251
+#: src/pyams_zfiles/interfaces.py:268
 msgid "Name of the principal which is owner of the document"
 msgstr "Nom du mandataire propriétaire du document"
 
-#: src/pyams_zfiles/interfaces.py:255
+#: src/pyams_zfiles/interfaces.py:272
 msgid "Document readers"
 msgstr "Lecteurs"
 
-#: src/pyams_zfiles/interfaces.py:256
+#: src/pyams_zfiles/interfaces.py:273
 msgid "Name of principals allowed to read the document"
 msgstr "Nom des mandataire autorisés à lire le contenu du document"
 
-#: src/pyams_zfiles/interfaces.py:260
+#: src/pyams_zfiles/interfaces.py:277
 msgid "Document managers"
 msgstr "Contributeurs"
 
-#: src/pyams_zfiles/interfaces.py:261
+#: src/pyams_zfiles/interfaces.py:278
 msgid "Name of principals allowed to update the document"
 msgstr "Nom des mandataires autorisés à modifier le document"
 
-#: src/pyams_zfiles/interfaces.py:296
+#: src/pyams_zfiles/interfaces.py:313
 msgid "Documents OID prefix"
 msgstr "Préfixe des OID"
 
-#: src/pyams_zfiles/interfaces.py:297
+#: src/pyams_zfiles/interfaces.py:314
 msgid ""
 "Prefix used to identify documents which were created locally (unlike "
 "documents which were created into another documents container and "
 "synchronized with this container)"
 msgstr ""
 "Préfixe utilisé pour identifier les documents créés localement ; on peut "
 "importer des documents en provenance d'un autre conteneur de documents, à la "
 "condition qu'ils utilisent un préfixe différent"
 
-#: src/pyams_zfiles/interfaces.py:303
+#: src/pyams_zfiles/interfaces.py:320
 msgid "Access menu from home"
 msgstr "Accès depuis l'accueil"
 
-#: src/pyams_zfiles/interfaces.py:304
+#: src/pyams_zfiles/interfaces.py:321
 msgid ""
 "If 'yes', a menu will be displayed to get access to documents container from "
 "site admin home page"
 msgstr ""
 "Si 'oui', un menu d'accès au conteneur de documents sera affiché depuis la "
 "page d'accueil de l'interface d'administration du site"
 
-#: src/pyams_zfiles/interfaces.py:336
+#: src/pyams_zfiles/interfaces.py:353
 msgid "Application managers"
 msgstr "Gestionnaires de l'application"
 
-#: src/pyams_zfiles/interfaces.py:337
+#: src/pyams_zfiles/interfaces.py:354
 msgid ""
 "These principals can only manage application properties; documents manager "
 "role is required to manage documents!"
 msgstr ""
 "Ces mandataires peuvent gérer les propriétés de l'application et ses rôles ; "
 "ils peuvent également gérer les propriétés des documents, et créer de "
 "nouveaux documents au nom d'autres utilisateurs"
 
-#: src/pyams_zfiles/interfaces.py:344
+#: src/pyams_zfiles/interfaces.py:361
 msgid "Documents creators"
 msgstr "Créateurs de documents"
 
-#: src/pyams_zfiles/interfaces.py:345
+#: src/pyams_zfiles/interfaces.py:362
 msgid "These principals will be allowed to create or import new documents"
 msgstr ""
 "Ces mandataires sont autorisés à créer ou importer de nouveaux documents, en "
 "leur nom propre ou au nom d'autres mandataires"
 
-#: src/pyams_zfiles/interfaces.py:350
+#: src/pyams_zfiles/interfaces.py:367
 msgid "Documents managers"
 msgstr "Gestionnaires de documents"
 
-#: src/pyams_zfiles/interfaces.py:351
+#: src/pyams_zfiles/interfaces.py:368
 msgid "These principals will be allowed to manage any document properties"
 msgstr ""
 "Ces mandataires sont autorisés à gérer les propriétés de tous les documents"
 
-#: src/pyams_zfiles/interfaces.py:356
+#: src/pyams_zfiles/interfaces.py:373
 msgid "Documents readers"
 msgstr "Lecteurs de documents"
 
-#: src/pyams_zfiles/interfaces.py:357
+#: src/pyams_zfiles/interfaces.py:374
 msgid "These principals will be allowed to read any document properties"
 msgstr "Ces mandataires sont autorisés à consulter tous les documents"
 
-#: src/pyams_zfiles/interfaces.py:393
+#: src/pyams_zfiles/interfaces.py:410
 msgid "Configuration name"
 msgstr "Nom de la configuration"
 
-#: src/pyams_zfiles/interfaces.py:394
+#: src/pyams_zfiles/interfaces.py:411
 msgid "Unique name of the configuration"
 msgstr "Nom unique donné à la configuration"
 
-#: src/pyams_zfiles/interfaces.py:398
+#: src/pyams_zfiles/interfaces.py:415
 msgid "Remote XML-RPC endpoint"
 msgstr "Point d'accès XML-RPC"
 
-#: src/pyams_zfiles/interfaces.py:399
+#: src/pyams_zfiles/interfaces.py:416
 msgid ""
 "URL of the remote documents container XML-RPC endpoint used for "
 "synchronization"
 msgstr ""
 "URL du point d'accès XML-RPC du conteneur distant vers lequel doit "
 "s'effectuer la synchronisation"
 
-#: src/pyams_zfiles/interfaces.py:403
+#: src/pyams_zfiles/interfaces.py:420
 msgid "User name"
 msgstr "Code utilisateur"
 
-#: src/pyams_zfiles/interfaces.py:404
+#: src/pyams_zfiles/interfaces.py:421
 msgid "Name of the remote user used for synchronization"
 msgstr "Nom de l'utilisateur distant utilisé pour la synchronisation"
 
-#: src/pyams_zfiles/interfaces.py:407
+#: src/pyams_zfiles/interfaces.py:424
 msgid "Password"
 msgstr "Mot de passe"
 
-#: src/pyams_zfiles/interfaces.py:408
+#: src/pyams_zfiles/interfaces.py:425
 msgid "Password of the remote user used for synchronization"
 msgstr "Mot de passe de l'utilisateur distant"
 
-#: src/pyams_zfiles/interfaces.py:411
+#: src/pyams_zfiles/interfaces.py:428
 msgid "Enabled configuration"
 msgstr "Configuration active"
 
-#: src/pyams_zfiles/interfaces.py:412
+#: src/pyams_zfiles/interfaces.py:429
 msgid "If 'no', this configuration will not be usable for synchronization"
 msgstr ""
 "Si 'non', cette configuration sera désactivée et ne pourra pas être utilisée "
 "pour effectuer une synchronisation de documents"
 
-#: src/pyams_zfiles/interfaces.py:424
+#: src/pyams_zfiles/interfaces.py:441
 msgid "Configuration users"
 msgstr "Synchroniseurs"
 
-#: src/pyams_zfiles/interfaces.py:425
+#: src/pyams_zfiles/interfaces.py:442
 msgid "Principals which are granted permission to call this configuration"
 msgstr "Liste des mandataires autorisés à utiliser cette configuration"
 
-#: src/pyams_zfiles/workflow.py:63
-msgid "draft created"
-msgstr "brouillon créé"
-
-#: src/pyams_zfiles/workflow.py:64
-msgid "published"
-msgstr "publié"
-
-#: src/pyams_zfiles/workflow.py:65
-msgid "archived"
-msgstr "archivé"
-
-#: src/pyams_zfiles/workflow.py:120
+#: src/pyams_zfiles/workflow.py:93
 #, python-format
 msgid "Published version {0}"
 msgstr "Version {0} publiée"
 
-#: src/pyams_zfiles/workflow.py:147
+#: src/pyams_zfiles/workflow.py:120
 msgid "Initialize"
 msgstr "Initialiser"
 
-#: src/pyams_zfiles/workflow.py:150
+#: src/pyams_zfiles/workflow.py:123
 msgid "Draft creation"
 msgstr "Brouillon créé"
 
-#: src/pyams_zfiles/workflow.py:153
+#: src/pyams_zfiles/workflow.py:126
 msgid "Publish"
 msgstr "Publier"
 
-#: src/pyams_zfiles/workflow.py:160
+#: src/pyams_zfiles/workflow.py:133
 msgid "Content published"
 msgstr "Contenu publié"
 
-#: src/pyams_zfiles/workflow.py:164
+#: src/pyams_zfiles/workflow.py:137
 msgid "Archive content"
 msgstr "Archiver"
 
-#: src/pyams_zfiles/workflow.py:170
+#: src/pyams_zfiles/workflow.py:143
 msgid "Content archived"
 msgstr "Contenu archivé"
 
-#: src/pyams_zfiles/workflow.py:174 src/pyams_zfiles/workflow.py:186
+#: src/pyams_zfiles/workflow.py:147 src/pyams_zfiles/workflow.py:159
 msgid "Create new version"
 msgstr "Créer une nouvelle version"
 
-#: src/pyams_zfiles/workflow.py:182 src/pyams_zfiles/workflow.py:194
+#: src/pyams_zfiles/workflow.py:155 src/pyams_zfiles/workflow.py:167
 msgid "New version created"
 msgstr "Nouvelle version créée"
 
-#: src/pyams_zfiles/workflow.py:198
+#: src/pyams_zfiles/workflow.py:171
 msgid "Delete version"
 msgstr "Supprimer la version"
 
-#: src/pyams_zfiles/workflow.py:205
+#: src/pyams_zfiles/workflow.py:178
 msgid "Version deleted"
 msgstr "Version supprimée"
 
-#: src/pyams_zfiles/workflow.py:222
+#: src/pyams_zfiles/workflow.py:195
 msgid "ZFiles document workflow"
 msgstr "Workflow de la GED ZFiles"
 
-#: src/pyams_zfiles/workflow.py:268 src/pyams_zfiles/workflow.py:301
+#: src/pyams_zfiles/workflow.py:241 src/pyams_zfiles/workflow.py:274
 #, python-format
 msgid "{state} {date}"
 msgstr "{state} {date}"
 
-#: src/pyams_zfiles/workflow.py:272 src/pyams_zfiles/workflow.py:297
+#: src/pyams_zfiles/workflow.py:245 src/pyams_zfiles/workflow.py:270
 msgid "Unknown state"
 msgstr "État inconnu"
 
-#: src/pyams_zfiles/workflow.py:295
+#: src/pyams_zfiles/workflow.py:268
 msgid "new version created"
 msgstr "nouvelle version créée"
 
-#: src/pyams_zfiles/workflow.py:299
+#: src/pyams_zfiles/workflow.py:272
 msgid "publication refused"
 msgstr "publication refusée"
 
-#: src/pyams_zfiles/utility.py:245
+#: src/pyams_zfiles/utility.py:244
 msgid "Document content update"
 msgstr "Mise à jour du contenu du document"
 
 #: src/pyams_zfiles/zmi/synchronizer.py:88
 msgid "Click icon to enable or disable configuration"
 msgstr "Cliquer pour activer ou désactiver la configuration"
 
@@ -489,16 +486,15 @@
 msgid "Search document"
 msgstr "Rechercher un document"
 
 #: src/pyams_zfiles/zmi/search.py:65
 msgid "Document OID"
 msgstr "OID"
 
-#: src/pyams_zfiles/zmi/search.py:69 src/pyams_zfiles/api/rest.py:129
-#: src/pyams_zfiles/api/rest.py:148 src/pyams_zfiles/api/graph.py:76
+#: src/pyams_zfiles/zmi/search.py:69 src/pyams_zfiles/api/graph.py:76
 #: src/pyams_zfiles/api/graph.py:131 src/pyams_zfiles/api/graph.py:149
 msgid "Document version"
 msgstr "Version du document"
 
 #: src/pyams_zfiles/zmi/search.py:76 src/pyams_zfiles/api/graph.py:175
 #: src/pyams_zfiles/api/graph.py:211
 msgid "Source application"
@@ -532,16 +528,15 @@
 #: src/pyams_zfiles/zmi/search.py:95
 msgid ""
 "Document tag; you can enter several tags by separating them with semicolons"
 msgstr ""
 "Vous pouvez sélectionner plusieurs tags en les séparant avec des points-"
 "virgules"
 
-#: src/pyams_zfiles/zmi/search.py:99 src/pyams_zfiles/api/rest.py:74
-#: src/pyams_zfiles/api/rest.py:165 src/pyams_zfiles/api/graph.py:132
+#: src/pyams_zfiles/zmi/search.py:99 src/pyams_zfiles/api/graph.py:132
 #: src/pyams_zfiles/api/graph.py:150
 msgid "Document status"
 msgstr "Statut du document"
 
 #: src/pyams_zfiles/zmi/search.py:100
 msgid "Workflow state of searched documents"
 msgstr "Statut des documents recherchés"
@@ -570,16 +565,15 @@
 msgid "Name of the principal owning the document"
 msgstr "Nom du mandataire propriétaire du document"
 
 #: src/pyams_zfiles/zmi/search.py:118
 msgid "Updater"
 msgstr "Mise à jour"
 
-#: src/pyams_zfiles/zmi/search.py:119 src/pyams_zfiles/api/rest.py:137
-#: src/pyams_zfiles/api/rest.py:179 src/pyams_zfiles/api/graph.py:79
+#: src/pyams_zfiles/zmi/search.py:119 src/pyams_zfiles/api/graph.py:79
 msgid "Last document updater principal ID"
 msgstr "ID du dernier mandataire ayant modifié le document"
 
 #: src/pyams_zfiles/zmi/search.py:122
 msgid "Modification dates"
 msgstr "Dates de modification"
 
@@ -591,16 +585,15 @@
 "Dates de dernière modification du document (ou de l'une de ses versions) ; "
 "la première date est incluse, la seconde est exclue"
 
 #: src/pyams_zfiles/zmi/search.py:129
 msgid "Status updater"
 msgstr "Changement de statut"
 
-#: src/pyams_zfiles/zmi/search.py:130 src/pyams_zfiles/api/rest.py:139
-#: src/pyams_zfiles/api/rest.py:184
+#: src/pyams_zfiles/zmi/search.py:130
 msgid "Last workflow status updater principal ID"
 msgstr "ID du dernier mandataire ayant modifié le statut du document"
 
 #: src/pyams_zfiles/zmi/search.py:133
 msgid "Status update dates"
 msgstr "Dates de changement"
 
@@ -660,187 +653,164 @@
 msgid "Documents container configuration"
 msgstr "Configuration du conteneur de documents"
 
 #: src/pyams_zfiles/zmi/__init__.py:126
 msgid "Base configuration"
 msgstr "Configuration de base"
 
-#: src/pyams_zfiles/zmi/workflow.py:79
+#: src/pyams_zfiles/zmi/workflow.py:80
 msgid "Delete definitively"
 msgstr "Supprimer définitivement"
 
-#: src/pyams_zfiles/zmi/document.py:99 src/pyams_zfiles/api/rest.py:206
+#: src/pyams_zfiles/zmi/document.py:99
 msgid "Document properties"
 msgstr "Propriétés du document"
 
-#: src/pyams_zfiles/api/rest.py:50
-msgid "List of requested fields names"
-msgstr "Liste des champs sélectionnés"
-
-#: src/pyams_zfiles/api/rest.py:63 src/pyams_zfiles/api/rest.py:101
 #: src/pyams_zfiles/api/graph.py:60 src/pyams_zfiles/api/graph.py:177
 msgid "File name"
 msgstr "Nom de fichier"
 
-#: src/pyams_zfiles/api/rest.py:66 src/pyams_zfiles/api/graph.py:61
+#: src/pyams_zfiles/api/graph.py:61
 msgid "Document custom properties"
 msgstr "Propriétés du document"
 
-#: src/pyams_zfiles/api/rest.py:68
-msgid "List of document tags"
-msgstr "Tags du document"
+#: src/pyams_zfiles/api/graph.py:63
+msgid "Document workflow state"
+msgstr "Statut du workflow"
 
-#: src/pyams_zfiles/api/rest.py:71 src/pyams_zfiles/api/rest.py:122
-#: src/pyams_zfiles/api/rest.py:136 src/pyams_zfiles/api/rest.py:176
 #: src/pyams_zfiles/api/graph.py:64 src/pyams_zfiles/api/graph.py:217
 msgid "Current document owner"
 msgstr "Propriétaire du document"
 
-#: src/pyams_zfiles/api/rest.py:84 src/pyams_zfiles/api/graph.py:66
+#: src/pyams_zfiles/api/graph.py:65
+msgid "Document access mode"
+msgstr "Mode d'accès au document"
+
+#: src/pyams_zfiles/api/graph.py:66
 msgid "Document readers IDs"
 msgstr "Liste des lecteurs du document"
 
-#: src/pyams_zfiles/api/rest.py:91 src/pyams_zfiles/api/graph.py:68
+#: src/pyams_zfiles/api/graph.py:67
+msgid "Document update mode"
+msgstr "Mode de mise à jour du document"
+
+#: src/pyams_zfiles/api/graph.py:68
 msgid "Document managers IDs"
 msgstr "Liste des gestionnaires du document"
 
-#: src/pyams_zfiles/api/rest.py:98 src/pyams_zfiles/api/rest.py:114
-msgid "Document data; may be provided in Base64 when using JSON"
-msgstr "Contenu du document, encodé en Base64 en JSON"
-
-#: src/pyams_zfiles/api/rest.py:112 src/pyams_zfiles/api/graph.py:213
-msgid "Document file name"
-msgstr "Nom du fichier"
-
-#: src/pyams_zfiles/api/rest.py:120 src/pyams_zfiles/api/rest.py:135
-#: src/pyams_zfiles/api/graph.py:78
-msgid "Document creation timestamp"
-msgstr "Date et heure de création"
-
-#.
 #. read-only attributes
-#: src/pyams_zfiles/api/rest.py:127 src/pyams_zfiles/api/graph.py:70
+#: src/pyams_zfiles/api/graph.py:70
 msgid "Document base REST API URL"
 msgstr "URl de base de l'API REST du document"
 
-#: src/pyams_zfiles/api/rest.py:130 src/pyams_zfiles/api/graph.py:72
+#: src/pyams_zfiles/api/graph.py:72
 msgid "Absolute URL of document data file"
 msgstr "URL absolue d'accès au contenu du document"
 
-#: src/pyams_zfiles/api/rest.py:131 src/pyams_zfiles/api/rest.py:157
 #: src/pyams_zfiles/api/graph.py:73
 msgid "SHA512 hash of document data file"
 msgstr "Hash du contenu du fichier au format SHA512"
 
-#: src/pyams_zfiles/api/rest.py:132 src/pyams_zfiles/api/graph.py:74
+#: src/pyams_zfiles/api/graph.py:74
 msgid "Document file size"
 msgstr "Taille du fichier"
 
-#: src/pyams_zfiles/api/rest.py:133 src/pyams_zfiles/api/graph.py:75
+#: src/pyams_zfiles/api/graph.py:75
 msgid "Document content type"
 msgstr "Type de contenu"
 
-#: src/pyams_zfiles/api/rest.py:134 src/pyams_zfiles/api/rest.py:171
 #: src/pyams_zfiles/api/graph.py:77
 msgid "Document creator principal ID"
 msgstr "ID du mandataire créateur du document"
 
-#: src/pyams_zfiles/api/rest.py:138 src/pyams_zfiles/api/graph.py:80
+#: src/pyams_zfiles/api/graph.py:78
+msgid "Document creation timestamp"
+msgstr "Date et heure de création"
+
+#: src/pyams_zfiles/api/graph.py:80
 msgid "Last document update timestamp"
 msgstr "Dernière mise à jour"
 
-#: src/pyams_zfiles/api/rest.py:140 src/pyams_zfiles/api/graph.py:82
-msgid "Last document status update timestamp"
-msgstr "Dernier changement de statut"
-
-#: src/pyams_zfiles/api/rest.py:145
-msgid "Document unique identifiers"
-msgstr "Identifiants uniques de documents"
-
-#: src/pyams_zfiles/api/rest.py:160
-msgid "Document properties, provided as a mapping"
-msgstr "Propriétés du document"
-
-#: src/pyams_zfiles/api/rest.py:162
-msgid "Document tags, separated with semicolons"
-msgstr "Liste des tags du document"
-
-#: src/pyams_zfiles/api/rest.py:173 src/pyams_zfiles/api/graph.py:109
-msgid "Document creation dates range"
-msgstr "Dates de création"
-
-#: src/pyams_zfiles/api/rest.py:181
-msgid "Document last update dates range"
-msgstr "Dates de mise à jour"
-
-#: src/pyams_zfiles/api/rest.py:186
-msgid "Last workflow status update dates range"
-msgstr "Dates de changement de statut"
-
-#: src/pyams_zfiles/api/rest.py:188
-msgid "List of requested field names"
-msgstr "Liste des champs sélectionnés"
-
-#: src/pyams_zfiles/api/rest.py:194
-msgid "List of documents to import in remote documents container"
-msgstr "Liste des documents à importer dans la GED distante"
-
-#: src/pyams_zfiles/api/rest.py:197
-msgid "List of documents to remove from remote documents container"
-msgstr "Liste des documents à supprimer de la GED distante"
-
-#: src/pyams_zfiles/api/rest.py:201
-msgid "Selected configuration name"
-msgstr "Nom de la configuration sélectionnée"
-
-#: src/pyams_zfiles/api/rest.py:207
-msgid "Document created"
-msgstr "Document créé"
-
-#: src/pyams_zfiles/api/rest.py:208
-msgid "Document not found"
-msgstr "Document non trouvé"
-
-#: src/pyams_zfiles/api/rest.py:209
-msgid "Forbidden access"
-msgstr "Accès interdit"
-
-#: src/pyams_zfiles/api/rest.py:210
-msgid "Missing arguments"
-msgstr "Arguments manquants"
-
-#: src/pyams_zfiles/api/graph.py:63
-msgid "Document workflow state"
-msgstr "Statut du workflow"
-
-#: src/pyams_zfiles/api/graph.py:65
-msgid "Document access mode"
-msgstr "Mode d'accès au document"
-
-#: src/pyams_zfiles/api/graph.py:67
-msgid "Document update mode"
-msgstr "Mode de mise à jour du document"
-
 #: src/pyams_zfiles/api/graph.py:81
 msgid "Last document status updater principal ID"
 msgstr "ID du dernier mandataire ayant modifié le statut du document"
 
+#: src/pyams_zfiles/api/graph.py:82
+msgid "Last document status update timestamp"
+msgstr "Dernier changement de statut"
+
 #: src/pyams_zfiles/api/graph.py:87 src/pyams_zfiles/api/graph.py:179
 #: src/pyams_zfiles/api/graph.py:215
 msgid "Document data in Base64 encoding"
 msgstr "Contenu du document encodé en Base64"
 
 #: src/pyams_zfiles/api/graph.py:104
 msgid "Properties query string"
 msgstr "Propriétés du document"
 
+#: src/pyams_zfiles/api/graph.py:109
+msgid "Document creation dates range"
+msgstr "Dates de création"
+
 #: src/pyams_zfiles/api/graph.py:113
 msgid "Document last modification dates range"
 msgstr "Dates de dernière modification du document"
 
 #: src/pyams_zfiles/api/graph.py:116
 msgid "Document last workflow update dates range"
 msgstr "Dates de dernière modification du statut du document"
 
+#: src/pyams_zfiles/api/graph.py:213
+msgid "Document file name"
+msgstr "Nom du fichier"
+
 #: src/pyams_zfiles/api/graph.py:219
 msgid "Document creation date"
 msgstr "Date de création"
+
+#~ msgid "List of requested fields names"
+#~ msgstr "Liste des champs sélectionnés"
+
+#~ msgid "List of document tags"
+#~ msgstr "Tags du document"
+
+#~ msgid "Document data; may be provided in Base64 when using JSON"
+#~ msgstr "Contenu du document, encodé en Base64 en JSON"
+
+#~ msgid "Document unique identifiers"
+#~ msgstr "Identifiants uniques de documents"
+
+#~ msgid "Document properties, provided as a mapping"
+#~ msgstr "Propriétés du document"
+
+#~ msgid "Document tags, separated with semicolons"
+#~ msgstr "Liste des tags du document"
+
+#~ msgid "Document last update dates range"
+#~ msgstr "Dates de mise à jour"
+
+#~ msgid "Last workflow status update dates range"
+#~ msgstr "Dates de changement de statut"
+
+#~ msgid "List of requested field names"
+#~ msgstr "Liste des champs sélectionnés"
+
+#~ msgid "List of documents to import in remote documents container"
+#~ msgstr "Liste des documents à importer dans la GED distante"
+
+#~ msgid "List of documents to remove from remote documents container"
+#~ msgstr "Liste des documents à supprimer de la GED distante"
+
+#~ msgid "Selected configuration name"
+#~ msgstr "Nom de la configuration sélectionnée"
+
+#~ msgid "Document created"
+#~ msgstr "Document créé"
+
+#~ msgid "Document not found"
+#~ msgstr "Document non trouvé"
+
+#~ msgid "Forbidden access"
+#~ msgstr "Accès interdit"
+
+#~ msgid "Missing arguments"
+#~ msgstr "Arguments manquants"
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/locales/pyams_zfiles.pot` & `pyams_zfiles-1.4.4/src/pyams_zfiles/locales/pyams_zfiles.pot`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-02-20 11:41+0100\n"
+"POT-Creation-Date: 2023-04-12 16:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -68,349 +68,346 @@
 msgid "Document reader (role)"
 msgstr ""
 
 #: ./src/pyams_zfiles/layer.py:36
 msgid "PyAMS ZFiles skin"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:127 ./src/pyams_zfiles/workflow.py:51
+#: ./src/pyams_zfiles/interfaces.py:132
 msgid "Draft"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:128 ./src/pyams_zfiles/workflow.py:52
+#: ./src/pyams_zfiles/interfaces.py:133
 msgid "Published"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:129 ./src/pyams_zfiles/workflow.py:53
+#: ./src/pyams_zfiles/interfaces.py:134
 msgid "Archived"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:130 ./src/pyams_zfiles/workflow.py:54
+#: ./src/pyams_zfiles/interfaces.py:135
 msgid "Deleted"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:152
+#: ./src/pyams_zfiles/interfaces.py:139
+msgid "draft created"
+msgstr ""
+
+#: ./src/pyams_zfiles/interfaces.py:140
+msgid "published"
+msgstr ""
+
+#: ./src/pyams_zfiles/interfaces.py:141
+msgid "archived"
+msgstr ""
+
+#: ./src/pyams_zfiles/interfaces.py:168
 msgid "Private"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:153
+#: ./src/pyams_zfiles/interfaces.py:169
 msgid "Protected"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:154
+#: ./src/pyams_zfiles/interfaces.py:170
 msgid "Public"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:181 ./src/pyams_zfiles/interfaces.py:273
-#: ./src/pyams_zfiles/zmi/search.py:66 ./src/pyams_zfiles/api/rest.py:128
-#: ./src/pyams_zfiles/api/graph.py:71 ./src/pyams_zfiles/api/graph.py:129
-#: ./src/pyams_zfiles/api/graph.py:147 ./src/pyams_zfiles/api/graph.py:207
+#: ./src/pyams_zfiles/interfaces.py:198 ./src/pyams_zfiles/interfaces.py:290
+#: ./src/pyams_zfiles/zmi/search.py:66 ./src/pyams_zfiles/api/graph.py:71
+#: ./src/pyams_zfiles/api/graph.py:129 ./src/pyams_zfiles/api/graph.py:147
+#: ./src/pyams_zfiles/api/graph.py:207
 msgid "Document unique identifier"
 msgstr ""
 
 #. 
 #. read-write attributes
-#: ./src/pyams_zfiles/interfaces.py:184 ./src/pyams_zfiles/zmi/search.py:72
-#: ./src/pyams_zfiles/api/rest.py:57 ./src/pyams_zfiles/api/rest.py:108
-#: ./src/pyams_zfiles/api/rest.py:151 ./src/pyams_zfiles/api/graph.py:58
-#: ./src/pyams_zfiles/api/graph.py:173 ./src/pyams_zfiles/api/graph.py:209
+#: ./src/pyams_zfiles/interfaces.py:201 ./src/pyams_zfiles/zmi/search.py:72
+#: ./src/pyams_zfiles/api/graph.py:58 ./src/pyams_zfiles/api/graph.py:173
+#: ./src/pyams_zfiles/api/graph.py:209
 msgid "Document title"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:185 ./src/pyams_zfiles/zmi/search.py:73
+#: ./src/pyams_zfiles/interfaces.py:202 ./src/pyams_zfiles/zmi/search.py:73
 msgid "User friendly name of the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:188 ./src/pyams_zfiles/api/rest.py:60
-#: ./src/pyams_zfiles/api/rest.py:110 ./src/pyams_zfiles/api/rest.py:154
-#: ./src/pyams_zfiles/api/graph.py:59
+#: ./src/pyams_zfiles/interfaces.py:205 ./src/pyams_zfiles/api/graph.py:59
 msgid "Source application name"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:189 ./src/pyams_zfiles/zmi/search.py:77
+#: ./src/pyams_zfiles/interfaces.py:206 ./src/pyams_zfiles/zmi/search.py:77
 msgid "Name of the application which submitted the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:193
+#: ./src/pyams_zfiles/interfaces.py:210
 msgid "Document data"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:194
+#: ./src/pyams_zfiles/interfaces.py:211
 msgid "This is where document content is stored"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:197
+#: ./src/pyams_zfiles/interfaces.py:214
 msgid "Document data hash"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:198
+#: ./src/pyams_zfiles/interfaces.py:215
 msgid "This unique signature is built using SHA512 algorithm"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:201 ./src/pyams_zfiles/api/rest.py:80
+#: ./src/pyams_zfiles/interfaces.py:218
 msgid "Access mode"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:202
+#: ./src/pyams_zfiles/interfaces.py:219
 msgid "Access mode on this document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:207 ./src/pyams_zfiles/api/rest.py:87
+#: ./src/pyams_zfiles/interfaces.py:224
 msgid "Update mode"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:208
+#: ./src/pyams_zfiles/interfaces.py:225
 msgid "Update mode on this document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:213 ./src/pyams_zfiles/zmi/search.py:86
+#: ./src/pyams_zfiles/interfaces.py:230 ./src/pyams_zfiles/zmi/search.py:86
 #: ./src/pyams_zfiles/zmi/document.py:76
 msgid "Properties"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:214
+#: ./src/pyams_zfiles/interfaces.py:231
 msgid ""
 "List of free additional properties which can be applied to the document; "
 "these properties can't be used for searching"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:221 ./src/pyams_zfiles/api/graph.py:62
+#: ./src/pyams_zfiles/interfaces.py:238 ./src/pyams_zfiles/api/graph.py:62
 msgid "Document tags"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:222
+#: ./src/pyams_zfiles/interfaces.py:239
 msgid ""
 "List of free additional tags which can be applied to the document; these tags"
 " can be used for searching"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:227
+#: ./src/pyams_zfiles/interfaces.py:244
 msgid "Last document updater"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:228
+#: ./src/pyams_zfiles/interfaces.py:245
 msgid "Name of the last principal which updated the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:245
+#: ./src/pyams_zfiles/interfaces.py:262
 msgid "Document creator"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:246 ./src/pyams_zfiles/zmi/search.py:105
+#: ./src/pyams_zfiles/interfaces.py:263 ./src/pyams_zfiles/zmi/search.py:105
 msgid "Name of the principal which created the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:250
+#: ./src/pyams_zfiles/interfaces.py:267
 msgid "Document owner"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:251
+#: ./src/pyams_zfiles/interfaces.py:268
 msgid "Name of the principal which is owner of the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:255
+#: ./src/pyams_zfiles/interfaces.py:272
 msgid "Document readers"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:256
+#: ./src/pyams_zfiles/interfaces.py:273
 msgid "Name of principals allowed to read the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:260
+#: ./src/pyams_zfiles/interfaces.py:277
 msgid "Document managers"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:261
+#: ./src/pyams_zfiles/interfaces.py:278
 msgid "Name of principals allowed to update the document"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:296
+#: ./src/pyams_zfiles/interfaces.py:313
 msgid "Documents OID prefix"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:297
+#: ./src/pyams_zfiles/interfaces.py:314
 msgid ""
 "Prefix used to identify documents which were created locally (unlike "
 "documents which were created into another documents container and "
 "synchronized with this container)"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:303
+#: ./src/pyams_zfiles/interfaces.py:320
 msgid "Access menu from home"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:304
+#: ./src/pyams_zfiles/interfaces.py:321
 msgid ""
 "If 'yes', a menu will be displayed to get access to documents container from "
 "site admin home page"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:336
+#: ./src/pyams_zfiles/interfaces.py:353
 msgid "Application managers"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:337
+#: ./src/pyams_zfiles/interfaces.py:354
 msgid ""
 "These principals can only manage application properties; documents manager "
 "role is required to manage documents!"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:344
+#: ./src/pyams_zfiles/interfaces.py:361
 msgid "Documents creators"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:345
+#: ./src/pyams_zfiles/interfaces.py:362
 msgid "These principals will be allowed to create or import new documents"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:350
+#: ./src/pyams_zfiles/interfaces.py:367
 msgid "Documents managers"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:351
+#: ./src/pyams_zfiles/interfaces.py:368
 msgid "These principals will be allowed to manage any document properties"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:356
+#: ./src/pyams_zfiles/interfaces.py:373
 msgid "Documents readers"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:357
+#: ./src/pyams_zfiles/interfaces.py:374
 msgid "These principals will be allowed to read any document properties"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:393
+#: ./src/pyams_zfiles/interfaces.py:410
 msgid "Configuration name"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:394
+#: ./src/pyams_zfiles/interfaces.py:411
 msgid "Unique name of the configuration"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:398
+#: ./src/pyams_zfiles/interfaces.py:415
 msgid "Remote XML-RPC endpoint"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:399
+#: ./src/pyams_zfiles/interfaces.py:416
 msgid ""
 "URL of the remote documents container XML-RPC endpoint used for "
 "synchronization"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:403
+#: ./src/pyams_zfiles/interfaces.py:420
 msgid "User name"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:404
+#: ./src/pyams_zfiles/interfaces.py:421
 msgid "Name of the remote user used for synchronization"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:407
+#: ./src/pyams_zfiles/interfaces.py:424
 msgid "Password"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:408
+#: ./src/pyams_zfiles/interfaces.py:425
 msgid "Password of the remote user used for synchronization"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:411
+#: ./src/pyams_zfiles/interfaces.py:428
 msgid "Enabled configuration"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:412
+#: ./src/pyams_zfiles/interfaces.py:429
 msgid "If 'no', this configuration will not be usable for synchronization"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:424
+#: ./src/pyams_zfiles/interfaces.py:441
 msgid "Configuration users"
 msgstr ""
 
-#: ./src/pyams_zfiles/interfaces.py:425
+#: ./src/pyams_zfiles/interfaces.py:442
 msgid "Principals which are granted permission to call this configuration"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:63
-msgid "draft created"
-msgstr ""
-
-#: ./src/pyams_zfiles/workflow.py:64
-msgid "published"
-msgstr ""
-
-#: ./src/pyams_zfiles/workflow.py:65
-msgid "archived"
-msgstr ""
-
-#: ./src/pyams_zfiles/workflow.py:120
+#: ./src/pyams_zfiles/workflow.py:93
 #, python-format
 msgid "Published version {0}"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:147
+#: ./src/pyams_zfiles/workflow.py:120
 msgid "Initialize"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:150
+#: ./src/pyams_zfiles/workflow.py:123
 msgid "Draft creation"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:153
+#: ./src/pyams_zfiles/workflow.py:126
 msgid "Publish"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:160
+#: ./src/pyams_zfiles/workflow.py:133
 msgid "Content published"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:164
+#: ./src/pyams_zfiles/workflow.py:137
 msgid "Archive content"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:170
+#: ./src/pyams_zfiles/workflow.py:143
 msgid "Content archived"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:174 ./src/pyams_zfiles/workflow.py:186
+#: ./src/pyams_zfiles/workflow.py:147 ./src/pyams_zfiles/workflow.py:159
 msgid "Create new version"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:182 ./src/pyams_zfiles/workflow.py:194
+#: ./src/pyams_zfiles/workflow.py:155 ./src/pyams_zfiles/workflow.py:167
 msgid "New version created"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:198
+#: ./src/pyams_zfiles/workflow.py:171
 msgid "Delete version"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:205
+#: ./src/pyams_zfiles/workflow.py:178
 msgid "Version deleted"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:222
+#: ./src/pyams_zfiles/workflow.py:195
 msgid "ZFiles document workflow"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:268 ./src/pyams_zfiles/workflow.py:301
+#: ./src/pyams_zfiles/workflow.py:241 ./src/pyams_zfiles/workflow.py:274
 #, python-format
 msgid "{state} {date}"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:272 ./src/pyams_zfiles/workflow.py:297
+#: ./src/pyams_zfiles/workflow.py:245 ./src/pyams_zfiles/workflow.py:270
 msgid "Unknown state"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:295
+#: ./src/pyams_zfiles/workflow.py:268
 msgid "new version created"
 msgstr ""
 
-#: ./src/pyams_zfiles/workflow.py:299
+#: ./src/pyams_zfiles/workflow.py:272
 msgid "publication refused"
 msgstr ""
 
-#: ./src/pyams_zfiles/utility.py:245
+#: ./src/pyams_zfiles/utility.py:244
 msgid "Document content update"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/synchronizer.py:88
 msgid "Click icon to enable or disable configuration"
 msgstr ""
 
@@ -469,16 +466,15 @@
 msgid "Search document"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:65
 msgid "Document OID"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/search.py:69 ./src/pyams_zfiles/api/rest.py:129
-#: ./src/pyams_zfiles/api/rest.py:148 ./src/pyams_zfiles/api/graph.py:76
+#: ./src/pyams_zfiles/zmi/search.py:69 ./src/pyams_zfiles/api/graph.py:76
 #: ./src/pyams_zfiles/api/graph.py:131 ./src/pyams_zfiles/api/graph.py:149
 msgid "Document version"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:76 ./src/pyams_zfiles/api/graph.py:175
 #: ./src/pyams_zfiles/api/graph.py:211
 msgid "Source application"
@@ -505,16 +501,15 @@
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:95
 msgid ""
 "Document tag; you can enter several tags by separating them with semicolons"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/search.py:99 ./src/pyams_zfiles/api/rest.py:74
-#: ./src/pyams_zfiles/api/rest.py:165 ./src/pyams_zfiles/api/graph.py:132
+#: ./src/pyams_zfiles/zmi/search.py:99 ./src/pyams_zfiles/api/graph.py:132
 #: ./src/pyams_zfiles/api/graph.py:150
 msgid "Document status"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:100
 msgid "Workflow state of searched documents"
 msgstr ""
@@ -541,16 +536,15 @@
 msgid "Name of the principal owning the document"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:118
 msgid "Updater"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/search.py:119 ./src/pyams_zfiles/api/rest.py:137
-#: ./src/pyams_zfiles/api/rest.py:179 ./src/pyams_zfiles/api/graph.py:79
+#: ./src/pyams_zfiles/zmi/search.py:119 ./src/pyams_zfiles/api/graph.py:79
 msgid "Last document updater principal ID"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:122
 msgid "Modification dates"
 msgstr ""
 
@@ -560,16 +554,15 @@
 "last time; first date is included, second one is excluded"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:129
 msgid "Status updater"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/search.py:130 ./src/pyams_zfiles/api/rest.py:139
-#: ./src/pyams_zfiles/api/rest.py:184
+#: ./src/pyams_zfiles/zmi/search.py:130
 msgid "Last workflow status updater principal ID"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/search.py:133
 msgid "Status update dates"
 msgstr ""
 
@@ -627,187 +620,116 @@
 msgid "Documents container configuration"
 msgstr ""
 
 #: ./src/pyams_zfiles/zmi/__init__.py:126
 msgid "Base configuration"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/workflow.py:79
+#: ./src/pyams_zfiles/zmi/workflow.py:80
 msgid "Delete definitively"
 msgstr ""
 
-#: ./src/pyams_zfiles/zmi/document.py:99 ./src/pyams_zfiles/api/rest.py:206
+#: ./src/pyams_zfiles/zmi/document.py:99
 msgid "Document properties"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:50
-msgid "List of requested fields names"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:63 ./src/pyams_zfiles/api/rest.py:101
 #: ./src/pyams_zfiles/api/graph.py:60 ./src/pyams_zfiles/api/graph.py:177
 msgid "File name"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:66 ./src/pyams_zfiles/api/graph.py:61
+#: ./src/pyams_zfiles/api/graph.py:61
 msgid "Document custom properties"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:68
-msgid "List of document tags"
+#: ./src/pyams_zfiles/api/graph.py:63
+msgid "Document workflow state"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:71 ./src/pyams_zfiles/api/rest.py:122
-#: ./src/pyams_zfiles/api/rest.py:136 ./src/pyams_zfiles/api/rest.py:176
 #: ./src/pyams_zfiles/api/graph.py:64 ./src/pyams_zfiles/api/graph.py:217
 msgid "Current document owner"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:84 ./src/pyams_zfiles/api/graph.py:66
-msgid "Document readers IDs"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:91 ./src/pyams_zfiles/api/graph.py:68
-msgid "Document managers IDs"
+#: ./src/pyams_zfiles/api/graph.py:65
+msgid "Document access mode"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:98 ./src/pyams_zfiles/api/rest.py:114
-msgid "Document data; may be provided in Base64 when using JSON"
+#: ./src/pyams_zfiles/api/graph.py:66
+msgid "Document readers IDs"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:112 ./src/pyams_zfiles/api/graph.py:213
-msgid "Document file name"
+#: ./src/pyams_zfiles/api/graph.py:67
+msgid "Document update mode"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:120 ./src/pyams_zfiles/api/rest.py:135
-#: ./src/pyams_zfiles/api/graph.py:78
-msgid "Document creation timestamp"
+#: ./src/pyams_zfiles/api/graph.py:68
+msgid "Document managers IDs"
 msgstr ""
 
-#. 
 #. read-only attributes
-#: ./src/pyams_zfiles/api/rest.py:127 ./src/pyams_zfiles/api/graph.py:70
+#: ./src/pyams_zfiles/api/graph.py:70
 msgid "Document base REST API URL"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:130 ./src/pyams_zfiles/api/graph.py:72
+#: ./src/pyams_zfiles/api/graph.py:72
 msgid "Absolute URL of document data file"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:131 ./src/pyams_zfiles/api/rest.py:157
 #: ./src/pyams_zfiles/api/graph.py:73
 msgid "SHA512 hash of document data file"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:132 ./src/pyams_zfiles/api/graph.py:74
+#: ./src/pyams_zfiles/api/graph.py:74
 msgid "Document file size"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:133 ./src/pyams_zfiles/api/graph.py:75
+#: ./src/pyams_zfiles/api/graph.py:75
 msgid "Document content type"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:134 ./src/pyams_zfiles/api/rest.py:171
 #: ./src/pyams_zfiles/api/graph.py:77
 msgid "Document creator principal ID"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/rest.py:138 ./src/pyams_zfiles/api/graph.py:80
-msgid "Last document update timestamp"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:140 ./src/pyams_zfiles/api/graph.py:82
-msgid "Last document status update timestamp"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:145
-msgid "Document unique identifiers"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:160
-msgid "Document properties, provided as a mapping"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:162
-msgid "Document tags, separated with semicolons"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:173 ./src/pyams_zfiles/api/graph.py:109
-msgid "Document creation dates range"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:181
-msgid "Document last update dates range"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:186
-msgid "Last workflow status update dates range"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:188
-msgid "List of requested field names"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:194
-msgid "List of documents to import in remote documents container"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:197
-msgid "List of documents to remove from remote documents container"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:201
-msgid "Selected configuration name"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:207
-msgid "Document created"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:208
-msgid "Document not found"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:209
-msgid "Forbidden access"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/rest.py:210
-msgid "Missing arguments"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/graph.py:63
-msgid "Document workflow state"
-msgstr ""
-
-#: ./src/pyams_zfiles/api/graph.py:65
-msgid "Document access mode"
+#: ./src/pyams_zfiles/api/graph.py:78
+msgid "Document creation timestamp"
 msgstr ""
 
-#: ./src/pyams_zfiles/api/graph.py:67
-msgid "Document update mode"
+#: ./src/pyams_zfiles/api/graph.py:80
+msgid "Last document update timestamp"
 msgstr ""
 
 #: ./src/pyams_zfiles/api/graph.py:81
 msgid "Last document status updater principal ID"
 msgstr ""
 
+#: ./src/pyams_zfiles/api/graph.py:82
+msgid "Last document status update timestamp"
+msgstr ""
+
 #: ./src/pyams_zfiles/api/graph.py:87 ./src/pyams_zfiles/api/graph.py:179
 #: ./src/pyams_zfiles/api/graph.py:215
 msgid "Document data in Base64 encoding"
 msgstr ""
 
 #: ./src/pyams_zfiles/api/graph.py:104
 msgid "Properties query string"
 msgstr ""
 
+#: ./src/pyams_zfiles/api/graph.py:109
+msgid "Document creation dates range"
+msgstr ""
+
 #: ./src/pyams_zfiles/api/graph.py:113
 msgid "Document last modification dates range"
 msgstr ""
 
 #: ./src/pyams_zfiles/api/graph.py:116
 msgid "Document last workflow update dates range"
 msgstr ""
 
+#: ./src/pyams_zfiles/api/graph.py:213
+msgid "Document file name"
+msgstr ""
+
 #: ./src/pyams_zfiles/api/graph.py:219
 msgid "Document creation date"
 msgstr ""
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/search.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,32 @@
 from pyams_utils.timezone import gmtime
 
 
 __docformat__ = 'restructuredtext'
 
 
 NULL_STRING = 'null'
+LIST_SEPARATOR = ','
 
 
 def get_list(value):
     """Check and convert given value to a set, if required
 
     >>> from pyams_zfiles.search import get_list
     >>> get_list(None) is None
     True
     >>> get_list('') is None
     True
-    >>> get_list('value1;value2')
+    >>> get_list('value1,value2')
+    ['value1', 'value2']
+    >>> get_list('value1, value2 ')
     ['value1', 'value2']
     """
     if value and isinstance(value, str):
-        value = list(map(str.strip, value.split(';')))
+        value = list(map(str.strip, value.split(LIST_SEPARATOR)))
     return value or None
 
 
 def get_properties(value):
     """Check and convert given mapping value to a list of properties
 
     >>> from pprint import pprint
@@ -155,15 +158,15 @@
     (datetime.datetime(2021, 12, 1, 0, 0, tzinfo=<StaticTzInfo 'GMT'>),
      datetime.datetime(2021, 12, 3, 0, 0, tzinfo=<StaticTzInfo 'GMT'>))
     >>> get_range('2021-12-01,2021-12-03')
     (datetime.datetime(2021, 12, 1, 0, 0, tzinfo=<StaticTzInfo 'GMT'>),
      datetime.datetime(2021, 12, 3, 0, 0, tzinfo=<StaticTzInfo 'GMT'>))
     """
     if isinstance(value, str):
-        value = value.split(',')
+        value = value.split(LIST_SEPARATOR)
     return tuple(map(get_date, value))
 
 
 class InList:
     """Check for list items
 
     Items are provided as a dict of sets, where dict keys are the names of searched properties
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/skin/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/skin/container.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/skin/container.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/skin/file.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/skin/file.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/synchronizer.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/tests/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/tests/test_utilsdocs.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/tests/test_utilsdocstrings.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/utility.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,16 @@
 from pyams_utils.registry import get_utility, query_utility
 from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 from pyams_workflow.interfaces import IWorkflowInfo, IWorkflowState, IWorkflowVersions
 from pyams_workflow.versions import get_last_version
 from pyams_zfiles.document import Document, DocumentVersion, get_hash
 from pyams_zfiles.folder import DocumentFolder
-from pyams_zfiles.interfaces import CREATE_DOCUMENT_WITH_OWNER_PERMISSION, DELETED_STATE, \
-    DRAFT_STATE, IDocumentContainer, IDocumentContainerRoles, IDocumentFolder, \
-    IDocumentVersion, MANAGE_DOCUMENT_PERMISSION, READ_DOCUMENT_PERMISSION
+from pyams_zfiles.interfaces import CREATE_DOCUMENT_WITH_OWNER_PERMISSION, IDocumentContainer, IDocumentContainerRoles, \
+    IDocumentFolder, IDocumentVersion, MANAGE_DOCUMENT_PERMISSION, READ_DOCUMENT_PERMISSION, STATE
 from pyams_zfiles.search import make_query
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_zfiles import _
 
@@ -233,25 +232,25 @@
                 data = None
                 _filename = properties.pop('filename', None)
             else:
                 # modified file content, check state and create new version if required
                 if request is None:
                     request = check_request()
                 state = IWorkflowState(document)
-                if state.state != DRAFT_STATE:
+                if state.state != STATE.DRAFT.value:
                     translate = request.localizer.translate
                     workflow_info = IWorkflowInfo(document)
                     document = workflow_info.fire_transition_toward(  # pylint: disable=assignment-from-no-return
-                        DRAFT_STATE,
+                        STATE.DRAFT.value,
                         comment=translate(_("Document content update")),
                         request=request)
                     request.response.status = HTTPCreated.code
         state = document.update(data, properties)
         request.registry.notify(ObjectModifiedEvent(document))
-        if state.state == DELETED_STATE:
+        if state.state == STATE.DELETED.value:
             return None
         return document
 
     def delete_document(self, oid, request=None):
         """Delete document or version"""
         if not oid:
             return None
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/workflow.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,111 +16,84 @@
 """
 
 from datetime import datetime
 
 from zope.copy import copy
 from zope.interface import implementer
 from zope.location import locate
-from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_utils.adapter import ContextAdapter, adapter_config
 from pyams_utils.date import format_datetime
 from pyams_utils.registry import get_pyramid_registry, utility_config
 from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 from pyams_workflow.interfaces import IWorkflow, IWorkflowInfo, IWorkflowPublicationInfo, \
     IWorkflowState, IWorkflowStateLabel, IWorkflowVersions, ObjectClonedEvent
 from pyams_workflow.workflow import Transition, Workflow
-from pyams_zfiles.interfaces import ARCHIVED_STATE, DELETED_STATE, DRAFT_STATE, \
-    IDocument, IDocumentFolder, IDocumentWorkflow, MANAGE_DOCUMENT_PERMISSION, PUBLISHED_STATE, \
-    ZFILES_WORKFLOW_NAME
+from pyams_zfiles.interfaces import IDocument, IDocumentFolder, IDocumentWorkflow, MANAGE_DOCUMENT_PERMISSION, STATE, \
+    STATES_HEADERS, STATES_VOCABULARY, ZFILES_WORKFLOW_NAME
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_zfiles import _
 
 
-STATES_IDS = (
-    DRAFT_STATE,
-    PUBLISHED_STATE,
-    ARCHIVED_STATE,
-    DELETED_STATE
-)
-
-STATES_LABELS = (
-    _("Draft"),
-    _("Published"),
-    _("Archived"),
-    _("Deleted")
-)
-
-STATES_VOCABULARY = SimpleVocabulary([
-    SimpleTerm(STATES_IDS[i], title=t)
-    for i, t in enumerate(STATES_LABELS)
-])
-
-STATES_HEADERS = {
-    DRAFT_STATE: _("draft created"),
-    PUBLISHED_STATE: _("published"),
-    ARCHIVED_STATE: _("archived")
-}
-
-UPDATE_STATES = (DRAFT_STATE, PUBLISHED_STATE)
+UPDATE_STATES = (STATE.DRAFT.value, STATE.PUBLISHED.value)
 '''Default states available in update mode'''
 
-READONLY_STATES = (ARCHIVED_STATE, DELETED_STATE)
+READONLY_STATES = (STATE.ARCHIVED.value, STATE.DELETED.value)
 '''Retired and archived contents can't be modified'''
 
 PROTECTED_STATES = ()
 '''Protected states are available to managers in update mode'''
 
 MANAGER_STATES = ()
 '''No custom state available to managers!'''
 
-PUBLISHED_STATES = (PUBLISHED_STATE,)
+PUBLISHED_STATES = (STATE.PUBLISHED.value,)
 '''Pre-published and published states are marked as published'''
 
-VISIBLE_STATES = (PUBLISHED_STATE,)
+VISIBLE_STATES = (STATE.PUBLISHED.value,)
 '''Only published state is visible in front-office'''
 
 WAITING_STATES = ()
 
 RETIRED_STATES = ()
 
-ARCHIVED_STATES = (ARCHIVED_STATE,)
+ARCHIVED_STATES = (STATE.ARCHIVED.value,)
 
 
 #
 # Workflow conditions
 #
 
 def can_create_new_version(wf, context):  # pylint: disable=invalid-name,unused-argument
     """Check if we can create a new version"""
     # can't create new version when previous draft already exists
     versions = IWorkflowVersions(context)
-    return not versions.has_version(DRAFT_STATE)
+    return not versions.has_version(STATE.DRAFT.value)
 
 
 #
 # Workflow actions
 #
 
 def publish_action(wf, context):  # pylint: disable=invalid-name,unused-argument
     """Publish version"""
     request = check_request()
     translate = request.localizer.translate
     publication_info = IWorkflowPublicationInfo(context)
     publication_info.publication_date = datetime.utcnow()
     publication_info.publisher = request.principal.id
     version_id = IWorkflowState(context).version_id
-    for version in IWorkflowVersions(context).get_versions((PUBLISHED_STATE, )):
+    for version in IWorkflowVersions(context).get_versions((STATE.PUBLISHED.value, )):
         if version is not context:
             IWorkflowInfo(version).fire_transition_toward(
-                ARCHIVED_STATE,
+                STATE.ARCHIVED.value,
                 comment=translate(_("Published version {0}")).format(version_id))
 
 
 def clone_action(wf, context):  # pylint: disable=invalid-name,unused-argument
     """Create new version"""
     result = copy(context)
     locate(result, context.__parent__)
@@ -142,66 +115,66 @@
 #
 # Workflow transitions
 #
 
 init = Transition(transition_id='init',
                   title=_("Initialize"),
                   source=None,
-                  destination=DRAFT_STATE,
+                  destination=STATE.DRAFT.value,
                   history_label=_("Draft creation"))
 
 draft_to_published = Transition(transition_id='draft_to_published',
                                 title=_("Publish"),
-                                source=DRAFT_STATE,
-                                destination=PUBLISHED_STATE,
+                                source=STATE.DRAFT.value,
+                                destination=STATE.PUBLISHED.value,
                                 permission=MANAGE_DOCUMENT_PERMISSION,
                                 action=publish_action,
                                 menu_icon_class='far fa-fw fa-thumbs-up',
                                 view_name='wf-publish.html',
                                 history_label=_("Content published"),
                                 order=1)
 
 published_to_archived = Transition(transition_id='published_to_archived',
                                    title=_("Archive content"),
-                                   source=PUBLISHED_STATE,
-                                   destination=ARCHIVED_STATE,
+                                   source=STATE.PUBLISHED.value,
+                                   destination=STATE.ARCHIVED.value,
                                    permission=MANAGE_DOCUMENT_PERMISSION,
                                    menu_icon_class='fas fa-fw fa-archive',
                                    view_name='wf-archive.html',
                                    history_label=_("Content archived"),
                                    order=2)
 
 published_to_draft = Transition(transition_id='published_to_draft',
                                 title=_("Create new version"),
-                                source=PUBLISHED_STATE,
-                                destination=DRAFT_STATE,
+                                source=STATE.PUBLISHED.value,
+                                destination=STATE.DRAFT.value,
                                 permission=MANAGE_DOCUMENT_PERMISSION,
                                 condition=can_create_new_version,
                                 action=clone_action,
                                 menu_icon_class='far fa-fw fa-copy',
                                 view_name='wf-clone.html',
                                 history_label=_("New version created"),
                                 order=3)
 
 archived_to_draft = Transition(transition_id='archived_to_draft',
                                title=_("Create new version"),
-                               source=ARCHIVED_STATE,
-                               destination=DRAFT_STATE,
+                               source=STATE.ARCHIVED.value,
+                               destination=STATE.DRAFT.value,
                                permission=MANAGE_DOCUMENT_PERMISSION,
                                condition=can_create_new_version,
                                action=clone_action,
                                menu_icon_class='far fa-fw fa-copy',
                                view_name='wf-clone.html',
                                history_label=_("New version created"),
                                order=4)
 
 delete = Transition(transition_id='delete',
                     title=_("Delete version"),
-                    source=DRAFT_STATE,
-                    destination=DELETED_STATE,
+                    source=STATE.DRAFT.value,
+                    destination=STATE.DELETED.value,
                     permission=MANAGE_DOCUMENT_PERMISSION,
                     action=delete_action,
                     menu_icon_class='fa fa-fw fa-trash',
                     view_name='wf-delete.html',
                     history_label=_("Version deleted"),
                     order=99)
 
@@ -220,15 +193,15 @@
     """PyAMS basic workflow"""
 
     label = _("ZFiles document workflow")
 
 
 ZFILES_WORKFLOW = DocumentWorkflow(wf_transitions,
                                    states=STATES_VOCABULARY,
-                                   initial_state=DRAFT_STATE,
+                                   initial_state=STATE.DRAFT.value,
                                    update_states=UPDATE_STATES,
                                    readonly_states=READONLY_STATES,
                                    protected_states=PROTECTED_STATES,
                                    manager_states=MANAGER_STATES,
                                    published_states=PUBLISHED_STATES,
                                    visible_states=VISIBLE_STATES,
                                    waiting_states=WAITING_STATES,
@@ -269,15 +242,15 @@
                     state=state_label,
                     date=format_datetime(state.state_date))
         else:
             state_label = translate(_("Unknown state"))
         return state_label
 
 
-@adapter_config(name=DRAFT_STATE,
+@adapter_config(name=STATE.DRAFT.value,
                 required=IDocumentWorkflow,
                 provides=IWorkflowStateLabel)
 class DraftWorkflowStateLabelAdapter(ContextAdapter):
     """Draft state label adapter"""
 
     @staticmethod
     def get_label(content, request=None, format=True):  # pylint: disable=redefined-builtin
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/__init__.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/document.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/document.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/properties.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/search.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/synchronizer.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles/zmi/workflow.py` & `pyams_zfiles-1.4.4/src/pyams_zfiles/zmi/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
 from pyams_utils.registry import get_utility
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_workflow.interfaces import IWorkflowState, IWorkflowVersion, IWorkflowVersions
 from pyams_workflow.zmi.transition import WorkflowContentTransitionForm
-from pyams_zfiles.interfaces import DELETED_STATE, IDocument, IDocumentContainer, IDocumentFolder, IDocumentVersion, \
-    MANAGE_DOCUMENT_PERMISSION
+from pyams_zfiles.interfaces import IDocument, IDocumentContainer, IDocumentFolder, IDocumentVersion, \
+    MANAGE_DOCUMENT_PERMISSION, STATE
 from pyams_zmi.interfaces import IAdminLayer
 
+
 __docformat__ = 'restructuredtext'
 
 from pyams_zfiles import _
 
 
 class BaseWorkflowForm(WorkflowContentTransitionForm):
     """Base workflow form"""
@@ -84,15 +85,15 @@
         if state.version_id == 1:  # remove the first and only version => remove all
             document = get_parent(self.context, IDocument)
             target = get_parent(document, IDocumentFolder)
             del target[document.__name__]
         else:
             versions = IWorkflowVersions(self.context)
             versions.remove_version(state.version_id,
-                                    state=DELETED_STATE,
+                                    state=STATE.DELETED.value,
                                     comment=data.get('comment'))
             target = versions.get_last_versions(count=1)[0]
         return target
 
     @property
     def deleted_target(self):
         """Redirect target when current content is deleted"""
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/PKG-INFO` & `pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-zfiles
-Version: 1.4.3
+Version: 1.4.4
 Summary: PyAMS files storage manager
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,19 @@
 ZFiles is just a storage manager for these documents; the lifecycle management is delegated to
 the applications which use it as storage backend.
 
 
 Changelog
 =========
 
+1.4.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+ - added enums for workflow states
+
 1.4.3
 -----
  - updated translations
 
 1.4.2
 -----
  - updated workflow delete view
```

### Comparing `pyams_zfiles-1.4.3/src/pyams_zfiles.egg-info/SOURCES.txt` & `pyams_zfiles-1.4.4/src/pyams_zfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

