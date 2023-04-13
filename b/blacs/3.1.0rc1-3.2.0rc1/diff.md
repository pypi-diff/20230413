# Comparing `tmp/blacs-3.1.0rc1.tar.gz` & `tmp/blacs-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacs-3.1.0rc1.tar", last modified: Fri Jan  7 07:24:18 2022, max compression
+gzip compressed data, was "blacs-3.2.0rc1.tar", last modified: Thu Apr 13 00:46:53 2023, max compression
```

## Comparing `blacs-3.1.0rc1.tar` & `blacs-3.2.0rc1.tar`

### file list

```diff
@@ -1,102 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.270166 blacs-3.1.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.274166 blacs-3.1.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.274166 blacs-3.1.0rc1/blacs/
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35880 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11444 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/analysis_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     5708 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/analysis_submission.ui
--rw-r--r--   0 runner    (1001) docker     (121)   165406 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/blacs.ico
--rw-r--r--   0 runner    (1001) docker     (121)    20912 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/blacs.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/compile_and_restart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/compile_and_restart.ui
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/desktop-app.json
--rw-r--r--   0 runner    (1001) docker     (121)    42310 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/device_base_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    50991 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/experiment_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)    21873 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/front_panel_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    27649 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/main.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.282167 blacs-3.1.0rc1/blacs/measure_ball/
--rw-r--r--   0 runner    (1001) docker     (121)  1998168 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/D3DX9_43.dll
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)  4232704 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/RabiBall.exe
--rw-r--r--   0 runner    (1001) docker     (121)    57248 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/data.win
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/options.ini
--rw-r--r--   0 runner    (1001) docker     (121)   679794 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/snd_mus_super_quantised_song.ogg
--rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/measure_ball/splash.png
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/notification_minimized_widget.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/notification_widget.ui
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)    37901 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/output_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugin_tab_frame.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.282167 blacs-3.1.0rc1/blacs/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.282167 blacs-3.1.0rc1/blacs/plugins/connection_table/
--rw-r--r--   0 runner    (1001) docker     (121)    21190 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/connection_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/connection_table/broken_device_notification.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5469 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/connection_table/connection_table.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/connection_table/notification.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.282167 blacs-3.1.0rc1/blacs/plugins/cycle_time/
--rw-r--r--   0 runner    (1001) docker     (121)     5208 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/cycle_time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/blacs/plugins/delete_repeated_shots/
--rw-r--r--   0 runner    (1001) docker     (121)     6322 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/delete_repeated_shots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4687 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/delete_repeated_shots/controls.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/blacs/plugins/general/
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/general/general.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/blacs/plugins/memory/
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/memory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/blacs/plugins/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (121)    16982 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/progress_bar/controls.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/blacs/plugins/theme/
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/plugins/theme/theme.ui
--rw-r--r--   0 runner    (1001) docker     (121)    58569 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/tab_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10190 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/tab_frame.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/tab_value_changed.ui
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/blacs/tab_value_changed_dds.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.274166 blacs-3.1.0rc1/blacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 07:24:17.000000 blacs-3.1.0rc1/blacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-07 07:24:18.000000 blacs-3.1.0rc1/blacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.286167 blacs-3.1.0rc1/docs/How to add a new device/
--rw-r--r--   0 runner    (1001) docker     (121)   192872 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/How to add a new device/main.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    72872 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/How to add a new device/main.tex
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/How to add a new device/pythonlisting.tex
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)   564324 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/UsingBLACS.docx
--rw-r--r--   0 runner    (1001) docker     (121)  1036936 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/UsingBLACS.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/_templates/components.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (121)   104672 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/blacs.ico
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/blacs_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12665 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14435 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13201 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-01-07 07:24:18.290167 blacs-3.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-01-07 07:24:12.000000 blacs-3.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.920793 blacs-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.892793 blacs-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.900793 blacs-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-13 00:46:53.920793 blacs-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.904793 blacs-3.2.0rc1/blacs/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36612 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/analysis_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/analysis_submission.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   165406 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/blacs.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    20912 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/blacs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/compile_and_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/compile_and_restart.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/desktop-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/device_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51011 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/experiment_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/front_panel_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/main.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/measure_ball/
+-rw-r--r--   0 runner    (1001) docker     (123)  1998168 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/D3DX9_43.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)  4232704 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/RabiBall.exe
+-rw-r--r--   0 runner    (1001) docker     (123)    57248 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/data.win
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   679794 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/snd_mus_super_quantised_song.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/measure_ball/splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/notification_minimized_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/notification_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37893 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/output_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugin_tab_frame.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/connection_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    21190 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/connection_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/connection_table/broken_device_notification.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/connection_table/connection_table.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/connection_table/notification.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/cycle_time/
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/cycle_time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/delete_repeated_shots/
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/delete_repeated_shots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/delete_repeated_shots/controls.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/general/general.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/memory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/progress_bar/controls.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.912793 blacs-3.2.0rc1/blacs/plugins/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/plugins/theme/theme.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    58573 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/tab_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/tab_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/tab_value_changed.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/blacs/tab_value_changed_dds.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.904793 blacs-3.2.0rc1/blacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 00:46:53.000000 blacs-3.2.0rc1/blacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/How to add a new device/
+-rw-r--r--   0 runner    (1001) docker     (123)   192872 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/How to add a new device/main.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    72872 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/How to add a new device/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/How to add a new device/pythonlisting.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   564324 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/UsingBLACS.docx
+-rw-r--r--   0 runner    (1001) docker     (123)  1036936 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/UsingBLACS.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.916793 blacs-3.2.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/device-tabs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:46:53.920793 blacs-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   104672 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   188028 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_monitoring.png
+-rw-r--r--   0 runner    (1001) docker     (123)   117641 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59805 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_pcie6363tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56164 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_pulseblastertab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39953 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_queueflowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   319475 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_queuemanagement.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41070 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/blacs_statemachine.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/shot-management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-13 00:46:53.920793 blacs-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 00:46:43.000000 blacs-3.2.0rc1/setup.py
```

### Comparing `blacs-3.1.0rc1/.github/workflows/release.yml` & `blacs-3.2.0rc1/.github/workflows/release.yml`

 * *Files 27% similar despite different names*

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
   PACKAGE_NAME: blacs
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
 
     if: github.repository == 'labscript-suite/blacs' && (github.event_name != 'create' || github.event.ref_type != 'branch')
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
     if: github.repository == 'labscript-suite/blacs' && (github.event_name != 'create' || github.event.ref_type != 'branch')
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

### Comparing `blacs-3.1.0rc1/.gitignore` & `blacs-3.2.0rc1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,8 +154,9 @@
 # conda build results
 conda_build/
 conda_packages/
 
 # Sphinx documentation
 docs/html/
 docs/source/_build/
-docs/source/components.rst
+docs/source/components.rst
+docs/source/api/_autosummary
```

### Comparing `blacs-3.1.0rc1/BSD-2-CLAUSE-LICENSE.txt` & `blacs-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/BSD-3-CLAUSE-LICENSE.txt` & `blacs-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/LICENSE.txt` & `blacs-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/NEWS.md` & `blacs-3.2.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/PKG-INFO` & `blacs-3.2.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: blacs
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Graphical labscript suite experiment queue and hardware interface
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/blacs
 Project-URL: Download, https://github.com/labscript-suite/blacs/releases
 Project-URL: Tracker, https://github.com/labscript-suite/blacs/issues
 Keywords: experiment control automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pyqt
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/blacs_32nx32n.svg" height="64" alt="the labscript suite – blacs" align="right">
@@ -39,9 +41,7 @@
 
 **blacs** supervises the execution of experiments controlled by the [*labscript suite*](https://github.com/labscript-suite/labscript-suite). It manages experiment queuing and hardware-timed execution, and provides manual control over devices between experiment shots.
 
 
 ## Installation
 
 blacs is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `blacs-3.1.0rc1/README.md` & `blacs-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/__init__.py` & `blacs-3.2.0rc1/blacs/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/__main__.py` & `blacs-3.2.0rc1/blacs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 #                                                                   #
 # This file is part of the program BLACS, in the labscript suite    #
 # (see http://labscriptsuite.org), and is licensed under the        #
 # Simplified BSD License. See the license.txt file in the root of   #
 # the project for the full license.                                 #
 #                                                                   #
 #####################################################################
+'''BLACS GUI and supporting code
+'''
 import labscript_utils.excepthook
 
 import os
 
 # Associate app windows with OS menu shortcuts:
 import desktop_app
 desktop_app.set_process_appid('blacs')
@@ -91,15 +93,15 @@
 from labscript_utils.labconfig import LabConfig
 from labscript_profile import hostname
 # Analysis Submission code
 from blacs.analysis_submission import AnalysisSubmission
 # Queue Manager Code
 from blacs.experiment_queue import QueueManager, QueueTreeview
 # Module containing hardware compatibility:
-import labscript_devices
+from labscript_utils import device_registry
 # Save/restore frontpanel code
 from blacs.front_panel_settings import FrontPanelSettings
 # Notifications system
 from blacs.notifications import Notifications
 # Preferences system
 from labscript_utils.settings import Settings
 #import settings_pages
@@ -262,15 +264,15 @@
                 self.settings_dict.setdefault(device_name,{"device_name":device_name})
                 # add common keys to settings:
                 self.settings_dict[device_name]["connection_table"] = self.connection_table
                 self.settings_dict[device_name]["front_panel_settings"] = settings[device_name] if device_name in settings else {}
                 self.settings_dict[device_name]["saved_data"] = tab_data[device_name]['data'] if device_name in tab_data else {}
                 # Instantiate the device
                 logger.info('instantiating %s'%device_name)
-                TabClass = labscript_devices.get_BLACS_tab(labscript_device_class_name)
+                TabClass = device_registry.get_BLACS_tab(labscript_device_class_name)
                 self.tablist[device_name] = TabClass(self.tab_widgets[0],self.settings_dict[device_name])
             except Exception:
                 self.failed_device_settings[device_name] = {"front_panel": self.settings_dict[device_name]["front_panel_settings"], "save_data": self.settings_dict[device_name]["saved_data"]}
                 del self.settings_dict[device_name]
                 del self.attached_devices[device_name]
                 self.connection_table.remove_device(device_name)
                 raise_exception_in_thread(sys.exc_info())
@@ -458,25 +460,34 @@
             # Anyway, no idea if this works cross platform (tested on windows 8)
             # Feel free to rewrite this, along with the code in front_panel_settings.py
             # which stores the values
             #
             # Actually this is a waste of time because if you close when maximized, reoopen and then
             # de-maximize, the window moves to a random position (not the position it was at before maximizing)
             # so bleh!
-            self.ui.move(tab_data['BLACS settings']["window_xpos"]-tab_data['BLACS settings']['window_frame_width']/2,tab_data['BLACS settings']["window_ypos"]-tab_data['BLACS settings']['window_frame_height']+tab_data['BLACS settings']['window_frame_width']/2)
-            self.ui.resize(tab_data['BLACS settings']["window_width"],tab_data['BLACS settings']["window_height"])
+            self.ui.move(
+                tab_data['BLACS settings']["window_xpos"]
+                - tab_data['BLACS settings']['window_frame_width'] // 2,
+                tab_data['BLACS settings']["window_ypos"]
+                - tab_data['BLACS settings']['window_frame_height']
+                + tab_data['BLACS settings']['window_frame_width'] // 2,
+            )
+            self.ui.resize(
+                tab_data['BLACS settings']["window_width"],
+                tab_data['BLACS settings']["window_height"],
+            )
 
             if 'window_maximized' in tab_data['BLACS settings'] and tab_data['BLACS settings']['window_maximized']:
                 self.ui.showMaximized()
 
             for pane_name,pane in self.panes.items():
                 pane.setSizes(tab_data['BLACS settings'][pane_name])
 
         except Exception as e:
-            logger.warning("Unable to load window and notebook defaults. Exception:"+str(e))
+            logger.exception("Unable to load window and notebook defaults. Exception:"+str(e))
 
     def order_tabs(self,tab_data):
         # Move the tabs to the correct notebook
         for tab_name in self.tablist.keys():
             notebook_num = 0
             if tab_name in tab_data:
                 notebook_num = int(tab_data[tab_name]["notebook"])
@@ -598,28 +609,38 @@
         # with h5py.File(self.settings_path,'r+') as h5file:
            # if 'connection table' in h5file:
                # del h5file['connection table']
 
         self.front_panel_settings.save_front_panel_to_h5(self.settings_path,data[0],data[1],data[2],data[3],{"overwrite":True},force_new_conn_table=True)
         logger.info('Shutting down workers')
         for tab in self.tablist.values():
-            tab.shutdown_workers()
+            # Tell tab to shutdown its workers if it has a method to do so.
+            if hasattr(tab, 'shutdown_workers'):
+                tab.shutdown_workers()
 
         QTimer.singleShot(100, self.finalise_quit)
 
     def finalise_quit(self, deadline=None, pending_threads=None):
         logger.info('finalise_quit called')
         WORKER_SHUTDOWN_TIMEOUT = 2
         if deadline is None:
             deadline = time.time() + WORKER_SHUTDOWN_TIMEOUT
         if pending_threads is None:
             pending_threads = {}
         overdue = time.time() > deadline
         # Check for worker shutdown completion:
         for name, tab in list(self.tablist.items()):
+            # Immediately close tabs that don't support finalise_close_tab()
+            if not hasattr(tab, 'finalise_close_tab'):
+                try:
+                    current_page = tab.close_tab(finalise=False)
+                except Exception as e:
+                    logger.error('Couldn\'t close tab:\n%s' % str(e))
+                del self.tablist[name]
+                continue
             fatal_error = tab.state == 'fatal error'
             if not tab.shutdown_workers_complete and overdue or fatal_error:
                 # Give up on cleanly shutting down this tab's worker processes:
                 tab.shutdown_workers_complete = True
             if tab.shutdown_workers_complete:
                 if name not in pending_threads:
                     # Either worker shutdown completed or we gave up. Close the tab.
```

### Comparing `blacs-3.1.0rc1/blacs/analysis_submission.py` & `blacs-3.2.0rc1/blacs/analysis_submission.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/analysis_submission.ui` & `blacs-3.2.0rc1/blacs/analysis_submission.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/blacs.ico` & `blacs-3.2.0rc1/blacs/blacs.ico`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/blacs.svg` & `blacs-3.2.0rc1/blacs/blacs.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/compile_and_restart.py` & `blacs-3.2.0rc1/blacs/compile_and_restart.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/compile_and_restart.ui` & `blacs-3.2.0rc1/blacs/compile_and_restart.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/device_base_class.py` & `blacs-3.2.0rc1/blacs/device_base_class.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/experiment_queue.py` & `blacs-3.2.0rc1/blacs/experiment_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #                                                                   #
 #####################################################################
 import queue
 import logging
 import os
 import threading
 import time
+import datetime
 import sys
 import shutil
 from collections import defaultdict
 from tempfile import gettempdir
 from binascii import hexlify
 
 from qtutils.qt.QtCore import *
@@ -594,15 +595,15 @@
                     stop_order = {}
                     for name in  hdf5_file['devices']:
                         device_properties = labscript_utils.properties.get(
                             hdf5_file, name, 'device_properties'
                         )
                         devices_in_use[name] = self.BLACS.tablist[name]
                         start_order[name] = device_properties.get('start_order', None)
-                        stop_order[name] = device_properties.get('start_order', None)
+                        stop_order[name] = device_properties.get('stop_order', None)
 
                 # Sort the devices into groups based on their start_order and stop_order
                 start_groups = defaultdict(set)
                 stop_groups = defaultdict(set)
                 for name in devices_in_use:
                     start_groups[start_order[name]].add(name)
                     stop_groups[stop_order[name]].add(name)
@@ -718,15 +719,15 @@
                 # Get front panel data, but don't save it to the h5 file until the experiment ends:
                 states,tab_positions,window_data,plugin_data = self.BLACS.front_panel_settings.get_save_data()
                 self.set_status("Running (program time: %.3fs)..."%(time.time() - start_time), path)
                     
                 # A Queue for event-based notification of when the experiment has finished.
                 experiment_finished_queue = queue.Queue()
                 logger.debug('About to start the master pseudoclock')
-                run_time = time.localtime()
+                run_time = datetime.datetime.now()
 
                 ##########################################################################################################################################
                 #                                                        Plugin callbacks                                                                #
                 ########################################################################################################################################## 
                 for callback in plugins.get_callbacks('science_starting'):
                     try:
                         callback(path)
@@ -846,15 +847,15 @@
             # start new try/except block here                   
             try:
                 with h5py.File(path,'r+') as hdf5_file:
                     self.BLACS.front_panel_settings.store_front_panel_in_h5(hdf5_file,states,tab_positions,window_data,plugin_data,save_conn_table=False, save_queue_data=False)
 
                     data_group = hdf5_file['/'].create_group('data')
                     # stamp with the run time of the experiment
-                    hdf5_file.attrs['run time'] = time.strftime('%Y%m%dT%H%M%S',run_time)
+                    hdf5_file.attrs['run time'] = run_time.strftime('%Y%m%dT%H%M%S.%f')
         
                 error_condition = False
                 response_list = {}
                 # Keep transitioning tabs to manual mode and waiting on them until they
                 # are all done or have all errored/restarted/failed. If one fails, we
                 # still have to transition the rest to manual mode:
                 while stop_groups:
```

### Comparing `blacs-3.1.0rc1/blacs/front_panel_settings.py` & `blacs-3.2.0rc1/blacs/front_panel_settings.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/main.ui` & `blacs-3.2.0rc1/blacs/main.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/D3DX9_43.dll` & `blacs-3.2.0rc1/blacs/measure_ball/D3DX9_43.dll`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/LICENSE` & `blacs-3.2.0rc1/blacs/measure_ball/LICENSE`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/RabiBall.exe` & `blacs-3.2.0rc1/blacs/measure_ball/RabiBall.exe`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/data.win` & `blacs-3.2.0rc1/blacs/measure_ball/data.win`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/snd_mus_super_quantised_song.ogg` & `blacs-3.2.0rc1/blacs/measure_ball/snd_mus_super_quantised_song.ogg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/measure_ball/splash.png` & `blacs-3.2.0rc1/blacs/measure_ball/splash.png`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/notification_minimized_widget.ui` & `blacs-3.2.0rc1/blacs/notification_minimized_widget.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/notification_widget.ui` & `blacs-3.2.0rc1/blacs/notification_widget.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/notifications.py` & `blacs-3.2.0rc1/blacs/notifications.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/output_classes.py` & `blacs-3.2.0rc1/blacs/output_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             # is an old-style unqualified class name expected to be in the globals()
             # dict of the unitconversions module, but does not exist.
             except (ImportError, AttributeError, KeyError):
                 cls = None
             if cls is None or not isinstance(calib_params, dict) or cls.base_unit != default_units:
                 # log an error:  
                 reason = ''
-                if calib_class is None:
+                if cls is None:
                     reason = f'The unit conversion class {calib_class} could not be imported. Ensure it is available on the computer running BLACS.'
                 elif not isinstance(calib_params, dict):
                     reason = 'The parameters for the unit conversion class are not a dictionary. Check your connection table code for errors and recompile it'
                 elif cls.base_unit != default_units:
                     reason = f'The base unit of your unit conversion class does not match this hardware channel. The hardware channel has base units {default_units} while your unit conversion class uses {cls.base_unit}'
                 self._logger.error('The unit conversion class (%s) could not be loaded. Reason: %s'%(calib_class,reason))   
                 # Use default units
```

### Comparing `blacs-3.1.0rc1/blacs/plugin_tab_frame.ui` & `blacs-3.2.0rc1/blacs/plugin_tab_frame.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/connection_table/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/connection_table/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/connection_table/broken_device_notification.ui` & `blacs-3.2.0rc1/blacs/plugins/connection_table/broken_device_notification.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/connection_table/connection_table.ui` & `blacs-3.2.0rc1/blacs/plugins/connection_table/connection_table.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/connection_table/notification.ui` & `blacs-3.2.0rc1/blacs/plugins/connection_table/notification.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/cycle_time/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/cycle_time/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/delete_repeated_shots/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/delete_repeated_shots/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/delete_repeated_shots/controls.ui` & `blacs-3.2.0rc1/blacs/plugins/delete_repeated_shots/controls.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/general/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/general/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/general/general.ui` & `blacs-3.2.0rc1/blacs/plugins/general/general.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/memory/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/progress_bar/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/progress_bar/controls.ui` & `blacs-3.2.0rc1/blacs/plugins/progress_bar/controls.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/theme/__init__.py` & `blacs-3.2.0rc1/blacs/plugins/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/plugins/theme/theme.ui` & `blacs-3.2.0rc1/blacs/plugins/theme/theme.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/tab_base_classes.py` & `blacs-3.2.0rc1/blacs/tab_base_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
             raise NotImplementedError(msg)
         remote_server_name = properties.get('worker', PRIMARY_BLACS)
         if remote_server_name != PRIMARY_BLACS:
             remote_server_device = table.find_by_name(remote_server_name)
             if remote_server_device.parent.name != PRIMARY_BLACS:
                 msg = "Multi-hop remote workers not yet supported by BLACS"
                 raise NotImplementedError(msg) 
-            remote_host, remote_port = remote_server_device.parent_port.split(':')
+            remote_host, remote_port = remote_server_device.parent_port.rsplit(':', 1)
             remote_port = int(remote_port)
             return RemoteProcessClient(remote_host, remote_port)
         return None
 
     def get_builtin_save_data(self):
         """Get builtin settings to be restored like whether the terminal is
         visible. Not to be overridden."""
```

### Comparing `blacs-3.1.0rc1/blacs/tab_frame.ui` & `blacs-3.2.0rc1/blacs/tab_frame.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/tab_value_changed.ui` & `blacs-3.2.0rc1/blacs/tab_value_changed.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs/tab_value_changed_dds.ui` & `blacs-3.2.0rc1/blacs/tab_value_changed_dds.ui`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/blacs.egg-info/PKG-INFO` & `blacs-3.2.0rc1/blacs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: blacs
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Graphical labscript suite experiment queue and hardware interface
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/blacs
 Project-URL: Download, https://github.com/labscript-suite/blacs/releases
 Project-URL: Tracker, https://github.com/labscript-suite/blacs/issues
 Keywords: experiment control automation
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pyqt
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/blacs_32nx32n.svg" height="64" alt="the labscript suite – blacs" align="right">
@@ -39,9 +41,7 @@
 
 **blacs** supervises the execution of experiments controlled by the [*labscript suite*](https://github.com/labscript-suite/labscript-suite). It manages experiment queuing and hardware-timed execution, and provides manual control over devices between experiment shots.
 
 
 ## Installation
 
 blacs is distributed as a Python package on [PyPI](https://pypi.org/user/labscript-suite) and [Anaconda Cloud](https://anaconda.org/labscript-suite), and should be installed with other components of the _labscript suite_. Please see the [installation guide](https://docs.labscriptsuite.org/en/latest/installation) for details.
-
-
```

### Comparing `blacs-3.1.0rc1/docs/How to add a new device/main.pdf` & `blacs-3.2.0rc1/docs/How to add a new device/main.pdf`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/How to add a new device/main.tex` & `blacs-3.2.0rc1/docs/How to add a new device/main.tex`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/How to add a new device/pythonlisting.tex` & `blacs-3.2.0rc1/docs/How to add a new device/pythonlisting.tex`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/Makefile` & `blacs-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/UsingBLACS.docx` & `blacs-3.2.0rc1/docs/UsingBLACS.docx`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/UsingBLACS.pdf` & `blacs-3.2.0rc1/docs/UsingBLACS.pdf`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/make.bat` & `blacs-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/_static/custom.css` & `blacs-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/_templates/components.rst` & `blacs-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/conf.py` & `blacs-3.2.0rc1/docs/source/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
+import copy
 import os
 from pathlib import Path
 from m2r import MdInclude
 from recommonmark.transform import AutoStructify
 from jinja2 import FileSystemLoader, Environment
 
 # -- Project information (unique to each project) -------------------------------------
@@ -35,24 +36,45 @@
 # -- General configuration (should be identical across all projects) ------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_rtd_theme",
     "recommonmark",
 ]
 
 autodoc_typehints = 'description'
+autosummary_generate = True
+numfig = True
+autodoc_mock_imports = ['labscript_utils']
+
+# mock missing site package methods
+import site
+mock_site_methods = {
+    # Format:
+    #   method name: return value
+    'getusersitepackages': '',
+    'getsitepackages': []
+}
+__fn = None
+for __name, __rval in mock_site_methods.items():
+    if not hasattr(site, __name):
+        __fn = lambda *args, __rval=copy.deepcopy(__rval), **kwargs: __rval
+        setattr(site, __name, __fn)
+del __name
+del __rval
+del __fn
 
 # Prefix each autosectionlabel with the name of the document it is in and a colon
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -68,23 +90,23 @@
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
@@ -219,7 +241,47 @@
             template.render(
                 intersphinx_mapping=intersphinx_mapping,
                 programs=labscript_suite_programs,
                 current_project=project,
                 img_path=img_path
             )
         )
+
+    # hooks to test docstring coverage
+    app.connect('autodoc-process-docstring', doc_coverage)
+    app.connect('build-finished', doc_report)
+
+
+members_to_watch = ['module', 'class', 'function', 'exception', 'method', 'attribute']
+doc_count = 0
+undoc_count = 0
+undoc_objects = []
+undoc_print_objects = False
+
+
+def doc_coverage(app, what, name, obj, options, lines):
+    global doc_count
+    global undoc_count
+    global undoc_objects
+
+    if (what in members_to_watch and len(lines) == 0):
+        # blank docstring detected
+        undoc_count += 1
+        undoc_objects.append(name)
+    else:
+        doc_count += 1
+
+
+def doc_report(app, exception):
+    global doc_count
+    global undoc_count
+    global undoc_objects
+    # print out report of documentation coverage
+    total_docs = undoc_count + doc_count
+    if total_docs != 0:
+        print(f'\nAPI Doc coverage of {doc_count/total_docs:.1%}')
+        if undoc_print_objects or os.environ.get('READTHEDOCS'):
+            print('\nItems lacking documentation')
+            print('===========================')
+            print(*undoc_objects, sep='\n')
+    else:
+        print('No docs counted, run \'make clean\' then rebuild to get the count.')
```

### Comparing `blacs-3.1.0rc1/docs/source/img/blacs.ico` & `blacs-3.2.0rc1/docs/source/img/blacs.ico`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/blacs_32nx32n.svg` & `blacs-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/blacs_64x64.svg` & `blacs-3.2.0rc1/docs/source/img/blacs_64x64.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/labscript_32nx32n.svg` & `blacs-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/lyse_32nx32n.svg` & `blacs-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/runmanager_32nx32n.svg` & `blacs-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/docs/source/img/runviewer_32nx32n.svg` & `blacs-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/readthedocs.yaml` & `blacs-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `blacs-3.1.0rc1/setup.cfg` & `blacs-3.2.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -14,39 +14,44 @@
 license = BSD
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	importlib_metadata
-	labscript_devices>=3.0.0
-	labscript_utils>=3.0.0
+	labscript_utils>=3.1.0b1
+	runmanager>=3.0.0
 	qtutils>=2.3.2
+	setuptools_scm>=4.1.0
 	zprocess>=2.14.1
 
 [options.entry_points]
 console_scripts = 
 	blacs = desktop_app:entry_point
 gui_scripts = 
 	blacs-gui = desktop_app:entry_point
 
 [options.extras_require]
 pyqt = PyQt5
 docs = 
 	PyQt5
-	Sphinx==3.0.1
-	sphinx-rtd-theme==0.4.3
+	Sphinx==4.4.0
+	sphinx-rtd-theme==0.5.2
 	recommonmark==0.6.0
 	m2r==0.2.1
+	mistune<2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

