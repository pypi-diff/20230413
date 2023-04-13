# Comparing `tmp/py-qgis-wps-1.8.5.tar.gz` & `tmp/py-qgis-wps-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-qgis-wps-1.8.5.tar", last modified: Tue Mar 28 09:49:47 2023, max compression
+gzip compressed data, was "py-qgis-wps-1.8.6.tar", last modified: Thu Apr 13 13:32:59 2023, max compression
```

## Comparing `py-qgis-wps-1.8.5.tar` & `py-qgis-wps-1.8.6.tar`

### file list

```diff
@@ -1,369 +1,369 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.761119 py-qgis-wps-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-03-28 09:49:47.761119 py-qgis-wps-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 09:49:46.000000 py-qgis-wps-1.8.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.725118 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/py_qgis_wps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.725118 py-qgis-wps-1.8.5/pyqgisservercontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgisservercontrib/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/core/componentmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/core/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/core/watchfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgisservercontrib/lizmapacl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/lizmapacl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgisservercontrib/lizmapacl/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgiswps/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/accesspolicy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgiswps/app/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/app/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/app/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/app/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/app/service.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-28 09:49:47.000000 py-qgis-wps-1.8.5/pyqgiswps/build.manifest
--rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgiswps/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgiswps/executors/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/io/datetimeio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/io/filesio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/io/geometryio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/io/layersio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/logstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/processfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/processingcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/processingexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/processingio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/executors/processingprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.729118 py-qgis-wps-1.8.5/pyqgiswps/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/basehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/oapihandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/owshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/processeshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/roothandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/statushandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/handlers/storehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.733118 py-qgis-wps-1.8.5/pyqgiswps/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.733118 py-qgis-wps-1.8.5/pyqgiswps/html/assets/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19188 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/assets/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.725118 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.733118 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    43852 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)    95910 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    76209 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    57721 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   178152 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   411645 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   144877 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   551641 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.737118 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   195855 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   326634 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    67742 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   273872 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   115048 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   195373 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    48944 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   161998 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/details.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/jquery.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.737118 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.737118 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/
--rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/data.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/octicons.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.753118 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/beaker.svg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bell.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/book.svg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bookmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/briefcase.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/broadcast.svg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/browser.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/calendar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/checklist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/circle-slash.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/circuit-board.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/clippy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/clock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/cloud-download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/cloud-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/comment-discussion.svg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/comment.svg
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/credit-card.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/dash.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/dashboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/database.svg
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/desktop-download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-camera-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-desktop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-mobile.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-added.svg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-ignored.svg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-modified.svg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-removed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-renamed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff.svg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/ellipsis.svg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/eye.svg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-binary.svg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-directory.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-media.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-submodule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-symlink-directory.svg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-symlink-file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-text.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/flame.svg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/fold.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gear.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gift.svg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gist-secret.svg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-branch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-commit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-compare.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-merge.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-pull-request.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/globe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/grabber.svg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/heart.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/history.svg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/horizontal-rule.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/hubot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/inbox.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-closed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-opened.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-reopened.svg
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/jersey.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/kebab-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/kebab-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/key.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/keyboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/law.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/light-bulb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/link-external.svg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/list-ordered.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/list-unordered.svg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/location.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/logo-gist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/logo-github.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail-read.svg
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail-reply.svg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mark-github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/megaphone.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mention.svg
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/milestone.svg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mirror.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mortar-board.svg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mute.svg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/no-newline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/note.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/octoface.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/organization.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/paintcan.svg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pencil.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/person.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plug.svg
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plus-small.svg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/primitive-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/primitive-square.svg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/project.svg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pulse.svg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/question.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/quote.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/radio-tower.svg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/reply.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-clone.svg
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-force-push.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-forked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-pull.svg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-push.svg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/rocket.svg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/rss.svg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/ruby.svg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/screen-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/screen-normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/shield.svg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sign-in.svg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/smiley.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/squirrel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/star.svg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sync.svg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tasklist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/telescope.svg
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/text-size.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/three-bars.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/thumbsdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/thumbsup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tools.svg
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/trashcan.svg
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unfold.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unmute.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unverified.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/verified.svg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/versions.svg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/watch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/zap.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.753118 py-qgis-wps-1.8.5/pyqgiswps/inout/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/literaltypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/inout/uoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.753118 py-qgis-wps-1.8.5/pyqgiswps/ogc/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.753118 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/api/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ogc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24982 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/ogc/traits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/conformance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/job_results.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/job_status.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/jobs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/landingpage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/paths.yml
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/process_description.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/process_execute.yml
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/openapi/processes.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/poolserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/poolserver/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/processing/ProcessingUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/qgscache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/qgscache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/qgscache/cachemanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/resources/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.725118 py-qgis-wps-1.8.5/pyqgiswps/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/README
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/bbox.json
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/crs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/geojson.json
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.757118 py-qgis-wps-1.8.5/pyqgiswps/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/filecache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/utils/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:49:47.761119 py-qgis-wps-1.8.5/pyqgiswps/validator/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/allowed_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/complexvalidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/literalvalidator.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/validator/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/pyqgiswps/wpsserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-28 09:49:47.761119 py-qgis-wps-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-28 09:49:31.000000 py-qgis-wps-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.938326 py-qgis-wps-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-04-13 13:32:59.938326 py-qgis-wps-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.898326 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/py_qgis_wps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.898326 py-qgis-wps-1.8.6/pyqgisservercontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgisservercontrib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/core/componentmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/core/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/core/watchfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgisservercontrib/lizmapacl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/lizmapacl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgisservercontrib/lizmapacl/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgiswps/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/accesspolicy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgiswps/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/app/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/app/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/app/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/app/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 13:32:59.000000 py-qgis-wps-1.8.6/pyqgiswps/build.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgiswps/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.902326 py-qgis-wps-1.8.6/pyqgiswps/executors/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/io/datetimeio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/io/filesio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/io/geometryio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/io/layersio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/logstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/processfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/processingcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/processingexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/processingio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/executors/processingprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.906326 py-qgis-wps-1.8.6/pyqgiswps/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/basehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/oapihandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/owshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/processeshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/roothandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/statushandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/handlers/storehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.906326 py-qgis-wps-1.8.6/pyqgiswps/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.906326 py-qgis-wps-1.8.6/pyqgiswps/html/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19188 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/assets/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.898326 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.906326 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    43852 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95910 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    76209 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    57721 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   178152 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   411645 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   144877 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   551641 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.910326 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   195855 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   326634 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    67742 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   273872 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   115048 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195373 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48944 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   161998 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/jquery.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.910326 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.910326 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/octicons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.930326 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/beaker.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bell.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bookmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/briefcase.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/broadcast.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/browser.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/calendar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/checklist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/circle-slash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/circuit-board.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/clippy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/clock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/cloud-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/cloud-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/comment-discussion.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/comment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/credit-card.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/dash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/dashboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/desktop-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-camera-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-added.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-ignored.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-modified.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-removed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-renamed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/ellipsis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-binary.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-directory.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-media.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-submodule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-symlink-directory.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-symlink-file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/flame.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/fold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gist-secret.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-branch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-commit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-compare.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-merge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-pull-request.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/globe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/grabber.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/heart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/history.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/horizontal-rule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/hubot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/inbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-opened.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-reopened.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/jersey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/kebab-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/kebab-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/key.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/keyboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/law.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/light-bulb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/link-external.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/list-ordered.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/list-unordered.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/location.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/logo-gist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/logo-github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail-read.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail-reply.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mark-github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/megaphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mention.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/milestone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mirror.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mortar-board.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/no-newline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/note.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/octoface.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/organization.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/paintcan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pencil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/person.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plus-small.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/primitive-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/primitive-square.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/project.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pulse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/question.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/quote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/radio-tower.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/reply.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-clone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-force-push.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-forked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-pull.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-push.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/rocket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/rss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/ruby.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/screen-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/screen-normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/shield.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sign-in.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/smiley.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/squirrel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/star.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sync.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tasklist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/telescope.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/text-size.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/three-bars.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/thumbsdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/thumbsup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tools.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/trashcan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unfold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unmute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unverified.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/verified.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/versions.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/watch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/zap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.930326 py-qgis-wps-1.8.6/pyqgiswps/inout/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/literaltypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/inout/uoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.930326 py-qgis-wps-1.8.6/pyqgiswps/ogc/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.930326 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/api/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ogc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.930326 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24982 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/ogc/traits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/conformance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/job_results.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/job_status.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/jobs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/landingpage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/paths.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/process_description.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/process_execute.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/openapi/processes.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/poolserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/poolserver/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/processing/ProcessingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/qgscache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/qgscache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/qgscache/cachemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/resources/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.898326 py-qgis-wps-1.8.6/pyqgiswps/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.934327 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/README
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/bbox.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/crs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/geojson.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/geometry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.938326 py-qgis-wps-1.8.6/pyqgiswps/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/filecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/utils/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:32:59.938326 py-qgis-wps-1.8.6/pyqgiswps/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/allowed_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/complexvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/literalvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/validator/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/pyqgiswps/wpsserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 13:32:59.938326 py-qgis-wps-1.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-13 13:32:41.000000 py-qgis-wps-1.8.6/setup.py
```

### Comparing `py-qgis-wps-1.8.5/LICENSE.txt` & `py-qgis-wps-1.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/PKG-INFO` & `py-qgis-wps-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-qgis-wps
-Version: 1.8.5
+Version: 1.8.6
 Summary: Py-Qgis-WPS is an implementation of the Web Processing Service standard from the Open Geospatial Consortium. qgis-wps is written in Python and is a fork of PyWPS 4.0.
 Home-page: https://github.com/3liz/py-qgis-wps
 Author: David Marteau
 Author-email: david.marteau@3liz.com
 Maintainer: David Marteau
 Maintainer-email: david.marteau@3liz.com
 Keywords: QGIS WPS OGC processing
```

### Comparing `py-qgis-wps-1.8.5/README.md` & `py-qgis-wps-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/py_qgis_wps.egg-info/PKG-INFO` & `py-qgis-wps-1.8.6/py_qgis_wps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-qgis-wps
-Version: 1.8.5
+Version: 1.8.6
 Summary: Py-Qgis-WPS is an implementation of the Web Processing Service standard from the Open Geospatial Consortium. qgis-wps is written in Python and is a fork of PyWPS 4.0.
 Home-page: https://github.com/3liz/py-qgis-wps
 Author: David Marteau
 Author-email: david.marteau@3liz.com
 Maintainer: David Marteau
 Maintainer-email: david.marteau@3liz.com
 Keywords: QGIS WPS OGC processing
```

### Comparing `py-qgis-wps-1.8.5/py_qgis_wps.egg-info/SOURCES.txt` & `py-qgis-wps-1.8.6/py_qgis_wps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgisservercontrib/core/componentmanager.py` & `py-qgis-wps-1.8.6/pyqgisservercontrib/core/componentmanager.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgisservercontrib/core/filters.py` & `py-qgis-wps-1.8.6/pyqgisservercontrib/core/filters.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgisservercontrib/core/watchfiles.py` & `py-qgis-wps-1.8.6/pyqgisservercontrib/core/watchfiles.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgisservercontrib/lizmapacl/filters.py` & `py-qgis-wps-1.8.6/pyqgisservercontrib/lizmapacl/filters.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/accesspolicy.py` & `py-qgis-wps-1.8.6/pyqgiswps/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/app/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/app/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/app/common.py` & `py-qgis-wps-1.8.6/pyqgiswps/app/common.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/app/process.py` & `py-qgis-wps-1.8.6/pyqgiswps/app/process.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/app/request.py` & `py-qgis-wps-1.8.6/pyqgiswps/app/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         if status_percentage is not None:
             self.status_percentage = status_percentage
 
         # Write response
         # rebuild the doc and update the status xml file
         self.document = self.get_execute_response()
         # check if storing of the status is requested
-        if self.document:
+        if len(self.document) > 0:
             self._write_response_doc(self.uuid, self.document)
         if self.status >= WPSResponse.STATUS.DONE_STATUS:
             self.process.clean()
 
         self._update_response(self.uuid)
 
     def _write_response_doc(self, request_uuid, doc):
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/app/service.py` & `py-qgis-wps-1.8.6/pyqgiswps/app/service.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/config.py` & `py-qgis-wps-1.8.6/pyqgiswps/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,22 @@
     CONFIG.set('server', 'processlifecycle', getenv('QGSWPS_SERVER_PROCESSLIFECYCLE', '1'))
     # Maximal number of waiting tasks - extra tasks will return a 509 in synchronous execution
     CONFIG.set('server', 'maxqueuesize', getenv('QGSWPS_SERVER_MAXQUEUESIZE', '100'))
     # Timeout for tasks execution
     CONFIG.set('server', 'response_timeout', getenv('QGSWPS_SERVER_RESPONSE_TIMEOUT', '1800'))
     # Expiration time in Redis cache for task responses
     CONFIG.set('server', 'response_expiration', getenv('QGSWPS_SERVER_RESPONSE_EXPIRATION', '86400'))
-    # Base url used for return WMS references (Qgis projects holding layers created by WPS tasks)
+    # XXX DEPRECATED Base url used for return WMS references (Qgis projects holding layers created by WPS tasks)
     CONFIG.set('server', 'wms_service_url', getenv('QGSWPS_SERVER_WMS_SERVICE_URL', '${wps.request:host_url}'))
+    # Base url used for return OWS references (Qgis projects holding layers created by WPS tasks)
+    CONFIG.set('server', 'ows_service_url', getenv('QGSWPS_SERVER_OWS_SERVICE_URL', '${wms_service_url}'))
     # Base uri used for the MAP argument in WMS references
     CONFIG.set('server', 'wps_result_map_uri', getenv('QGSWPS_SERVER_RESULTS_MAP_URI', 'wps-results:'))
     # Full URL used for returning  WPS references
-    CONFIG.set('server', 'wms_response_url', '${wms_service_url}?MAP={map_url}&service=WMS&request=GetCapabilities')
+    CONFIG.set('server', 'wms_response_url', '${ows_service_url}?MAP={map_url}&service=WMS&request=GetCapabilities')
     # Cleanup interval in seconds
     CONFIG.set('server', 'cleanup_interval', '600')
     # Download API expiration ttl for a download URL
     CONFIG.set('server', 'download_ttl', getenv('QGSWPS_DOWNLOAD_TTL', '30'))
     # Enable middleware filters from extensions
     CONFIG.set('server', 'enable_filters', getenv('QGSWPS_SERVER_ENABLE_FILTERS', 'no'))
     # Path for pre-installed extensions
@@ -206,17 +208,17 @@
     # XXX Not functional yet
     CONFIG.add_section('qgis.settings')
 
     #
     # Qgis projects
     #
     CONFIG.add_section('qgis.projects')
-    # Set this to force the the advertised WMS url in the Qgis projects
+    # Set this to force the the advertised OWS urls in the Qgis projects
     # created by pyqgiswps
-    CONFIG.set('qgis.projects', 'wmsurl', getenv('QGSWPS_ADVERTISED_WMSURL', '${server:wms_service_url}'))
+    CONFIG.set('qgis.projects', 'advertised_ows_url', getenv('QGSWPS_ADVERTISED_OWS_URL', '${server:ows_service_url}'))
 
     #
     # Metadata
     #
     CONFIG.add_section('metadata')
     CONFIG.set('metadata', 'identification_fees', 'NONE')
     CONFIG.set('metadata', 'identification_accessconstraints', 'NONE')
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/dependencies.py` & `py-qgis-wps-1.8.6/pyqgiswps/dependencies.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/exceptions.py` & `py-qgis-wps-1.8.6/pyqgiswps/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/io/datetimeio.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/io/datetimeio.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/io/filesio.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/io/filesio.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/io/geometryio.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/io/geometryio.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
                              LiteralOutput,
                              ComplexOutput,
                              BoundingBoxOutput)
 
 from pyqgiswps.exceptions import (NoApplicableCode,
                                   InvalidParameterValue)
 
-from qgis.core import (QgsCoordinateReferenceSystem,
-                       QgsWkbTypes,
+from qgis.core import (Qgis,
+                       QgsCoordinateReferenceSystem,
                        QgsGeometry,
                        QgsReferencedGeometry,
                        QgsRectangle,
                        QgsReferencedRectangle,
                        QgsReferencedPointXY,
                        QgsProcessingParameterDefinition,
                        QgsProcessingParameterGeometry,
@@ -46,14 +46,31 @@
 
 Geometry = Union[QgsGeometry, QgsReferencedGeometry]
 
 LOGGER = logging.getLogger('SRVLOG')
 
 GeometryParameterTypes = (QgsProcessingParameterPoint, QgsProcessingParameterGeometry)
 
+if Qgis.QGIS_VERSION_INT >= 33000:
+    # Geometry displaystring
+    GeomTypeDisplayString = {
+        Qgis.GeometryType.PointGeometry: 'Point',
+        Qgis.GeometryType.LineGeometry: 'Line',
+        Qgis.GeometryType.PolygonGeometry: 'Polygon',
+        Qgis.GeometryType.NullGeometry: 'Null',
+    }
+
+    def GetGeomTypeDisplayString(geomtype):
+        return GeomTypeDisplayString.get(geomtype, "Unknown")
+else:
+    from qgis.core import QgsWkbTypes
+
+    def GetGeomTypeDisplayString(geomtype):
+        return QgsWkbTypes.geometryDisplayString(geomtype)
+
 # ------------------------------------
 # Processing parameters ->  WPS input
 # ------------------------------------
 
 
 def parse_extent_input(param: QgsProcessingParameterDefinition, kwargs,
                        context: MapContext = None) -> BoundingBoxInput:
@@ -92,15 +109,15 @@
     elif isinstance(param, GeometryParameterTypes):
         kwargs['supported_formats'] = [Format.from_definition(FORMATS.GEOJSON),
                                        Format.from_definition(FORMATS.GML),
                                        Format.from_definition(FORMATS.WKT)]
         if isinstance(param, QgsProcessingParameterGeometry):
             # Add metadata from requiered geometryTypes
             kwargs['metadata'].extend(
-                Metadata('processing:geometryType', QgsWkbTypes.geometryDisplayString(geomtype))
+                Metadata('processing:geometryType', GetGeomTypeDisplayString(geomtype))
                 for geomtype in param.geometryTypes()
             )
             if param.allowMultipart():
                 kwargs['metadata'].append(Metadata('processing:allowMultipart'))
         return ComplexInput(**kwargs)
 
     return None
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/io/layersio.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/io/layersio.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/logstore.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/logstore.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/processfactory.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/processfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,16 @@
         # Do not intialize twice
         if self.qgisapp is not None:
             return
 
         logprefix = "[qgis:%s]" % os.getpid()
 
         settings = {
-            "Processing/Configuration/PREFER_FILENAME_AS_LAYER_NAME": "false"
+            "Processing/Configuration/PREFER_FILENAME_AS_LAYER_NAME": "false",  # Qgis < 3.30
+            "qgis/configuration/prefer-filename-as-layer-name": "false"         # Qgis >= 3.30
         }
 
         def _folders_setting(setting, folders):
             folders = folders.split(';')
             folders = chain(*(glob(f) for f in folders))
             folders = ';'.join(f for f in folders if os.path.isdir(f))
             if folders:
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/processingcontext.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/processingcontext.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,24 +96,26 @@
             if not path.exists():
                 raise FileNotFoundError(path.as_posix())
             return path
         except Exception:
             LOGGER.error(traceback.format_exc())
             raise
 
-    def write_result(self, workdir: str, name: str, wmsurl: Optional[str] = None) -> bool:
+    def write_result(self, workdir: str, name: str, advertised_url: Optional[str] = None) -> bool:
         """ Save results to disk
         """
         LOGGER.debug("Writing Results to %s", workdir)
 
         project = self.destination_project
 
         # Set project settings
-        if wmsurl:
-            project.writeEntry('WMSUrl', '/', wmsurl)
+        if advertised_url:
+            project.writeEntry('WMSUrl', '/', advertised_url)
+            project.writeEntry('WCSUrl', '/', advertised_url)
+            project.writeEntry('WFSUrl', '/', advertised_url)
 
         def _layers_for(layertype):
             return (lid for lid, lyr in project.mapLayers().items() if lyr.type() == layertype)
 
         # Publishing vector layers in WFS and raster layers in WCS
         project.writeEntry("WFSLayers", "/", list(_layers_for(QgsMapLayer.VectorLayer)))
         project.writeEntry("WCSLayers", "/", list(_layers_for(QgsMapLayer.RasterLayer)))
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/processingexecutor.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/processingexecutor.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/processingio.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/processingio.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/executors/processingprocess.py` & `py-qgis-wps-1.8.6/pyqgiswps/executors/processingprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,18 +366,18 @@
 
         context.wms_url = output_url
 
         run_algorithm(alg, parameters, feedback=feedback, context=context,
                       outputs=response.outputs,
                       create_context=create_context)
 
-        # Build advertised WMS url
-        wmsurl = f"{confservice.get('server','wms_service_url')}?MAP={output_map_url}"
+        # Build advertised OWS services url
+        advertised_url = f"{confservice.get('qgis.projects','advertised_ows_url')}?MAP={output_map_url}"
 
-        ok = context.write_result(context.workdir, destination, wmsurl)
+        ok = context.write_result(context.workdir, destination, advertised_url)
         if not ok:
             raise ProcessException("Failed to write %s" % destination)
 
         LOGGER.info("Task finished %s:%s", request.identifier, uuid_str)
 
         return response
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/basehandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/basehandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/oapihandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/oapihandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/owshandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/owshandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/processeshandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/processeshandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/roothandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/roothandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/statushandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/statushandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/handlers/storehandler.py` & `py-qgis-wps-1.8.6/pyqgiswps/handlers/storehandler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/healthcheck.py` & `py-qgis-wps-1.8.6/pyqgiswps/healthcheck.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/assets/popper.min.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/assets/popper.min.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.min.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/css/bootstrap.min.css.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.js.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.min.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/bootstrap/js/bootstrap.min.js.map` & `py-qgis-wps-1.8.6/pyqgiswps/html/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.html` & `py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.html`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/dashboard.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/dashboard.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/details.html` & `py-qgis-wps-1.8.6/pyqgiswps/html/details.html`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/icons.css` & `py-qgis-wps-1.8.6/pyqgiswps/html/icons.css`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/jquery.slim.min.js` & `py-qgis-wps-1.8.6/pyqgiswps/html/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/LICENSE` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/LICENSE`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/data.json` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/data.json`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/alert.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/alert.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-down.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-left.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-left.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-right.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-right.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-down.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-down.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-left.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-left.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-right.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-right.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-small-up.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-small-up.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/arrow-up.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/arrow-up.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/beaker.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/beaker.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bell.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bell.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bold.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bold.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/book.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/book.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bookmark.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bookmark.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/briefcase.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/briefcase.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/broadcast.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/broadcast.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/browser.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/browser.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/bug.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/bug.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/calendar.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/calendar.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/check.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/check.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/checklist.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/checklist.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-down.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-down.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-left.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-left.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-right.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-right.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/chevron-up.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/chevron-up.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/circle-slash.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/circle-slash.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/circuit-board.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/circuit-board.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/clippy.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/clippy.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/clock.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/clock.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/cloud-download.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/cloud-download.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/cloud-upload.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/cloud-upload.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/code.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/code.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/comment-discussion.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/comment-discussion.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/comment.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/comment.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/credit-card.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/credit-card.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/dash.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/dash.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/dashboard.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/dashboard.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/database.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/database.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/desktop-download.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/desktop-download.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-camera-video.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-camera-video.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-camera.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-camera.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-desktop.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-desktop.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/device-mobile.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/device-mobile.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-added.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-added.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-ignored.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-ignored.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-modified.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-modified.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-removed.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-removed.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff-renamed.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff-renamed.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/diff.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/diff.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/ellipsis.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/ellipsis.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/eye.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/eye.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-binary.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-binary.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-code.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-code.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-directory.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-directory.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-media.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-media.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-pdf.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-submodule.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-submodule.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-symlink-directory.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-symlink-directory.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-symlink-file.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-symlink-file.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file-zip.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file-zip.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/file.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/file.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/flame.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/flame.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/fold.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/fold.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gear.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gear.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gift.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gift.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gist-secret.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gist-secret.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/gist.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/gist.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-branch.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-branch.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-commit.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-commit.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-compare.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-compare.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-merge.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-merge.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/git-pull-request.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/git-pull-request.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/globe.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/globe.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/grabber.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/grabber.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/graph.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/graph.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/heart.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/heart.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/history.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/history.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/home.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/home.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/horizontal-rule.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/horizontal-rule.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/hubot.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/hubot.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/inbox.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/inbox.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/info.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/info.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-closed.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-closed.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-opened.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-opened.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/issue-reopened.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/issue-reopened.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/italic.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/italic.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/jersey.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/jersey.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/kebab-horizontal.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/kebab-horizontal.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/kebab-vertical.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/kebab-vertical.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/key.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/key.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/keyboard.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/keyboard.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/law.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/law.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/light-bulb.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/light-bulb.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/link-external.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/link-external.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/link.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/link.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/list-ordered.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/list-ordered.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/list-unordered.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/list-unordered.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/location.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/location.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/lock.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/lock.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/logo-gist.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/logo-gist.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/logo-github.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/logo-github.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail-read.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail-read.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail-reply.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail-reply.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mail.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mail.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mark-github.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/markdown.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/markdown.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/megaphone.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/megaphone.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mention.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mention.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/milestone.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/milestone.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mirror.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mirror.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mortar-board.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mortar-board.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/mute.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/mute.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/no-newline.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/no-newline.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/note.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/note.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/octoface.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/octoface.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/organization.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/organization.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/package.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/package.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/paintcan.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/paintcan.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pencil.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pencil.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/person.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/person.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pin.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pin.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plug.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plug.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plus-small.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plus-small.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/plus.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/primitive-dot.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/primitive-dot.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/primitive-square.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/primitive-square.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/project.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/project.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/pulse.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/pulse.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/question.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/question.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/quote.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/quote.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/radio-tower.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/radio-tower.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/reply.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/reply.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-clone.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-clone.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-force-push.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-force-push.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-forked.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-forked.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-pull.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-pull.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo-push.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo-push.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/repo.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/repo.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/rocket.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/rocket.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/rss.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/rss.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/ruby.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/ruby.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/screen-full.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/screen-full.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/screen-normal.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/screen-normal.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/search.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/search.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/server.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/server.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/settings.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/settings.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/shield.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/shield.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sign-in.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sign-in.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sign-out.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sign-out.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/smiley.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/smiley.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/squirrel.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/squirrel.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/star.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/star.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/stop.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/stop.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/sync.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/sync.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tag.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tag.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tasklist.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tasklist.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/telescope.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/telescope.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/terminal.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/terminal.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/text-size.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/text-size.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/three-bars.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/three-bars.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/thumbsdown.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/thumbsdown.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/thumbsup.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/thumbsup.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/tools.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/tools.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/trashcan.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/trashcan.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-down.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-down.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-left.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-left.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-right.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-right.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/triangle-up.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/triangle-up.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unfold.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unfold.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unmute.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unmute.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/unverified.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/unverified.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/verified.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/verified.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/versions.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/versions.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/watch.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/watch.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/x.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/x.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/html/octicons/lib/svg/zap.svg` & `py-qgis-wps-1.8.6/pyqgiswps/html/octicons/lib/svg/zap.svg`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/basic.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/basic.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/formats.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/formats.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/httpclient.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/httpclient.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/inputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/inputs.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/literaltypes.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/literaltypes.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/outputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/outputs.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/inout/uoms.py` & `py-qgis-wps-1.8.6/pyqgiswps/inout/uoms.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/logger.py` & `py-qgis-wps-1.8.6/pyqgiswps/logger.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/middleware.py` & `py-qgis-wps-1.8.6/pyqgiswps/middleware.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/inputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/inputs.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/outputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/outputs.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/process.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/process.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/request.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/request.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/api/response.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/api/response.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ogc.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ogc.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/inputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         if self.abstract:
             doc.append(OWS.Abstract(self.abstract))
 
         for m in self.metadata:
             doc.append(m.describe_xml())
 
-        if self.supported_formats is not None:
+        if self.supported_formats:
             default_format_el = self.supported_formats[0].describe_xml()
             supported_format_elements = [f.describe_xml() for f in self.supported_formats]
             doc.append(
                 E.ComplexData(
                     E.Default(default_format_el),
                     E.Supported(*supported_format_elements)
                 )
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/outputs.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/outputs.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/process.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/process.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/request.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/request.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/response.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/response.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/ows/schema.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/ows/schema.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/ogc/traits.py` & `py-qgis-wps-1.8.6/pyqgiswps/ogc/traits.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/conformance.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/conformance.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/job_results.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/job_results.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/job_status.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/job_status.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/jobs.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/jobs.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/landingpage.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/landingpage.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/process_description.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/process_description.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/process_execute.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/process_execute.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/openapi/processes.yml` & `py-qgis-wps-1.8.6/pyqgiswps/openapi/processes.yml`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/__main__.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/__main__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/client.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         context = zmq.asyncio.Context.instance()
 
         socket = context.socket(zmq.ROUTER)
         socket.setsockopt(zmq.LINGER, 500)
         socket.setsockopt(zmq.ROUTER_MANDATORY, 1)
         socket.bind(bindaddr)
 
-        self._running = False
         self._handlers = {}
         self._socket = socket
         self._maxqueue = maxqueue
 
         # Get track of available workers
         self._worker_q = asyncio.Queue()
         self._worker_s = []
```

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/pool.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/pool.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/server.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/server.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/supervisor.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/supervisor.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/utils.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/utils.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/poolserver/worker.py` & `py-qgis-wps-1.8.6/pyqgiswps/poolserver/worker.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/processing/ProcessingUtils.py` & `py-qgis-wps-1.8.6/pyqgiswps/processing/ProcessingUtils.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/qgscache/cachemanager.py` & `py-qgis-wps-1.8.6/pyqgiswps/qgscache/cachemanager.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/file_handler.py` & `py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/file_handler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/qgscache/handlers/postgres_handler.py` & `py-qgis-wps-1.8.6/pyqgiswps/qgscache/handlers/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/runtime.py` & `py-qgis-wps-1.8.6/pyqgiswps/runtime.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/crs.json` & `py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/crs.json`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/geojson.json` & `py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/geojson.json`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/schemas/geojson/geometry.json` & `py-qgis-wps-1.8.6/pyqgiswps/schemas/geojson/geometry.json`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/tests.py` & `py-qgis-wps-1.8.6/pyqgiswps/tests.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/contexts.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/decorators.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/filecache.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/lru.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/lru.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/plugins.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/qgis.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/qgis.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/utils/styles.py` & `py-qgis-wps-1.8.6/pyqgiswps/utils/styles.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/__init__.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/allowed_value.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/allowed_value.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/base.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/base.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/complexvalidator.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/complexvalidator.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/formats.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/formats.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/literalvalidator.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/literalvalidator.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/validator/mode.py` & `py-qgis-wps-1.8.6/pyqgiswps/validator/mode.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/version.py` & `py-qgis-wps-1.8.6/pyqgiswps/version.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/pyqgiswps/wpsserver.py` & `py-qgis-wps-1.8.6/pyqgiswps/wpsserver.py`

 * *Files identical despite different names*

### Comparing `py-qgis-wps-1.8.5/setup.py` & `py-qgis-wps-1.8.6/setup.py`

 * *Files identical despite different names*

