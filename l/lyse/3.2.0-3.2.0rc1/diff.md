# Comparing `tmp/lyse-3.2.0.tar.gz` & `tmp/lyse-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyse-3.2.0.tar", last modified: Thu Apr 13 00:08:08 2023, max compression
+gzip compressed data, was "lyse-3.2.0rc1.tar", last modified: Wed Apr 12 23:58:15 2023, max compression
```

## Comparing `lyse-3.2.0.tar` & `lyse-3.2.0rc1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.472197 lyse-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.440197 lyse-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.448197 lyse-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-13 00:07:56.000000 lyse-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-13 00:07:56.000000 lyse-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:07:56.000000 lyse-3.2.0/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 00:07:56.000000 lyse-3.2.0/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-13 00:07:56.000000 lyse-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-13 00:07:56.000000 lyse-3.2.0/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-13 00:08:08.472197 lyse-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-13 00:07:56.000000 lyse-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.452197 lyse-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    41708 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/gui.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/header.tex
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/listing_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/listing_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/listing_3.py
--rw-r--r--   0 runner    (1001) docker     (123)   131235 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/lyse.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/lyse.tex
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/minted.sty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.456197 lyse-3.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.456197 lyse-3.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.456197 lyse-3.2.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.460197 lyse-3.2.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.460197 lyse-3.2.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54825 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/gui.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/lyse_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:07:56.000000 lyse-3.2.0/docs/source/pyqt5-modified-objects.inv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.468197 lyse-3.2.0/lyse/
--rw-r--r--   0 runner    (1001) docker     (123)    49690 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109625 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/analysis_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/dataframe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/edit_columns.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/figure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/filebox.ui
--rw-r--r--   0 runner    (1001) docker     (123)   160912 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (123)   236310 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/lyse.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/plot_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/routinebox.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-13 00:07:56.000000 lyse-3.2.0/lyse/tempfile2clipboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:08:08.472197 lyse-3.2.0/lyse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 00:08:08.000000 lyse-3.2.0/lyse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 00:07:56.000000 lyse-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:07:56.000000 lyse-3.2.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 00:08:08.472197 lyse-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:07:56.000000 lyse-3.2.0/setup.py
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

### Comparing `lyse-3.2.0/.github/workflows/release.yml` & `lyse-3.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/.gitignore` & `lyse-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/BSD-2-CLAUSE-LICENSE.txt` & `lyse-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/BSD-3-CLAUSE-LICENSE.txt` & `lyse-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/LICENSE.txt` & `lyse-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/NEWS.md` & `lyse-3.2.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/PKG-INFO` & `lyse-3.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
```

### Comparing `lyse-3.2.0/README.md` & `lyse-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/Makefile` & `lyse-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/gui.pdf` & `lyse-3.2.0rc1/docs/gui.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/header.tex` & `lyse-3.2.0rc1/docs/header.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/listing_2.py` & `lyse-3.2.0rc1/docs/listing_2.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/listing_3.py` & `lyse-3.2.0rc1/docs/listing_3.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/lyse.pdf` & `lyse-3.2.0rc1/docs/lyse.pdf`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/lyse.tex` & `lyse-3.2.0rc1/docs/lyse.tex`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/make.bat` & `lyse-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/minted.sty` & `lyse-3.2.0rc1/docs/minted.sty`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/_static/custom.css` & `lyse-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/_templates/autosummary-class.rst` & `lyse-3.2.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/_templates/autosummary-module.rst` & `lyse-3.2.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/_templates/components.rst` & `lyse-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/conf.py` & `lyse-3.2.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/examples.rst` & `lyse-3.2.0rc1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/blacs_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/gui.svg` & `lyse-3.2.0rc1/docs/source/img/gui.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/labscript_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/lyse.ico` & `lyse-3.2.0rc1/docs/source/img/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/lyse_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/lyse_64x64.svg` & `lyse-3.2.0rc1/docs/source/img/lyse_64x64.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/runmanager_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/img/runviewer_32nx32n.svg` & `lyse-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/index.rst` & `lyse-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/introduction.rst` & `lyse-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/docs/source/pyqt5-modified-objects.inv` & `lyse-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/__init__.py` & `lyse-3.2.0rc1/lyse/__init__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/__main__.py` & `lyse-3.2.0rc1/lyse/__main__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/__version__.py` & `lyse-3.2.0rc1/lyse/__version__.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/analysis_subprocess.py` & `lyse-3.2.0rc1/lyse/analysis_subprocess.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/dataframe_utilities.py` & `lyse-3.2.0rc1/lyse/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/edit_columns.ui` & `lyse-3.2.0rc1/lyse/edit_columns.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/figure_manager.py` & `lyse-3.2.0rc1/lyse/figure_manager.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/filebox.ui` & `lyse-3.2.0rc1/lyse/filebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/lyse.ico` & `lyse-3.2.0rc1/lyse/lyse.ico`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/lyse.svg` & `lyse-3.2.0rc1/lyse/lyse.svg`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/main.ui` & `lyse-3.2.0rc1/lyse/main.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/plot_window.ui` & `lyse-3.2.0rc1/lyse/plot_window.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/routinebox.ui` & `lyse-3.2.0rc1/lyse/routinebox.ui`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse/tempfile2clipboard.py` & `lyse-3.2.0rc1/lyse/tempfile2clipboard.py`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/lyse.egg-info/PKG-INFO` & `lyse-3.2.0rc1/lyse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyse
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Automated analysis queue for labscript suite experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/lyse
 Project-URL: Download, https://github.com/labscript-suite/lyse/releases
```

### Comparing `lyse-3.2.0/lyse.egg-info/SOURCES.txt` & `lyse-3.2.0rc1/lyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/readthedocs.yaml` & `lyse-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lyse-3.2.0/setup.cfg` & `lyse-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*

