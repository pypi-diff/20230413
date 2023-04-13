# Comparing `tmp/lyse-3.1.0.tar.gz` & `tmp/lyse-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyse-3.1.0.tar", last modified: Tue Dec  7 15:56:40 2021, max compression
+gzip compressed data, was "lyse-3.2.0rc1.tar", last modified: Wed Apr 12 23:58:15 2023, max compression
```

## Comparing `lyse-3.1.0.tar` & `lyse-3.2.0rc1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.526799 lyse-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.518799 lyse-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.518799 lyse-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     9111 2021-12-07 15:56:34.000000 lyse-3.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-12-07 15:56:34.000000 lyse-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-12-07 15:56:34.000000 lyse-3.1.0/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-12-07 15:56:34.000000 lyse-3.1.0/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-12-07 15:56:34.000000 lyse-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-12-07 15:56:34.000000 lyse-3.1.0/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-12-07 15:56:40.526799 lyse-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2021-12-07 15:56:34.000000 lyse-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.518799 lyse-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    41708 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/gui.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/header.tex
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/listing_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/listing_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/listing_3.py
--rw-r--r--   0 runner    (1001) docker     (121)   131235 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/lyse.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    13294 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/lyse.tex
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     8434 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/minted.sty
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.518799 lyse-3.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.518799 lyse-3.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.522799 lyse-3.1.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.522799 lyse-3.1.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9626 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.522799 lyse-3.1.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    54825 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/gui.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)   102420 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (121)    12665 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11081 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/lyse_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14435 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13201 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5439 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    64143 2021-12-07 15:56:34.000000 lyse-3.1.0/docs/source/pyqt5-modified-objects.inv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.522799 lyse-3.1.0/lyse/
--rw-r--r--   0 runner    (1001) docker     (121)    47345 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   109625 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18140 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/analysis_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/dataframe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/edit_columns.ui
--rw-r--r--   0 runner    (1001) docker     (121)     6020 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/figure_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8823 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/filebox.ui
--rw-r--r--   0 runner    (1001) docker     (121)   160912 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (121)   236310 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/lyse.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7761 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/main.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/plot_window.ui
--rw-r--r--   0 runner    (1001) docker     (121)     8063 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/routinebox.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2021-12-07 15:56:34.000000 lyse-3.1.0/lyse/tempfile2clipboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:56:40.526799 lyse-3.1.0/lyse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-07 15:56:40.000000 lyse-3.1.0/lyse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-07 15:56:34.000000 lyse-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-07 15:56:34.000000 lyse-3.1.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-12-07 15:56:40.526799 lyse-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-12-07 15:56:34.000000 lyse-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    41708 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/gui.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/header.tex
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/listing_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131235 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/lyse.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/lyse.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/minted.sty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.865846 lyse-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54825 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/gui.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/lyse_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.869846 lyse-3.2.0rc1/lyse/
+-rw-r--r--   0 runner    (1001) docker     (123)    49690 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109625 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/analysis_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/dataframe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/edit_columns.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/figure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/filebox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   160912 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/lyse.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   236310 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/lyse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/plot_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/routinebox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/lyse/tempfile2clipboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/lyse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 23:58:15.000000 lyse-3.2.0rc1/lyse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-12 23:58:15.873847 lyse-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 23:58:05.000000 lyse-3.2.0rc1/setup.py
```

### Comparing `lyse-3.1.0/.github/workflows/release.yml` & `lyse-3.2.0rc1/.github/workflows/release.yml`

 * *Files 26% similar despite different names*

```diff
@@ -5,21 +5,16 @@
     branches:
       - master
       - maintenance/*
   create:
     tags:
       - 'v[0-9]+.[0-9]+.[0-9]+*'
 
-defaults:
-  run:
-    shell: bash
-
 env:
   PACKAGE_NAME: lyse
-  SCM_VERSION_SCHEME: release-branch-semver
   SCM_LOCAL_SCHEME: no-local-version
   ANACONDA_USER: labscript-suite
 
   # Configuration for a package with compiled extensions:
   # PURE: false
   # NOARCH: false
 
@@ -38,238 +33,224 @@
 jobs:
   build:
     name: Build
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
-          - { os: ubuntu-latest,   python: 3.8,  arch: x64 }
-          # - { os: ubuntu-latest,   python: 3.7,  arch: x64 }
-          # - { os: ubuntu-latest,   python: 3.6,  arch: x64 }
-
-          # - { os: macos-latest,    python: 3.8,  arch: x64 }
-          # - { os: macos-latest,    python: 3.7,  arch: x64 }
-          # - { os: macos-latest,    python: 3.6,  arch: x64 }
-
-          # - { os: windows-latest,  python: 3.8,  arch: x64 }
-          # - { os: windows-latest,  python: 3.7,  arch: x64 }
-          # - { os: windows-latest,  python: 3.6,  arch: x64 }
-
-          # - { os: windows-latest,  python: 3.8,  arch: x86 }
-          # - { os: windows-latest,  python: 3.7,  arch: x86 }
-          # - { os: windows-latest,  python: 3.6,  arch: x86 }
+          - { os: ubuntu-latest,   python: '3.11',  arch: x64, conda: true}
+         # - { os: ubuntu-latest,   python: '3.10',  arch: x64, conda: true }
+         # - { os: ubuntu-latest,   python: '3.9',  arch: x64, conda: true }
+         # - { os: ubuntu-latest,   python: '3.8',  arch: x64, conda: true }
+         # - { os: ubuntu-latest,   python: '3.7',  arch: x64, conda: true }
+
+         # - { os: macos-11,    python: '3.11',  arch: x64, conda: true }
+         # - { os: macos-11,    python: '3.10',  arch: x64, conda: true }
+         # - { os: macos-11,    python: '3.9',  arch: x64, conda: true }
+         # - { os: macos-11,    python: '3.8',  arch: x64, conda: true }
+         # - { os: macos-11,    python: '3.7',  arch: x64, conda: true }
+
+         # - { os: windows-latest,  python: '3.11',  arch: x64, conda: true }
+         # - { os: windows-latest,  python: '3.10',  arch: x64, conda: true }
+         # - { os: windows-latest,  python: '3.9',  arch: x64, conda: true }
+         # - { os: windows-latest,  python: '3.8',  arch: x64, conda: true }
+         # - { os: windows-latest,  python: '3.7',  arch: x64, conda: true }
+
+         # - { os: windows-latest,  python: '3.11',  arch: x86, conda: false } # conda not yet available
+         # - { os: windows-latest,  python: '3.10',  arch: x86, conda: true }
+         # - { os: windows-latest,  python: '3.9',  arch: x86, conda: true }
+         # - { os: windows-latest,  python: '3.8',  arch: x86, conda: true }
+         # - { os: windows-latest,  python: '3.7',  arch: x86, conda: true }
 
     if: github.repository == 'labscript-suite/lyse' && (github.event_name != 'create' || github.event.ref_type != 'branch')
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Ignore Tags
         if: github.event.ref_type != 'tag'
         run: git tag -d $(git tag --points-at HEAD)
 
       - name: Install Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           architecture: ${{ matrix.arch }}
 
       - name: Source Distribution
         if: strategy.job-index == 0
         run: |
-          python -m pip install --upgrade pip setuptools wheel pep517
-          python -m pep517.build -s .
+          python -m pip install --upgrade pip setuptools wheel build
+          python -m build -s .
 
       - name: Wheel Distribution
         # Impure Linux wheels are built in the manylinux job.
         if: (env.PURE == 'true' && strategy.job-index == 0) || (env.PURE == 'false' && runner.os != 'Linux')
         run: |
-          python -m pip install --upgrade pip setuptools wheel pep517
-          python -m pep517.build -b .
+          python -m pip install --upgrade pip setuptools wheel build
+          python -m build -w .
 
       - name: Upload Artifact
         if: strategy.job-index == 0 || (env.PURE == 'false' && runner.os != 'Linux')
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
           path: ./dist
 
       - name: Set Variables for Conda Build
+        if: matrix.conda
+        shell: bash
         run: |
-          if [ $RUNNER_OS == Windows ] && [ ${{ matrix.arch }} == x64 ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Windows-x86_64.exe
-          elif [ $RUNNER_OS == Windows ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Windows-x86.exe
-          elif [ $RUNNER_OS == Linux ]; then
-              CONDA_INSTALLER=Miniconda3-latest-Linux-x86_64.sh
-          else
-              CONDA_INSTALLER=Miniconda3-latest-MacOSX-x86_64.sh
-          fi
           if [ $NOARCH == true ]; then
               CONDA_BUILD_ARGS="--noarch"
           else
               CONDA_BUILD_ARGS=""
           fi
-          echo "CONDA_INSTALLER=$CONDA_INSTALLER" >> $GITHUB_ENV
           echo "CONDA_BUILD_ARGS=$CONDA_BUILD_ARGS" >> $GITHUB_ENV
 
+      - name: Install Miniconda
+        if: matrix.conda
+        uses: conda-incubator/setup-miniconda@v2
+        with:
+          auto-update-conda: true
+          python-version: ${{ matrix.python }}
+          architecture: ${{ matrix.arch }}
+          miniconda-version: "latest"
+
+      - name: Workaround conda-build incompatibility with xcode 12+
+        if: runner.os == 'macOS'
+        uses: maxim-lobanov/setup-xcode@v1
+        with:
+          xcode-version: 11.7
+
       - name: Conda package (Unix)
-        if: runner.os != 'Windows'
+        if: (matrix.conda && runner.os != 'Windows')
+        shell: bash -l {0}
         run: |
-          curl -LO https://repo.continuum.io/miniconda/$CONDA_INSTALLER
-          bash "$CONDA_INSTALLER" -b -p .miniconda
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
-          conda update -n base -c defaults conda
-          conda create -n py${{ matrix.python }} python=${{ matrix.python }}
-          conda activate py${{ matrix.python }}
-          conda install -c cbillington setuptools-conda
-          pip install --upgrade setuptools_scm
+          conda install -c labscript-suite setuptools-conda
           setuptools-conda build $CONDA_BUILD_ARGS .
 
       - name: Conda Package (Windows)
-        if: runner.os == 'Windows'
-        shell: cmd
+        if: (matrix.conda && runner.os == 'Windows')
+        shell: cmd /C CALL {0}
         run: |
-          curl -LO https://repo.continuum.io/miniconda/%CONDA_INSTALLER%
-          %CONDA_INSTALLER% /S /D=%CD%\.miniconda && ^
-          .miniconda\Scripts\activate && ^
-          conda update -n base -c defaults conda && ^
-          conda create -n py${{ matrix.python }} python=${{ matrix.python }} && ^
-          conda activate py${{ matrix.python }} && ^
-          conda install -c cbillington setuptools-conda && ^
-          pip install --upgrade setuptools_scm && ^
-          setuptools-conda build %CONDA_BUILD_ARGS% .
+          conda install -c labscript-suite setuptools-conda && ^
+          setuptools-conda build %CONDA_BUILD_ARGS% --croot ${{ runner.temp }}\cb .
 
       - name: Upload Artifact
-        uses: actions/upload-artifact@v2
+        if: matrix.conda
+        uses: actions/upload-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
 
   manylinux:
     name: Build Manylinux
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        include:
-          - { python: 'cp36-cp36m cp37-cp37m cp38-cp38' }
-
     if: github.repository == 'labscript-suite/lyse' && (github.event_name != 'create' || github.event.ref_type != 'branch')
     steps:
       - name: Checkout
         if: env.PURE == 'false'
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Ignore Tags
         if: github.event.ref_type != 'tag' && env.PURE == 'false'
         run: git tag -d $(git tag --points-at HEAD)
 
       - name: Build Manylinux Wheels
         if: env.PURE == 'false'
-        uses: RalfG/python-wheels-manylinux-build@v0.2.2-manylinux2010_x86_64
+        uses: RalfG/python-wheels-manylinux-build@v0.4.2
         with:
-          python-versions: ${{ matrix.python }}
+          python-versions: 'cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310 cp311-cp311'
+          pre-build-command: 'git config --global --add safe.directory "*"'
 
       - name: Upload Artifact
         if: env.PURE == 'false'
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
-          path: wheelhouse/*manylinux*.whl
+          path: dist/*manylinux*.whl
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [build, manylinux]
     steps:
 
       - name: Download Artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: dist
           path: ./dist
 
       - name: Download Artifact
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
-      - name: Publish on TestPyPI
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          user: __token__
-          password: ${{ secrets.testpypi }}
-          repository_url: https://test.pypi.org/legacy/
-
       - name: Get Version Number
         if: github.event.ref_type == 'tag'
         run: |
           VERSION="${GITHUB_REF/refs\/tags\/v/}"
           echo "VERSION=$VERSION" >> $GITHUB_ENV
 
-      - name: Create GitHub Release
+      - name: Create GitHub Release and Upload Release Asset
         if: github.event.ref_type == 'tag'
-        id: create_release
-        uses: actions/create-release@latest
+        uses: softprops/action-gh-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.event.ref }}
-          release_name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
+          name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
           draft: true
           prerelease: ${{ contains(github.event.ref, 'rc') }}
+          files: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
 
-      - name: Upload Release Asset
-        if: github.event.ref_type == 'tag'
-        uses: actions/upload-release-asset@v1
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      - name: Publish on TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          upload_url: ${{ steps.create_release.outputs.upload_url }}
-          asset_path: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_name: ${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_content_type: application/gzip
+          user: __token__
+          password: ${{ secrets.testpypi }}
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish on PyPI
         if: github.event.ref_type == 'tag'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi }}
 
-      - name: Install Miniconda and cloud client
-        run: |
-          curl -LO https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh 
-          bash Miniconda3-latest-Linux-x86_64.sh -b -p .miniconda
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
-          conda install anaconda-client
+      - name: Install Miniconda
+        uses: conda-incubator/setup-miniconda@v2
+        with:
+          auto-update-conda: true
+
+      - name: Install Anaconda cloud client
+        shell: bash -l {0}
+        run: conda install anaconda-client
 
       - name: Publish to Anaconda test label
         if: github.event.ref_type != 'tag'
+        shell: bash -l {0}
         run: |
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
           anaconda \
             --token ${{ secrets.ANACONDA_API_TOKEN }} \
             upload \
             --user $ANACONDA_USER \
             --label test \
             conda_packages/*/*
 
       - name: Publish to Anaconda main label
+        shell: bash -l {0}
         if: github.event.ref_type == 'tag'
         run: |
-          source .miniconda/etc/profile.d/conda.sh
-          conda activate
           anaconda \
             --token ${{ secrets.ANACONDA_API_TOKEN }} \
             upload \
             --user $ANACONDA_USER \
             conda_packages/*/*
```

### Comparing `lyse-3.1.0/.gitignore` & `lyse-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/BSD-2-CLAUSE-LICENSE.txt` & `lyse-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/BSD-3-CLAUSE-LICENSE.txt` & `lyse-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/LICENSE.txt` & `lyse-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/NEWS.md` & `lyse-3.2.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/PKG-INFO` & `lyse-3.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.1.0
+Version: 3.2.0rc1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
 Project-URL: Tracker, https://github.com/labscript-suite/lyse/issues
 Keywords: experiment analysis automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pyqt
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/lyse_32nx32n.svg" height="64" alt="the labscript suite – lyse" align="right">
@@ -67,9 +68,7 @@
 
 † In this example, these are publication quality figures generated for the manuscript *Science* **364**, pp. 1267 (2019) [doi:10.1126/science.aat5793](https://doi.org/10.1126/science.aat5793).
 
 
 ## Installation
 
 lyse is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `lyse-3.1.0/README.md` & `lyse-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/Makefile` & `lyse-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/gui.pdf` & `lyse-3.2.0rc1/docs/gui.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/header.tex` & `lyse-3.2.0rc1/docs/header.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/listing_2.py` & `lyse-3.2.0rc1/docs/listing_2.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/listing_3.py` & `lyse-3.2.0rc1/docs/listing_3.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/lyse.pdf` & `lyse-3.2.0rc1/docs/lyse.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/lyse.tex` & `lyse-3.2.0rc1/docs/lyse.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/make.bat` & `lyse-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/minted.sty` & `lyse-3.2.0rc1/docs/minted.sty`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/_static/custom.css` & `lyse-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/_templates/autosummary-class.rst` & `lyse-3.2.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/_templates/autosummary-module.rst` & `lyse-3.2.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/_templates/components.rst` & `lyse-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/conf.py` & `lyse-3.2.0rc1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 #
 import copy
 import os
 from pathlib import Path
 from m2r import MdInclude
 from recommonmark.transform import AutoStructify
 from jinja2 import FileSystemLoader, Environment
+try:
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    import importlib_metadata
 
 # -- Project information (unique to each project) -------------------------------------
 
 project = "lyse"
 copyright = "2020, labscript suite"
 author = "labscript suite contributors"
 
 # The full version, including alpha/beta/rc tags
-from lyse import __version__ as version  # noqa: E402
+version = importlib_metadata.version('lyse')
 
 release = version
 
 # HTML icons
 img_path = 'img'
 html_logo = img_path + "/lyse_64x64.svg"
 html_favicon = img_path + "/lyse.ico"
@@ -90,23 +94,23 @@
 master_doc = 'index'
 
 # intersphinx allows us to link directly to other repos sphinxdocs.
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
     'qtutils': ('https://qtutils.readthedocs.io/en/stable/', None),
     'pyqtgraph': (
         'https://pyqtgraph.readthedocs.io/en/latest/',
         None,
     ),  # change to stable once v0.11 is published
-    'matplotlib': ('https://matplotlib.org/', None),
-    'h5py': ('http://docs.h5py.org/en/stable/', None),
+    'matplotlib': ('https://matplotlib.org/stable/', None),
+    'h5py': ('https://docs.h5py.org/en/stable/', None),
     'pydaqmx': ('https://pythonhosted.org/PyDAQmx/', None),
     'qt': (
         '',
         'pyqt5-modified-objects.inv',
     )  # from https://github.com/MSLNZ/msl-qt/blob/master/docs/create_pyqt_objects.py
     # under MIT License
     # TODO
```

### Comparing `lyse-3.1.0/docs/source/examples.rst` & `lyse-3.2.0rc1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/blacs_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/gui.svg` & `lyse-3.2.0rc1/docs/source/img/gui.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/labscript_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/lyse.ico` & `lyse-3.2.0rc1/docs/source/img/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/lyse_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/lyse_64x64.svg` & `lyse-3.2.0rc1/docs/source/img/lyse_64x64.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/runmanager_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/img/runviewer_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/index.rst` & `lyse-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/introduction.rst` & `lyse-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/docs/source/pyqt5-modified-objects.inv` & `lyse-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/__init__.py` & `lyse-3.2.0rc1/lyse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import inspect
 import sys
 import threading
 
 import labscript_utils.h5_lock, h5py
 from labscript_utils.labconfig import LabConfig
 import pandas
-from numpy import array, ndarray
+from numpy import array, ndarray, where
 import types
 
 from .__version__ import __version__
 
 from labscript_utils import dedent
 from labscript_utils.ls_zprocess import zmq_get
 
@@ -384,33 +384,78 @@
             dict: Dictionary of attributes.
         """
         with h5py.File(self.h5_path, 'r') as h5_file:
             if not group in h5_file:
                 raise Exception('The group \'%s\' does not exist'%group)
             return get_attributes(h5_file[group])
 
-    def get_trace(self,name):
+    def get_trace(self, name, raw_data=False):
         """Return the saved data trace `name`.
         
         Args:
             name (str): Name of saved data trace to get.
+            raw_data (bool, optional): option to return the h5_data directly 
+                without interpreting it as a 2-D time trace.
 
         Raises:
             Exception: If `name` trace does not exist.
 
         Returns:
             :obj:`numpy:numpy.ndarray`: Returns 2-D timetrace of times `'t'`
             and values `'values'`.
         """
         with h5py.File(self.h5_path, 'r') as h5_file:
             if not name in h5_file['data']['traces']:
                 raise Exception('The trace \'%s\' does not exist'%name)
             trace = h5_file['data']['traces'][name]
-            return array(trace['t'],dtype=float),array(trace['values'],dtype=float)         
+            
+            if raw_data:
+                data = trace[()]
+            else:
+                data = array(trace['t'],dtype=float),array(trace['values'],dtype=float)  
+            
+            return data
 
+    def get_wait(self,name):
+        """Returns the wait paramteres: label, timeout, duration, and time out status.
+
+        Args:
+            name (str): Name of the wait to get.
+
+        Raises:
+            KeyError if `name` wait does not exist.
+
+        Returns:
+            tuple: Tuple of the wait parameters.
+        """
+        with h5py.File(self.h5_path,'r') as h5_file:
+            if not 'data' in h5_file:
+                raise Exception('The shot has no data group')
+            name=name.encode()
+            if not name in h5_file['data']['waits']['label']:
+                raise Exception('The wait \'%s\' does not exist'%name.decode())
+            name_index, =where(h5_file['data']['waits']['label']==name)[0]
+            return h5_file['data']['waits'][name_index]
+
+    def get_waits(self):
+        """Returns the parameters of all waits in the experiment.
+
+        Raises:
+            Exception: If the experiment has no waits.
+
+        Returns:
+            :obj:`numpy:numpy.ndarray`: Returns 2D structured numpy array of the waits and their parameters.
+        """
+        with h5py.File(self.h5_path,'r') as h5_file:
+            if not 'data' in h5_file:
+                raise Exception('The shot has no data group')
+            if not 'waits' in h5_file['data']:
+                raise Exception('The shot has no waits')
+            return h5_file['data']['waits'][()]
+        
     def get_result_array(self,group,name):
         """Returns saved results data.
 
         Args:
             group (str): Group to look in for the array. Typically the name of
                 the analysis script that created it.
             name (str): Name of the results array to return.
@@ -717,15 +762,15 @@
             **kwargs: Passed through to `save_result_array` as kwargs.
         """
         names = args[::2]
         values = args[1::2]
         for name, value in zip(names, values):
             self.save_result_array(name, value, **kwargs)
     
-    def get_image(self,orientation,label,image):
+    def get_image(self, orientation, label, image):
         """Get previously saved image from the h5 file.
 
         h5 path to saved image is `/images/orientation/label/image`
 
         Args:
             orientation (str): Orientation label for saved image.
             label (str): Label of saved image.
@@ -744,15 +789,15 @@
                 raise Exception('File does not contain any images with orientation \'%s\''%orientation)
             if not label in h5_file['images'][orientation]:
                 raise Exception('File does not contain any images with label \'%s\''%label)
             if not image in h5_file['images'][orientation][label]:
                 raise Exception('Image \'%s\' not found in file'%image)
             return array(h5_file['images'][orientation][label][image])
     
-    def get_images(self,orientation,label, *images):
+    def get_images(self, orientation, label, *images):
         """Get multiple saved images from orientation and label.
 
         Iteratively calls :obj:`self.get_image(orientation,label,image) <get_image>` for
         each image argument.
 
         Args:
             orientation (str): Orientation label of saved images.
@@ -762,15 +807,34 @@
         Returns:
             :obj:`list` of :obj:`numpy:numpy.ndarray`: List of 2-D images.
         """
         results = []
         for image in images:
             results.append(self.get_image(orientation,label,image))
         return results
-        
+
+    def get_images_dict(self, orientation, label, *images):
+        """Get multiple saved images from orientation and label.
+
+        Iteratively calls :obj:`self.get_image(orientation,label,image) <get_image>` for
+        each image argument.
+
+        Args:
+            orientation (str): Orientation label of saved images.
+            label (str): Label of saved images.
+            *images (str): Collection of images to return
+
+        Returns:
+            :obj:`dict` of :obj:`numpy:numpy.ndarray`: Dictionary of 2-D images.
+        """
+        results = self.get_images(orientation,label, *images)
+
+        return {k:v for k,v in zip(images, results)}
+
+
     def get_all_image_labels(self):
         """Return all existing images labels in the h5 file.
 
         Returns:
             dict: Dictionary of the form `{orientation:[label1,label2]}`
         """
         images_list = {}
```

### Comparing `lyse-3.1.0/lyse/__main__.py` & `lyse-3.2.0rc1/lyse/__main__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/__version__.py` & `lyse-3.2.0rc1/lyse/__version__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/analysis_subprocess.py` & `lyse-3.2.0rc1/lyse/analysis_subprocess.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/dataframe_utilities.py` & `lyse-3.2.0rc1/lyse/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/edit_columns.ui` & `lyse-3.2.0rc1/lyse/edit_columns.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/figure_manager.py` & `lyse-3.2.0rc1/lyse/figure_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,8 @@
     global figuremanager
     import matplotlib.pyplot
     import matplotlib.figure
 
     figuremanager = FigureManager()
     matplotlib.pyplot.figure = figuremanager
     matplotlib.pyplot.close = figuremanager.close
-    matplotlib.pyplot.show = figuremanager.show
+    matplotlib.pyplot.show = lambda: figuremanager.show
```

### Comparing `lyse-3.1.0/lyse/filebox.ui` & `lyse-3.2.0rc1/lyse/filebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/lyse.ico` & `lyse-3.2.0rc1/lyse/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/lyse.svg` & `lyse-3.2.0rc1/lyse/lyse.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/main.ui` & `lyse-3.2.0rc1/lyse/main.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/plot_window.ui` & `lyse-3.2.0rc1/lyse/plot_window.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/routinebox.ui` & `lyse-3.2.0rc1/lyse/routinebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse/tempfile2clipboard.py` & `lyse-3.2.0rc1/lyse/tempfile2clipboard.py`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/lyse.egg-info/PKG-INFO` & `lyse-3.2.0rc1/lyse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.1.0
+Version: 3.2.0rc1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
 Project-URL: Tracker, https://github.com/labscript-suite/lyse/issues
 Keywords: experiment analysis automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pyqt
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/lyse_32nx32n.svg" height="64" alt="the labscript suite – lyse" align="right">
@@ -67,9 +68,7 @@
 
 † In this example, these are publication quality figures generated for the manuscript *Science* **364**, pp. 1267 (2019) [doi:10.1126/science.aat5793](https://doi.org/10.1126/science.aat5793).
 
 
 ## Installation
 
 lyse is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `lyse-3.1.0/lyse.egg-info/SOURCES.txt` & `lyse-3.2.0rc1/lyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/readthedocs.yaml` & `lyse-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lyse-3.1.0/setup.cfg` & `lyse-3.2.0rc1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.6
 install_requires = 
@@ -45,16 +47,17 @@
 gui_scripts = 
 	lyse-gui = desktop_app:entry_point
 
 [options.extras_require]
 pyqt = PyQt5
 docs = 
 	PyQt5
-	Sphinx==3.5.3
+	Sphinx==4.4.0
 	sphinx-rtd-theme==0.5.2
 	recommonmark==0.6.0
 	m2r==0.2.1
+	mistune<2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

