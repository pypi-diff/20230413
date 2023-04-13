# Comparing `tmp/labscript-3.3.0.tar.gz` & `tmp/labscript-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-3.3.0.tar", last modified: Thu Apr 13 00:47:55 2023, max compression
+gzip compressed data, was "labscript-3.3.0rc1.tar", last modified: Thu Apr 13 00:44:20 2023, max compression
```

## Comparing `labscript-3.3.0.tar` & `labscript-3.3.0rc1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.187404 labscript-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.179403 labscript-3.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-13 00:47:41.000000 labscript-3.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-13 00:47:41.000000 labscript-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:47:41.000000 labscript-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-13 00:47:55.187404 labscript-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-13 00:47:41.000000 labscript-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   168705 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/Using the labscript API.docx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/labscript-dev/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/clock_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/header.tex
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/intermediatedevice_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    95705 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/main.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/labscript-dev/minted.sty
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.183403 labscript-3.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/connection_table.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.187404 labscript-3.3.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)   519203 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/connection_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:47:41.000000 labscript-3.3.0/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-13 00:47:41.000000 labscript-3.3.0/example.py
--rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-04-13 00:47:41.000000 labscript-3.3.0/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-04-13 00:47:41.000000 labscript-3.3.0/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.187404 labscript-3.3.0/labscript/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 00:47:41.000000 labscript-3.3.0/labscript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 00:47:41.000000 labscript-3.3.0/labscript/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-04-13 00:47:41.000000 labscript-3.3.0/labscript/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   186368 2023-04-13 00:47:41.000000 labscript-3.3.0/labscript/labscript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:55.187404 labscript-3.3.0/labscript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-13 00:47:55.000000 labscript-3.3.0/labscript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-13 00:47:55.000000 labscript-3.3.0/labscript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:47:55.000000 labscript-3.3.0/labscript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:47:54.000000 labscript-3.3.0/labscript.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 00:47:55.000000 labscript-3.3.0/labscript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 00:47:55.000000 labscript-3.3.0/labscript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 00:47:41.000000 labscript-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:47:41.000000 labscript-3.3.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-13 00:47:55.187404 labscript-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:47:41.000000 labscript-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.939310 labscript-3.3.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.931311 labscript-3.3.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.931311 labscript-3.3.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-13 00:44:20.939310 labscript-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   168705 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/Using the labscript API.docx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/labscript-dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/clock_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/header.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/intermediatedevice_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95705 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/main.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/labscript-dev/minted.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/connection_table.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.935310 labscript-3.3.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   519203 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/connection_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.939310 labscript-3.3.0rc1/labscript/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/labscript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/labscript/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/labscript/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186368 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/labscript/labscript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:44:20.939310 labscript-3.3.0rc1/labscript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 00:44:20.000000 labscript-3.3.0rc1/labscript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-13 00:44:20.939310 labscript-3.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:44:10.000000 labscript-3.3.0rc1/setup.py
```

### Comparing `labscript-3.3.0/.github/workflows/release.yml` & `labscript-3.3.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/.gitignore` & `labscript-3.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/LICENSE.txt` & `labscript-3.3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/PKG-INFO` & `labscript-3.3.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: The labscript compiler — expressive control of harware-timed experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript
 Project-URL: Download, https://github.com/labscript-suite/labscript/releases
```

### Comparing `labscript-3.3.0/README.md` & `labscript-3.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/Makefile` & `labscript-3.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/Using the labscript API.docx` & `labscript-3.3.0rc1/docs/Using the labscript API.docx`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/labscript-dev/header.tex` & `labscript-3.3.0rc1/docs/labscript-dev/header.tex`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/labscript-dev/intermediatedevice_example.py` & `labscript-3.3.0rc1/docs/labscript-dev/intermediatedevice_example.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/labscript-dev/main.pdf` & `labscript-3.3.0rc1/docs/labscript-dev/main.pdf`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/labscript-dev/main.tex` & `labscript-3.3.0rc1/docs/labscript-dev/main.tex`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/labscript-dev/minted.sty` & `labscript-3.3.0rc1/docs/labscript-dev/minted.sty`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/make.bat` & `labscript-3.3.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/_static/custom.css` & `labscript-3.3.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/_templates/autosummary-class.rst` & `labscript-3.3.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/_templates/autosummary-module.rst` & `labscript-3.3.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/_templates/components.rst` & `labscript-3.3.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/conf.py` & `labscript-3.3.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/connection_table.rst` & `labscript-3.3.0rc1/docs/source/connection_table.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/blacs_32nx32n.svg` & `labscript-3.3.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/connection_diagram.png` & `labscript-3.3.0rc1/docs/source/img/connection_diagram.png`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg` & `labscript-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/labscript.ico` & `labscript-3.3.0rc1/docs/source/img/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/labscript_32nx32n.svg` & `labscript-3.3.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/labscript_64x64.svg` & `labscript-3.3.0rc1/docs/source/img/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/lyse_32nx32n.svg` & `labscript-3.3.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/runmanager_32nx32n.svg` & `labscript-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/img/runviewer_32nx32n.svg` & `labscript-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/index.rst` & `labscript-3.3.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/introduction.rst` & `labscript-3.3.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/docs/source/pyqt5-modified-objects.inv` & `labscript-3.3.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/example.py` & `labscript-3.3.0rc1/example.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/icon.png` & `labscript-3.3.0rc1/icon.png`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/icon.svg` & `labscript-3.3.0rc1/icon.svg`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/labscript/__init__.py` & `labscript-3.3.0rc1/labscript/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/labscript/__version__.py` & `labscript-3.3.0rc1/labscript/__version__.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/labscript/functions.py` & `labscript-3.3.0rc1/labscript/functions.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/labscript/labscript.py` & `labscript-3.3.0rc1/labscript/labscript.py`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/labscript.egg-info/PKG-INFO` & `labscript-3.3.0rc1/labscript.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: The labscript compiler — expressive control of harware-timed experiments
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript
 Project-URL: Download, https://github.com/labscript-suite/labscript/releases
```

### Comparing `labscript-3.3.0/labscript.egg-info/SOURCES.txt` & `labscript-3.3.0rc1/labscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/readthedocs.yaml` & `labscript-3.3.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-3.3.0/setup.cfg` & `labscript-3.3.0rc1/setup.cfg`

 * *Files identical despite different names*

