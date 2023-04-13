# Comparing `tmp/runviewer-3.2.0.tar.gz` & `tmp/runviewer-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runviewer-3.2.0.tar", last modified: Thu Apr 13 00:41:13 2023, max compression
+gzip compressed data, was "runviewer-3.2.0rc1.tar", last modified: Thu Apr 13 00:36:19 2023, max compression
```

## Comparing `runviewer-3.2.0.tar` & `runviewer-3.2.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.733052 runviewer-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.717052 runviewer-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-13 00:40:58.000000 runviewer-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-13 00:40:58.000000 runviewer-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:40:58.000000 runviewer-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-13 00:41:13.733052 runviewer-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-13 00:40:58.000000 runviewer-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.725052 runviewer-3.2.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.729052 runviewer-3.2.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)   103187 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer.ico
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)   133946 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer_detail.png
--rw-r--r--   0 runner    (1001) docker     (123)    78458 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer_interface.png
--rw-r--r--   0 runner    (1001) docker     (123)   142366 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/img/runviewer_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-13 00:40:58.000000 runviewer-3.2.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 00:40:58.000000 runviewer-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:40:58.000000 runviewer-3.2.0/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.729052 runviewer-3.2.0/runviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78201 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)   159417 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/runviewer.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-04-13 00:40:58.000000 runviewer-3.2.0/runviewer/runviewer.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:41:13.733052 runviewer-3.2.0/runviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 00:41:13.000000 runviewer-3.2.0/runviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-13 00:41:13.733052 runviewer-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:40:58.000000 runviewer-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.382624 runviewer-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.386624 runviewer-3.2.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   103187 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   133946 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer_detail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78458 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer_interface.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142366 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/img/runviewer_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/runviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78201 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   159417 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/runviewer.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/runviewer/runviewer.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/runviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 00:36:19.000000 runviewer-3.2.0rc1/runviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-13 00:36:19.390624 runviewer-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:36:08.000000 runviewer-3.2.0rc1/setup.py
```

### Comparing `runviewer-3.2.0/.github/workflows/release.yml` & `runviewer-3.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/.gitignore` & `runviewer-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/LICENSE.txt` & `runviewer-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/PKG-INFO` & `runviewer-3.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runviewer
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: A program to view shots compiled by labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runviewer
 Project-URL: Download, https://github.com/labscript-suite/runviewer/releases
```

### Comparing `runviewer-3.2.0/README.md` & `runviewer-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/Makefile` & `runviewer-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/make.bat` & `runviewer-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/_static/custom.css` & `runviewer-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/_templates/components.rst` & `runviewer-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/conf.py` & `runviewer-3.2.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/blacs_32nx32n.svg` & `runviewer-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/labscript_32nx32n.svg` & `runviewer-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/lyse_32nx32n.svg` & `runviewer-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runmanager_32nx32n.svg` & `runviewer-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer.ico` & `runviewer-3.2.0rc1/docs/source/img/runviewer.ico`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer_32nx32n.svg` & `runviewer-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer_64x64.svg` & `runviewer-3.2.0rc1/docs/source/img/runviewer_64x64.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer_detail.png` & `runviewer-3.2.0rc1/docs/source/img/runviewer_detail.png`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer_interface.png` & `runviewer-3.2.0rc1/docs/source/img/runviewer_interface.png`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/img/runviewer_overview.png` & `runviewer-3.2.0rc1/docs/source/img/runviewer_overview.png`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/index.rst` & `runviewer-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/introduction.rst` & `runviewer-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/pyqt5-modified-objects.inv` & `runviewer-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/docs/source/usage.rst` & `runviewer-3.2.0rc1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/readthedocs.yaml` & `runviewer-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/__init__.py` & `runviewer-3.2.0rc1/runviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/__main__.py` & `runviewer-3.2.0rc1/runviewer/__main__.py`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/__version__.py` & `runviewer-3.2.0rc1/runviewer/__version__.py`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/main.ui` & `runviewer-3.2.0rc1/runviewer/main.ui`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/runviewer.ico` & `runviewer-3.2.0rc1/runviewer/runviewer.ico`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer/runviewer.svg` & `runviewer-3.2.0rc1/runviewer/runviewer.svg`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/runviewer.egg-info/PKG-INFO` & `runviewer-3.2.0rc1/runviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runviewer
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: A program to view shots compiled by labscript
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/runviewer
 Project-URL: Download, https://github.com/labscript-suite/runviewer/releases
```

### Comparing `runviewer-3.2.0/runviewer.egg-info/SOURCES.txt` & `runviewer-3.2.0rc1/runviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runviewer-3.2.0/setup.cfg` & `runviewer-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*

