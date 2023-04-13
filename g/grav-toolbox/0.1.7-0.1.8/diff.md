# Comparing `tmp/grav-toolbox-0.1.7.tar.gz` & `tmp/grav-toolbox-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.1.7.tar", last modified: Mon Apr  3 11:30:45 2023, max compression
+gzip compressed data, was "grav-toolbox-0.1.8.tar", last modified: Thu Apr 13 12:58:31 2023, max compression
```

## Comparing `grav-toolbox-0.1.7.tar` & `grav-toolbox-0.1.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.578861 grav-toolbox-0.1.7/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-03 11:30:45.578861 grav-toolbox-0.1.7/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.1.7/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.562861 grav-toolbox-0.1.7/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.1.7/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.566861 grav-toolbox-0.1.7/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2021 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-04-03 11:30:45.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.1.7/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.566861 grav-toolbox-0.1.7/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.566861 grav-toolbox-0.1.7/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.1.7/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-04-03 11:29:54.000000 grav-toolbox-0.1.7/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.574861 grav-toolbox-0.1.7/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    60214 2023-03-31 11:19:29.000000 grav-toolbox-0.1.7/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-03-31 11:19:29.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9024 2023-03-31 11:19:29.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9520 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-03-31 11:19:29.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-03-31 11:19:29.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1805 2023-03-31 11:19:30.000000 grav-toolbox-0.1.7/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   190618 2023-04-03 11:25:58.000000 grav-toolbox-0.1.7/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-03-31 08:24:27.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-03-31 08:32:08.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-03-31 08:29:00.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-03-31 08:25:52.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-03-31 08:27:05.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-03-31 08:28:03.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-03-31 08:22:46.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-03-31 08:21:45.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10182 2023-04-03 11:19:10.000000 grav-toolbox-0.1.7/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.574861 grav-toolbox-0.1.7/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    47182 2023-04-03 11:25:58.000000 grav-toolbox-0.1.7/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    37918 2023-04-03 08:53:52.000000 grav-toolbox-0.1.7/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    39519 2023-03-25 23:21:42.000000 grav-toolbox-0.1.7/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35851 2023-03-25 23:21:42.000000 grav-toolbox-0.1.7/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-03-31 11:55:07.000000 grav-toolbox-0.1.7/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18595 2023-03-25 23:21:42.000000 grav-toolbox-0.1.7/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    21887 2023-03-25 23:21:42.000000 grav-toolbox-0.1.7/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    86806 2023-04-03 11:29:54.000000 grav-toolbox-0.1.7/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32293 2023-04-03 08:52:18.000000 grav-toolbox-0.1.7/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.578861 grav-toolbox-0.1.7/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9350 2023-03-29 20:27:47.000000 grav-toolbox-0.1.7/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-03 11:30:45.578861 grav-toolbox-0.1.7/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.1.7/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-04-03 11:30:45.578861 grav-toolbox-0.1.7/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.1.8/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.286594 grav-toolbox-0.1.8/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.1.8/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.286594 grav-toolbox-0.1.8/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2021 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.290593 grav-toolbox-0.1.8/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.290593 grav-toolbox-0.1.8/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.1.8/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-04-13 12:47:38.000000 grav-toolbox-0.1.8/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.302594 grav-toolbox-0.1.8/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    60214 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9024 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1805 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   191439 2023-04-05 13:08:26.000000 grav-toolbox-0.1.8/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.306594 grav-toolbox-0.1.8/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    47182 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    37918 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    39571 2023-04-13 12:34:11.000000 grav-toolbox-0.1.8/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35903 2023-04-13 12:34:49.000000 grav-toolbox-0.1.8/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18647 2023-04-13 12:35:28.000000 grav-toolbox-0.1.8/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    21920 2023-04-13 12:57:26.000000 grav-toolbox-0.1.8/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    86806 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32345 2023-04-13 12:35:06.000000 grav-toolbox-0.1.8/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.306594 grav-toolbox-0.1.8/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9492 2023-04-05 12:55:15.000000 grav-toolbox-0.1.8/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/setup.cfg
```

### Comparing `grav-toolbox-0.1.7/LICENSE` & `grav-toolbox-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/PKG-INFO` & `grav-toolbox-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.7
+Version: 0.1.8
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.7/README.md` & `grav-toolbox-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/adjust.py` & `grav-toolbox-0.1.8/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.1.8/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/command_line.py` & `grav-toolbox-0.1.8/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/drift_mlr.py` & `grav-toolbox-0.1.8/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/init.py` & `grav-toolbox-0.1.8/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/output.py` & `grav-toolbox-0.1.8/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/plots.py` & `grav-toolbox-0.1.8/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/schwaus.py` & `grav-toolbox-0.1.8/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/settings.py` & `grav-toolbox-0.1.8/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/bev_legacy/utils.py` & `grav-toolbox-0.1.8/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.1.8/grav_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.7
+Version: 0.1.8
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.7/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.1.8/grav_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.1.8/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.1.8/gravtools/CG5_utils/cg5_survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/__init__.py` & `grav-toolbox-0.1.8/gravtools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.1.7/gravtools/const.py` & `grav-toolbox-0.1.8/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/MainWindow.py` & `grav-toolbox-0.1.8/gravtools/gui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/__init__.py` & `grav-toolbox-0.1.8/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_about.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_corrections.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_gis_export_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,25 +34,31 @@
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_2.addItem(spacerItem)
         self.verticalLayout_3.addWidget(self.groupBox_general_settings)
         self.groupBox_export_lsm_run_results = QtWidgets.QGroupBox(Dialog_gis_settings)
         self.groupBox_export_lsm_run_results.setObjectName("groupBox_export_lsm_run_results")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.groupBox_export_lsm_run_results)
         self.verticalLayout.setObjectName("verticalLayout")
+        self.formLayout_3 = QtWidgets.QFormLayout()
+        self.formLayout_3.setObjectName("formLayout_3")
         self.radioButton_campaign_output_dir = QtWidgets.QRadioButton(self.groupBox_export_lsm_run_results)
         self.radioButton_campaign_output_dir.setChecked(True)
         self.radioButton_campaign_output_dir.setObjectName("radioButton_campaign_output_dir")
         self.buttonGroup_output_dir = QtWidgets.QButtonGroup(Dialog_gis_settings)
         self.buttonGroup_output_dir.setObjectName("buttonGroup_output_dir")
         self.buttonGroup_output_dir.addButton(self.radioButton_campaign_output_dir)
-        self.verticalLayout.addWidget(self.radioButton_campaign_output_dir)
+        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.radioButton_campaign_output_dir)
+        self.lineEdit_output_subdir = QtWidgets.QLineEdit(self.groupBox_export_lsm_run_results)
+        self.lineEdit_output_subdir.setObjectName("lineEdit_output_subdir")
+        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.lineEdit_output_subdir)
         self.radioButton_selected_output_dir = QtWidgets.QRadioButton(self.groupBox_export_lsm_run_results)
         self.radioButton_selected_output_dir.setObjectName("radioButton_selected_output_dir")
         self.buttonGroup_output_dir.addButton(self.radioButton_selected_output_dir)
-        self.verticalLayout.addWidget(self.radioButton_selected_output_dir)
+        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.radioButton_selected_output_dir)
+        self.verticalLayout.addLayout(self.formLayout_3)
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
         self.pushButton_select_gis_output_dir = QtWidgets.QPushButton(self.groupBox_export_lsm_run_results)
         self.pushButton_select_gis_output_dir.setEnabled(False)
         self.pushButton_select_gis_output_dir.setObjectName("pushButton_select_gis_output_dir")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.pushButton_select_gis_output_dir)
         self.lineEdit_gis_output_dir = QtWidgets.QLineEdit(self.groupBox_export_lsm_run_results)
@@ -93,17 +99,18 @@
 
     def retranslateUi(self, Dialog_gis_settings):
         _translate = QtCore.QCoreApplication.translate
         Dialog_gis_settings.setWindowTitle(_translate("Dialog_gis_settings", "GIS data export settings"))
         self.groupBox_general_settings.setTitle(_translate("Dialog_gis_settings", "General settings"))
         self.label.setText(_translate("Dialog_gis_settings", "EPSG code of station coordinates"))
         self.lineEdit_stat_coord_epsg.setToolTip(_translate("Dialog_gis_settings", "EPSG code that defines the coordiante reference system of the station coordinates loaded from the station data file or from the observation input file(s)."))
-        self.groupBox_export_lsm_run_results.setToolTip(_translate("Dialog_gis_settings", "Settings for the GIs data export in the Results tab (export of LSM run results for data visualization)."))
+        self.groupBox_export_lsm_run_results.setToolTip(_translate("Dialog_gis_settings", "Settings for the GIS data export in the Results tab (export of LSM run results for data visualization)."))
         self.groupBox_export_lsm_run_results.setTitle(_translate("Dialog_gis_settings", "Export for visualizing LSM run results"))
         self.radioButton_campaign_output_dir.setText(_translate("Dialog_gis_settings", "Write GIS files to campaign output directory"))
+        self.lineEdit_output_subdir.setToolTip(_translate("Dialog_gis_settings", "<html><head/><body><p>Subdirectory in the campaign\'s output directory for writing the results shapefiles.</p></body></html>"))
         self.radioButton_selected_output_dir.setText(_translate("Dialog_gis_settings", "Write GIS files to different output directroy"))
         self.pushButton_select_gis_output_dir.setToolTip(_translate("Dialog_gis_settings", "Select export directory"))
         self.pushButton_select_gis_output_dir.setText(_translate("Dialog_gis_settings", "Select export directory"))
         self.lineEdit_gis_output_dir.setToolTip(_translate("Dialog_gis_settings", "Export directory (derfault: campaign output directory)"))
         self.checkBox_export_stat_results_shp.setText(_translate("Dialog_gis_settings", "Export station results (shapefile)"))
         self.lineEdit_filename_stat_results_shp.setToolTip(_translate("Dialog_gis_settings", "Filename without \".shp\""))
         self.checkBox_export_obs_results_shp.setText(_translate("Dialog_gis_settings", "Export observation results (shapefile)"))
```

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_options.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/dialog_setup_data.py` & `grav-toolbox-0.1.8/gravtools/gui/dialog_setup_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_main.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,26 @@
             epsg_code = int(self.dlg_gis_export_settings.lineEdit_stat_coord_epsg.text())
         except ValueError:
             QMessageBox.critical(self, 'Error!', 'Invalid EPSG code. Need to be an integer value.')
             return
 
         # Get output directory:
         if self.dlg_gis_export_settings.radioButton_campaign_output_dir.isChecked():
-            gis_output_dir = self.campaign.output_directory
+            if self.dlg_gis_export_settings.lineEdit_output_subdir.text():
+                gis_output_dir = os.path.join(self.campaign.output_directory,
+                                              self.dlg_gis_export_settings.lineEdit_output_subdir.text())
+                if not os.path.isdir(gis_output_dir):
+                    try:
+                        os.mkdir(gis_output_dir)
+                    except PermissionError:
+                        QMessageBox.critical(self, 'Error!',
+                                             f'Cannot create the output directory for GIS results: {gis_output_dir}')
+                        return
+            else:
+                gis_output_dir = self.campaign.output_directory
         else:
             gis_output_dir = self.dlg_gis_export_settings.lineEdit_gis_output_dir.text()
         if not os.path.isdir(gis_output_dir):
             QMessageBox.critical(self, 'Error!',
                                  f'Invalid output directory for GIS files: {gis_output_dir}')
         else:
             # Export station results:
@@ -3027,14 +3038,15 @@
                     QMessageBox.warning(self,
                                         'Warning!',
                                         f'the current campaign already contains a survey named {new_cg5_survey.name}. '
                                         f'Survey names have to be unique within a campaign.')
                     self.statusBar().showMessage(f"No survey data added.")
             finally:
                 self.set_up_proxy_station_model()  # Re-connect the sort & filter proxy model to the station view.
+                self.set_up_survey_view_model()
                 self.on_checkBox_filter_observed_stat_only_toggled(
                     state=self.checkBox_filter_observed_stat_only.checkState())
                 self.enable_station_view_options_based_on_model()
                 # Show observed stations only based on Checkbox state:
                 self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
                                                                    auto_range_stations_plot=True)
         else:
@@ -3243,14 +3255,16 @@
         super().__init__(parent)
 
         # Run the .setupUi() method to show the GUI
         self.setupUi(self)
 
         # Connect signals and slots:
         self.pushButton_select_gis_output_dir.clicked.connect(self.get_output_directory_dialog)
+        # Set up GUI widgets:
+        self.lineEdit_output_subdir.setText(settings.GIS_RESULTS_OUTPUT_SUBDIR)
 
     def get_output_directory_dialog(self):
         """Open dialog to get the output directory."""
         if self.lineEdit_gis_output_dir.text():
             initial_folder_path = os.path.dirname(os.path.abspath(self.lineEdit_gis_output_dir.text()))
         else:
             try:
```

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_misc.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_setup_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.1.8/gravtools/gui/gui_model_survey_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,22 @@
 
     @property
     def get_data(self):
         return self._data
 
     def row_index_of_survey(self, survey_name: str):
         """Returns the row index of a survey in the current model"""
-        return self._survey_name_list.index(survey_name)
+        if self.no_data:
+            return None
+        else:
+            return self._survey_name_list.index(survey_name)
 
     def emit_data_changed_survey(self, survey_name: str):
         """Emits the data changed signal for the row of specifies survey."""
-        index_left = self.index(self.row_index_of_survey(survey_name), 0)
-        index_right = self.index(self.row_index_of_survey(survey_name), self.columnCount() - 1)
-        self.dataChanged.emit(index_left, index_right)
+        if not self.no_data:
+            index_left = self.index(self.row_index_of_survey(survey_name), 0)
+            index_right = self.index(self.row_index_of_survey(survey_name), self.columnCount() - 1)
+            self.dataChanged.emit(index_left, index_right)
+
+    @property
+    def no_data(self):
+        return not self._data
```

### Comparing `grav-toolbox-0.1.7/gravtools/models/__init__.py` & `grav-toolbox-0.1.8/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/campaign.py` & `grav-toolbox-0.1.8/gravtools/models/campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/exceptions.py` & `grav-toolbox-0.1.8/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/lsm.py` & `grav-toolbox-0.1.8/gravtools/models/lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/lsm_diff.py` & `grav-toolbox-0.1.8/gravtools/models/lsm_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,15 @@
             raise AssertionError('g and/or sd(g) is missing for at least one datum station! Both values are required'
                                  'for ALL datum stations.')
 
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (differential LSM) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
+            tmp_str += f'Comment: {self.comment}\n'
             tmp_str += f'\n'
             tmp_str += f'---- Input data and settings ----\n'
             tmp_str += f'Method: {settings.ADJUSTMENT_METHODS[self.lsm_method]}\n'
             tmp_str += f'Number of surveys: {number_of_surveys}\n'
             tmp_str += f'Number of stations: {number_of_stations}\n'
             tmp_str += f'Number of differential observations: {number_of_diff_obs}\n'
             tmp_str += f'Number of estimated parameters: {number_of_parameters}\n'
```

### Comparing `grav-toolbox-0.1.7/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.1.8/gravtools/models/lsm_nondiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
             raise AssertionError('g and/or sd(g) is missing for at least one datum station! Both values are required'
                                  'for ALL datum stations.')
 
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (non-differential LSM) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
+            tmp_str += f'Comment: {self.comment}\n'
             tmp_str += f'\n'
             tmp_str += f'---- Input data and settings ----\n'
             tmp_str += f'Method: {settings.ADJUSTMENT_METHODS[self.lsm_method]}\n'
             tmp_str += f'Number of surveys: {number_of_surveys}\n'
             tmp_str += f'Number of stations: {number_of_stations}\n'
             tmp_str += f'Number of observations: {number_of_observations}\n'
             tmp_str += f'Number of estimated parameters: {number_of_parameters}\n'
```

### Comparing `grav-toolbox-0.1.7/gravtools/models/misc.py` & `grav-toolbox-0.1.8/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.1.8/gravtools/models/mlr_bev_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
             raise AssertionError('Setup IDs are not unique within the campaign!')
 
         # Write log:
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (MLR, BEV legacy) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
+            tmp_str += f'Comment: {self.comment}\n'
             tmp_str += f'\n'
             tmp_str += f'---- Input data and settings ----\n'
             tmp_str += f'Number of surveys: {number_of_surveys}\n'
             tmp_str += f'Number of stations: {number_of_stations}\n'
             tmp_str += f'Number of observations: {number_of_observations}\n'
             # tmp_str += f'Number of estimated parameters: {number_of_parameters}\n'  # obsolet
             # tmp_str += f'Number of datum stations: {number_of_datum_stations}\n'  # ????????????????????ß
```

### Comparing `grav-toolbox-0.1.7/gravtools/models/station.py` & `grav-toolbox-0.1.8/gravtools/models/station.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,15 @@
         tmp_df.rename(columns={'lon_deg': 'long_deg', 'alt_m': 'height_m'}, inplace=True)
         tmp_df = self._stat_df_add_columns(tmp_df)
         tmp_df = self._stat_df_reorder_columns(tmp_df)
         tmp_df['is_datum'] = False
         tmp_df['is_observed'] = True
         tmp_df['source_type'] = 'obs_file'
         tmp_df['source_name'] = survey.name  # survey name
+        tmp_df['in_survey'] = ''
         tmp_df.reset_index(drop=True, inplace=True)
         tmp_df = tmp_df.astype(self._STAT_DF_COLUMNS_DTYPES)
 
         self.add_stations(tmp_df, data_source_type='obs_file', verbose=verbose)
 
         # # Add missing stations to stat_df by matching the station names only (location parameters of observed stations
         # # may differ!):
```

### Comparing `grav-toolbox-0.1.7/gravtools/models/survey.py` & `grav-toolbox-0.1.8/gravtools/models/survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/models/vg_lsm.py` & `grav-toolbox-0.1.8/gravtools/models/vg_lsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,15 @@
         if len(set(setup_ids)) != len(setup_ids):
             raise AssertionError('Setup IDs are not unique within the campaign!')
 
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (VG LGM estimation based on non-differential observations) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
+            tmp_str += f'Comment: {self.comment}\n'
             tmp_str += f'\n'
             tmp_str += f'---- Input data and settings ----\n'
             tmp_str += f'Method: {settings.ADJUSTMENT_METHODS[self.lsm_method]}\n'
             tmp_str += f'Number of stations (i.e. height levels): {number_of_stations}\n'
             tmp_str += f'Number of observations: {number_of_observations}\n'
             tmp_str += f'Number of estimated parameters: {number_of_parameters}\n'
             tmp_str += f'Degree of freedom: {number_of_observations - number_of_parameters}\n'
```

### Comparing `grav-toolbox-0.1.7/gravtools/scripts/__init__.py` & `grav-toolbox-0.1.8/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/scripts/run_gui.py` & `grav-toolbox-0.1.8/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/settings.py` & `grav-toolbox-0.1.8/gravtools/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
 # List of LSM methods where export of gis files is allowed:
 LSM_METHODS_GIS_EXPORT = [
     'LSM_diff',
     'LSM_non_diff',
 ]
 
+# Default subdirectory in the campaign's output directory for exporting the results as shapefiles:
+GIS_RESULTS_OUTPUT_SUBDIR = 'GIS_results'
+
 # List of LSM methods where VG plots are created (and should be saved as PNG files):
 LSM_METHODS_VG_PLOT = [
     'VG_LSM_nondiff',
 ]
 
 # Available iteration approaches for scaling the SD of setup observations:
 ITERATION_APPROACHES = {
```

### Comparing `grav-toolbox-0.1.7/gravtools/tides/__init__.py` & `grav-toolbox-0.1.8/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/gravtools/tides/longman1959.py` & `grav-toolbox-0.1.8/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.7/setup.cfg` & `grav-toolbox-0.1.8/setup.cfg`

 * *Files identical despite different names*

