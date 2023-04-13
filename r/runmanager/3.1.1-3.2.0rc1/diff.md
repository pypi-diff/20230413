# Comparing `tmp/runmanager-3.1.1.tar.gz` & `tmp/runmanager-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runmanager-3.1.1.tar", last modified: Tue Dec  7 13:12:48 2021, max compression
+gzip compressed data, was "runmanager-3.2.0rc1.tar", last modified: Thu Apr 13 00:42:01 2023, max compression
```

## Comparing `runmanager-3.1.1.tar` & `runmanager-3.2.0rc1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.151569 runmanager-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.143569 runmanager-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.143569 runmanager-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     9129 2021-12-07 13:12:36.000000 runmanager-3.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2021-12-07 13:12:36.000000 runmanager-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-12-07 13:12:36.000000 runmanager-3.1.1/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-12-07 13:12:36.000000 runmanager-3.1.1/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-12-07 13:12:36.000000 runmanager-3.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2021-12-07 13:12:48.151569 runmanager-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-12-07 13:12:36.000000 runmanager-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.143569 runmanager-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.147570 runmanager-3.1.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.147570 runmanager-3.1.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.147570 runmanager-3.1.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.147570 runmanager-3.1.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10412 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.147570 runmanager-3.1.1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12665 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)   106126 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager.ico
--rw-r--r--   0 runner    (1001) docker     (121)    14435 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12704 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (121)   113429 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_axes.png
--rw-r--r--   0 runner    (1001) docker     (121)   217480 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_bools.png
--rw-r--r--   0 runner    (1001) docker     (121)   243887 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_complex_globals.png
--rw-r--r--   0 runner    (1001) docker     (121)   250190 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_eval_error.png
--rw-r--r--   0 runner    (1001) docker     (121)   200741 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_groups.png
--rw-r--r--   0 runner    (1001) docker     (121)   239956 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_interface.png
--rw-r--r--   0 runner    (1001) docker     (121)   131423 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runmanager_overview.png
--rw-r--r--   0 runner    (1001) docker     (121)    13201 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    64143 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)    28615 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)   245000 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/using_runmanager.docx
--rw-r--r--   0 runner    (1001) docker     (121)   679785 2021-12-07 13:12:36.000000 runmanager-3.1.1/docs/using_runmanager.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-07 13:12:36.000000 runmanager-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-07 13:12:36.000000 runmanager-3.1.1/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.151569 runmanager-3.1.1/runmanager/
--rw-r--r--   0 runner    (1001) docker     (121)    48648 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   189841 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/batch_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/globals_diff.bat
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/globals_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/group.ui
--rw-r--r--   0 runner    (1001) docker     (121)    36893 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/main.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)   167461 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/runmanager.ico
--rw-r--r--   0 runner    (1001) docker     (121)    21924 2021-12-07 13:12:36.000000 runmanager-3.1.1/runmanager/runmanager.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 13:12:48.151569 runmanager-3.1.1/runmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 13:12:47.000000 runmanager-3.1.1/runmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-07 13:12:48.000000 runmanager-3.1.1/runmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-12-07 13:12:48.151569 runmanager-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-12-07 13:12:36.000000 runmanager-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.817341 runmanager-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.821341 runmanager-3.2.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.825341 runmanager-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106126 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113429 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_axes.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217480 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_bools.png
+-rw-r--r--   0 runner    (1001) docker     (123)   243887 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_complex_globals.png
+-rw-r--r--   0 runner    (1001) docker     (123)   250190 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_eval_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   200741 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_groups.png
+-rw-r--r--   0 runner    (1001) docker     (123)   239956 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_interface.png
+-rw-r--r--   0 runner    (1001) docker     (123)   131423 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runmanager_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    28615 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   245000 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/using_runmanager.docx
+-rw-r--r--   0 runner    (1001) docker     (123)   679785 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/docs/using_runmanager.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/runmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    48648 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189841 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/batch_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/globals_diff.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/globals_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/group.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167461 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/runmanager.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/runmanager/runmanager.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/runmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 00:42:01.000000 runmanager-3.2.0rc1/runmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 00:42:01.829341 runmanager-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:41:49.000000 runmanager-3.2.0rc1/setup.py
```

### Comparing `runmanager-3.1.1/.github/workflows/release.yml` & `runmanager-3.2.0rc1/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

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
   PACKAGE_NAME: runmanager
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
 
     if: github.repository == 'labscript-suite/runmanager' && (github.event_name != 'create' || github.event.ref_type != 'branch')
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
     if: github.repository == 'labscript-suite/runmanager' && (github.event_name != 'create' || github.event.ref_type != 'branch')
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

### Comparing `runmanager-3.1.1/.gitignore` & `runmanager-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/BSD-2-CLAUSE-LICENSE.txt` & `runmanager-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/BSD-3-CLAUSE-LICENSE.txt` & `runmanager-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/LICENSE.txt` & `runmanager-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/PKG-INFO` & `runmanager-3.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: runmanager
-Version: 3.1.1
+Version: 3.2.0rc1
 Summary: Graphical control of parameterised experiments composed in labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runmanager
 Project-URL: Download, https://github.com/labscript-suite/runmanager/releases
 Project-URL: Tracker, https://github.com/labscript-suite/runmanager/issues
 Keywords: experiment control automation
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
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runmanager_32nx32n.svg" height="64" alt="the labscript suite – runmanager" align="right">
@@ -44,9 +45,7 @@
 
 runmanager can be run on any host with network access to the hardware supervisor [**blacs**](https://github.com/labscript-suite/blacs), and includes a remote programming interface for automation.
 
 
 ## Installation
 
 runmanager is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `runmanager-3.1.1/README.md` & `runmanager-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/Makefile` & `runmanager-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/make.bat` & `runmanager-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/_static/custom.css` & `runmanager-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/_templates/autosummary-class.rst` & `runmanager-3.2.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/_templates/autosummary-module.rst` & `runmanager-3.2.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/_templates/components.rst` & `runmanager-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/conf.py` & `runmanager-3.2.0rc1/docs/source/conf.py`

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
 
 project = "runmanager"
 copyright = "2020, labscript suite"
 author = "labscript suite contributors"
 
 # The full version, including alpha/beta/rc tags
-from runmanager import __version__ as version  # noqa: E402
+version = importlib_metadata.version('runmanager')
 
 release = version
 
 # HTML icons
 img_path = 'img'
 html_logo = img_path + "/runmanager_64x64.svg"
 html_favicon = img_path + "/runmanager.ico"
@@ -120,23 +124,23 @@
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

### Comparing `runmanager-3.1.1/docs/source/img/blacs_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/labscript_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/lyse_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager.ico` & `runmanager-3.2.0rc1/docs/source/img/runmanager.ico`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_64x64.svg` & `runmanager-3.2.0rc1/docs/source/img/runmanager_64x64.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_axes.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_axes.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_bools.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_bools.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_complex_globals.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_complex_globals.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_eval_error.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_eval_error.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_groups.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_groups.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_interface.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_interface.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runmanager_overview.png` & `runmanager-3.2.0rc1/docs/source/img/runmanager_overview.png`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/img/runviewer_32nx32n.svg` & `runmanager-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/index.rst` & `runmanager-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/introduction.rst` & `runmanager-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/pyqt5-modified-objects.inv` & `runmanager-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/source/usage.rst` & `runmanager-3.2.0rc1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/using_runmanager.docx` & `runmanager-3.2.0rc1/docs/using_runmanager.docx`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/docs/using_runmanager.pdf` & `runmanager-3.2.0rc1/docs/using_runmanager.pdf`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/readthedocs.yaml` & `runmanager-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/__init__.py` & `runmanager-3.2.0rc1/runmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/__main__.py` & `runmanager-3.2.0rc1/runmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/__version__.py` & `runmanager-3.2.0rc1/runmanager/__version__.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/batch_compiler.py` & `runmanager-3.2.0rc1/runmanager/batch_compiler.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/functions.py` & `runmanager-3.2.0rc1/runmanager/functions.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/group.ui` & `runmanager-3.2.0rc1/runmanager/group.ui`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/main.ui` & `runmanager-3.2.0rc1/runmanager/main.ui`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/remote.py` & `runmanager-3.2.0rc1/runmanager/remote.py`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/runmanager.ico` & `runmanager-3.2.0rc1/runmanager/runmanager.ico`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager/runmanager.svg` & `runmanager-3.2.0rc1/runmanager/runmanager.svg`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/runmanager.egg-info/PKG-INFO` & `runmanager-3.2.0rc1/runmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: runmanager
-Version: 3.1.1
+Version: 3.2.0rc1
 Summary: Graphical control of parameterised experiments composed in labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runmanager
 Project-URL: Download, https://github.com/labscript-suite/runmanager/releases
 Project-URL: Tracker, https://github.com/labscript-suite/runmanager/issues
 Keywords: experiment control automation
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
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runmanager_32nx32n.svg" height="64" alt="the labscript suite – runmanager" align="right">
@@ -44,9 +45,7 @@
 
 runmanager can be run on any host with network access to the hardware supervisor [**blacs**](https://github.com/labscript-suite/blacs), and includes a remote programming interface for automation.
 
 
 ## Installation
 
 runmanager is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `runmanager-3.1.1/runmanager.egg-info/SOURCES.txt` & `runmanager-3.2.0rc1/runmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runmanager-3.1.1/setup.cfg` & `runmanager-3.2.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
@@ -40,16 +42,17 @@
 gui_scripts = 
 	runmanager-gui = desktop_app:entry_point
 
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

