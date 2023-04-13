# Comparing `tmp/pyams_thesaurus-1.3.3.tar.gz` & `tmp/pyams_thesaurus-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_thesaurus-1.3.3.tar", last modified: Mon Feb  6 08:37:04 2023, max compression
+gzip compressed data, was "dist/pyams_thesaurus-1.3.4.tar", last modified: Thu Apr 13 12:51:07 2023, max compression
```

## Comparing `pyams_thesaurus-1.3.3.tar` & `pyams_thesaurus-1.3.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2971 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1185 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2876 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/api/
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6720 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    20045 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/data/
--rw-rw-rw-   0 root         (0) root         (0)  2939491 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
--rw-rw-rw-   0 root         (0) root         (0)  2735784 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/
--rw-rw-rw-   0 root         (0) root         (0)     2049 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/extension.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/index.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     7494 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/term.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/
--rw-rw-rw-   0 root         (0) root         (0)    10069 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10638 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/skos.py
--rw-rw-rw-   0 root         (0) root         (0)     8442 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/superdoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13444 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
--rw-rw-rw-   0 root         (0) root         (0)    21406 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
--rw-rw-rw-   0 root         (0) root         (0)    16589 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/pyams_thesaurus.pot
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    19509 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    21783 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/extension.py
--rw-rw-rw-   0 root         (0) root         (0)    15093 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    16738 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
--rw-rw-rw-   0 root         (0) root         (0)     7147 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/sass/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/extract-terms.pt
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/terms-tree.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
--rw-rw-rw-   0 root         (0) root         (0)    13424 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/test.py
--rw-rw-rw-   0 root         (0) root         (0)     8168 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/thesaurus.py
--rw-rw-rw-   0 root         (0) root         (0)    13892 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/tree.py
--rw-rw-rw-   0 root         (0) root         (0)     9096 2023-02-06 08:36:42.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2971 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2518 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      345 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-02-06 08:37:04.000000 pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2876 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7316 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    20142 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/
+-rw-rw-rw-   0 root         (0) root         (0)  2939491 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2735784 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7494 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/
+-rw-rw-rw-   0 root         (0) root         (0)    10069 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10638 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/skos.py
+-rw-rw-rw-   0 root         (0) root         (0)     8442 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/superdoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13065 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
+-rw-rw-rw-   0 root         (0) root         (0)    21065 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/pyams_thesaurus.pot
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    19509 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    21783 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)    15093 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    16738 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
+-rw-rw-rw-   0 root         (0) root         (0)     7147 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/extract-terms.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/terms-tree.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)    13424 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     8168 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/thesaurus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13892 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     9096 2023-04-13 12:50:45.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-13 12:51:07.000000 pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/top_level.txt
```

### Comparing `pyams_thesaurus-1.3.3/LICENSE` & `pyams_thesaurus-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/PKG-INFO` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_thesaurus
-Version: 1.3.3
+Name: pyams-thesaurus
+Version: 1.3.4
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -49,14 +49,22 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+1.3.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
+1.3.3
+-----
+ - version mismatch
+
 1.3.2
 -----
  - added check for undefined thesaurus name in terms selection widget
  - added support for Python 3.11
 
 1.3.1
 -----
```

### Comparing `pyams_thesaurus-1.3.3/docs/HISTORY.rst` & `pyams_thesaurus-1.3.4/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.3.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
+1.3.3
+-----
+ - version mismatch
+
 1.3.2
 -----
  - added check for undefined thesaurus name in terms selection widget
  - added support for Python 3.11
 
 1.3.1
 -----
```

### Comparing `pyams_thesaurus-1.3.3/docs/README.rst` & `pyams_thesaurus-1.3.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/setup.py` & `pyams_thesaurus-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.3.3'
+version = '1.3.4'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/api/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/api/rest.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/api/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,193 +15,204 @@
 Thesaurus REST API module.
 """
 
 import sys
 
 from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
-from cornice.validators import colander_querystring_validator
+from cornice.validators import colander_validator
 from hypatia.text import ParseError
-from pyramid.httpexceptions import HTTPOk
+from pyramid.httpexceptions import HTTPBadRequest, HTTPOk
 
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_thesaurus.interfaces import REST_EXTRACTS_GETTER_ROUTE, REST_TERMS_SEARCH_ROUTE
-
-
-__docformat__ = 'restructuredtext'
-
-from pyams_thesaurus import _
 from pyams_thesaurus.interfaces.term import STATUS_ARCHIVED
 from pyams_thesaurus.interfaces.thesaurus import IThesaurus, IThesaurusExtracts
 from pyams_utils.list import unique
 from pyams_utils.registry import query_utility
+from pyams_utils.rest import BaseResponseSchema, BaseStatusSchema, STATUS, http_error, rest_responses
+
+
+__docformat__ = 'restructuredtext'
 
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
 #
 # Thesaurus extracts getter services
 #
 
-class ThesaurusExtractsGetterSchema(MappingSchema):
+class ThesaurusExtractsQuery(MappingSchema):
     """Thesaurus extracts getter schema"""
     thesaurus_name = SchemaNode(String(),
-                                description=_("Selected thesaurus name"))
+                                description="Selected thesaurus name")
 
 
-class ThesaurusExtractResultSchema(MappingSchema):
+class ThesaurusExtract(MappingSchema):
     """Thesaurus extracts getter result schema"""
+    id = SchemaNode(String(),
+                    description="Extract ID")
+    text = SchemaNode(String(),
+                      description="Extract name")
 
 
-class ThesaurusExtractsResults(SequenceSchema):
+class ThesaurusExtractsList(SequenceSchema):
     """Thesaurus extracts result schema"""
-    result = ThesaurusExtractResultSchema()
+    extract = ThesaurusExtract()
 
 
-class ThesaurusExtractsResultsSchema(MappingSchema):
+class ThesaurusExtractsSearchResults(BaseStatusSchema):
     """Thesaurus extracts results schema"""
-    results = ThesaurusExtractsResults(description=_("Results list"))
-
-
-extracts_search_response = {
-    HTTPOk.code: ThesaurusExtractsResultsSchema(description=_("Search results"))
-}
-if TEST_MODE:
-    extracts_service_params = {}
-else:
-    extracts_service_params = {
-        'response_schemas': extracts_search_response
-    }
+    results = ThesaurusExtractsList(description="Thesaurus extracts list",
+                                    missing=drop)
 
 
 extracts_service = Service(name=REST_EXTRACTS_GETTER_ROUTE,
                            pyramid_route=REST_EXTRACTS_GETTER_ROUTE,
                            description="Thesaurus extracts management")
 
 
-@extracts_service.options(validators=(check_cors_origin, set_cors_headers),
-                          **extracts_service_params)
+@extracts_service.options(validators=(check_cors_origin, set_cors_headers))
 def extracts_options(request):  # pylint: disable=unused-argument
     """Extracts service OPTIONS handler"""
     return ''
 
 
+class ThesaurusExtractsRequest(MappingSchema):
+    """Thesaurus extracts request"""
+    querystring = ThesaurusExtractsQuery()
+
+
+class ThesaurusExtractsResponse(MappingSchema):
+    """Thesaurus extracts getter response"""
+    body = ThesaurusExtractsSearchResults()
+
+
+extracts_get_responses = rest_responses.copy()
+extracts_get_responses[HTTPOk.code] = ThesaurusExtractsResponse(
+    description="Thesaurus extracts query response")
+
+
 @extracts_service.get(permission=VIEW_SYSTEM_PERMISSION,
-                      schema=ThesaurusExtractsGetterSchema(),
-                      validators=(check_cors_origin, colander_querystring_validator,
-                                  set_cors_headers),
-                      **extracts_service_params)
+                      schema=ThesaurusExtractsRequest(),
+                      validators=(check_cors_origin, colander_validator, set_cors_headers),
+                      response_schemas=extracts_get_responses)
 def get_extracts(request):
     """Get thesaurus extracts list"""
-    if TEST_MODE:
-        thesaurus_name = request.params.get('thesaurus_name')
-    else:
-        thesaurus_name = request.validated.get('thesaurus_name')
+    params = request.params if TEST_MODE else request.validated.get('querystring', {})
+    thesaurus_name = params.get('thesaurus_name')
     if not thesaurus_name:
-        return {}
+        return http_error(request, HTTPBadRequest, 'missing argument')
     thesaurus = query_utility(IThesaurus, name=thesaurus_name)
     if thesaurus is None:
-        return {}
+        return http_error(request, HTTPBadRequest, 'bad thesaurus name')
     extracts = IThesaurusExtracts(thesaurus)
     return {
+        'status': STATUS.SUCCESS.value,
         'results': [
             {
                 'id': extract.name,
                 'text': extract.name
             }
             for extract in extracts.values()
         ]
     }
 
 
 #
 # Thesaurus terms search services
 #
 
-class ThesaurusTermsSearchQuerySchema(MappingSchema):
+class ThesaurusTermsQuery(MappingSchema):
     """Thesaurus terms search schema"""
     thesaurus_name = SchemaNode(String(),
-                                description=_("Selected thesaurus name"))
+                                description="Selected thesaurus name")
     extract_name = SchemaNode(String(),
-                              description=_("Selected extract name"),
+                              description="Selected extract name",
                               missing=drop)
     term = SchemaNode(String(),
-                      description=_("Terms search string"))
+                      description="Terms search string")
 
 
-class ThesaurusTermResultSchema(MappingSchema):
-    """Thesaurus term result schema"""
+class ThesaurusTerm(MappingSchema):
+    """Thesaurus term"""
     id = SchemaNode(String(),
-                    description=_("Term ID"))
+                    description="Term ID")
     text = SchemaNode(String(),
-                      description=_("Term label"))
+                      description="Term label")
 
 
-class ThesaurusSearchResults(SequenceSchema):
+class ThesaurusTermsList(SequenceSchema):
     """Thesaurus search results interface"""
-    result = ThesaurusTermResultSchema()
+    term = ThesaurusTerm()
 
 
-class ThesaurusSearchResultsSchema(MappingSchema):
+class ThesaurusTermsSearchResults(BaseResponseSchema):
     """Thesaurus search results schema"""
-    results = ThesaurusSearchResults(description=_("Results list"))
-
-
-terms_search_response = {
-    HTTPOk.code: ThesaurusSearchResultsSchema(description=_("Search results"))
-}
-if TEST_MODE:
-    terms_service_params = {}
-else:
-    terms_service_params = {
-        'response_schemas': terms_search_response
-    }
+    results = ThesaurusTermsList(description="Results list",
+                                 missing=drop)
 
 
 terms_service = Service(name=REST_TERMS_SEARCH_ROUTE,
                         pyramid_route=REST_TERMS_SEARCH_ROUTE,
                         description="Thesaurus terms management")
 
 
-@terms_service.options(validators=(check_cors_origin, set_cors_headers),
-                       **terms_service_params)
+@terms_service.options(validators=(check_cors_origin, set_cors_headers))
 def terms_options(request):  # pylint: disable=unused-argument
     """Terms service OPTIONS handler"""
     return ''
 
 
+class ThesaurusTermsRequest(MappingSchema):
+    """Terms getter request"""
+    querystring = ThesaurusTermsQuery()
+
+
+class ThesaurusTermsResponse(MappingSchema):
+    """Terms getter response"""
+    body = ThesaurusTermsSearchResults()
+
+
+terms_get_responses = rest_responses.copy()
+terms_get_responses[HTTPOk.code] = ThesaurusTermsResponse(
+    description="List of terms matching given query")
+
+
 @terms_service.get(permission=VIEW_SYSTEM_PERMISSION,
-                   schema=ThesaurusTermsSearchQuerySchema(),
-                   validators=(check_cors_origin, colander_querystring_validator,
-                               set_cors_headers),
-                   **terms_service_params)
+                   schema=ThesaurusTermsRequest(),
+                   validators=(check_cors_origin, colander_validator, set_cors_headers),
+                   response_schemas=terms_get_responses)
 def get_terms(request):
     """Returns list of terms matching given query"""
-    if TEST_MODE:
-        thesaurus_name = request.params.get('thesaurus_name')
-        extract_name = request.params.get('extract_name')
-        query = request.params.get('term')
-    else:
-        thesaurus_name = request.validated.get('thesaurus_name')
-        extract_name = request.validated.get('extract_name')
-        query = request.validated.get('term')
+    params = request.params if TEST_MODE else request.validated.get('querystring', {})
+    thesaurus_name = params.get('thesaurus_name')
+    extract_name = params.get('extract_name')
+    query = params.get('term')
     if not (thesaurus_name or query):
-        return {}
+        return {
+            'status': STATUS.ERROR.value,
+            'message': "Missing arguments"
+        }
     thesaurus = query_utility(IThesaurus, name=thesaurus_name)
     if thesaurus is None:
-        return {}
+        return {
+            'status': STATUS.ERROR.value,
+            'message': "Thesaurus not found"
+        }
     try:
         return {
+            'status': STATUS.SUCCESS.value,
             'results': [
                 {
                     'id': term.label,
                     'text': term.label
                 }
                 for term in unique(thesaurus.find_terms(query, extract_name,
                                                         exact=True, stemmed=True))
                 if term.status != STATUS_ARCHIVED
             ]
         }
     except ParseError:
-        return []
+        return {}
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/README.rst` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     >>> config = setUp(hook_zca=True)
     >>> config.registry.settings['zodbconn.uri'] = 'memory://'
 
     >>> from pyramid_zodbconn import includeme as include_zodbconn
     >>> include_zodbconn(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
+    >>> from cornice_swagger import includeme as include_swagger
+    >>> include_swagger(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_i18n import includeme as include_i18n
     >>> include_i18n(config)
     >>> from pyams_security import includeme as include_security
     >>> include_security(config)
     >>> from pyams_catalog import includeme as include_catalog
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/interfaces.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/extension/html/zmi/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/extension/html/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/generations/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/include.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/include.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/index.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/extension.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/index.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/loader.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/loader.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/term.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/interfaces/thesaurus.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/interfaces/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/config.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/config.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/skos.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/skos.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/loader/superdoc.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/loader/superdoc.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -344,41 +344,29 @@
 
 msgid "Published"
 msgstr "Publié"
 
 msgid "Publisher"
 msgstr "Éditeur"
 
-msgid "Results list"
-msgstr "Liste de résultats"
-
 msgid "Rich text description"
 msgstr "Texte enrichi"
 
-msgid "Search results"
-msgstr "Résultats de la recherche"
-
 msgid "Search term..."
 msgstr "Rechercher un terme..."
 
 msgid "Select file encoding, for formats which don't provide it internally"
 msgstr ""
 "Sélectionner l'encodage si le format ne prend pas en charge cette information"
 
 msgid "Select file language, for formats which don't provide it internally"
 msgstr ""
 "Sélectionner la langue si le format sélectionné ne prend pas en charge cette "
 "information"
 
-msgid "Selected extract name"
-msgstr "Nom de l'extrait"
-
-msgid "Selected thesaurus name"
-msgstr "Nom du thésaurus"
-
 msgid "Short abbreviation used to distinguish the extract"
 msgstr "Courte abréviation utilisée pour identifier l'extrait"
 
 msgid "Show/hide extract"
 msgstr "Afficher/masquer l'extrait"
 
 msgid "Specifics terms"
@@ -389,17 +377,14 @@
 
 msgid "Subject"
 msgstr "Contenu"
 
 msgid "Synonyms"
 msgstr "Synonymes"
 
-msgid "Term ID"
-msgstr "Identifiant du terme"
-
 msgid "Term can't be deleted"
 msgstr "Ce terme ne peut pas être supprimé."
 
 msgid "Term label"
 msgstr "Libellé"
 
 msgid "Term not found"
@@ -416,17 +401,14 @@
 msgstr ""
 "Position du terme parmi ses termes frères ; lorsqu'il n'est pas spécifié, "
 "l'ordre par défaut est alphabétique"
 
 msgid "Term: {}"
 msgstr "Terme : {}"
 
-msgid "Terms search string"
-msgstr "Texte de recherche des termes"
-
 msgid "Terms tree"
 msgstr "Termes"
 
 msgid "Terms tree view"
 msgstr "Arborescence des termes"
 
 msgid "Test thesaurus widgets"
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS_thesaurus 1.0\n"
-"POT-Creation-Date: 2022-10-15 01:18+0200\n"
+"POT-Creation-Date: 2023-04-12 16:01+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -221,15 +221,15 @@
 msgstr "Créateur"
 
 #: src/pyams_thesaurus/interfaces/thesaurus.py:61
 msgid "Publisher"
 msgstr "Éditeur"
 
 #: src/pyams_thesaurus/interfaces/thesaurus.py:64
-#: src/pyams_thesaurus/interfaces/term.py:150
+#: src/pyams_thesaurus/interfaces/term.py:151
 msgid "Creation date"
 msgstr "Date de création"
 
 #: src/pyams_thesaurus/interfaces/thesaurus.py:76
 msgid "Thesaurus top-terms"
 msgstr "Termes de premier niveau"
 
@@ -304,172 +304,171 @@
 msgid "List of principals which can manage extract contents"
 msgstr "Liste de mandataires autorisés à gérer le contenu de l'extrait"
 
 #: src/pyams_thesaurus/interfaces/thesaurus.py:234
 msgid "Thesaurus extract"
 msgstr "Nom de l'extrait"
 
-#: src/pyams_thesaurus/interfaces/term.py:42
+#: src/pyams_thesaurus/interfaces/term.py:43
 msgid "Candidate"
 msgstr "Candidat"
 
-#: src/pyams_thesaurus/interfaces/term.py:43
+#: src/pyams_thesaurus/interfaces/term.py:44
 msgid "Published"
 msgstr "Publié"
 
-#: src/pyams_thesaurus/interfaces/term.py:44
+#: src/pyams_thesaurus/interfaces/term.py:45
 msgid "Archived"
 msgstr "Archivé"
 
-#: src/pyams_thesaurus/interfaces/term.py:57
-#: src/pyams_thesaurus/api/rest.py:138
+#: src/pyams_thesaurus/interfaces/term.py:58
 msgid "Term label"
 msgstr "Libellé"
 
-#: src/pyams_thesaurus/interfaces/term.py:58
+#: src/pyams_thesaurus/interfaces/term.py:59
 msgid "Full keyword for the given term"
 msgstr "Libellé complet du terme"
 
 #. pylint: disable=unsupported-membership-test
-#: src/pyams_thesaurus/interfaces/term.py:65
+#: src/pyams_thesaurus/interfaces/term.py:66
 msgid "'/' character is forbidden in term's label"
 msgstr "Le caractère '/' n'est pas autorisé dans le libellé d'un terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:71
+#: src/pyams_thesaurus/interfaces/term.py:72
 msgid "Alternate label"
 msgstr "Libellé de substitution"
 
-#: src/pyams_thesaurus/interfaces/term.py:72
+#: src/pyams_thesaurus/interfaces/term.py:73
 msgid "Not to be confused with synonyms 'usage' label, given below..."
 msgstr ""
 "S'il est renseigné, ce libellé sera utilisé à la place du \"Libellé\" dans "
 "les composants de sélection des termes"
 
-#: src/pyams_thesaurus/interfaces/term.py:76
+#: src/pyams_thesaurus/interfaces/term.py:77
 msgid "Definition"
 msgstr "Définition"
 
-#: src/pyams_thesaurus/interfaces/term.py:77
+#: src/pyams_thesaurus/interfaces/term.py:78
 msgid "Long definition, mostly for complicated terms"
 msgstr "Définition complète, utilisée principalement pour les termes complexes"
 
-#: src/pyams_thesaurus/interfaces/term.py:80
+#: src/pyams_thesaurus/interfaces/term.py:81
 msgid "Term's application note"
 msgstr "Note d'application"
 
-#: src/pyams_thesaurus/interfaces/term.py:81
+#: src/pyams_thesaurus/interfaces/term.py:82
 msgid "Application note for the given term"
 msgstr "Directives d'applications éventuelles de ce terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:84
+#: src/pyams_thesaurus/interfaces/term.py:85
 msgid "Generic term"
 msgstr "Terme générique"
 
-#: src/pyams_thesaurus/interfaces/term.py:85
+#: src/pyams_thesaurus/interfaces/term.py:86
 msgid "Parent generic term of the current term"
 msgstr "Terme de rattachement de ce terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:88
+#: src/pyams_thesaurus/interfaces/term.py:89
 msgid "Order"
 msgstr "Ordre"
 
-#: src/pyams_thesaurus/interfaces/term.py:89
+#: src/pyams_thesaurus/interfaces/term.py:90
 msgid ""
 "Term's position between it's siblings; default terms order is alphabetical"
 msgstr ""
 "Position du terme parmi ses termes frères ; lorsqu'il n'est pas spécifié, "
 "l'ordre par défaut est alphabétique"
 
-#: src/pyams_thesaurus/interfaces/term.py:93
+#: src/pyams_thesaurus/interfaces/term.py:94
 msgid "Specifics terms"
 msgstr "Termes spécifiques"
 
-#: src/pyams_thesaurus/interfaces/term.py:94
+#: src/pyams_thesaurus/interfaces/term.py:95
 msgid "Child more specifics terms of the current term"
 msgstr "Autres termes rattachés à ce terme en tant que terme générique"
 
-#: src/pyams_thesaurus/interfaces/term.py:98
+#: src/pyams_thesaurus/interfaces/term.py:99
 msgid "Associated terms"
 msgstr "Termes associés"
 
-#: src/pyams_thesaurus/interfaces/term.py:99
+#: src/pyams_thesaurus/interfaces/term.py:100
 msgid "Other terms associated to the current term"
 msgstr "Autres termes associés à ce terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:103
+#: src/pyams_thesaurus/interfaces/term.py:104
 msgid "Usage"
 msgstr "Terme d'usage"
 
-#: src/pyams_thesaurus/interfaces/term.py:104
+#: src/pyams_thesaurus/interfaces/term.py:105
 msgid "For synonyms, specify here the term's descriptor to use"
 msgstr ""
 "Dans le cas de synonymes, le terme d'usage est le terme 'officiel' à utiliser"
 
-#: src/pyams_thesaurus/interfaces/term.py:108
+#: src/pyams_thesaurus/interfaces/term.py:109
 msgid "Synonyms"
 msgstr "Synonymes"
 
-#: src/pyams_thesaurus/interfaces/term.py:109
+#: src/pyams_thesaurus/interfaces/term.py:110
 msgid "For a given allowed descriptor, specify here the list of synonyms"
 msgstr "Autres synonymes rattachés à ce terme en tant que terme d'usage"
 
-#: src/pyams_thesaurus/interfaces/term.py:118
+#: src/pyams_thesaurus/interfaces/term.py:119
 msgid "A term can't be a synonym and attached to a generic term"
 msgstr "Un terme ne peut pas être un synonyme et attaché à un terme générique"
 
-#: src/pyams_thesaurus/interfaces/term.py:120
+#: src/pyams_thesaurus/interfaces/term.py:121
 msgid ""
 "A term used as synonym can't have it's own synonyms (all synonyms should be "
 "attached to the descriptor)"
 msgstr ""
 "Un terme défini comme synonyme ne peut pas avoir ses propres synonymes (tous "
 "les synonymes devraient être rattachés au même terme principal)"
 
-#: src/pyams_thesaurus/interfaces/term.py:123
+#: src/pyams_thesaurus/interfaces/term.py:124
 msgid "Extracts"
 msgstr "Extraits"
 
-#: src/pyams_thesaurus/interfaces/term.py:124
+#: src/pyams_thesaurus/interfaces/term.py:125
 msgid "List of thesaurus extracts including this term"
 msgstr "Liste des extraits du thésaurus incluant ce terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:128
+#: src/pyams_thesaurus/interfaces/term.py:129
 msgid "Extensions"
 msgstr "Extensions"
 
-#: src/pyams_thesaurus/interfaces/term.py:129
+#: src/pyams_thesaurus/interfaces/term.py:130
 msgid "List of available extensions applied to this term"
 msgstr "Liste des extensions disponibles appliquées à ce terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:133
+#: src/pyams_thesaurus/interfaces/term.py:134
 msgid "Status"
 msgstr "Statut"
 
-#: src/pyams_thesaurus/interfaces/term.py:134
+#: src/pyams_thesaurus/interfaces/term.py:135
 msgid "Term status"
 msgstr "Statut du terme"
 
-#: src/pyams_thesaurus/interfaces/term.py:141
+#: src/pyams_thesaurus/interfaces/term.py:142
 msgid "Micro-thesaurus?"
 msgstr "Micro-thésaurus"
 
-#: src/pyams_thesaurus/interfaces/term.py:142
+#: src/pyams_thesaurus/interfaces/term.py:143
 msgid "Is the term part of a micro-thesaurus?"
 msgstr "Indique si le terme fait partie d'un micro-thésaurus"
 
-#: src/pyams_thesaurus/interfaces/term.py:145
+#: src/pyams_thesaurus/interfaces/term.py:146
 msgid "First level parent"
 msgstr "Parent de niveau 1"
 
-#: src/pyams_thesaurus/interfaces/term.py:146
+#: src/pyams_thesaurus/interfaces/term.py:147
 msgid "Parent at level 1 of the current term, or None"
 msgstr ""
 "Parent de niveau 1 de ce terme ; non renseigné dans le cas des synonymes"
 
-#: src/pyams_thesaurus/interfaces/term.py:153
+#: src/pyams_thesaurus/interfaces/term.py:154
 msgid "Modification date"
 msgstr "Date de modification"
 
 #: src/pyams_thesaurus/zmi/__init__.py:71
 msgid "Thesaurus container"
 msgstr "Gestionnaire de thésaurus"
 
@@ -546,15 +545,15 @@
 msgid "Thesaurus test form"
 msgstr "Test d'utilisation du thésaurus"
 
 #: src/pyams_thesaurus/zmi/test.py:87
 msgid "Thesaurus widget test"
 msgstr "Test de widgets du thésaurus"
 
-#: src/pyams_thesaurus/zmi/widget.py:172 src/pyams_thesaurus/zmi/widget.py:228
+#: src/pyams_thesaurus/zmi/widget.py:173 src/pyams_thesaurus/zmi/widget.py:229
 msgid "No selected term"
 msgstr "Aucun terme sélectionné"
 
 #: src/pyams_thesaurus/zmi/thesaurus.py:66
 msgid "Another thesaurus is already registered with this name!"
 msgstr "Un autre thésaurus est déjà enregistré sous ce nom !"
 
@@ -676,30 +675,24 @@
 msgid "Extract terms"
 msgstr "Termes de l'extrait"
 
 #: src/pyams_thesaurus/zmi/templates/terms-tree.pt:19
 msgid "Search term..."
 msgstr "Rechercher un terme..."
 
-#: src/pyams_thesaurus/api/rest.py:50 src/pyams_thesaurus/api/rest.py:125
-msgid "Selected thesaurus name"
-msgstr "Nom du thésaurus"
+#~ msgid "Selected thesaurus name"
+#~ msgstr "Nom du thésaurus"
 
-#: src/pyams_thesaurus/api/rest.py:64 src/pyams_thesaurus/api/rest.py:148
-msgid "Results list"
-msgstr "Liste de résultats"
-
-#: src/pyams_thesaurus/api/rest.py:68 src/pyams_thesaurus/api/rest.py:152
-msgid "Search results"
-msgstr "Résultats de la recherche"
+#~ msgid "Results list"
+#~ msgstr "Liste de résultats"
 
-#: src/pyams_thesaurus/api/rest.py:127
-msgid "Selected extract name"
-msgstr "Nom de l'extrait"
+#~ msgid "Search results"
+#~ msgstr "Résultats de la recherche"
+
+#~ msgid "Selected extract name"
+#~ msgstr "Nom de l'extrait"
+
+#~ msgid "Terms search string"
+#~ msgstr "Texte de recherche des termes"
 
-#: src/pyams_thesaurus/api/rest.py:130
-msgid "Terms search string"
-msgstr "Texte de recherche des termes"
-
-#: src/pyams_thesaurus/api/rest.py:136
-msgid "Term ID"
-msgstr "Identifiant du terme"
+#~ msgid "Term ID"
+#~ msgstr "Identifiant du terme"
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/locales/pyams_thesaurus.pot` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/locales/pyams_thesaurus.pot`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-10-15 01:18+0200\n"
+"POT-Creation-Date: 2023-04-12 16:01+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -214,15 +214,15 @@
 msgstr ""
 
 #: ./src/pyams_thesaurus/interfaces/thesaurus.py:61
 msgid "Publisher"
 msgstr ""
 
 #: ./src/pyams_thesaurus/interfaces/thesaurus.py:64
-#: ./src/pyams_thesaurus/interfaces/term.py:150
+#: ./src/pyams_thesaurus/interfaces/term.py:151
 msgid "Creation date"
 msgstr ""
 
 #: ./src/pyams_thesaurus/interfaces/thesaurus.py:76
 msgid "Thesaurus top-terms"
 msgstr ""
 
@@ -292,164 +292,163 @@
 msgid "List of principals which can manage extract contents"
 msgstr ""
 
 #: ./src/pyams_thesaurus/interfaces/thesaurus.py:234
 msgid "Thesaurus extract"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:42
+#: ./src/pyams_thesaurus/interfaces/term.py:43
 msgid "Candidate"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:43
+#: ./src/pyams_thesaurus/interfaces/term.py:44
 msgid "Published"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:44
+#: ./src/pyams_thesaurus/interfaces/term.py:45
 msgid "Archived"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:57
-#: ./src/pyams_thesaurus/api/rest.py:138
+#: ./src/pyams_thesaurus/interfaces/term.py:58
 msgid "Term label"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:58
+#: ./src/pyams_thesaurus/interfaces/term.py:59
 msgid "Full keyword for the given term"
 msgstr ""
 
 #. pylint: disable=unsupported-membership-test
-#: ./src/pyams_thesaurus/interfaces/term.py:65
+#: ./src/pyams_thesaurus/interfaces/term.py:66
 msgid "'/' character is forbidden in term's label"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:71
+#: ./src/pyams_thesaurus/interfaces/term.py:72
 msgid "Alternate label"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:72
+#: ./src/pyams_thesaurus/interfaces/term.py:73
 msgid "Not to be confused with synonyms 'usage' label, given below..."
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:76
+#: ./src/pyams_thesaurus/interfaces/term.py:77
 msgid "Definition"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:77
+#: ./src/pyams_thesaurus/interfaces/term.py:78
 msgid "Long definition, mostly for complicated terms"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:80
+#: ./src/pyams_thesaurus/interfaces/term.py:81
 msgid "Term's application note"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:81
+#: ./src/pyams_thesaurus/interfaces/term.py:82
 msgid "Application note for the given term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:84
+#: ./src/pyams_thesaurus/interfaces/term.py:85
 msgid "Generic term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:85
+#: ./src/pyams_thesaurus/interfaces/term.py:86
 msgid "Parent generic term of the current term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:88
+#: ./src/pyams_thesaurus/interfaces/term.py:89
 msgid "Order"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:89
+#: ./src/pyams_thesaurus/interfaces/term.py:90
 msgid ""
 "Term's position between it's siblings; default terms order is alphabetical"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:93
+#: ./src/pyams_thesaurus/interfaces/term.py:94
 msgid "Specifics terms"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:94
+#: ./src/pyams_thesaurus/interfaces/term.py:95
 msgid "Child more specifics terms of the current term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:98
+#: ./src/pyams_thesaurus/interfaces/term.py:99
 msgid "Associated terms"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:99
+#: ./src/pyams_thesaurus/interfaces/term.py:100
 msgid "Other terms associated to the current term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:103
+#: ./src/pyams_thesaurus/interfaces/term.py:104
 msgid "Usage"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:104
+#: ./src/pyams_thesaurus/interfaces/term.py:105
 msgid "For synonyms, specify here the term's descriptor to use"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:108
+#: ./src/pyams_thesaurus/interfaces/term.py:109
 msgid "Synonyms"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:109
+#: ./src/pyams_thesaurus/interfaces/term.py:110
 msgid "For a given allowed descriptor, specify here the list of synonyms"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:118
+#: ./src/pyams_thesaurus/interfaces/term.py:119
 msgid "A term can't be a synonym and attached to a generic term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:120
+#: ./src/pyams_thesaurus/interfaces/term.py:121
 msgid ""
 "A term used as synonym can't have it's own synonyms (all synonyms should be "
 "attached to the descriptor)"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:123
+#: ./src/pyams_thesaurus/interfaces/term.py:124
 msgid "Extracts"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:124
+#: ./src/pyams_thesaurus/interfaces/term.py:125
 msgid "List of thesaurus extracts including this term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:128
+#: ./src/pyams_thesaurus/interfaces/term.py:129
 msgid "Extensions"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:129
+#: ./src/pyams_thesaurus/interfaces/term.py:130
 msgid "List of available extensions applied to this term"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:133
+#: ./src/pyams_thesaurus/interfaces/term.py:134
 msgid "Status"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:134
+#: ./src/pyams_thesaurus/interfaces/term.py:135
 msgid "Term status"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:141
+#: ./src/pyams_thesaurus/interfaces/term.py:142
 msgid "Micro-thesaurus?"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:142
+#: ./src/pyams_thesaurus/interfaces/term.py:143
 msgid "Is the term part of a micro-thesaurus?"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:145
+#: ./src/pyams_thesaurus/interfaces/term.py:146
 msgid "First level parent"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:146
+#: ./src/pyams_thesaurus/interfaces/term.py:147
 msgid "Parent at level 1 of the current term, or None"
 msgstr ""
 
-#: ./src/pyams_thesaurus/interfaces/term.py:153
+#: ./src/pyams_thesaurus/interfaces/term.py:154
 msgid "Modification date"
 msgstr ""
 
 #: ./src/pyams_thesaurus/zmi/__init__.py:71
 msgid "Thesaurus container"
 msgstr ""
 
@@ -528,16 +527,16 @@
 msgid "Thesaurus test form"
 msgstr ""
 
 #: ./src/pyams_thesaurus/zmi/test.py:87
 msgid "Thesaurus widget test"
 msgstr ""
 
-#: ./src/pyams_thesaurus/zmi/widget.py:172
-#: ./src/pyams_thesaurus/zmi/widget.py:228
+#: ./src/pyams_thesaurus/zmi/widget.py:173
+#: ./src/pyams_thesaurus/zmi/widget.py:229
 msgid "No selected term"
 msgstr ""
 
 #: ./src/pyams_thesaurus/zmi/thesaurus.py:66
 msgid "Another thesaurus is already registered with this name!"
 msgstr ""
 
@@ -658,31 +657,7 @@
 #: ./src/pyams_thesaurus/zmi/extract.py:413
 msgid "Extract terms"
 msgstr ""
 
 #: ./src/pyams_thesaurus/zmi/templates/terms-tree.pt:19
 msgid "Search term..."
 msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:50 ./src/pyams_thesaurus/api/rest.py:125
-msgid "Selected thesaurus name"
-msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:64 ./src/pyams_thesaurus/api/rest.py:148
-msgid "Results list"
-msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:68 ./src/pyams_thesaurus/api/rest.py:152
-msgid "Search results"
-msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:127
-msgid "Selected extract name"
-msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:130
-msgid "Terms search string"
-msgstr ""
-
-#: ./src/pyams_thesaurus/api/rest.py:136
-msgid "Term ID"
-msgstr ""
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/manager.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/schema.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/term.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/test_utilsdocs.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/tests/test_utilsdocstrings.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/thesaurus.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/__init__.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/extension.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/extract.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/extract.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/interfaces.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/js/thesaurus.js` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/extract-terms.pt` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/extract-terms.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/terms-tree.pt` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/terms-tree.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/term.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/test.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/test.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/thesaurus.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/tree.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus/zmi/widget.py` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/PKG-INFO` & `pyams_thesaurus-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-thesaurus
-Version: 1.3.3
+Name: pyams_thesaurus
+Version: 1.3.4
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -49,14 +49,22 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+1.3.4
+-----
+ - updated Colander API schemas for better OpenAPI specifications
+
+1.3.3
+-----
+ - version mismatch
+
 1.3.2
 -----
  - added check for undefined thesaurus name in terms selection widget
  - added support for Python 3.11
 
 1.3.1
 -----
```

### Comparing `pyams_thesaurus-1.3.3/src/pyams_thesaurus.egg-info/SOURCES.txt` & `pyams_thesaurus-1.3.4/src/pyams_thesaurus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

