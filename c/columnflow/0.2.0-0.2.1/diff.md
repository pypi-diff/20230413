# Comparing `tmp/columnflow-0.2.0.tar.gz` & `tmp/columnflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columnflow-0.2.0.tar", last modified: Thu Feb 23 13:47:35 2023, max compression
+gzip compressed data, was "columnflow-0.2.1.tar", last modified: Thu Apr 13 08:49:16 2023, max compression
```

## Comparing `columnflow-0.2.0.tar` & `columnflow-0.2.1.tar`

### file list

```diff
@@ -1,84 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.316426 columnflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-23 13:47:19.000000 columnflow-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-02-23 13:47:35.316426 columnflow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-02-23 13:47:19.000000 columnflow-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.300425 columnflow-0.2.0/columnflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow/calibration/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23343 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/cms/jets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24321 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/cms/jets_coffea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/cms/met.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/calibration/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   110289 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/columnar_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow/inference/
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow/inference/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/inference/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/inference/cms/datacard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.308426 columnflow-0.2.0/columnflow/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/plotting/plot_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/plotting/plot_functions_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/plotting/plot_functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/plotting/plot_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.308426 columnflow-0.2.0/columnflow/production/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/categories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.312426 columnflow-0.2.0/columnflow/production/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/btag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/gen_top_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/mc_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/muon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/cms/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/production/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.312426 columnflow-0.2.0/columnflow/selection/
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/selection/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.316426 columnflow-0.2.0/columnflow/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.316426 columnflow-0.2.0/columnflow/tasks/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/cms/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/cms/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    24207 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/cutflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.316426 columnflow-0.2.0/columnflow/tasks/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43077 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    37415 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25099 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/production.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/tasks/union.py
--rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-02-23 13:47:19.000000 columnflow-0.2.0/columnflow/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:47:35.304426 columnflow-0.2.0/columnflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 13:47:35.000000 columnflow-0.2.0/columnflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 13:47:35.316426 columnflow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-02-23 13:47:19.000000 columnflow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 08:49:01.000000 columnflow-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 08:49:16.855717 columnflow-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-04-13 08:49:01.000000 columnflow-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/calibration/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/jets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24321 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/jets_coffea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/met.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110900 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/columnar_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/inference/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/cms/datacard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_functions_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/production/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/categories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/production/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/btag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/gen_top_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/mc_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/muon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/selection/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/json_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/met_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cutflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43500 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/yields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25276 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:49:16.855717 columnflow-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-13 08:49:02.000000 columnflow-0.2.1/setup.py
```

### Comparing `columnflow-0.2.0/LICENSE` & `columnflow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/PKG-INFO` & `columnflow-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: columnflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: columnflow
-Home-page: https://github.com/uhh-cms/columnflow
-Author: The Columnflow Team
-Author-email: todo@uni-hamburg.de
+Home-page: https://github.com/columnflow/columnflow
+Author: The columnflow team
+Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,28 +20,28 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <center>
-  <a href="https://github.com/uhh-cms/columnflow">
-    <img src="https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/logo_dark.png" width="480" />
+  <a href="https://github.com/columnflow/columnflow">
+    <img src="https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/logo_dark.png" width="480" />
   </a>
 </center>
 
 
 <!-- marker-after-logo -->
 
 
-[![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml)
+[![Build status](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml)
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
-[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=master)](http://columnflow.readthedocs.io)
-[![Code coverge](https://codecov.io/gh/uhh-cms/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow)
-[![License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https://github.com/uhh-cms/columnflow/blob/master/LICENSE)
+[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
+[![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
+[![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
 
 <!-- marker-after-header -->
 
 
@@ -49,24 +49,24 @@
 
 This project is currently in a beta phase.
 The project setup, suggested workflows, definitions of particular tasks, and the signatures of various helper classes and functions are mostly frozen but could still be subject to changes in the near future.
 At this point (December 2022), four large-scale analyses based upon columnflow are being developed, and in the process, help test and verify various aspects of its core.
 The first released version is expected in early 2023.
 However, if you would like to join early on, contribute or just give it a spin, feel free to get in touch!
 
-![Columnflow analytics](https://repobeats.axiom.co/api/embed/bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics")
+![Columnflow analytics](https://repobeats.axiom.co/api/embed/b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics")
 
 
 ## Quickstart
 
-To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/uhh-cms/columnflow/tree/master/analysis_templates).
+To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/columnflow/columnflow/tree/master/analysis_templates)).
 The following command (no previous git clone required) interactively asks for a handful of names and settings, and creates a minimal, yet fully functioning project structure for you!
 
 ```shell
-bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/columnflow/master/create_analysis.sh)"
+bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/columnflow/master/create_analysis.sh)"
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
@@ -76,15 +76,15 @@
   2. Run local tests & linting checks to verify that the analysis is setup correctly.
     > ./tests/run_all
 
   3. Create a GRID proxy if you intend to run tasks that need one
     > voms-proxy-init -voms cms -rfc -valid 196:00
 
   4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/master/start.html
+    https://columnflow.readthedocs.io/en/stable/start.html
 
     Suggestions for tasks to run:
 
     a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
        default dataset using the default calibrator and default selector
        (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
@@ -95,15 +95,15 @@
     c) Include the ttbar dataset and also plot jet1_eta:
       > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 
     d) Create cms-style datacards for the example model in hgg/inference/example.py:
       > law run cf.CreateDatacards --version dev1 --inference-model example
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
@@ -115,36 +115,36 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=kramerto" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=kramerto" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mschrode" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=jolange" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mschrode" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=jolange" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 
 
 ## Development
 
-- Source hosted at [GitHub](https://github.com/uhh-cms/columnflow)
-- Report issues, questions, feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/issues)
+- Source hosted at [GitHub](https://github.com/columnflow/columnflow)
+- Report issues, questions, feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/issues)
 
 
 <!-- marker-after-body -->
```

#### html2text {}

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1 Name: columnflow Version: 0.2.0 Summary: columnflow Home-
-page: https://github.com/uhh-cms/columnflow Author: The Columnflow Team Author-
-email: todo@uni-hamburg.de License: BSD-3-Clause Keywords:
+Metadata-Version: 2.1 Name: columnflow Version: 0.2.1 Summary: columnflow Home-
+page: https://github.com/columnflow/columnflow Author: The columnflow team
+Author-email: github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Development Status :: 4 - Beta Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology Requires-Python: >=3.7,
 <4 Description-Content-Type: text/markdown License-File: LICENSE
- [https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/
+[https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/
                                 logo_dark.png]
- [![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/
-lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/
-workflows/lint_and_test.yaml) [![Package version](https://img.shields.io/pypi/
-v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow) [!
-[Documentation status](https://readthedocs.org/projects/columnflow/badge/
-?version=master)](http://columnflow.readthedocs.io) [![Code coverge](https://
-codecov.io/gh/uhh-cms/columnflow/branch/master/graph/
-badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow) [!
-[License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https:
-//github.com/uhh-cms/columnflow/blob/master/LICENSE) Backend for columnar,
-fully orchestrated HEP analyses with pure Python, [law](https://github.com/
-riga/law) and [order](https://github.com/riga/order).  ## Note on current
-development This project is currently in a beta phase. The project setup,
-suggested workflows, definitions of particular tasks, and the signatures of
-various helper classes and functions are mostly frozen but could still be
+ [![Build status](https://github.com/columnflow/columnflow/actions/workflows/
+lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/
+actions/workflows/lint_and_test.yaml) [![Package version](https://
+img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/
+columnflow) [![Documentation status](https://readthedocs.org/projects/
+columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
+coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
+badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
+[License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
+(https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
+columnar, fully orchestrated HEP analyses with pure Python, [law](https://
+github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
+current development This project is currently in a beta phase. The project
+setup, suggested workflows, definitions of particular tasks, and the signatures
+of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
 analytics](https://repobeats.axiom.co/api/embed/
-bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics") ##
+b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics") ##
 Quickstart To create an analysis using columnflow, it is recommended to start
 from a predefined template (located in [analysis_templates](https://github.com/
-uhh-cms/columnflow/tree/master/analysis_templates). The following command (no
-previous git clone required) interactively asks for a handful of names and
+columnflow/columnflow/tree/master/analysis_templates)). The following command
+(no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
-you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/
+you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
 repository and install the environment. > source setup.sh [optional_setup_name]
 2. Run local tests & linting checks to verify that the analysis is setup
 correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
 that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
 'Getting started' guide to run your first tasks. https://
-columnflow.readthedocs.io/en/master/start.html Suggestions for tasks to run: a)
+columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
 law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
 distribution for the single top dataset: > law run cf.PlotVariables1D --version
 dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
 plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
 --variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
 model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
 --inference-model example ``` For a better overview of the tasks that are
 triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827). ##
+graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
 Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
 hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
 github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
 /github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
 (https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
 events with CMS. - [analysis playground](https://github.com/uhh-cms/
 analysis_playground): A testing playground for HEP analyses. ## Contributors
@@ -75,10 +75,10 @@
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
                       ð»                ð»          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. ## Development - Source hosted at
-[GitHub](https://github.com/uhh-cms/columnflow) - Report issues, questions,
-feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/
+[GitHub](https://github.com/columnflow/columnflow) - Report issues, questions,
+feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/
 issues)
```

### Comparing `columnflow-0.2.0/README.md` & `columnflow-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <center>
-  <a href="https://github.com/uhh-cms/columnflow">
-    <img src="https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/logo_dark.png" width="480" />
+  <a href="https://github.com/columnflow/columnflow">
+    <img src="https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/logo_dark.png" width="480" />
   </a>
 </center>
 
 
 <!-- marker-after-logo -->
 
 
-[![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml)
+[![Build status](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml)
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
-[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=master)](http://columnflow.readthedocs.io)
-[![Code coverge](https://codecov.io/gh/uhh-cms/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow)
-[![License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https://github.com/uhh-cms/columnflow/blob/master/LICENSE)
+[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
+[![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
+[![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
 
 <!-- marker-after-header -->
 
 
@@ -24,24 +24,24 @@
 
 This project is currently in a beta phase.
 The project setup, suggested workflows, definitions of particular tasks, and the signatures of various helper classes and functions are mostly frozen but could still be subject to changes in the near future.
 At this point (December 2022), four large-scale analyses based upon columnflow are being developed, and in the process, help test and verify various aspects of its core.
 The first released version is expected in early 2023.
 However, if you would like to join early on, contribute or just give it a spin, feel free to get in touch!
 
-![Columnflow analytics](https://repobeats.axiom.co/api/embed/bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics")
+![Columnflow analytics](https://repobeats.axiom.co/api/embed/b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics")
 
 
 ## Quickstart
 
-To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/uhh-cms/columnflow/tree/master/analysis_templates).
+To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/columnflow/columnflow/tree/master/analysis_templates)).
 The following command (no previous git clone required) interactively asks for a handful of names and settings, and creates a minimal, yet fully functioning project structure for you!
 
 ```shell
-bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/columnflow/master/create_analysis.sh)"
+bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/columnflow/master/create_analysis.sh)"
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
@@ -51,15 +51,15 @@
   2. Run local tests & linting checks to verify that the analysis is setup correctly.
     > ./tests/run_all
 
   3. Create a GRID proxy if you intend to run tasks that need one
     > voms-proxy-init -voms cms -rfc -valid 196:00
 
   4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/master/start.html
+    https://columnflow.readthedocs.io/en/stable/start.html
 
     Suggestions for tasks to run:
 
     a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
        default dataset using the default calibrator and default selector
        (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
@@ -70,15 +70,15 @@
     c) Include the ttbar dataset and also plot jet1_eta:
       > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 
     d) Create cms-style datacards for the example model in hgg/inference/example.py:
       > law run cf.CreateDatacards --version dev1 --inference-model example
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
@@ -90,36 +90,36 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=kramerto" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=kramerto" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mschrode" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=jolange" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mschrode" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=jolange" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 
 
 ## Development
 
-- Source hosted at [GitHub](https://github.com/uhh-cms/columnflow)
-- Report issues, questions, feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/issues)
+- Source hosted at [GitHub](https://github.com/columnflow/columnflow)
+- Report issues, questions, feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/issues)
 
 
 <!-- marker-after-body -->
```

#### html2text {}

```diff
@@ -1,58 +1,58 @@
- [https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/
+[https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/
                                 logo_dark.png]
- [![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/
-lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/
-workflows/lint_and_test.yaml) [![Package version](https://img.shields.io/pypi/
-v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow) [!
-[Documentation status](https://readthedocs.org/projects/columnflow/badge/
-?version=master)](http://columnflow.readthedocs.io) [![Code coverge](https://
-codecov.io/gh/uhh-cms/columnflow/branch/master/graph/
-badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow) [!
-[License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https:
-//github.com/uhh-cms/columnflow/blob/master/LICENSE) Backend for columnar,
-fully orchestrated HEP analyses with pure Python, [law](https://github.com/
-riga/law) and [order](https://github.com/riga/order).  ## Note on current
-development This project is currently in a beta phase. The project setup,
-suggested workflows, definitions of particular tasks, and the signatures of
-various helper classes and functions are mostly frozen but could still be
+ [![Build status](https://github.com/columnflow/columnflow/actions/workflows/
+lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/
+actions/workflows/lint_and_test.yaml) [![Package version](https://
+img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/
+columnflow) [![Documentation status](https://readthedocs.org/projects/
+columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
+coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
+badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
+[License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
+(https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
+columnar, fully orchestrated HEP analyses with pure Python, [law](https://
+github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
+current development This project is currently in a beta phase. The project
+setup, suggested workflows, definitions of particular tasks, and the signatures
+of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
 analytics](https://repobeats.axiom.co/api/embed/
-bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics") ##
+b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics") ##
 Quickstart To create an analysis using columnflow, it is recommended to start
 from a predefined template (located in [analysis_templates](https://github.com/
-uhh-cms/columnflow/tree/master/analysis_templates). The following command (no
-previous git clone required) interactively asks for a handful of names and
+columnflow/columnflow/tree/master/analysis_templates)). The following command
+(no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
-you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/
+you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
 repository and install the environment. > source setup.sh [optional_setup_name]
 2. Run local tests & linting checks to verify that the analysis is setup
 correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
 that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
 'Getting started' guide to run your first tasks. https://
-columnflow.readthedocs.io/en/master/start.html Suggestions for tasks to run: a)
+columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
 law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
 distribution for the single top dataset: > law run cf.PlotVariables1D --version
 dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
 plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
 --variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
 model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
 --inference-model example ``` For a better overview of the tasks that are
 triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827). ##
+graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
 Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
 hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
 github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
 /github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
 (https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
 events with CMS. - [analysis playground](https://github.com/uhh-cms/
 analysis_playground): A testing playground for HEP analyses. ## Contributors
@@ -62,10 +62,10 @@
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
                       ð»                ð»          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. ## Development - Source hosted at
-[GitHub](https://github.com/uhh-cms/columnflow) - Report issues, questions,
-feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/
+[GitHub](https://github.com/columnflow/columnflow) - Report issues, questions,
+feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/
 issues)
```

### Comparing `columnflow-0.2.0/columnflow/__init__.py` & `columnflow-0.2.1/columnflow/__init__.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/calibration/__init__.py` & `columnflow-0.2.1/columnflow/calibration/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         if mc_only and data_only:
             raise Exception(f"calibrator {cls_name} received both mc_only and data_only")
         if mc_only or data_only:
             if cls_dict.get("skip_func"):
                 raise Exception(f"calibrator {cls_name} received custom skip_func, but mc_only or data_only are set")
 
             def skip_func(self):
-                return getattr(self, "dataset_inst", None) and self.dataset_inst.is_mc != bool(mc_only)
+                # never skip when there is not dataset
+                if not getattr(self, "dataset_inst", None):
+                    return False
+
+                return self.dataset_inst.is_mc != bool(mc_only)
 
             cls_dict["skip_func"] = skip_func
 
         # create the subclass
         subclass = Calibrator.derive(cls_name, bases=bases, cls_dict=cls_dict, module=module)
 
         return subclass
```

### Comparing `columnflow-0.2.0/columnflow/calibration/cms/jets.py` & `columnflow-0.2.1/columnflow/calibration/cms/jets_coffea.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,298 +1,272 @@
 # coding: utf-8
 
 """
-Jet energy corrections and jet resolution smearing.
+Calibration methods for jets
 """
 
+import os
 import functools
 
+import law
+
+from columnflow.util import maybe_import, memoize
 from columnflow.calibration import Calibrator, calibrator
-from columnflow.calibration.util import ak_random, propagate_met
+from columnflow.calibration.util import propagate_met, ak_random
 from columnflow.production.util import attach_coffea_behavior
-from columnflow.util import maybe_import
-from columnflow.columnar_util import set_ak_column, layout_ak_array
+from columnflow.columnar_util import set_ak_column
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
+coffea_extractor = maybe_import("coffea.lookup_tools.extractor")
+coffea_jetmet_tools = maybe_import("coffea.jetmet_tools")
+coffea_txt_converters = maybe_import("coffea.lookup_tools.txt_converters")
+
 
 #
-# helper functions
+# first, some utility functions
 #
 
 set_ak_column_f32 = functools.partial(set_ak_column, value_type=np.float32)
 
 
-def get_evaluators(correction_set, names):
+def get_basenames(struct):
     """
-    Helper function to get a list of correction evaluators from a correctionlib
-    *CorrectionSet* object given a list of *names*. The *names* can refer to either
-    simple or compound corrections.
-
-    Throws a *KeyError* if any of the *names* are not found.
-    """
-    # raise nice error if keys not found
-    available_keys = set(correction_set.keys()).union(correction_set.compound.keys())
-    missing_keys = set(names) - available_keys
-    if missing_keys:
-        raise RuntimeError("Corrections not found:" + "".join(
-            f"\n  - {name}" for name in names if name in missing_keys
-        ) + "\nAvailable:" + "".join(
-            f"\n  - {name}" for name in sorted(available_keys)
-        ))
-
-    # retrieve the evaluators
-    return [
-        correction_set.compound[name]
-        if name in correction_set.compound
-        else correction_set[name]
-        for name in names
-    ]
+    Replace full file paths in an arbitrary struct by the file basenames.
+    """
+    return law.util.map_struct(
+        lambda p: os.path.splitext(os.path.basename(p[0] if isinstance(p, tuple) else p))[0],
+        struct,
+    )
 
 
-def ak_evaluate(evaluator, *args):
+@memoize
+def get_lookup_provider(files, conversion_func, provider_cls, names=None):
     """
-    Evaluate a correctionlib *Correction* using one or more awkward arrays as inputs.
-    """
-    # fail if no arguments
-    if not args:
-        raise ValueError("Expected at least one argument.")
-
-    # collect arguments that are awkward arrays
-    ak_args = [
-        arg for arg in args if isinstance(arg, ak.Array)
-    ]
+    Create a coffea helper object for looking up information in files of various formats.
 
-    # broadcast akward arrays together and flatten
-    if ak_args:
-        bc_args = ak.broadcast_arrays(*ak_args)
-        flat_args = (
-            np.asarray(ak.flatten(bc_arg, axis=None))
-            for bc_arg in bc_args
-        )
-        output_layout_array = bc_args[0]
+    This function reads in the *files* containing lookup tables (e.g. JEC text files), extracts
+    the table of values ("weights") using the conversion function *conversion_func* implemented
+    in coffea, and uses them to construct a helper object of type *provider_cls* that can be
+    passed event data to yield the lookup values (e.g. a :py:class:`FactorizedJetCorrector` or
+    :py:class:`JetCorrectionUncertainty`).
+
+    Optionally, a list of *names* can be supplied to select only a subset of weight tables
+    for constructing the provider object (the default is to use all of them). This is intended
+    to be useful for e.g. selecting only a particular set of jet energy uncertainties from an
+    "UncertaintySources" file. By convention, the *names* always start with the basename of the
+    file that contains the corresponding weight table.
+
+    Entries in *names* may also be tuples of the form (*src_name*, *dst_name*), in which case the
+    *src_name* will be replaced by *dst_name* when passing the names to the *provider_cls*.
+
+    The user must ensure that the *files* can be parsed by the *conversion_func* supplied, and that
+    the information contained in the files is meaningful in connection with the *provider_cls*.
+    """
+    # the extractor reads the information contained in the files
+    extractor = coffea_extractor.extractor()
+
+    # files contain one or more lookup tables, each identified by a name
+    all_names = []
+    for file_ in files:
+        # the actual file parsing is done here
+        weights = conversion_func(file_)
+        for (name, type_), value in weights.items():
+            extractor.add_weight_set(name, type_, value)
+            all_names.append(name)
+
+    extractor.finalize()
+
+    # if user provided explicit names, check that corresponding
+    # weight tables have been read
+    if names is not None:
+        src_dst_names = [n if isinstance(n, tuple) else (n, n) for n in names]
+        unknown_names = set(src_name for src_name, _ in src_dst_names) - set(all_names)
+        if unknown_names:
+            unknown_names = ", ".join(sorted(list(unknown_names)))
+            available = ", ".join(sorted(list(all_names)))
+            raise ValueError(
+                f"no weight tables found for the following names: {unknown_names}, "
+                f"available: {available}",
+            )
     else:
-        flat_args = iter(())
-        output_layout_array = None
+        names = [(n, n) for n in all_names]
 
-    # multiplex flattened and non-awkward inputs
-    all_flat_args = [
-        next(flat_args) if isinstance(arg, ak.Array) else arg
-        for arg in args
-    ]
-
-    # apply evaluator to flattened/multiplexed inputs
-    result = evaluator.evaluate(*all_flat_args)
+    # the evaluator does the actual lookup for each separate name
+    evaluator = extractor.make_evaluator()
 
-    # apply broadcasted layout to result
-    if output_layout_array is not None:
-        result = layout_ak_array(result, output_layout_array)
+    # the provider combines lookup results from multiple names
+    provider = provider_cls(**{
+        dst_name: evaluator[src_name]
+        for src_name, dst_name in names
+    })
 
-    return result
+    return provider
 
 
 #
-# jet energy corrections
+# Jet energy corrections
 #
 
 @calibrator(
     uses={
         "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.area", "Jet.rawFactor",
-        "Jet.jetId", "fixedGridRhoFastjetAll", "Rho.fixedGridRhoFastjetAll",
+        "Jet.jetId",
+        "Rho.fixedGridRhoFastjetAll", "fixedGridRhoFastjetAll",
         attach_coffea_behavior,
     },
     produces={
         "Jet.pt", "Jet.mass", "Jet.rawFactor",
     },
     # custom uncertainty sources, defaults to config when empty
     uncertainty_sources=None,
     # toggle for propagation to MET
     propagate_met=True,
 )
-def jec(
+def jec_coffea(
     self: Calibrator,
     events: ak.Array,
     min_pt_met_prop: float = 15.0,
     max_eta_met_prop: float = 5.2,
     **kwargs,
 ) -> ak.Array:
     """
-    Performs the jet energy corrections and uncertainty shifts using the correctionlib, optionally
-    propagating the changes to the MET.
-
-    Requires an external file in the config, for instance:
-
-    .. code-block:: python
-
-        "jet_jerc": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz", "v1")  # noqa
-
-    An auxiliary entry in the config specifying the jet energy correction details is also
-    required, e.g.:
-
-    .. code-block:: python
-
-        cfg.x.jec = {
-            "campaign": "Summer19UL17",
-            "version": "V5",
-            "jet_type": "AK4PFchs",
-            "levels": ["L1L2L3Res"],  # or individual correction levels
-            "levels_for_type1_met": ["L1FastJet"],
-            "uncertainty_sources": [
-                "Total",
-                "CorrelationGroupMPFInSitu",
-                "CorrelationGroupIntercalibration",
-                "CorrelationGroupbJES",
-                "CorrelationGroupFlavor",
-                "CorrelationGroupUncorrelated",
-            ]
-        }
-
-    If running on data, the datasets must have an auxiliary field *jec_era* defined, e.g. "RunF".
+    Apply jet energy corrections and calculate shifts for jet energy uncertainty sources.
     """
     # calculate uncorrected pt, mass
     events = set_ak_column_f32(events, "Jet.pt_raw", events.Jet.pt * (1 - events.Jet.rawFactor))
     events = set_ak_column_f32(events, "Jet.mass_raw", events.Jet.mass * (1 - events.Jet.rawFactor))
 
-    def correct_jets(pt, area, eta, rho, evaluator_key="jec"):
-        # variable naming convention
-        variable_map = {
-            "JetA": area,
-            "JetEta": eta,
-            "JetPt": pt,
-            "Rho": ak.values_astype(rho, np.float32),
-        }
-
-        # apply all correctors sequentially, updating the pt each time
-        full_correction = ak.ones_like(pt, dtype=np.float32)
-        for corrector in self.evaluators[evaluator_key]:
-            # determine correct inputs (change depending on corrector)
-            inputs = [
-                variable_map[inp.name]
-                for inp in corrector.inputs
-            ]
-            correction = ak_evaluate(corrector, *inputs)
-            # update pt for subsequent correctors
-            variable_map["JetPt"] = variable_map["JetPt"] * correction
-            full_correction = full_correction * correction
-
-        return full_correction
+    # build/retrieve lookup providers for JECs and uncertainties
+    # NOTE: could also be moved to `jec_setup`, but keep here in case the provider ever needs
+    #       to change based on the event content (JEC change in the middle of a run)
+    jec_provider = get_lookup_provider(
+        self.jec_files,
+        coffea_txt_converters.convert_jec_txt_file,
+        coffea_jetmet_tools.FactorizedJetCorrector,
+        names=self.jec_names,
+    )
+    jec_provider_only_l1 = get_lookup_provider(
+        self.jec_files_only_l1,
+        coffea_txt_converters.convert_jec_txt_file,
+        coffea_jetmet_tools.FactorizedJetCorrector,
+        names=self.jec_names_only_l1,
+    )
+    if self.junc_names:
+        junc_provider = get_lookup_provider(
+            self.junc_files,
+            coffea_txt_converters.convert_junc_txt_file,
+            coffea_jetmet_tools.JetCorrectionUncertainty,
+            names=self.junc_names,
+        )
 
     # obtain rho, which might be located at different routes, depending on the nano version
     rho = (
         events.fixedGridRhoFastjetAll
         if "fixedGridRhoFastjetAll" in events.fields else
         events.Rho.fixedGridRhoFastjetAll
     )
 
-    # correct jets with only a subset of correction levels
-    # (for calculating TypeI MET correction)
-    if self.propagate_met:
-        # get correction factors
-        jec_factors_subset_type1_met = correct_jets(
-            pt=events.Jet.pt_raw,
-            eta=events.Jet.eta,
-            area=events.Jet.area,
-            rho=rho,
-            evaluator_key="jec_subset_type1_met",
-        )
+    # look up JEC correction factors
+    jec_factors = jec_provider.getCorrection(
+        JetEta=events.Jet.eta,
+        JetPt=events.Jet.pt_raw,
+        JetA=events.Jet.area,
+        Rho=rho,
+    )
+    jec_factors_only_l1 = jec_provider_only_l1.getCorrection(
+        JetEta=events.Jet.eta,
+        JetPt=events.Jet.pt_raw,
+        JetA=events.Jet.area,
+        Rho=rho,
+    )
 
-        # temporarily apply the new factors with only subset of corrections
-        events = set_ak_column_f32(events, "Jet.pt", events.Jet.pt_raw * jec_factors_subset_type1_met)
-        events = set_ak_column_f32(events, "Jet.mass", events.Jet.mass_raw * jec_factors_subset_type1_met)
-        events = self[attach_coffea_behavior](events, collections=["Jet"], **kwargs)
+    # apply the new factors with only L1 corrections
+    events = set_ak_column_f32(events, "Jet.pt", events.Jet.pt_raw * jec_factors_only_l1)
+    events = set_ak_column_f32(events, "Jet.mass", events.Jet.mass_raw * jec_factors_only_l1)
+    events = self[attach_coffea_behavior](events, collections=["Jet"], **kwargs)
 
-        # store pt and phi of the full jet system for MET propagation, including a selection in raw info
-        # see https://twiki.cern.ch/twiki/bin/view/CMS/JECAnalysesRecommendations?rev=19#Minimum_jet_selection_cuts
+    # store pt and phi of the full jet system for MET propagation, including a selection in raw info
+    # see https://twiki.cern.ch/twiki/bin/view/CMS/JECAnalysesRecommendations?rev=19#Minimum_jet_selection_cuts
+    if self.propagate_met:
         met_prop_mask = (events.Jet.pt_raw > min_pt_met_prop) & (abs(events.Jet.eta) < max_eta_met_prop)
         jetsum = events.Jet[met_prop_mask].sum(axis=1)
-        jetsum_pt_subset_type1_met = jetsum.pt
-        jetsum_phi_subset_type1_met = jetsum.phi
+        jet_pt_only_l1 = jetsum.pt
+        jet_phi_only_l1 = jetsum.phi
 
-    # factors for full jet correction with all levels
-    jec_factors = correct_jets(
-        pt=events.Jet.pt_raw,
-        eta=events.Jet.eta,
-        area=events.Jet.area,
-        rho=rho,
-        evaluator_key="jec",
-    )
-
-    # apply full jet correction
+    # full jet correction with all levels
     events = set_ak_column_f32(events, "Jet.pt", events.Jet.pt_raw * jec_factors)
     events = set_ak_column_f32(events, "Jet.mass", events.Jet.mass_raw * jec_factors)
     events = set_ak_column_f32(events, "Jet.rawFactor", (1 - events.Jet.pt_raw / events.Jet.pt))
     events = self[attach_coffea_behavior](events, collections=["Jet"], **kwargs)
 
     # nominal met propagation
     if self.propagate_met:
         # get pt and phi of all jets after correcting
         jetsum = events.Jet[met_prop_mask].sum(axis=1)
-        jetsum_pt_all_levels = jetsum.pt
-        jetsum_phi_all_levels = jetsum.phi
+        jet_pt_all_levels = jetsum.pt
+        jet_phi_all_levels = jetsum.phi
 
-        # propagate changes to MET, starting from jets corrected with subset of JEC levels
-        # (recommendation is to propagate only L2 corrections and onwards)
+        # propagate changes from L2 corrections and onwards (i.e. no L1) to MET
         met_pt, met_phi = propagate_met(
-            jetsum_pt_subset_type1_met,
-            jetsum_phi_subset_type1_met,
-            jetsum_pt_all_levels,
-            jetsum_phi_all_levels,
+            jet_pt_only_l1,
+            jet_phi_only_l1,
+            jet_pt_all_levels,
+            jet_phi_all_levels,
             events.RawMET.pt,
             events.RawMET.phi,
         )
         events = set_ak_column_f32(events, "MET.pt", met_pt)
         events = set_ak_column_f32(events, "MET.phi", met_phi)
 
-    # jet energy uncertainty components
-    for name, evaluator in self.evaluators["junc"].items():
-        # get uncertainty
-        jec_uncertainty = ak_evaluate(
-            evaluator,
-            events.Jet.eta,
-            events.Jet.pt_raw,
+    # look up JEC uncertainties
+    if self.junc_names:
+        jec_uncertainties = junc_provider.getUncertainty(
+            JetEta=events.Jet.eta,
+            JetPt=events.Jet.pt_raw,
         )
-
-        # apply jet uncertainty shifts
-        events = set_ak_column_f32(events, f"Jet.pt_jec_{name}_up", events.Jet.pt * (1.0 + jec_uncertainty))
-        events = set_ak_column_f32(events, f"Jet.pt_jec_{name}_down", events.Jet.pt * (1.0 - jec_uncertainty))
-        events = set_ak_column_f32(events, f"Jet.mass_jec_{name}_up", events.Jet.mass * (1.0 + jec_uncertainty))
-        events = set_ak_column_f32(events, f"Jet.mass_jec_{name}_down", events.Jet.mass * (1.0 - jec_uncertainty))
-
-        # propagate shifts to MET
-        if self.propagate_met:
-            jet_pt_up = events.Jet[met_prop_mask][f"pt_jec_{name}_up"]
-            jet_pt_down = events.Jet[met_prop_mask][f"pt_jec_{name}_down"]
-            met_pt_up, met_phi_up = propagate_met(
-                jetsum_pt_all_levels,
-                jetsum_phi_all_levels,
-                jet_pt_up,
-                events.Jet[met_prop_mask].phi,
-                met_pt,
-                met_phi,
-            )
-            met_pt_down, met_phi_down = propagate_met(
-                jetsum_pt_all_levels,
-                jetsum_phi_all_levels,
-                jet_pt_down,
-                events.Jet[met_prop_mask].phi,
-                met_pt,
-                met_phi,
-            )
-            events = set_ak_column_f32(events, f"MET.pt_jec_{name}_up", met_pt_up)
-            events = set_ak_column_f32(events, f"MET.pt_jec_{name}_down", met_pt_down)
-            events = set_ak_column_f32(events, f"MET.phi_jec_{name}_up", met_phi_up)
-            events = set_ak_column_f32(events, f"MET.phi_jec_{name}_down", met_phi_down)
+        for name, jec_unc_factors in jec_uncertainties:
+            # jec_unc_factors[I_EVT][I_JET][I_VAR]
+            events = set_ak_column_f32(events, f"Jet.pt_jec_{name}_up", events.Jet.pt * jec_unc_factors[:, :, 0])
+            events = set_ak_column_f32(events, f"Jet.pt_jec_{name}_down", events.Jet.pt * jec_unc_factors[:, :, 1])
+            events = set_ak_column_f32(events, f"Jet.mass_jec_{name}_up", events.Jet.mass * jec_unc_factors[:, :, 0])
+            events = set_ak_column_f32(events, f"Jet.mass_jec_{name}_down", events.Jet.mass * jec_unc_factors[:, :, 1])
+
+            # shifted MET propagation
+            if self.propagate_met:
+                jet_pt_up = events.Jet[met_prop_mask][f"pt_jec_{name}_up"]
+                jet_pt_down = events.Jet[met_prop_mask][f"pt_jec_{name}_down"]
+                met_pt_up, met_phi_up = propagate_met(
+                    jet_pt_all_levels,
+                    jet_phi_all_levels,
+                    jet_pt_up,
+                    events.Jet[met_prop_mask].phi,
+                    met_pt,
+                    met_phi,
+                )
+                met_pt_down, met_phi_down = propagate_met(
+                    jet_pt_all_levels,
+                    jet_phi_all_levels,
+                    jet_pt_down,
+                    events.Jet[met_prop_mask].phi,
+                    met_pt,
+                    met_phi,
+                )
+                events = set_ak_column_f32(events, f"MET.pt_jec_{name}_up", met_pt_up)
+                events = set_ak_column_f32(events, f"MET.pt_jec_{name}_down", met_pt_down)
+                events = set_ak_column_f32(events, f"MET.phi_jec_{name}_up", met_phi_up)
+                events = set_ak_column_f32(events, f"MET.phi_jec_{name}_down", met_phi_down)
 
     return events
 
 
-@jec.init
-def jec_init(self: Calibrator) -> None:
+@jec_coffea.init
+def jec_coffea_init(self: Calibrator) -> None:
     """
     Add JEC uncertainty shifts to the list of produced columns.
     """
     sources = self.uncertainty_sources
     if sources is None:
         sources = self.config_inst.x.jec.uncertainty_sources
 
@@ -314,73 +288,105 @@
             f"MET.{shifted_var}_jec_{junc_name}_{junc_dir}"
             for shifted_var in ("pt", "phi")
             for junc_name in sources
             for junc_dir in ("up", "down")
         }
 
 
-@jec.requires
-def jec_requires(self: Calibrator, reqs: dict) -> None:
+@jec_coffea.requires
+def jec_coffea_requires(self: Calibrator, reqs: dict) -> None:
+    """
+    Add external files bundle (for JEC text files) to dependencies.
+    """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
-@jec.setup
-def jec_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+@jec_coffea.setup
+def jec_coffea_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+    """
+    Determine correct JEC files for task based on config/dataset and inject them
+    into the calibrator function call.
+    """
+    # get external files bundle that contains JEC text files
     bundle = reqs["external_files"]
 
-    # import the correction sets from the external file
-    import correctionlib
-    correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.jet_jerc.load(formatter="gzip").decode("utf-8"),
-    )
-
-    # compute JEC keys from config information
-    jec = self.config_inst.x.jec
-
-    def make_jme_keys(names, jec=jec, is_data=self.dataset_inst.is_data):
-        if is_data:
-            jec_era = self.dataset_inst.get_aux("jec_era", None)
-            # if no special JEC era is specified, infer based on 'era'
-            if jec_era is None:
-                jec_era = "Run" + self.dataset_inst.get_aux("era")
-
-        return [
-            f"{jec.campaign}_{jec_era}_{jec.version}_DATA_{name}_{jec.jet_type}"
-            if is_data else
-            f"{jec.campaign}_{jec.version}_MC_{name}_{jec.jet_type}"
-            for name in names
-        ]
+    # make selector for JEC text files based on sample type (and era for data)
+    if self.dataset_inst.is_data:
+        jec_era = self.dataset_inst.get_aux("jec_era", None)
+        # if no special JEC era is specified, infer based on 'era'
+        if jec_era is None:
+            jec_era = "Run" + self.dataset_inst.get_aux("era")
+
+        resolve_samples = lambda x: x.data[jec_era]
+    else:
+        resolve_samples = lambda x: x.mc
+
+    # store jec files with all correction levels
+    self.jec_files = [
+        t.path
+        for t in resolve_samples(bundle.files.jec).values()
+    ]
+    self.jec_names = list(zip(
+        get_basenames(self.jec_files),
+        get_basenames(resolve_samples(self.config_inst.x.external_files.jec).values()),
+    ))
+
+    # store jec files with only L1* corrections for MET propagation
+    self.jec_files_only_l1 = [
+        t.path
+        for level, t in resolve_samples(bundle.files.jec).items()
+        if level.startswith("L1")
+    ]
+    self.jec_names_only_l1 = list(zip(
+        get_basenames(self.jec_files_only_l1),
+        get_basenames([
+            src
+            for level, src in resolve_samples(self.config_inst.x.external_files.jec).items()
+            if level.startswith("L1")
+        ]),
+    ))
+
+    # store uncertainty
+    self.junc_files = [
+        t.path
+        for t in resolve_samples(bundle.files.junc)
+    ]
+    self.junc_names = list(zip(
+        get_basenames(self.junc_files),
+        get_basenames(resolve_samples(self.config_inst.x.external_files.junc)),
+    ))
+
+    # ensure exactly one 'UncertaintySources' file is passed
+    if len(self.junc_names) != 1:
+        raise ValueError(
+            f"expected exactly one 'UncertaintySources' file, got {len(self.junc_names)}",
+        )
 
-    # take sources from constructor or config
     sources = self.uncertainty_sources
     if sources is None:
-        sources = jec.uncertainty_sources
+        sources = self.config_inst.x.jec.uncertainty_sources
 
-    jec_keys = make_jme_keys(jec.levels)
-    jec_keys_subset_type1_met = make_jme_keys(jec.levels_for_type1_met)
-    junc_keys = make_jme_keys(sources, is_data=False)  # uncertainties only stored as MC keys
-
-    # store the evaluators
-    self.evaluators = {
-        "jec": get_evaluators(correction_set, jec_keys),
-        "jec_subset_type1_met": get_evaluators(correction_set, jec_keys_subset_type1_met),
-        "junc": dict(zip(sources, get_evaluators(correction_set, junc_keys))),
-    }
+    # update the weight names to include the uncertainty sources specified in the config
+    self.junc_names = [
+        (f"{basename}_{src}", f"{orig_basename}_{src}")
+        for basename, orig_basename in self.junc_names
+        for src in sources
+    ]
 
 
 # custom jec calibrator that only runs nominal correction
-jec_nominal = jec.derive("jec_nominal", cls_dict={"uncertainty_sources": []})
+jec_coffea_nominal = jec_coffea.derive("jec_coffea_nominal", cls_dict={"uncertainty_sources": []})
 
 
 #
-# jet energy resolution smearing
+# Jet energy resolution smearing
 #
 
 @calibrator(
     uses={
         "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.genJetIdx",
         "Rho.fixedGridRhoFastjetAll", "fixedGridRhoFastjetAll",
         "nGenJet", "GenJet.pt", "GenJet.eta", "GenJet.phi",
@@ -395,79 +401,63 @@
         "MET.pt_jer_up", "MET.pt_jer_down", "MET.phi_jer_up", "MET.phi_jer_down",
     },
     # toggle for propagation to MET
     propagate_met=True,
     # only run on mc
     mc_only=True,
 )
-def jer(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
+def jer_coffea(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
     """
-    Applies the jet energy resolution smearing in MC and calculates the associated uncertainty shifts
-    using the correctionlib, following the recommendations given in
-    https://twiki.cern.ch/twiki/bin/viewauth/CMS/JetResolution.
-    Requires an external file in the config as (e.g.)
-
-    .. code-block:: python
-
-        "jet_jerc": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz", "v1")  # noqa
-
-    as well as an auxiliary entry in the config specifying the jet energy resolution details, e.g.:
-
-    .. code-block:: python
-
-        cfg.x.jer = {
-            "campaign": "Summer19UL17",
-            "version": "JRV2",
-            "jet_type": "AK4PFchs",
-        },
-
-    Throws an error if running on data.
+    Apply jet energy resolution smearing and calculate shifts for JER scale factor variations.
+    Follows the recommendations given in https://twiki.cern.ch/twiki/bin/viewauth/CMS/JetResolution.
     """
-    # fail when running on data
-    if self.dataset_inst.is_data:
-        raise ValueError("attempt to apply jet energy resolution smearing in data")
-
     # save the unsmeared properties in case they are needed later
     events = set_ak_column_f32(events, "Jet.pt_unsmeared", events.Jet.pt)
     events = set_ak_column_f32(events, "Jet.mass_unsmeared", events.Jet.mass)
 
     # use event numbers in chunk to seed random number generator
-    # TODO: use deterministic seeds!
+    # TODO: use seeds!
     rand_gen = np.random.Generator(np.random.SFC64(events.event.to_list()))
 
     # obtain rho, which might be located at different routes, depending on the nano version
     rho = (
         events.fixedGridRhoFastjetAll
         if "fixedGridRhoFastjetAll" in events.fields else
         events.Rho.fixedGridRhoFastjetAll
     )
 
-    # pt resolution
-    jer = ak_evaluate(
-        self.evaluators["jer"],
-        events.Jet.eta,
-        events.Jet.pt,
-        rho,
+    # build/retrieve lookup providers for JECs and uncertainties
+    # NOTE: could also be moved to `jer_setup`, but keep here in case the provider ever needs
+    #       to change based on the event content (JER change in the middle of a run)
+    jer_provider = get_lookup_provider(
+        self.jer_files,
+        coffea_txt_converters.convert_jr_txt_file,
+        coffea_jetmet_tools.JetResolution,
+        names=self.jer_names,
+    )
+    jersf_provider = get_lookup_provider(
+        self.jersf_files,
+        coffea_txt_converters.convert_jersf_txt_file,
+        coffea_jetmet_tools.JetResolutionScaleFactor,
+        names=self.jersf_names,
     )
 
-    # JER scale factors and systematic variations
-    jersf = {
-        syst: ak_evaluate(
-            self.evaluators["sf"],
-            events.Jet.eta,
-            syst,
-        )
-        for syst in ("nom", "up", "down")
-    }
-
-    # array with all JER scale factor variations as an additional axis
-    # (note: axis needs to be regular for broadcasting to work correctly)
-    jersf = ak.concatenate(
-        [jersf[syst][..., None] for syst in ("nom", "up", "down")],
-        axis=-1,
+    # look up jet energy resolutions
+    # jer[I_EVT][I_JET]
+    jer = ak.materialized(jer_provider.getResolution(
+        JetEta=events.Jet.eta,
+        JetPt=events.Jet.pt,
+        Rho=rho,
+    ))
+
+    # look up jet energy resolution scale factors
+    # jersf[I_EVT][I_JET][I_VAR]
+    jersf = jersf_provider.getScaleFactor(
+        JetEta=events.Jet.eta,
+        JetPt=events.Jet.pt,
     )
 
     # -- stochastic smearing
 
     # normally distributed random numbers according to JER
     jer_random_normal = ak_random(0, jer, rand_func=rand_gen.normal)
 
@@ -518,16 +508,16 @@
 
     # ensure array is not nullable (avoid ambiguity on Arrow/Parquet conversion)
     smear_factors = ak.fill_none(smear_factors, 0.0)
 
     # store pt and phi of the full jet system
     if self.propagate_met:
         jetsum = events.Jet.sum(axis=1)
-        jetsum_pt_before = jetsum.pt
-        jetsum_phi_before = jetsum.phi
+        jet_pt_before = jetsum.pt
+        jet_phi_before = jetsum.phi
 
     # apply the smearing factors to the pt and mass
     # (note: apply variations first since they refer to the original pt)
     events = set_ak_column_f32(events, "Jet.pt_jer_up", events.Jet.pt * smear_factors[:, :, 1])
     events = set_ak_column_f32(events, "Jet.mass_jer_up", events.Jet.mass * smear_factors[:, :, 1])
     events = set_ak_column_f32(events, "Jet.pt_jer_down", events.Jet.pt * smear_factors[:, :, 2])
     events = set_ak_column_f32(events, "Jet.mass_jer_down", events.Jet.mass * smear_factors[:, :, 2])
@@ -541,56 +531,54 @@
     if self.propagate_met:
         # save unsmeared quantities
         events = set_ak_column_f32(events, "MET.pt_unsmeared", events.MET.pt)
         events = set_ak_column_f32(events, "MET.phi_unsmeared", events.MET.phi)
 
         # get pt and phi of all jets after correcting
         jetsum = events.Jet.sum(axis=1)
-        jetsum_pt_after = jetsum.pt
-        jetsum_phi_after = jetsum.phi
+        jet_pt_after = jetsum.pt
+        jet_phi_after = jetsum.phi
 
         # propagate changes to MET
         met_pt, met_phi = propagate_met(
-            jetsum_pt_before,
-            jetsum_phi_before,
-            jetsum_pt_after,
-            jetsum_phi_after,
+            jet_pt_before,
+            jet_phi_before,
+            jet_pt_after,
+            jet_phi_after,
             events.MET.pt,
             events.MET.phi,
         )
-        events = set_ak_column_f32(events, "MET.pt", met_pt)
-        events = set_ak_column_f32(events, "MET.phi", met_phi)
-
-        # syst variations on top of corrected MET
         met_pt_up, met_phi_up = propagate_met(
-            jetsum_pt_after,
-            jetsum_phi_after,
+            jet_pt_after,
+            jet_phi_after,
             events.Jet.pt_jer_up,
             events.Jet.phi,
             met_pt,
             met_phi,
         )
         met_pt_down, met_phi_down = propagate_met(
-            jetsum_pt_after,
-            jetsum_phi_after,
+            jet_pt_after,
+            jet_phi_after,
             events.Jet.pt_jer_down,
             events.Jet.phi,
             met_pt,
             met_phi,
         )
+        events = set_ak_column_f32(events, "MET.pt", met_pt)
+        events = set_ak_column_f32(events, "MET.phi", met_phi)
         events = set_ak_column_f32(events, "MET.pt_jer_up", met_pt_up)
         events = set_ak_column_f32(events, "MET.pt_jer_down", met_pt_down)
         events = set_ak_column_f32(events, "MET.phi_jer_up", met_phi_up)
         events = set_ak_column_f32(events, "MET.phi_jer_down", met_phi_down)
 
     return events
 
 
-@jer.init
-def jer_init(self: Calibrator) -> None:
+@jer_coffea.init
+def jer_coffea_init(self: Calibrator) -> None:
     """
     Initialization of dynamic components of the jer calibrator.
     """
     if not self.propagate_met:
         return
 
     self.uses |= {
@@ -598,73 +586,78 @@
     }
     self.produces |= {
         "MET.pt", "MET.phi", "MET.pt_jer_up", "MET.pt_jer_down", "MET.phi_jer_up",
         "MET.phi_jer_down", "MET.pt_unsmeared", "MET.phi_unsmeared",
     }
 
 
-@jer.requires
-def jer_requires(self: Calibrator, reqs: dict) -> None:
+@jer_coffea.requires
+def jer_coffea_requires(self: Calibrator, reqs: dict) -> None:
     """
     Add external files bundle (for JR text files) to dependencies.
     """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
-@jer.setup
-def jer_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+@jer_coffea.setup
+def jer_coffea_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
     """
     Determine correct JR files for task based on config/dataset and inject them
     into the calibrator function call.
     """
+    # get external files bundle that contains JR text files
     bundle = reqs["external_files"]
 
-    # import the correction sets from the external file
-    import correctionlib
-    correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.jet_jerc.load(formatter="gzip").decode("utf-8"),
-    )
+    resolve_sample = lambda x: x.mc
 
-    # compute JER keys from config information
-    jer = self.config_inst.x.jer
-    jer_keys = {
-        "jer": f"{jer.campaign}_{jer.version}_MC_PtResolution_{jer.jet_type}",
-        "sf": f"{jer.campaign}_{jer.version}_MC_ScaleFactor_{jer.jet_type}",
-    }
+    # pass text files to calibrator method
+    for key in ("jer", "jersf"):
+        # pass the paths to the text files that contain the corrections/uncertainties
+        files = [
+            t.path for t in resolve_sample(bundle.files[key])
+        ]
+        setattr(self, f"{key}_files", files)
 
-    # store the evaluators
-    self.evaluators = {
-        name: get_evaluators(correction_set, [key])[0]
-        for name, key in jer_keys.items()
-    }
+        # also pass a list of tuples encoding the correspondence between the
+        # file basenames on disk (as determined by `BundleExternalFiles`) and the
+        # original file basenames (needed by coffea to identify the weights correctly)
+        basenames = get_basenames(files)
+        orig_basenames = get_basenames(resolve_sample(self.config_inst.x.external_files[key]))
+        setattr(self, f"{key}_names", list(zip(basenames, orig_basenames)))
+
+        # ensure exactly one file is passed
+        if len(files) != 1:
+            raise ValueError(
+                f"Expected exactly one file for key '{key}', got {len(files)}.",
+            )
 
 
 #
-# single calibrator for doing both JEC and JER smearing
+# General jets calibrator
 #
 
 @calibrator(
-    uses={jec, jer},
-    produces={jec, jer},
+    uses={jec_coffea, jer_coffea},
+    produces={jec_coffea, jer_coffea},
     # toggle for propagation to MET
     propagate_met=True,
 )
-def jets(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
+def jets_coffea(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
     # apply jet energy corrections
-    events = self[jec](events, **kwargs)
+    events = self[jec_coffea](events, **kwargs)
 
     # apply jer smearing on MC only
     if self.dataset_inst.is_mc:
-        events = self[jer](events, **kwargs)
+        events = self[jer_coffea](events, **kwargs)
 
     return events
 
 
-@jets.init
-def jets_init(self: Calibrator) -> None:
+@jets_coffea.init
+def jets_coffea_init(self: Calibrator) -> None:
     # forward the propagate_met argument to the producers
-    self.deps_kwargs[jec] = {"propagate_met": self.propagate_met}
-    self.deps_kwargs[jer] = {"propagate_met": self.propagate_met}
+    self.deps_kwargs[jec_coffea] = {"propagate_met": self.propagate_met}
+    self.deps_kwargs[jer_coffea] = {"propagate_met": self.propagate_met}
```

### Comparing `columnflow-0.2.0/columnflow/calibration/cms/met.py` & `columnflow-0.2.1/columnflow/calibration/cms/met.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,31 +12,42 @@
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 @calibrator(
     uses={"run", "PV.npvs", "MET.pt", "MET.phi"},
     produces={"MET.pt", "MET.phi"},
+    # function to determine the correction file
+    get_met_file=(lambda self, external_files: external_files.met_phi_corr),
+    # function to determine met correction config
+    get_met_config=(lambda self: self.config_inst.x.met_phi_correction_set),
 )
 def met_phi(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
     """
     Performs the MET phi (type II) correction using the correctionlib. Requires an external file in
-    the config as (e.g.)
+    the config under ``met_phi_corr``:
 
     .. code-block:: python
 
-        "met_phi_corr": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/met.json.gz", "v1")  # noqa
+        cfg.x.external_files = DotDict.wrap({
+            "met_phi_corr": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/met.json.gz",  # noqa
+        })
 
-    as well as an auxiliary entry in the config to refer to the name of the correction set such as
+    *get_met_file* can be adapted in a subclass in case it is stored differently in the external
+    files.
+
+    The name of the correction set should be present as an auxiliary entry in the config:
 
     .. code-block:: python
 
         cfg.x.met_phi_correction_set = "{variable}_metphicorr_pfmet_{data_source}"
 
     where "variable" and "data_source" are placeholders that are inserted in the calibrator setup.
+    *get_met_correction_set* can be adapted in a subclass in case it is stored differently in the
+    config.
     """
     args = (
         events.MET.pt,
         events.MET.phi,
         ak.values_astype(events.PV.npvs, np.float32),
         ak.values_astype(events.run, np.float32),
     )
@@ -61,17 +72,22 @@
 @met_phi.setup
 def met_phi_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
     bundle = reqs["external_files"]
 
     # create the pt and phi correctors
     import correctionlib
     correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.met_phi_corr.load(formatter="gzip").decode("utf-8"),
+        self.get_met_file(bundle.files).load(formatter="gzip").decode("utf-8"),
     )
-    self.met_pt_corrector = correction_set[self.config_inst.x.met_phi_correction_set.format(
+    name_tmpl = self.get_met_config()
+    self.met_pt_corrector = correction_set[name_tmpl.format(
         variable="pt",
         data_source=self.dataset_inst.data_source,
     )]
-    self.met_phi_corrector = correction_set[self.config_inst.x.met_phi_correction_set.format(
+    self.met_phi_corrector = correction_set[name_tmpl.format(
         variable="phi",
         data_source=self.dataset_inst.data_source,
     )]
+
+    # check versions
+    assert self.met_pt_corrector.version in [1]
+    assert self.met_phi_corrector.version in [1]
```

### Comparing `columnflow-0.2.0/columnflow/calibration/util.py` & `columnflow-0.2.1/columnflow/calibration/util.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/columnar_util.py` & `columnflow-0.2.1/columnflow/columnar_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 dak = maybe_import("dask_awkward")
 uproot = maybe_import("uproot")
 coffea = maybe_import("coffea")
 maybe_import("coffea.nanoevents")
 maybe_import("coffea.nanoevents.methods.base")
+maybe_import("coffea.nanoevents.methods.nanoaod")
 pq = maybe_import("pyarrow.parquet")
 
 logger = law.logger.get_logger(__name__)
 logger_perf = law.logger.get_logger(f"{__name__}-perf")
 
 
 #: Columns that are always required when opening a nano file with coffea.
@@ -989,16 +990,17 @@
     Attaches behavior of type *type_name* to an awkward array *ak_array* and returns it. *type_name*
     must be a key of a *behavior* dictionary which defaults to the "behavior" attribute of
     *ak_array* when present. Otherwise, a *ValueError* is raised.
 
     By default, all subfields of *ak_array* are kept. For further control, *skip_fields* can contain
     names or name patterns of fields that are filtered.
     """
+
     if behavior is None:
-        behavior = getattr(ak_array, "behavior", None)
+        behavior = getattr(ak_array, "behavior", None) or coffea.nanoevents.methods.nanoaod.behavior
         if behavior is None:
             raise ValueError(
                 f"behavior for type '{type_name}' is not set and not existing in input array",
             )
 
     # prepare field skipping
     keep_field = lambda field: True
@@ -1299,14 +1301,15 @@
     # class-level attributes as defaults
     call_func = None
     init_func = None
     skip_func = None
     uses = set()
     produces = set()
     _dependency_sets = {"uses", "produces"}
+    log_runtime = law.config.get_expanded_boolean("analysis", "log_array_function_runtime")
 
     # flags for declaring inputs (via uses) or outputs (via produces)
     class IOFlag(enum.Flag):
         AUTO = enum.auto()
         USES = enum.auto()
         PRODUCES = enum.auto()
 
@@ -1359,25 +1362,28 @@
     def __init__(
         self,
         call_func: Callable | None = law.no_value,
         init_func: Callable | None = law.no_value,
         skip_func: Callable | None = law.no_value,
         deferred_init: bool | None = True,
         instance_cache: dict | None = None,
+        log_runtime: bool | None = None,
         **kwargs,
     ):
         super().__init__()
 
         # add class-level attributes as defaults for unset arguments (no_value)
         if call_func == law.no_value:
             call_func = self.__class__.call_func
         if init_func == law.no_value:
             init_func = self.__class__.init_func
         if skip_func == law.no_value:
             skip_func = self.__class__.skip_func
+        if log_runtime is not None:
+            self.log_runtime = log_runtime
 
         # when a custom funcs are passed, bind them to this instance
         if call_func:
             self.call_func = call_func.__get__(self, self.__class__)
         if init_func:
             self.init_func = init_func.__get__(self, self.__class__)
         if skip_func:
@@ -1606,15 +1612,23 @@
         # raise in case the call is actually being skipped
         if callable(self.skip_func) and self.skip_func():
             raise Exception(
                 f"skip_func of {self} returned True, cannot invoke call_func; skip_func code: \n\n"
                 f"{get_source_code(self.skip_func, indent=4)}",
             )
 
-        return self.call_func(*args, **kwargs)
+        t1 = time.perf_counter()
+        try:
+            return self.call_func(*args, **kwargs)
+        finally:
+            if self.log_runtime:
+                duration = time.perf_counter() - t1
+                logger_perf.info(
+                    f"runtime of '{self.cls_name}': {law.util.human_duration(seconds=duration)}",
+                )
 
 
 class TaskArrayFunction(ArrayFunction):
     """
     Subclass of :py:class:`ArrayFunction` providing an interface to certain task features such as
     declaring dependent or produced shifts, task requirements, and defining a custom setup
     function. In addition, there is the option to update all these configurations based on task
```

### Comparing `columnflow-0.2.0/columnflow/config_util.py` & `columnflow-0.2.1/columnflow/config_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 Collection of general helpers and utilities.
 """
 
 from __future__ import annotations
 
 __all__ = [
     "get_root_processes_from_campaign", "add_shift_aliases", "get_shifts_from_sources",
-    "create_category_combinations",
+    "create_category_id", "add_category", "create_category_combinations",
 ]
 
 import re
 import itertools
 from typing import Callable, Any
 
+import law
 import order as od
 
 
 def get_root_processes_from_campaign(campaign: od.Campaign) -> od.UniqueObjectIndex:
     """
     Extracts all root process objects from datasets contained in an order campaign and returns them
     in a unique object index.
@@ -79,14 +80,53 @@
             [config.get_shift(f"{s}_up"), config.get_shift(f"{s}_down")]
             for s in shift_sources
         ),
         [],
     )
 
 
+def create_category_id(
+    config: od.Config,
+    category_name: str,
+    hash_len: int = 8,
+    salt: Any = None,
+) -> int:
+    """
+    Creates a unique id for a :py:class:`order.Category` named *category_name* in a
+    :py:class:`order.Config` object *config* and returns it. Internally,
+    :py:func:`law.util.create_hash` is used which receives *hash_len*. In case of an unintentional
+    (yet unlikely) collision of two ids, there is the option to add a custom *salt* value.
+    """
+    # create the hash
+    h = law.util.create_hash((config.name, config.id, category_name, salt), l=hash_len)
+    h = int(h, base=16)
+
+    # add an offset to ensure that are hashes are above a threshold
+    digits = len(str(int("F" * hash_len, base=16)))
+    h += int(10 ** digits)
+
+    return h
+
+
+def add_category(config: od.Config, **kwargs) -> od.Category:
+    """
+    Creates a :py:class:`order.Category` instance by forwarding all *kwargs* to its constructor,
+    adds it to a :py:class:`order.Config` object *config* and returns it. When *kwargs* do not
+    contain a field *id*, :py:func:`create_category_id` is used to create one.
+    """
+    if "name" not in kwargs:
+        fields = ",".join(map(str, kwargs))
+        raise ValueError(f"a field 'name' is required to create a category, got '{fields}'")
+
+    if "id" not in kwargs:
+        kwargs["id"] = create_category_id(config, kwargs["name"])
+
+    return config.add_category(**kwargs)
+
+
 def create_category_combinations(
     config: od.Config,
     categories: dict[str, list[od.Categories]],
     name_fn: Callable[[Any], str],
     kwargs_fn: Callable[[Any], dict] | None = None,
     skip_existing: bool = True,
 ) -> int:
@@ -99,19 +139,19 @@
     should be combined. The names are used as keyword arguments in a callable *name_fn* that is
     supposed to return the name of newly created categories (see example below).
 
     Each newly created category is instantiated with this name as well as arbitrary keyword
     arguments as returned by *kwargs_fn*. This function is called with the categories (in a
     dictionary, mapped to the sequence names as given in *categories*) that contribute to the newly
     created category and should return a dictionary. If the fields ``"id"`` and ``"selection"`` are
-    missing, they are filled with reasonable defaults leading to an auto-incremented id and a list
-    of all parent selection statements.
+    missing, they are filled with reasonable defaults leading to a auto-generated, deterministic id
+    and a list of all parent selection statements.
 
-    If the name of a new category is already known to *config* it skipped unless *skip_existing* is
-    *False*.
+    If the name of a new category is already known to *config* it is skipped unless *skip_existing*
+    is *False*.
 
     Example:
 
     .. code-block:: python
 
         categories = {
             "lepton": [cfg.get_category("e"), cfg.get_category("mu")],
@@ -164,24 +204,29 @@
 
                 # skip when already existing
                 if skip_existing and config.has_category(cat_name, deep=True):
                     continue
 
                 # create arguments for the new category
                 kwargs = kwargs_fn(root_cats) if callable(kwargs_fn) else {}
-                kwargs.setdefault("id", "+")
-                kwargs.setdefault("selection", [c.selection for c in root_cats.values()])
+                if "id" not in kwargs:
+                    kwargs["id"] = create_category_id(config, cat_name)
+                if "selection" not in kwargs:
+                    kwargs["selection"] = [c.selection for c in root_cats.values()]
 
                 # create the new category
                 cat = od.Category(name=cat_name, **kwargs)
                 n_created_categories += 1
 
                 # find direct parents and connect them
                 for _parent_group_names in itertools.combinations(_group_names, _n_groups - 1):
-                    parent_cat_name = name_fn(**{
-                        group_name: root_cats[group_name].name
-                        for group_name in _parent_group_names
-                    })
+                    if len(_parent_group_names) == 1:
+                        parent_cat_name = root_cats[_parent_group_names[0]].name
+                    else:
+                        parent_cat_name = name_fn(**{
+                            group_name: root_cats[group_name].name
+                            for group_name in _parent_group_names
+                        })
                     parent_cat = config.get_category(parent_cat_name, deep=True)
                     parent_cat.add_category(cat)
 
     return n_created_categories
```

### Comparing `columnflow-0.2.0/columnflow/inference/__init__.py` & `columnflow-0.2.1/columnflow/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/inference/cms/datacard.py` & `columnflow-0.2.1/columnflow/inference/cms/datacard.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/plotting/plot_all.py` & `columnflow-0.2.1/columnflow/plotting/plot_all.py`

 * *Files 11% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     style_config expects fields (all optional):
     "ax_cfg": dict,
     "rax_cfg": dict,
     "legend_cfg": dict,
     "cms_label_cfg": dict,
     """
     # available plot methods mapped to their names
-    plot_methods = {  # noqa
+    plot_methods = {
         func.__name__: func
         for func in [draw_error_bands, draw_stack, draw_hist, draw_errorbars]
     }
 
     plt.style.use(mplhep.style.CMS)
 
     rax = None
@@ -233,18 +233,19 @@
             handles = shuffle(handles, in_stack)
             labels = shuffle(labels, in_stack)
 
         # make legend using ordered handles/labels
         ax.legend(handles, labels, **legend_kwargs)
 
     # custom annotation
+    log_x = style_config.get("ax_cfg", {}).get("xscale", "linear") == "log"
     annotate_kwargs = {
         "text": "",
         "xy": (
-            get_position(*ax.get_xlim(), factor=0.05, logscale=False),
+            get_position(*ax.get_xlim(), factor=0.05, logscale=log_x),
             get_position(*ax.get_ylim(), factor=0.95, logscale=log_y),
         ),
         "xycoords": "data",
         "color": "black",
         "fontsize": 22,
         "horizontalalignment": "left",
         "verticalalignment": "top",
@@ -253,17 +254,19 @@
     ax.annotate(**annotate_kwargs)
 
     # cms label
     if cms_label != "skip":
         label_options = {
             "wip": "Work in progress",
             "pre": "Preliminary",
+            "pw": "Private work",
             "sim": "Simulation",
             "simwip": "Simulation work in progress",
             "simpre": "Simulation preliminary",
+            "simpw": "Simulation private work",
             "public": "",
         }
         cms_label_kwargs = {
             "ax": ax,
             "llabel": label_options[cms_label],
             "fontsize": 22,
             "data": False,
```

### Comparing `columnflow-0.2.0/columnflow/plotting/plot_functions_1d.py` & `columnflow-0.2.1/columnflow/plotting/plot_functions_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     shape_norm: bool | None = False,
     yscale: str | None = "",
     hide_errors: bool | None = None,
     process_settings: dict | None = None,
     variable_settings: dict | None = None,
     **kwargs,
 ) -> plt.Figure:
-
+    """
+    TODO.
+    """
     remove_residual_axis(hists, "shift")
 
-    hists = apply_variable_settings(hists, variable_insts, variable_settings)
     variable_inst = variable_insts[0]
-
+    hists = apply_variable_settings(hists, variable_insts, variable_settings)
     hists = apply_process_settings(hists, process_settings)
-
     hists = apply_density_to_hists(hists, density)
 
     plot_config = prepare_plot_config(
         hists,
         shape_norm=shape_norm,
         hide_errors=hide_errors,
     )
@@ -81,20 +81,21 @@
     density: bool | None = False,
     shape_norm: bool = False,
     yscale: str | None = None,
     hide_errors: bool | None = None,
     variable_settings: dict | None = None,
     **kwargs,
 ) -> plt.Figure:
-
+    """
+    TODO.
+    """
     remove_residual_axis(hists, "shift")
 
-    hists = apply_variable_settings(hists, variable_insts, variable_settings)
     variable_inst = variable_insts[0]
-
+    hists = apply_variable_settings(hists, variable_insts, variable_settings)
     hists = apply_density_to_hists(hists, density)
 
     plot_config = OrderedDict()
 
     # for updating labels of individual selector steps
     selector_step_labels = config_inst.x("selector_step_labels", {})
 
@@ -141,20 +142,20 @@
     yscale: str | None = None,
     hide_errors: bool | None = None,
     legend_title: str | None = None,
     process_settings: dict | None = None,
     variable_settings: dict | None = None,
     **kwargs,
 ) -> plt.Figure:
-
-    hists = apply_variable_settings(hists, variable_insts, variable_settings)
+    """
+    TODO.
+    """
     variable_inst = variable_insts[0]
-
+    hists = apply_variable_settings(hists, variable_insts, variable_settings)
     hists = apply_process_settings(hists, process_settings)
-
     hists = apply_density_to_hists(hists, density)
 
     # create the sum of histograms over all processes
     h_sum = sum(list(hists.values())[1:], list(hists.values())[0].copy())
 
     # setup plotting configs
     plot_config = {}
@@ -226,19 +227,20 @@
     density: bool | None = False,
     shape_norm: bool = False,
     yscale: str | None = None,
     hide_errors: bool | None = None,
     process_settings: dict | None = None,
     **kwargs,
 ) -> plt.Figure:
-
+    """
+    TODO.
+    """
     remove_residual_axis(hists, "shift")
 
     hists = apply_process_settings(hists, process_settings)
-
     hists = apply_density_to_hists(hists, density)
 
     # setup plotting config
     plot_config = prepare_plot_config(
         hists,
         shape_norm=shape_norm,
         hide_errors=hide_errors,
```

### Comparing `columnflow-0.2.0/columnflow/plotting/plot_functions_2d.py` & `columnflow-0.2.1/columnflow/plotting/plot_functions_2d.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/plotting/plot_util.py` & `columnflow-0.2.1/columnflow/plotting/plot_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,21 @@
     shape_norm: bool | None = False,
     yscale: str | None = "",
 ) -> dict:
     """
     small helper function that sets up a default style config based on the instances
     of the config, category and variable
     """
-
     if not yscale:
         yscale = "log" if variable_inst.log_y else "linear"
 
-    xlim = (variable_inst.x("x_min", variable_inst.x_min), variable_inst.x("x_max", variable_inst.x_max))
+    xlim = (
+        variable_inst.x("x_min", variable_inst.x_min),
+        variable_inst.x("x_max", variable_inst.x_max),
+    )
 
     style_config = {
         "ax_cfg": {
             "xlim": xlim,
             "ylabel": variable_inst.get_full_y_title(bin_width="" if density else None),
             "xlabel": variable_inst.get_full_x_title(),
             "yscale": yscale,
@@ -168,15 +170,16 @@
         "cms_label_cfg": {
             "lumi": config_inst.x.luminosity.get("nominal") / 1000,  # pb -> fb
         },
     }
 
     # disable minor ticks based on variable_inst
     if variable_inst.discrete_x:
-        style_config["ax_cfg"]["xticks"] = range(int(xlim[0]), int(xlim[1]) + 1)
+        # TODO: find sth better than plain bin edges or possibly memory intense range(*xlim)
+        style_config["ax_cfg"]["xticks"] = variable_inst.bin_edges
         style_config["ax_cfg"]["minorxticks"] = []
     if variable_inst.discrete_y:
         style_config["ax_cfg"]["minoryticks"] = []
 
     return style_config
 
 
@@ -227,15 +230,15 @@
         # first process is on top
         h_mc_stack = hist.Stack(*mc_hists[::-1])
 
     # setup plotting configs
     plot_config = OrderedDict()
 
     # draw stack + error bands
-    if h_mc_stack:
+    if h_mc_stack is not None:
         mc_norm = sum(h_mc.values()) if shape_norm else 1
         plot_config["mc_stack"] = {
             "method": "draw_stack",
             "hist": h_mc_stack,
             "kwargs": {
                 "norm": mc_norm,
                 "label": mc_labels[::-1],
@@ -275,21 +278,22 @@
         data_norm = sum(h_data.values()) if shape_norm else 1
         plot_config["data"] = {
             "method": "draw_errorbars",
             "hist": h_data,
             "kwargs": {
                 "norm": data_norm,
                 "label": "Data",
-                "yerr": False if data_hide_errors[i] else None,
-            },
-            "ratio_kwargs": {
-                "norm": h_mc.values() * data_norm / mc_norm,
-                "yerr": False if data_hide_errors[i] else None,
+                "yerr": False if any(data_hide_errors) else None,
             },
         }
+        if h_mc is not None:
+            plot_config["ratio_kwargs"] = {
+                "norm": h_mc.values() * data_norm / mc_norm,
+                "yerr": False if any(data_hide_errors) else None,
+            }
 
     return plot_config
 
 
 def get_position(minimum: float, maximum: float, factor: float = 1.4, logscale: bool = False) -> float:
     """ get a relative position between a min and max value based on the scale """
     if logscale:
```

### Comparing `columnflow-0.2.0/columnflow/production/__init__.py` & `columnflow-0.2.1/columnflow/production/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         if mc_only and data_only:
             raise Exception(f"producer {cls_name} received both mc_only and data_only")
         if mc_only or data_only:
             if cls_dict.get("skip_func"):
                 raise Exception(f"producer {cls_name} received custom skip_func, but mc_only or data_only are set")
 
             def skip_func(self):
-                return getattr(self, "dataset_inst", None) and self.dataset_inst.is_mc != bool(mc_only)
+                # never skip when there is not dataset
+                if not getattr(self, "dataset_inst", None):
+                    return False
+
+                return self.dataset_inst.is_mc != bool(mc_only)
 
             cls_dict["skip_func"] = skip_func
 
         # create the subclass
         subclass = Producer.derive(cls_name, bases=bases, cls_dict=cls_dict, module=module)
 
         return subclass
```

### Comparing `columnflow-0.2.0/columnflow/production/categories.py` & `columnflow-0.2.1/columnflow/production/categories.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/production/cms/btag.py` & `columnflow-0.2.1/columnflow/production/cms/btag.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,39 +17,49 @@
 
 @producer(
     uses={
         "Jet.hadronFlavour", "Jet.eta", "Jet.pt", "Jet.btagDeepFlavB",
     },
     # only run on mc
     mc_only=True,
+    # function to determine the correction file
+    get_btag_file=(lambda self, external_files: external_files.btag_sf_corr),
+    # function to determine the muon weight config
+    get_btag_config=(lambda self: self.config_inst.x.btag_sf),
 )
 def btag_weights(
     self: Producer,
     events: ak.Array,
     jet_mask: ak.Array | type(Ellipsis) = Ellipsis,
     **kwargs,
 ) -> ak.Array:
     """
-    B-tag scale factor weight producer. Requires an external file in the config as (e.g.)
+    B-tag scale factor weight producer. Requires an external file in the config as under
+    ``btag_sf_corr``:
 
     .. code-block:: python
 
-        "btag_sf_corr": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/BTV/2017_UL/btagging.json.gz", "v1"),  # noqa
+        cfg.x.external_files = DotDict.wrap({
+            "btag_sf_corr": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/BTV/2017_UL/btagging.json.gz",  # noqa
+        })
 
-    as well as an auxiliary entry in the config to refer to the b-tag correction set.
+    *get_btag_file* can be adapted in a subclass in case it is stored differently in the external
+    files.
+
+    The name of the correction set as well as a list of JEC uncertainty sources which should be
+    propagated through the weight calculation should be given as an auxiliary entry in the config:
 
     .. code-block:: python
 
-        cfg.x.btag_sf_correction_set = "deepJet_shape"
+        cfg.x.btag_sf = ("deepJet_shape", ["Absolute", "FlavorQCD", ...])
 
-    In addition, JEC uncertainty sources are propagated and weight columns are written if an
-    auxiliary config entry ``btag_sf_jec_sources`` exists.
+    *get_btag_config* can be adapted in a subclass in case it is stored differently in the config.
 
-    Optionally, a *jet_mask* can be supplied to compute the scale factor weight
-    based only on a subset of jets.
+    Optionally, a *jet_mask* can be supplied to compute the scale factor weight based only on a
+    subset of jets.
 
     Resources:
 
        - https://twiki.cern.ch/twiki/bin/view/CMS/BTagShapeCalibration?rev=26
        - https://indico.cern.ch/event/1096988/contributions/4615134/attachments/2346047/4000529/Nov21_btaggingSFjsons.pdf
     """
     # get the total number of jets in the chunk
@@ -137,15 +147,15 @@
         return
 
     # to handle this efficiently in one spot, store jec information
     self.jec_source = self.shift_inst.x.jec_source if self.shift_inst.has_tag("jec") else None
     btag_sf_jec_source = "" if self.jec_source == "Total" else self.jec_source
     self.shift_is_known_jec_source = (
         self.jec_source and
-        btag_sf_jec_source in self.config_inst.x("btag_sf_jec_sources", [])
+        btag_sf_jec_source in self.get_btag_config()[1]
     )
 
     # save names of method-intrinsic uncertainties
     self.btag_uncs = {
         "hf": "hf",
         "lf": "lf",
         "hfstats1": "hfstats1_{year}",
@@ -186,10 +196,14 @@
 def btag_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
     bundle = reqs["external_files"]
 
     # create the btag sf corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.btag_sf_corr.load(formatter="gzip").decode("utf-8"),
+        self.get_btag_file(bundle.files).load(formatter="gzip").decode("utf-8"),
     )
-    self.btag_sf_corrector = correction_set[self.config_inst.x.btag_sf_correction_set]
+    corrector_name = self.get_btag_config()[0]
+    self.btag_sf_corrector = correction_set[corrector_name]
+
+    # check versions
+    assert self.btag_sf_corrector.version in [3]
```

### Comparing `columnflow-0.2.0/columnflow/production/cms/electron.py` & `columnflow-0.2.1/columnflow/production/cms/electron.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,56 +20,65 @@
         "Electron.pt", "Electron.eta", "Electron.deltaEtaSC",
     },
     produces={
         "electron_weight", "electron_weight_up", "electron_weight_down",
     },
     # only run on mc
     mc_only=True,
+    # function to determine the correction file
+    get_electron_file=(lambda self, external_files: external_files.electron_sf),
+    # function to determine the electron weight config
+    get_electron_config=(lambda self: self.config_inst.x.electron_sf_names),
 )
 def electron_weights(
     self: Producer,
     events: ak.Array,
     electron_mask: ak.Array | type(Ellipsis) = Ellipsis,
     **kwargs,
 ) -> ak.Array:
     """
-    Electron scale factor producer. Requires an external file in the config as (e.g.)
+    Creates electron weights using the correctionlib. Requires an external file in the config under
+    ``electron_sf``:
 
     .. code-block:: python
 
-        "electron_sf": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/EGM/2017_UL/electron.json.gz", "v1"),  # noqa
+        cfg.x.external_files = DotDict.wrap({
+            "electron_sf": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/EGM/2017_UL/electron.json.gz",  # noqa
+        })
 
-    as well as an auxiliary entry in the config to refer to three values in a tuple, i.e., the name
-    of the correction set, a year string to be used as a correctionlib input, and the name of the
-    selection working point.
+    *get_electron_file* can be adapted in a subclass in case it is stored differently in the
+    external files.
+
+    The name of the correction set, the year string for the weight evaluation, and the name of the
+    working point should be given as an auxiliary entry in the config:
 
     .. code-block:: python
 
         cfg.x.electron_sf_names = ("UL-Electron-ID-SF", "2017", "wp80iso")
 
+    *get_electron_config* can be adapted in a subclass in case it is stored differently in the
+    config.
+
     Optionally, an *electron_mask* can be supplied to compute the scale factor weight
     based only on a subset of electrons.
     """
-    # get year string and working point name
-    sf_year, wp = self.config_inst.x.electron_sf_names[1:]
-
     # flat super cluster eta and pt views
     sc_eta = flat_np_view((
         events.Electron.eta[electron_mask] +
         events.Electron.deltaEtaSC[electron_mask]
     ), axis=1)
     pt = flat_np_view(events.Electron.pt[electron_mask], axis=1)
 
     # loop over systematics
     for syst, postfix in [
         ("sf", ""),
         ("sfup", "_up"),
         ("sfdown", "_down"),
     ]:
-        sf_flat = self.electron_sf_corrector(sf_year, syst, wp, sc_eta, pt)
+        sf_flat = self.electron_sf_corrector(self.year, syst, self.wp, sc_eta, pt)
 
         # add the correct layout to it
         sf = layout_ak_array(sf_flat, events.Electron.pt[electron_mask])
 
         # create the product over all electrons in one event
         weight = ak.prod(sf, axis=1, mask_identity=False)
 
@@ -92,11 +101,14 @@
 def electron_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
     bundle = reqs["external_files"]
 
     # create the corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.electron_sf.load(formatter="gzip").decode("utf-8"),
+        self.get_electron_file(bundle.files).load(formatter="gzip").decode("utf-8"),
     )
-    corrector_name = self.config_inst.x.electron_sf_names[0]
+    corrector_name, self.year, self.wp = self.get_electron_config()
     self.electron_sf_corrector = correction_set[corrector_name]
+
+    # check versions
+    assert self.electron_sf_corrector.version in [2]
```

### Comparing `columnflow-0.2.0/columnflow/production/cms/mc_weight.py` & `columnflow-0.2.1/columnflow/production/cms/mc_weight.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/production/cms/muon.py` & `columnflow-0.2.1/columnflow/production/cms/muon.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,56 +20,61 @@
         "nMuon", "Muon.pt", "Muon.eta",
     },
     produces={
         "muon_weight", "muon_weight_up", "muon_weight_down",
     },
     # only run on mc
     mc_only=True,
+    # function to determine the correction file
+    get_muon_file=(lambda self, external_files: external_files.muon_sf),
+    # function to determine the muon weight config
+    get_muon_config=(lambda self: self.config_inst.x.muon_sf_names),
 )
 def muon_weights(
     self: Producer,
     events: ak.Array,
     muon_mask: ak.Array | type(Ellipsis) = Ellipsis,
     **kwargs,
 ) -> ak.Array:
     """
-    Reads the muon scale factor from the external file given in the config,
-    using the keys from the corresponding auxiliary entry in the config.
-    As of 10.2022, external files originating from a specific commit of
-    https://gitlab.cern.ch/cms-nanoAOD/jsonpog-integration/-/tree/master/POG/MUO
-
-    Example of external file in config:
+    Creates muon weights using the correctionlib. Requires an external file in the config under
+    ``muon_sf``:
 
     .. code-block:: python
 
-        "muon_sf": ("/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/MUO/2017_UL/muon_z.json.gz", "v1"),  # noqa
+        cfg.x.external_files = DotDict.wrap({
+            "muon_sf": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-d0a522ea/POG/MUO/2017_UL/muon_z.json.gz",  # noqa
+        })
+
+    *get_muon_file* can be adapted in a subclass in case it is stored differently in the external
+    files.
 
-    Example of the corresponding auxiliary entry to read the correct sets from the json file:
+    The name of the correction set and the year string for the weight evaluation should be given as
+    an auxiliary entry in the config:
 
     .. code-block:: python
 
         cfg.x.muon_sf_names = ("NUM_TightRelIso_DEN_TightIDandIPCut", "2017_UL")
 
-    Optionally, a *muon_mask* can be supplied to compute the scale factor weight
-    based only on a subset of muons.
-    """
-    # get year string
-    sf_year = self.config_inst.x.muon_sf_names[1]
+    *get_muon_config* can be adapted in a subclass in case it is stored differently in the config.
 
+    Optionally, a *muon_mask* can be supplied to compute the scale factor weight based only on a
+    subset of muons.
+    """
     # flat absolute eta and pt views
     abs_eta = flat_np_view(abs(events.Muon.eta[muon_mask]), axis=1)
     pt = flat_np_view(events.Muon.pt[muon_mask], axis=1)
 
     # loop over systematics
     for syst, postfix in [
         ("sf", ""),
         ("systup", "_up"),
         ("systdown", "_down"),
     ]:
-        sf_flat = self.muon_sf_corrector(sf_year, abs_eta, pt, syst)
+        sf_flat = self.muon_sf_corrector(self.year, abs_eta, pt, syst)
 
         # add the correct layout to it
         sf = layout_ak_array(sf_flat, events.Muon.pt[muon_mask])
 
         # create the product over all muons in one event
         weight = ak.prod(sf, axis=1, mask_identity=False)
 
@@ -92,11 +97,14 @@
 def muon_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
     bundle = reqs["external_files"]
 
     # create the corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
-        bundle.files.muon_sf.load(formatter="gzip").decode("utf-8"),
+        self.get_muon_file(bundle.files).load(formatter="gzip").decode("utf-8"),
     )
-    corrector_name = self.config_inst.x.muon_sf_names[0]
+    corrector_name, self.year = self.get_muon_config()
     self.muon_sf_corrector = correction_set[corrector_name]
+
+    # check versions
+    assert self.muon_sf_corrector.version in [1]
```

### Comparing `columnflow-0.2.0/columnflow/production/cms/pdf.py` & `columnflow-0.2.1/columnflow/production/cms/pdf.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/production/cms/pileup.py` & `columnflow-0.2.1/columnflow/production/cms/pileup.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/production/cms/seeds.py` & `columnflow-0.2.1/columnflow/production/cms/seeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     """
     # create the event seeds
     events = self[deterministic_event_seeds](events, **kwargs)
 
     # create the per jet seeds
     prime_offset = 18
     jet_seed = events.deterministic_seed + (
-        primes[prime_offset] * ak.values_astype(ak.local_index(events.Jet), np.uint64)
+        primes[prime_offset] * ak.values_astype(ak.local_index(events.Jet, axis=1), np.uint64)
     )
     np_jet_seed = np.asarray(ak.flatten(jet_seed))
     np_jet_seed[:] = self[deterministic_event_seeds].create_seed(np_jet_seed)
 
     # store them
     events = set_ak_column(events, "Jet.deterministic_seed", jet_seed)
```

### Comparing `columnflow-0.2.0/columnflow/production/normalization.py` & `columnflow-0.2.1/columnflow/production/normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         - py:attr:`selection_stats`: The stats dict loaded from the output of MergeSelectionsStats.
         - py:attr:`sum_weights_table`: A sparse array serving as a lookup table for the sum of event
           weights per process id.
         - py:attr:`xs_table`: A sparse array serving as a lookup table for cross sections of all
           processes known to the config of the task, with keys being process ids.
     """
     # load the selection stats
-    selection_stats = inputs["selection_stats"]["collection"][0].load(formatter="json")
+    selection_stats = inputs["selection_stats"]["collection"][0]["stats"].load(formatter="json")
 
     # for the lookup tables below, determine the maximum process id
     process_insts = [
         process_inst
         for process_inst, _, _ in self.config_inst.walk_processes()
         if process_inst.is_mc
     ]
```

### Comparing `columnflow-0.2.0/columnflow/production/processes.py` & `columnflow-0.2.1/columnflow/production/processes.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/production/util.py` & `columnflow-0.2.1/columnflow/production/util.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/selection/__init__.py` & `columnflow-0.2.1/columnflow/selection/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,19 @@
         if mc_only and data_only:
             raise Exception(f"selector {cls_name} received both mc_only and data_only")
         if mc_only or data_only:
             if cls_dict.get("skip_func"):
                 raise Exception(f"selector {cls_name} received custom skip_func, but mc_only or data_only are set")
 
             def skip_func(self):
-                return getattr(self, "dataset_inst", None) and self.dataset_inst.is_mc != bool(mc_only)
+                # never skip when there is not dataset
+                if not getattr(self, "dataset_inst", None):
+                    return False
+
+                return self.dataset_inst.is_mc != bool(mc_only)
 
             cls_dict["skip_func"] = skip_func
 
         # create the subclass
         subclass = Selector.derive(cls_name, bases=bases, cls_dict=cls_dict, module=module)
 
         return subclass
```

### Comparing `columnflow-0.2.0/columnflow/selection/matching.py` & `columnflow-0.2.1/columnflow/selection/matching.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/tasks/calibration.py` & `columnflow-0.2.1/columnflow/tasks/calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,16 @@
     reqs = Requirements(
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
     )
 
     register_calibrator_shifts = True
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         # add calibrator dependent requirements
         reqs["calibrator"] = self.calibrator_inst.run_requires()
 
         return reqs
@@ -51,15 +49,15 @@
 
         # add calibrator dependent requirements
         reqs["calibrator"] = self.calibrator_inst.run_requires()
 
         return reqs
 
     def output(self):
-        return self.target(f"calib_{self.branch}.parquet")
+        return {"columns": self.target(f"calib_{self.branch}.parquet")}
 
     @law.decorator.log
     @ensure_proxy
     @law.decorator.localize(input=False, output=True)
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
@@ -113,15 +111,15 @@
 
             # save as parquet via a thread in the same pool
             chunk = tmp_dir.child(f"file_{lfn_index}_{pos.index}.parquet", type="f")
             output_chunks[(lfn_index, pos.index)] = chunk
             self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
 
         # merge output files
-        with output.localize("w") as outp:
+        with output["columns"].localize("w") as outp:
             sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
             law.pyarrow.merge_parquet_task(self, sorted_chunks, outp, local=True)
 
 
 # overwrite class defaults
 check_finite_tasks = law.config.get_expanded("analysis", "check_finite_output", [], split_csv=True)
 CalibrateEvents.check_finite = ChunkedIOMixin.check_finite.copy(
```

### Comparing `columnflow-0.2.0/columnflow/tasks/cms/external.py` & `columnflow-0.2.1/columnflow/tasks/cms/external.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/tasks/cms/inference.py` & `columnflow-0.2.1/columnflow/tasks/cms/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,16 @@
         MergeHistograms=MergeHistograms,
         MergeShiftedHistograms=MergeShiftedHistograms,
     )
 
     def create_branch_map(self):
         return list(self.inference_model_inst.categories)
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # simply require the requirements of all branch tasks right now
         reqs["merged_hists"] = set(sum((
             law.util.flatten(t.requires())
             for t in self.get_branch_tasks().values()
         ), []))
 
@@ -132,15 +130,15 @@
                             f"dataset '{dataset}' does not contain process '{process_inst.name}' "
                             "or any of its subprocesses which indicates a misconfiguration in the "
                             f"inference model '{self.inference_model}'",
                         )
                         continue
 
                     # open the histogram and work on a copy
-                    h = _inp["collection"][0][variable_inst.name].load(formatter="pickle").copy()
+                    h = _inp["collection"][0]["hists"][variable_inst.name].load(formatter="pickle").copy()
 
                     # axis selections
                     h = h[{
                         "process": [
                             hist.loc(p.id)
                             for p in sub_process_insts
                             if p.id in h.axes["process"]
```

### Comparing `columnflow-0.2.0/columnflow/tasks/cutflow.py` & `columnflow-0.2.1/columnflow/tasks/cutflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,42 +37,43 @@
 ):
     sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
 
     selector_steps_order_sensitive = True
 
     initial_step = "Initial"
 
-    default_variables = ("mc_weight", "cf_*")
+    default_variables = ("event", "cf_*")
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         MergeSelectionMasks=MergeSelectionMasks,
     )
 
     def create_branch_map(self):
         # dummy branch map
         return [None]
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
-        reqs["masks"] = self.reqs.MergeSelectionMasks.req(self, tree_index=0, _exclude={"branches"})
+        reqs["selection"] = self.reqs.MergeSelectionMasks.req(self, tree_index=0, _exclude={"branches"})
 
         return reqs
 
     def requires(self):
         return {
-            "masks": self.reqs.MergeSelectionMasks.req(self, tree_index=0, branch=0),
+            "selection": self.reqs.MergeSelectionMasks.req(self, tree_index=0, branch=0),
         }
 
     def output(self):
-        return {var: self.target(f"cutflow_hist__var_{var}.pickle") for var in self.variables}
+        return {
+            var: self.target(f"cutflow_hist__{var}.pickle")
+            for var in self.variables
+        }
 
     @law.decorator.log
     @law.decorator.localize(input=True, output=False)
     @law.decorator.safe_output
     def run(self):
         import hist
         import awkward as ak
@@ -85,15 +86,17 @@
         tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
         tmp_dir.touch()
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # define columns that need to be read
-        read_columns = {"category_ids", "process_id", "normalization_weight"} | set(aliases.values())
+        read_columns = {"category_ids", "process_id"} | set(aliases.values())
+        if self.dataset_inst.is_mc:
+            read_columns |= {"normalization_weight"}
         read_columns = {Route(c) for c in read_columns}
 
         # define steps
         steps = self.selector_steps
 
         # prepare expressions
         expressions = {}
@@ -106,14 +109,17 @@
                 if isinstance(expr, str):
                     route = Route(expr)
                     expr = functools.partial(route.apply, null_value=variable_inst.null_value)
                     read_columns.add(route)
                 # TODO: handle variable_inst with custom expressions, can they declare columns?
                 expressions[variable_inst.name] = expr
 
+        # prepare columns to load
+        load_columns = {("events" + route) for route in read_columns} | {Route("steps.*")}
+
         # prepare histograms
         histograms = {}
         def prepare_hists(steps):
             for var_key, var_names in self.variable_tuples.items():
                 variable_insts = [self.config_inst.get_variable(var_name) for var_name in var_names]
 
                 # create histogram of not already existing
@@ -132,17 +138,17 @@
                             name=variable_inst.name,
                             label=variable_inst.get_full_x_title(),
                         )
                     # enable weights and store it
                     histograms[var_key] = h.Weight()
 
         for arr, pos in self.iter_chunked_io(
-            inputs["masks"].path,
+            inputs["selection"]["masks"].path,
             source_type="awkward_parquet",
-            read_columns={("events" + route) for route in read_columns} | {Route("steps.*")},
+            read_columns=load_columns,
         ):
             events = arr.events
 
             # overwrite steps if not defined yet
             if not steps:
                 steps = arr.steps.fields
 
@@ -160,15 +166,19 @@
                 # helper to build the point for filling, except for the step which does
                 # not support broadcasting
                 def get_point(mask=Ellipsis):
                     point = {
                         "process": events.process_id[mask],
                         "category": category_ids[mask],
                         "shift": self.global_shift_inst.id,
-                        "weight": events.normalization_weight[mask],
+                        "weight": (
+                            events.normalization_weight[mask]
+                            if self.dataset_inst.is_mc
+                            else 1.0
+                        ),
                     }
                     for var_name in var_names:
                         point[var_name] = expressions[var_name](events)[mask]
                     return point
 
                 # fill the raw point
                 fill_kwargs = get_point()
@@ -235,14 +245,20 @@
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
     plot_function = PlotBase.plot_function.copy(
         default="columnflow.plotting.plot_functions_1d.plot_cutflow",
         add_default_to_description=True,
     )
+    variable = luigi.Parameter(
+        default=CreateCutflowHistograms.default_variables[0],
+        significant=False,
+        description="name of the variable to use for obtaining event counts; "
+        f"default: '{CreateCutflowHistograms.default_variables[0]}'",
+    )
 
     # upstream requirements
     reqs = Requirements(
         PlotCutflowBase.reqs,
         RemoteWorkflow.reqs,
     )
 
@@ -252,48 +268,44 @@
             raise Exception(
                 f"{self.__class__.__name__} task cannot build branch map when no categories are "
                 "set",
             )
 
         return list(self.categories)
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["hists"] = [
             self.reqs.CreateCutflowHistograms.req(
                 self,
                 dataset=d,
-                variables=("mc_weight",),
-                _prefer_cli={"variables"},
+                variables=(self.variable,),
                 _exclude={"branches"},
             )
             for d in self.datasets
         ]
         return reqs
 
     def requires(self):
         return {
             d: self.reqs.CreateCutflowHistograms.req(
                 self,
                 branch=0,
                 dataset=d,
-                variables=("mc_weight",),
-                _prefer_cli={"variables"},
+                variables=(self.variable,),
             )
             for d in self.datasets
         }
 
     def output(self):
-        return [
+        return {"plots": [
             self.target(name)
             for name in self.get_plot_names(f"cutflow__cat_{self.branch_data}")
-        ]
+        ]}
 
     @law.decorator.log
     @view_output_plots
     def run(self):
         import hist
 
         # prepare config objects
@@ -307,15 +319,15 @@
 
         # histogram data per process
         hists = {}
 
         with self.publish_step(f"plotting cutflow in {category_inst.name}"):
             for dataset, inp in self.input().items():
                 dataset_inst = self.config_inst.get_dataset(dataset)
-                h_in = inp["mc_weight"].load(formatter="pickle")
+                h_in = inp[self.variable].load(formatter="pickle")
 
                 # sanity checks
                 n_shifts = len(h_in.axes["shift"])
                 if n_shifts != 1:
                     raise Exception(f"shift axis is supposed to only contain 1 bin, found {n_shifts}")
 
                 # loop and extract one histogram per process
@@ -338,15 +350,15 @@
                             hist.loc(c.id)
                             for c in leaf_category_insts
                             if c.id in h.axes["category"]
                         ],
                     }]
 
                     # axis reductions
-                    h = h[{"process": sum, "category": sum, "mc_weight": sum}]
+                    h = h[{"process": sum, "category": sum, self.variable: sum}]
 
                     # add the histogram
                     if process_inst in hists:
                         hists[process_inst] += h
                     else:
                         hists[process_inst] = h
 
@@ -366,29 +378,29 @@
                 hists=hists,
                 config_inst=self.config_inst,
                 category_inst=category_inst.copy_shallow(),
                 **self.get_plot_parameters(),
             )
 
             # save the plot
-            for outp in self.output():
+            for outp in self.output()["plots"]:
                 outp.dump(fig, formatter="mpl")
 
 
 PlotCutflowWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=PlotCutflow,
     enable=["configs", "skip_configs", "shifts", "skip_shifts"],
 )
 
 
 class PlotCutflowVariablesBase(
-    PlotCutflowBase,
     VariablePlotSettingMixin,
     ProcessPlotSettingMixin,
+    PlotCutflowBase,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
     only_final_step = luigi.BoolParameter(
         default=False,
         significant=False,
         description="when True, only create plots for the final selector step; default: False",
@@ -553,38 +565,38 @@
     # TODO: combine these hard-coded plot function name with law parameter
     plot_function_per_process = "columnflow.plotting.plot_functions_1d.plot_variable_per_process"
     plot_function_per_step = "columnflow.plotting.plot_functions_1d.plot_variable_variants"
 
     def output(self):
         b = self.branch_data
         if self.per_plot == "processes":
-            return law.SiblingFileCollection({
+            return {"plots": law.SiblingFileCollection({
                 s: [
                     self.local_target(name) for name in self.get_plot_names(
                         f"plot__step{i}_{s}__proc_{self.processes_repr}__cat_{b.category}__var_{b.variable}",
                     )
                 ]
                 for i, s in enumerate(self.chosen_steps)
-            })
+            })}
         else:  # per_plot == "steps"
-            return law.SiblingFileCollection({
+            return {"plots": law.SiblingFileCollection({
                 p: [
                     self.local_target(name)
                     for name in self.get_plot_names(f"plot__proc_{p}__cat_{b.category}__var_{b.variable}")
                 ]
                 for p in self.processes
-            })
+            })}
 
     def run_postprocess(self, hists, category_inst, variable_insts):
         import hist
 
         if len(variable_insts) != 1:
-            raise Exception(f"Task {self.task_family} is only working for single variables.")
+            raise Exception(f"task {self.task_family} is only viable for single variables")
 
-        outputs = self.output()
+        outputs = self.output()["plots"]
         if self.per_plot == "processes":
             for step in self.chosen_steps:
                 step_hists = OrderedDict(
                     (process_inst.copy_shallow(), h[{"step": hist.loc(step)}])
                     for process_inst, h in hists.items()
                 )
 
@@ -633,27 +645,27 @@
     plot_function = PlotBase.plot_function.copy(
         default="columnflow.plotting.plot_functions_2d.plot_2d",
         add_default_to_description=True,
     )
 
     def output(self):
         b = self.branch_data
-        return law.SiblingFileCollection({
+        return {"plots": law.SiblingFileCollection({
             s: [
                 self.local_target(name) for name in self.get_plot_names(
                     f"plot__step{i}_{s}__proc_{self.processes_repr}__cat_{b.category}__var_{b.variable}",
                 )
             ]
             for i, s in enumerate(self.chosen_steps)
-        })
+        })}
 
     def run_postprocess(self, hists, category_inst, variable_insts):
         import hist
 
-        outputs = self.output()
+        outputs = self.output()["plots"]
 
         for step in self.chosen_steps:
             step_hists = OrderedDict(
                 (process_inst.copy_shallow(), h[{"step": hist.loc(step)}])
                 for process_inst, h in hists.items()
             )
```

### Comparing `columnflow-0.2.0/columnflow/tasks/external.py` & `columnflow-0.2.1/columnflow/tasks/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         if self.validate and len(lfns) != self.dataset_info_inst.n_files:
             raise ValueError(
                 f"number of obtained lfns ({len(lfns)}) does not match number of files "
                 f"for dataset {self.dataset_inst.name} ({self.dataset_info_inst.n_files})",
             )
 
-        self.logger.info(f"found {len(lfns)} lfns for dataset {self.dataset}")
+        self.logger.info(f"found {len(lfns)} lfn(s) for dataset {self.dataset}")
 
         tmp = law.LocalFileTarget(is_tmp=True)
         tmp.dump(lfns, indent=4, formatter="json")
         self.transfer(tmp)
 
     def get_dataset_lfns_dasgoclient(
         self,
```

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/base.py` & `columnflow-0.2.1/columnflow/tasks/framework/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     message_cache_size = 25
     local_workflow_require_branches = False
     output_collection_cls = law.SiblingFileCollection
 
     # defaults for targets
     default_store = "$CF_STORE_LOCAL"
-    default_wlcg_fs = "wlcg_fs"
+    default_wlcg_fs = law.config.get_expanded("target", "default_wlcg_fs")
     default_output_location = "config"
 
     @classmethod
     def resolve_param_values(cls, params: dict) -> dict:
         # store a reference to the analysis inst
         if "analysis_inst" not in params and "analysis" in params:
             params["analysis_inst"] = cls.get_analysis_inst(params["analysis"])
@@ -168,17 +168,24 @@
         for req in cls.reqs.values():
             upstream_shifts |= set.union(*(req.get_known_shifts(config_inst, params) or (set(),)))
 
         return set(), upstream_shifts
 
     @classmethod
     def get_array_function_kwargs(cls, task=None, **params):
+        if task:
+            analysis_inst = task.analysis_inst
+        elif "analysis_inst" in params:
+            analysis_inst = params["analysis_inst"]
+        else:
+            analysis_inst = cls.get_analysis_inst(params["analysis"])
+
         return {
             "task": task,
-            "analysis_inst": task.analysis_inst if task else cls.get_analysis_inst(params["analysis"]),
+            "analysis_inst": analysis_inst,
         }
 
     @classmethod
     def get_calibrator_kwargs(cls, *args, **kwargs):
         # implemented here only for simplified mro control
         return cls.get_array_function_kwargs(*args, **kwargs)
 
@@ -427,18 +434,22 @@
             return task.config_inst.get_aux("versions", {})
 
         return super().get_version_map(task)
 
     @classmethod
     def get_array_function_kwargs(cls, task=None, **params):
         kwargs = super().get_array_function_kwargs(task=task, **params)
+
         if task:
             kwargs["config_inst"] = task.config_inst
+        elif "config_inst" in params:
+            kwargs["config_inst"] = params["config_inst"]
         elif "config" in params and "analysis_inst" in kwargs:
             kwargs["config_inst"] = kwargs["analysis_inst"].get_config(params["config"])
+
         return kwargs
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # store a reference to the config instance
         self.config_inst = self.analysis_inst.get_config(self.config)
@@ -619,18 +630,22 @@
         else:
             params += ("dataset",)
         return params
 
     @classmethod
     def get_array_function_kwargs(cls, task=None, **params):
         kwargs = super().get_array_function_kwargs(task=task, **params)
+
         if task:
             kwargs["dataset_inst"] = task.dataset_inst
+        elif "dataset_inst" in params:
+            kwargs["dataset_inst"] = params["dataset_inst"]
         elif "dataset" in params and "config_inst" in kwargs:
             kwargs["dataset_inst"] = kwargs["config_inst"].get_dataset(params["dataset"])
+
         return kwargs
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # store references to the dataset instance
         self.dataset_inst = self.config_inst.get_dataset(self.dataset)
```

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/decorators.py` & `columnflow-0.2.1/columnflow/tasks/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/mixins.py` & `columnflow-0.2.1/columnflow/tasks/framework/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ak = maybe_import("awkward")
 
 
 class CalibratorMixin(ConfigTask):
 
     calibrator = luigi.Parameter(
         default=law.NO_STR,
-        description="the name of the calibrator to the applied; default: value of the "
+        description="the name of the calibrator to be applied; default: value of the "
         "'default_calibrator' config",
     )
 
     # decibes whether the task itself runs the calibrator and implements its shifts
     register_calibrator_shifts = False
 
     @classmethod
@@ -175,15 +175,15 @@
         return parts
 
 
 class SelectorMixin(ConfigTask):
 
     selector = luigi.Parameter(
         default=law.NO_STR,
-        description="the name of the selector to the applied; default: value of the "
+        description="the name of the selector to be applied; default: value of the "
         "'default_selector' config",
     )
 
     # decibes whether the task itself runs the selector and implements its shifts
     register_selector_shifts = False
 
     @classmethod
@@ -265,19 +265,22 @@
     selector_steps_order_sensitive = False
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
         # expand selector step groups
-        if "config_inst" in params and len(params.get("selector_steps", ())) == 1:
+        if "config_inst" in params and len(params.get("selector_steps", [])) == 1:
             config_inst = params["config_inst"]
             step_group = params["selector_steps"][0]
-            if step_group in config_inst.x("selector_step_groups", {}):
-                params["selector_steps"] = tuple(config_inst.x.selector_step_groups[step_group])
+            params["selector_steps"] = (
+                tuple(config_inst.x.selector_step_groups[step_group])
+                if step_group in config_inst.x("selector_step_groups", {}) else
+                tuple()
+            )
 
         # sort selector steps when the order does not matter
         if not cls.selector_steps_order_sensitive and "selector_steps" in params:
             params["selector_steps"] = tuple(sorted(params["selector_steps"]))
 
         return params
 
@@ -293,15 +296,15 @@
         return parts
 
 
 class ProducerMixin(ConfigTask):
 
     producer = luigi.Parameter(
         default=law.NO_STR,
-        description="the name of the producer to the applied; default: value of the "
+        description="the name of the producer to be applied; default: value of the "
         "'default_producer' config",
     )
 
     # decibes whether the task itself runs the producer and implements its shifts
     register_producer_shifts = False
 
     @classmethod
@@ -439,121 +442,328 @@
             if len(self.producers) > 5:
                 part += f"__{law.util.create_hash(self.producers[5:])}"
         parts.insert_before("version", "producers", f"prod__{part}")
 
         return parts
 
 
-class MLModelMixinBase(ConfigTask):
+class MLModelMixinBase(AnalysisTask):
 
-    @classmethod
-    def get_ml_model_inst(cls, ml_model: str, config_inst: od.Config) -> MLModel:
-        return MLModel.get_cls(ml_model)(config_inst)
+    ml_model = luigi.Parameter(
+        description="the name of the ML model to be applied",
+    )
 
-    def events_used_in_training(self, dataset_inst: od.Dataset, shift_inst: od.Shift) -> bool:
+    exclude_params_repr_empty = {"ml_model"}
+
+    @classmethod
+    def get_ml_model_inst(
+        cls,
+        ml_model: str,
+        analysis_inst: od.Analysis,
+        requested_configs: list[str] | None = None,
+        **kwargs,
+    ) -> MLModel:
+        ml_model_inst = MLModel.get_cls(ml_model)(analysis_inst, **kwargs)
+
+        if requested_configs:
+            configs = ml_model_inst.training_configs(list(requested_configs))
+            if configs:
+                ml_model_inst._setup(configs)
+
+        return ml_model_inst
+
+    def events_used_in_training(
+        self,
+        config_inst: od.Config,
+        dataset_inst: od.Dataset,
+        shift_inst: od.Shift,
+    ) -> bool:
         # evaluate whether the events for the combination of dataset_inst and shift_inst
         # shall be used in the training
         return (
-            dataset_inst in self.ml_model_inst.used_datasets and
+            dataset_inst in self.ml_model_inst.datasets(config_inst) and
             not shift_inst.has_tag("disjoint_from_nominal")
         )
 
 
-class MLModelDataMixin(MLModelMixinBase):
+class MLModelTrainingMixin(MLModelMixinBase):
 
-    ml_model = luigi.Parameter(
-        default=law.NO_STR,
-        significant=False,
-        description="the name of the ML model to the applied; default: value of the "
-        "'default_ml_model' config",
+    configs = law.CSVParameter(
+        default=(),
+        description="comma-separated names of analysis config to use; should only contain a single "
+        "name in case the ml model is bound to a single config; when empty, the ml model is "
+        "expected to fully define the configs it uses; empty default",
+    )
+    calibrators = law.MultiCSVParameter(
+        default=(),
+        description="multiple comma-separated sequences of names of calibrators to apply, "
+        "separated by ':'; each sequence corresponds to a config in --configs; when empty, the "
+        "'default_calibrator' setting of each config is used if set, or the model is expected to "
+        "fully define the calibrators it requires upstream; empty default",
     )
-    ml_model_store = luigi.Parameter(default=law.NO_STR)
+    selectors = law.CSVParameter(
+        default=(),
+        description="comma-separated names of selectors to apply; each selector corresponds to a "
+        "config in --configs; when empty, the 'default_selector' setting of each config is used if "
+        "set, or the ml model is expected to fully define the selector it uses requires upstream; "
+        "empty default",
+    )
+    producers = law.MultiCSVParameter(
+        default=(),
+        description="multiple comma-separated sequences of names of producers to apply, "
+        "separated by ':'; each sequence corresponds to a config in --configs; when empty, the "
+        "'default_producer' setting of each config is used if set, or ml model is expected to "
+        "fully define the producers it requires upstream; empty default",
+    )
+
+    @classmethod
+    def resolve_calibrators(
+        cls,
+        ml_model_inst: MLModel,
+        params: dict[str, Any],
+    ) -> tuple[tuple[str]]:
+        calibrators = params.get("calibrators", ())
+
+        # use config defaults in case each config has one
+        if not calibrators:
+            defaults = tuple(
+                CalibratorsMixin.get_default_calibrators(config_inst)
+                for config_inst in ml_model_inst.config_insts
+            )
+            if all(defaults):
+                calibrators = defaults
+
+        # broadcast to configs
+        n_configs = len(ml_model_inst.config_insts)
+        if len(calibrators) == 1 and n_configs != 1:
+            calibrators = tuple(calibrators * n_configs)
+
+        # validate number of sequences
+        if len(calibrators) != n_configs:
+            raise Exception(
+                f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
+                f"{len(calibrators)} calibrator sequences",
+            )
+
+        # final check by model
+        calibrators = tuple(
+            tuple(ml_model_inst.training_calibrators(config_inst, list(_calibrators)))
+            for config_inst, _calibrators in zip(ml_model_inst.config_insts, calibrators)
+        )
+
+        # instantiate them once
+        for config_inst, _calibrators in zip(ml_model_inst.config_insts, calibrators):
+            init_kwargs = law.util.merge_dicts(params, {"config_inst": config_inst})
+            for calibrator in _calibrators:
+                CalibratorMixin.get_calibrator_inst(calibrator, kwargs=init_kwargs)
+
+        return calibrators
+
+    @classmethod
+    def resolve_selectors(
+        cls,
+        ml_model_inst: MLModel,
+        params: dict[str, Any],
+    ) -> tuple[str]:
+        selectors = params.get("selectors", ())
+
+        # use config defaults in case each config has one
+        if not selectors:
+            defaults = tuple(
+                SelectorMixin.get_default_selector(config_inst)
+                for config_inst in ml_model_inst.config_insts
+            )
+            if all(defaults):
+                selectors = defaults
+
+        # broadcast to configs
+        n_configs = len(ml_model_inst.config_insts)
+        if len(selectors) == 1 and n_configs != 1:
+            selectors = tuple(selectors * n_configs)
+
+        # validate sequence length
+        if len(selectors) != n_configs:
+            raise Exception(
+                f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
+                f"{len(selectors)} selectors",
+            )
+
+        # final check by model
+        selectors = tuple(
+            ml_model_inst.training_selector(config_inst, selector)
+            for config_inst, selector in zip(ml_model_inst.config_insts, selectors)
+        )
+
+        # instantiate them once
+        for config_inst, selector in zip(ml_model_inst.config_insts, selectors):
+            init_kwargs = law.util.merge_dicts(params, {"config_inst": config_inst})
+            SelectorMixin.get_selector_inst(selector, kwargs=init_kwargs)
+
+        return selectors
+
+    @classmethod
+    def resolve_producers(
+        cls,
+        ml_model_inst: MLModel,
+        params: dict[str, Any],
+    ) -> tuple[tuple[str]]:
+        producers = params.get("producers", ())
+
+        # use config defaults in case each config has one
+        if not producers:
+            defaults = tuple(
+                ProducersMixin.get_default_producers(config_inst)
+                for config_inst in ml_model_inst.config_insts
+            )
+            if all(defaults):
+                producers = defaults
+
+        # broadcast to configs
+        n_configs = len(ml_model_inst.config_insts)
+        if len(producers) == 1 and n_configs != 1:
+            producers = tuple(producers * n_configs)
+
+        # validate number of sequences
+        if len(producers) != n_configs:
+            raise Exception(
+                f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
+                f"{len(producers)} producer sequences",
+            )
+
+        # final check by model
+        producers = tuple(
+            tuple(ml_model_inst.training_producers(config_inst, list(_producers)))
+            for config_inst, _producers in zip(ml_model_inst.config_insts, producers)
+        )
 
-    # skip passing ml_model_store
-    exclude_params_index = {"ml_model_store"}
-    exclude_params_req = {"ml_model_store"}
-    exclude_params_repr = {"ml_model_store"}
-    exclude_params_sandbox = {"ml_model_store"}
-    exclude_params_remote_workflow = {"ml_model_store"}
+        # instantiate them once
+        for config_inst, _producers in zip(ml_model_inst.config_insts, producers):
+            init_kwargs = law.util.merge_dicts(params, {"config_inst": config_inst})
+            for producer in _producers:
+                ProducerMixin.get_producer_inst(producer, kwargs=init_kwargs)
+
+        return producers
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
-        # add the default ml model when empty
-        if "config_inst" in params:
-            config_inst = params["config_inst"]
-            if params.get("ml_model") in (None, law.NO_STR) and config_inst.x("default_ml_model", None):
-                params["ml_model"] = config_inst.x.default_ml_model
+        if "analysis_inst" in params and "ml_model" in params:
+            analysis_inst = params["analysis_inst"]
+            ml_model_inst = cls.get_ml_model_inst(params["ml_model"], analysis_inst)
+            params["ml_model_inst"] = ml_model_inst
+
+            # resolve configs
+            _configs = params.get("configs", ())
+            params["configs"] = tuple(ml_model_inst.training_configs(list(_configs)))
+            if not params["configs"]:
+                raise Exception(
+                    f"MLModel '{ml_model_inst.cls_name}' received configs '{_configs}' to define "
+                    "training configs, but did not define any",
+                )
+            ml_model_inst._set_configs(params["configs"])
+
+            # resolve calibrators
+            params["calibrators"] = cls.resolve_calibrators(ml_model_inst, params)
 
-            # initialize it and get the store name
-            if params.get("ml_model") not in (None, law.NO_STR):
-                model_inst = cls.get_ml_model_inst(params["ml_model"], config_inst)
-                params["ml_model_store"] = model_inst.store_name or model_inst.cls_name
+            # resolve selectors
+            params["selectors"] = cls.resolve_selectors(ml_model_inst, params)
+
+            # resolve producers
+            params["producers"] = cls.resolve_producers(ml_model_inst, params)
+
+            # call the model's setup hook
+            ml_model_inst._setup()
 
         return params
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the ML model instance
-        self.ml_model_inst = self.get_ml_model_inst(self.ml_model, self.config_inst)
-
-    def store_parts(self) -> law.util.InsertableDict:
-        parts = super().store_parts()
-        parts.insert_before("version", "ml_data", f"ml__{self.ml_model_store}")
-        return parts
+        self.ml_model_inst = self.get_ml_model_inst(
+            self.ml_model,
+            self.analysis_inst,
+            configs=list(self.configs),
+        )
 
 
-class MLModelMixin(MLModelMixinBase):
+class MLModelMixin(ConfigTask, MLModelMixinBase):
 
     ml_model = luigi.Parameter(
         default=law.NO_STR,
-        description="the name of the ML model to the applied; default: value of the "
+        description="the name of the ML model to be applied; default: value of the "
         "'default_ml_model' config",
     )
 
     allow_empty_ml_model = True
 
     exclude_params_repr_empty = {"ml_model"}
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
         # add the default ml model when empty
-        if "config_inst" in params:
+        if "analysis_inst" in params and "config_inst" in params:
+            analysis_inst = params["analysis_inst"]
             config_inst = params["config_inst"]
-            if params.get("ml_model") in (None, law.NO_STR) and config_inst.x("default_ml_model", None):
+            if (
+                params.get("ml_model") in (None, law.NO_STR) and
+                config_inst.x("default_ml_model", None)
+            ):
                 params["ml_model"] = config_inst.x.default_ml_model
 
             # initialize it once to trigger its set_config hook which might, in turn,
             # add objects to the config itself
             if params.get("ml_model") not in (None, law.NO_STR):
-                cls.get_ml_model_inst(params["ml_model"], config_inst)
+                params["ml_model_inst"] = cls.get_ml_model_inst(
+                    params["ml_model"],
+                    analysis_inst,
+                    requested_configs=[config_inst],
+                )
             elif not cls.allow_empty_ml_model:
                 raise Exception(f"no ml_model configured for {cls.task_family}")
 
         return params
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the ML model instance
         self.ml_model_inst = None
         if self.ml_model != law.NO_STR:
-            self.ml_model_inst = self.get_ml_model_inst(self.ml_model, self.config_inst)
+            self.ml_model_inst = self.get_ml_model_inst(
+                self.ml_model,
+                self.analysis_inst,
+                requested_configs=[self.config_inst],
+            )
 
     def store_parts(self) -> law.util.InsertableDict:
         parts = super().store_parts()
         if self.ml_model_inst:
             parts.insert_before("version", "ml_model", f"ml__{self.ml_model_inst.cls_name}")
         return parts
 
 
+class MLModelDataMixin(MLModelMixin):
+
+    allow_empty_ml_model = False
+
+    def store_parts(self) -> law.util.InsertableDict:
+        parts = super().store_parts()
+
+        # replace the ml_model entry
+        store_name = self.ml_model_inst.store_name or self.ml_model_inst.cls_name
+        parts.insert_before("ml_model", "ml_data", f"ml__{store_name}")
+        parts.pop("ml_model")
+
+        return parts
+
+
 class MLModelsMixin(ConfigTask):
 
     ml_models = law.CSVParameter(
         default=(),
         description="comma-separated names of ML models to be applied; empty default",
         brace_expand=True,
     )
@@ -562,34 +772,45 @@
 
     exclude_params_repr_empty = {"ml_models"}
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
-        if "config_inst" in params:
+        if "analysis_inst" in params and "config_inst" in params:
+            analysis_inst = params["analysis_inst"]
             config_inst = params["config_inst"]
             if not params.get("ml_models") and config_inst.x("default_ml_model", None):
                 params["ml_models"] = (config_inst.x.default_ml_model,)
 
             # special case: initialize them once to trigger their set_config hook
             if params.get("ml_models"):
-                for ml_model in params["ml_models"]:
-                    MLModelMixin.get_ml_model_inst(ml_model, config_inst)
+                params["ml_model_insts"] = [
+                    MLModelMixinBase.get_ml_model_inst(
+                        ml_model,
+                        analysis_inst,
+                        requested_configs=[config_inst],
+                    )
+                    for ml_model in params["ml_models"]
+                ]
             elif not cls.allow_empty_ml_models:
                 raise Exception(f"no ml_models configured for {cls.task_family}")
 
         return params
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the ML model instances
         self.ml_model_insts = [
-            MLModelMixin.get_ml_model_inst(ml_model, self.config_inst)
+            MLModelMixinBase.get_ml_model_inst(
+                ml_model,
+                self.analysis_inst,
+                requested_configs=[self.config_inst],
+            )
             for ml_model in self.ml_models
         ]
 
     def store_parts(self) -> law.util.InsertableDict:
         parts = super().store_parts()
         if self.ml_model_insts:
             part = "__".join(self.ml_models)
@@ -597,15 +818,15 @@
         return parts
 
 
 class InferenceModelMixin(ConfigTask):
 
     inference_model = luigi.Parameter(
         default=law.NO_STR,
-        description="the name of the inference model to the used; default: value of the "
+        description="the name of the inference model to be used; default: value of the "
         "'default_inference_model' config",
     )
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
```

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/parameters.py` & `columnflow-0.2.1/columnflow/tasks/framework/parameters.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/plotting.py` & `columnflow-0.2.1/columnflow/tasks/framework/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     )
     skip_legend = law.OptionalBoolParameter(
         default=None,
         significant=False,
         description="when True, no legend is drawn; default: None",
     )
     cms_label = luigi.ChoiceParameter(
-        choices=("wip", "pre", "sim", "simwip", "simpre", "public", "skip"),
+        choices=("wip", "pre", "pw", "sim", "simwip", "simpre", "simpw", "public", "skip"),
         default="wip",
         significant=False,
         description="Parameter to set the type of CMS logo; choices: "
-        "wip,pre,sim,simwip,simpre,public,skip; default: wip",
+        "wip,pre,pw,sim,simwip,simpre,simpw,public,skip; default: wip",
     )
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
         if "config_inst" not in params:
```

### Comparing `columnflow-0.2.0/columnflow/tasks/framework/remote.py` & `columnflow-0.2.1/columnflow/tasks/framework/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     @law.decorator.safe_output
     def run(self):
         # create the bundle
         bundle = law.LocalFileTarget(is_tmp="tgz")
         self.bundle(bundle)
 
         # log the size
-        size, unit = law.util.human_bytes(bundle.stat().st_size)
-        self.publish_message(f"size is {size:.2f} {unit}")
+        self.publish_message(f"size is {law.util.human_bytes(bundle.stat().st_size, fmt=True)}")
 
         # transfer the bundle
         self.transfer(bundle)
 
 
 class BundleSoftware(AnalysisTask, law.tasks.TransferLocalFile):
 
@@ -147,17 +146,20 @@
         BuildBashSandbox=BuildBashSandbox,
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the name and install path of the sandbox
+        from cf_sandbox_file_hash import create_sandbox_file_hash
         sandbox_file = os.path.expandvars(os.path.expanduser(self.sandbox_file))
+        self.sandbox_file_hash = create_sandbox_file_hash(sandbox_file)
         self.venv_name = os.path.splitext(os.path.basename(sandbox_file))[0]
-        self.venv_path = os.path.join(os.environ["CF_VENV_BASE"], self.venv_name)
+        self.venv_name_hashed = f"{self.venv_name}_{self.sandbox_file_hash}"
+        self.venv_path = os.path.join(os.environ["CF_VENV_BASE"], self.venv_name_hashed)
 
         # checksum cache
         self._checksum = None
 
     def requires(self):
         return self.reqs.BuildBashSandbox.req(self)
 
@@ -173,15 +175,15 @@
                     content = (flag_file, f.read().strip())
                 self._checksum = law.util.create_hash(content)
 
         return self._checksum
 
     def single_output(self):
         checksum = self.checksum or "TO_BE_INSTALLED"
-        return self.target(f"{self.venv_name}.{checksum}.tgz")
+        return self.target(f"{self.venv_name_hashed}.{checksum}.tgz")
 
     def get_file_pattern(self):
         path = os.path.expandvars(os.path.expanduser(self.single_output().path))
         return self.get_replicated_path(path, i=None if self.replicas <= 0 else r"[^\.]+")
 
     @law.decorator.log
     @law.decorator.safe_output
@@ -196,16 +198,15 @@
             return tarinfo
 
         # create the archive with a custom filter
         with self.publish_step(f"bundling venv {self.venv_name} ..."):
             bundle.dump(self.venv_path, add_kwargs={"filter": _filter}, formatter="tar")
 
         # log the size
-        size, unit = law.util.human_bytes(bundle.stat().st_size)
-        self.publish_message(f"size is {size:.2f} {unit}")
+        self.publish_message(f"size is {law.util.human_bytes(bundle.stat().st_size, fmt=True)}")
 
         # transfer the bundle
         self.transfer(bundle)
 
 
 class BundleCMSSWSandbox(AnalysisTask, law.cms.BundleCMSSW, law.tasks.TransferLocalFile):
 
@@ -223,56 +224,59 @@
 
     # upstream requirements
     reqs = Requirements(
         BuildBashSandbox=BuildBashSandbox,
     )
 
     def __init__(self, *args, **kwargs):
-        # cached bash sandbox that wraps the cmssw environment
-        self._cmssw_sandbox = None
-
         super().__init__(*args, **kwargs)
 
+        # get the name and install path of the sandbox
+        from cf_sandbox_file_hash import create_sandbox_file_hash
+        sandbox_file = os.path.expandvars(os.path.expanduser(self.sandbox_file))
+        self.sandbox_file_hash = create_sandbox_file_hash(sandbox_file)
+        self.cmssw_env_name = os.path.splitext(os.path.basename(sandbox_file))[0]
+        self.cmssw_env_name_hashed = f"{self.cmssw_env_name}_{self.sandbox_file_hash}"
+
     def requires(self):
         return self.reqs.BuildBashSandbox.req(self)
 
     def get_cmssw_path(self):
         # invoking .env will already trigger building the sandbox
         return self.requires().sandbox_inst.env["CMSSW_BASE"]
 
-    def get_file_pattern(self):
-        path = os.path.expandvars(os.path.expanduser(self.single_output().path))
-        return self.get_replicated_path(path, i=None if self.replicas <= 0 else r"[^\.]+")
-
     def single_output(self):
         cmssw_path = os.path.basename(self.get_cmssw_path())
-        return self.target(f"{cmssw_path}.{self.checksum}.tgz")
+        return self.target(f"{self.cmssw_env_name_hashed}_{cmssw_path}.{self.checksum}.tgz")
 
     def output(self):
         return law.tasks.TransferLocalFile.output(self)
 
+    def get_file_pattern(self):
+        path = os.path.expandvars(os.path.expanduser(self.single_output().path))
+        return self.get_replicated_path(path, i=None if self.replicas <= 0 else r"[^\.]+")
+
     @law.decorator.log
     def run(self):
         # create the bundle
         bundle = law.LocalFileTarget(is_tmp="tgz")
         self.bundle(bundle)
 
         # log the size
-        size, unit = law.util.human_bytes(bundle.stat().st_size)
-        self.publish_message(f"size is {size:.2f} {unit}")
+        self.publish_message(f"size is {law.util.human_bytes(bundle.stat().st_size, fmt=True)}")
 
         # transfer the bundle and mark the task as complete
         self.transfer(bundle)
 
 
 _default_htcondor_flavor = law.config.get_expanded("analysis", "htcondor_flavor", "cern")
 _default_htcondor_share_software = law.config.get_expanded_boolean("analysis", "htcondor_share_software", False)
 
 
-class HTCondorWorkflow(law.htcondor.HTCondorWorkflow):
+class HTCondorWorkflow(AnalysisTask, law.htcondor.HTCondorWorkflow):
 
     transfer_logs = luigi.BoolParameter(
         default=True,
         significant=False,
         description="transfer job logs to the output directory; default: True",
     )
     max_runtime = law.DurationParameter(
@@ -442,15 +446,15 @@
         if self.htcondor_memory > 0:
             config.custom_content.append(("Request_Memory", self.htcondor_memory))
 
         # helper to return uris and a file pattern for replicated bundles
         reqs = self.htcondor_workflow_requires()
         join_bash = lambda seq: " ".join(map('"{}"'.format, seq))
         def get_bundle_info(task):
-            uris = task.output().dir.uri(cmd="filecopy", return_all=True)
+            uris = task.output().dir.uri(base_name="filecopy", return_all=True)
             pattern = os.path.basename(task.get_file_pattern())
             return ",".join(uris), pattern
 
         # add repo variables
         uris, pattern = get_bundle_info(reqs["repo"])
         config.render_variables["cf_repo_uris"] = uris
         config.render_variables["cf_repo_pattern"] = pattern
@@ -504,15 +508,15 @@
         return True
 
 
 _default_slurm_flavor = law.config.get_expanded("analysis", "slurm_flavor", "maxwell")
 _default_slurm_partition = law.config.get_expanded("analysis", "slurm_partition", "cms-uhh")
 
 
-class SlurmWorkflow(law.slurm.SlurmWorkflow):
+class SlurmWorkflow(AnalysisTask, law.slurm.SlurmWorkflow):
 
     transfer_logs = luigi.BoolParameter(
         default=True,
         significant=False,
         description="transfer job logs to the output directory; default: True",
     )
     max_runtime = law.DurationParameter(
```

### Comparing `columnflow-0.2.0/columnflow/tasks/histograms.py` & `columnflow-0.2.1/columnflow/tasks/histograms.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,16 @@
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
         MLEvaluation=MLEvaluation,
     )
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot:
             if self.producers:
                 reqs["producers"] = [
@@ -80,15 +78,17 @@
                 for m in self.ml_models
             ]
 
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return self.target(f"histograms__vars_{self.variables_repr}__{self.branch}.pickle")
+        return {
+            "hists": self.target(f"histograms__vars_{self.variables_repr}__{self.branch}.pickle"),
+        }
 
     @law.decorator.log
     @law.decorator.localize(input=True, output=False)
     @law.decorator.safe_output
     def run(self):
         import hist
         import numpy as np
@@ -124,19 +124,19 @@
             read_columns |= {Route(column) for column in self.dataset_inst.x("event_weights", [])}
         read_columns = {Route(c) for c in read_columns}
 
         # empty float array to use when input files have no entries
         empty_f32 = ak.Array(np.array([], dtype=np.float32))
 
         # iterate over chunks of events and diffs
-        files = [inputs["events"]["collection"][0].path]
+        files = [inputs["events"]["collection"][0]["events"].path]
         if self.producers:
-            files.extend([inp.path for inp in inputs["producers"]])
+            files.extend([inp["columns"].path for inp in inputs["producers"]])
         if self.ml_models:
-            files.extend([inp.path for inp in inputs["ml"]])
+            files.extend([inp["mlcolumns"].path for inp in inputs["ml"]])
         for (events, *columns), pos in self.iter_chunked_io(
             files,
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             # add additional columns
             events = update_ak_array(events, *columns)
@@ -200,15 +200,15 @@
                     # apply it
                     fill_kwargs[variable_inst.name] = expr(events)
                 # broadcast and fill
                 arrays = (ak.flatten(a) for a in ak.broadcast_arrays(*fill_kwargs.values()))
                 histograms[var_key].fill(**dict(zip(fill_kwargs, arrays)))
 
         # merge output files
-        self.output().dump(histograms, formatter="pickle")
+        self.output()["hists"].dump(histograms, formatter="pickle")
 
 
 CreateHistogramsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=CreateHistograms,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
 )
@@ -243,18 +243,16 @@
         CreateHistograms=CreateHistograms,
     )
 
     def create_branch_map(self):
         # create a dummy branch map so that this task could as a job
         return {0: None}
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["hists"] = self.as_branch().requires()
 
         return reqs
 
     def requires(self):
         # optional dynamic behavior: determine not yet created variables and require only those
@@ -272,39 +270,39 @@
             branch=-1,
             variables=tuple(variables),
             _exclude={"branches"},
             _prefer_cli=prefer_cli,
         )
 
     def output(self):
-        return law.SiblingFileCollection({
+        return {"hists": law.SiblingFileCollection({
             variable_name: self.target(f"hist__{variable_name}.pickle")
             for variable_name in self.variables
-        })
+        })}
 
     @law.decorator.log
     def run(self):
         # preare inputs and outputs
         inputs = self.input()["collection"]
         outputs = self.output()
 
         # load input histograms
         hists = [
-            inp.load(formatter="pickle")
+            inp["hists"].load(formatter="pickle")
             for inp in self.iter_progress(inputs.targets.values(), len(inputs), reach=(0, 50))
         ]
 
         # create a separate file per output variable
         variable_names = list(hists[0].keys())
         for variable_name in self.iter_progress(variable_names, len(variable_names), reach=(50, 100)):
             self.publish_message(f"merging histograms for '{variable_name}'")
 
             variable_hists = [h[variable_name] for h in hists]
             merged = sum(variable_hists[1:], variable_hists[0].copy())
-            outputs[variable_name].dump(merged, formatter="pickle")
+            outputs["hists"][variable_name].dump(merged, formatter="pickle")
 
         # optionally remove inputs
         if self.remove_previous:
             inputs.remove()
 
 
 MergeHistogramsWrapper = wrapper_factory(
@@ -341,18 +339,16 @@
         MergeHistograms=MergeHistograms,
     )
 
     def create_branch_map(self):
         # create a dummy branch map so that this task could as a job
         return {0: None}
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # add nominal and both directions per shift source
         for shift in ["nominal"] + self.shifts:
             reqs[shift] = self.reqs.MergeHistograms.req(self, shift=shift, _prefer_cli={"variables"})
 
         return reqs
 
@@ -364,31 +360,31 @@
 
     def store_parts(self):
         parts = super().store_parts()
         parts.insert_after("dataset", "shift_sources", f"shifts_{self.shift_sources_repr}")
         return parts
 
     def output(self):
-        return law.SiblingFileCollection({
+        return {"hists": law.SiblingFileCollection({
             variable_name: self.target(f"shifted_hist__{variable_name}.pickle")
             for variable_name in self.variables
-        })
+        })}
 
     @law.decorator.log
     def run(self):
         # preare inputs and outputs
         inputs = self.input()
-        outputs = self.output().targets
+        outputs = self.output()["hists"].targets
 
         for variable_name, outp in self.iter_progress(outputs.items(), len(outputs)):
             self.publish_message(f"merging histograms for '{variable_name}'")
 
             # load hists
             variable_hists = [
-                coll.targets[variable_name].load(formatter="pickle")
+                coll["hists"].targets[variable_name].load(formatter="pickle")
                 for coll in inputs.values()
             ]
 
             # merge and write the output
             merged = sum(variable_hists[1:], variable_hists[0].copy())
             outp.dump(merged, formatter="pickle")
```

### Comparing `columnflow-0.2.0/columnflow/tasks/ml.py` & `columnflow-0.2.1/columnflow/tasks/ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 """
 
 import law
 import luigi
 
 from columnflow.tasks.framework.base import Requirements, AnalysisTask, DatasetTask, wrapper_factory
 from columnflow.tasks.framework.mixins import (
-    CalibratorsMixin, SelectorMixin, ProducersMixin, MLModelDataMixin, MLModelMixin, ChunkedIOMixin,
+    CalibratorsMixin,
+    SelectorMixin,
+    ProducersMixin,
+    MLModelDataMixin,
+    MLModelTrainingMixin,
+    MLModelMixin,
+    ChunkedIOMixin,
 )
 from columnflow.tasks.framework.remote import RemoteWorkflow
 from columnflow.tasks.reduction import MergeReducedEventsUser, MergeReducedEvents
 from columnflow.tasks.production import ProduceColumns
 from columnflow.util import dev_sandbox, safe_div
 
 
@@ -39,25 +45,28 @@
         ProduceColumns=ProduceColumns,
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # complain when this task is run for events that are not needed for training
-        if not self.events_used_in_training(self.dataset_inst, self.global_shift_inst):
+        if not self.events_used_in_training(
+            self.config_inst,
+            self.dataset_inst,
+            self.global_shift_inst,
+        ):
             raise Exception(
                 f"for ML model '{self.ml_model_inst.cls_name}', the dataset "
-                f"'{self.dataset_inst.name}' with shift '{self.global_shift_inst.name}' is not "
-                f"intended to be run by {self.__class__.__name__}",
+                f"'{self.dataset_inst.name}' of config '{self.config_inst.name}' with shift "
+                f"'{self.global_shift_inst.name}' is not intended to be run by "
+                f"{self.__class__.__name__}",
             )
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot and self.producers:
             reqs["producers"] = [
                 self.reqs.ProduceColumns.req(self, producer=p)
@@ -74,18 +83,18 @@
                 for p in self.producers
             ]
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
         k = self.ml_model_inst.folds
-        return law.SiblingFileCollection([
+        return {"mlevents": law.SiblingFileCollection([
             self.target(f"mlevents_fold{f}of{k}_{self.branch}.parquet")
             for f in range(k)
-        ])
+        ])}
 
     @law.decorator.log
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, sorted_ak_to_parquet, update_ak_array, add_ak_aliases,
@@ -100,29 +109,29 @@
         tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
         tmp_dir.touch()
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # define columns that will to be written
-        write_columns = self.ml_model_inst.used_columns
+        write_columns = set.union(*self.ml_model_inst.used_columns.values())
         route_filter = RouteFilter(write_columns)
 
         # define columns that need to be read
         read_columns = write_columns | {"deterministic_seed"} | set(aliases.values())
         read_columns = {Route(c) for c in read_columns}
 
         # stats for logging
         n_events = 0
         n_fold_events = self.ml_model_inst.folds * [0]
 
         # iterate over chunks of events and columns
-        files = [inputs["events"]["collection"][0].path]
+        files = [inputs["events"]["collection"][0]["events"].path]
         if self.producers:
-            files.extend([inp.path for inp in inputs["producers"]])
+            files.extend([inp["columns"].path for inp in inputs["producers"]])
         for (events, *columns), pos in self.iter_chunked_io(
             files,
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             n_events += len(events)
 
@@ -149,15 +158,15 @@
 
                 # save as parquet via a thread in the same pool
                 chunk = tmp_dir.child(f"file_{f}_{pos.index}.parquet", type="f")
                 output_chunks[f][pos.index] = chunk
                 self.chunked_io.queue(sorted_ak_to_parquet, (fold_events, chunk.path))
 
         # merge output files of all folds
-        for _output_chunks, output in zip(output_chunks, outputs.targets):
+        for _output_chunks, output in zip(output_chunks, outputs["mlevents"].targets):
             sorted_chunks = [_output_chunks[key] for key in sorted(_output_chunks)]
             law.pyarrow.merge_parquet_task(self, sorted_chunks, output, local=True)
 
         # some logs
         self.publish_message(f"total events: {n_events}")
         for f, n in enumerate(n_fold_events):
             r = 100 * safe_div(n, n_events)
@@ -240,40 +249,37 @@
     def merge_requires(self, start_leaf, end_leaf):
         return [
             self.reqs.PrepareMLEvents.req(self, branch=i)
             for i in range(start_leaf, end_leaf)
         ]
 
     def trace_merge_inputs(self, inputs):
-        return super().trace_merge_inputs([inp[self.fold] for inp in inputs])
+        return super().trace_merge_inputs([inp["mlevents"][self.fold] for inp in inputs])
 
     def merge_output(self):
         k = self.ml_model_inst.folds
-        return self.target(f"mlevents_f{self.fold}of{k}.parquet")
+        return {"mlevents": self.target(f"mlevents_f{self.fold}of{k}.parquet")}
 
     @law.decorator.log
     def run(self):
         return super().run()
 
     def merge(self, inputs, output):
-        law.pyarrow.merge_parquet_task(self, inputs, output)
+        law.pyarrow.merge_parquet_task(self, inputs, output["mlevents"])
 
 
 MergeMLEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=MergeMLEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets"],
 )
 
 
 class MLTraining(
-    MLModelMixin,
-    ProducersMixin,
-    SelectorMixin,
-    CalibratorsMixin,
+    MLModelTrainingMixin,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
 
     allow_empty_ml_model = False
 
     # upstream requirements
@@ -295,43 +301,73 @@
     def fold(self):
         return self.branch if self.is_branch() else None
 
     def create_branch_map(self):
         # each fold to train corresponds to one branch
         return list(range(self.ml_model_inst.folds))
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["events"] = {
-            dataset_inst.name: [
-                self.reqs.MergeMLEvents.req(self, dataset=dataset_inst.name, fold=fold, tree_index=-1)
-                for fold in range(self.ml_model_inst.folds)
-            ]
-            for dataset_inst in self.ml_model_inst.used_datasets
+            config_inst.name: {
+                dataset_inst.name: [
+                    self.reqs.MergeMLEvents.req(
+                        self,
+                        config=config_inst.name,
+                        dataset=dataset_inst.name,
+                        calibrators=_calibrators,
+                        selector=_selector,
+                        producers=_producers,
+                        fold=fold,
+                        tree_index=-1)
+                    for fold in range(self.ml_model_inst.folds)
+                ]
+                for dataset_inst in dataset_insts
+            }
+            for (config_inst, dataset_insts), _calibrators, _selector, _producers in zip(
+                self.ml_model_inst.used_datasets.items(),
+                self.calibrators,
+                self.selectors,
+                self.producers,
+            )
         }
 
         # ml model requirements
         reqs["model"] = self.ml_model_inst.requires(self)
 
         return reqs
 
     def requires(self):
         reqs = {}
 
         # require prepared events
         reqs["events"] = {
-            dataset_inst.name: [
-                self.reqs.MergeMLEvents.req(self, dataset=dataset_inst.name, fold=f)
-                for f in range(self.ml_model_inst.folds)
-                if f != self.branch
-            ]
-            for dataset_inst in self.ml_model_inst.used_datasets
+            config_inst.name: {
+                dataset_inst.name: [
+                    self.reqs.MergeMLEvents.req(
+                        self,
+                        config=config_inst.name,
+                        dataset=dataset_inst.name,
+                        calibrators=_calibrators,
+                        selector=_selector,
+                        producers=_producers,
+                        fold=f,
+                    )
+                    for f in range(self.ml_model_inst.folds)
+                    if f != self.branch
+                ]
+                for dataset_inst in dataset_insts
+            }
+            for (config_inst, dataset_insts), _calibrators, _selector, _producers in zip(
+                self.ml_model_inst.used_datasets.items(),
+                self.calibrators,
+                self.selectors,
+                self.producers,
+            )
         }
 
         # ml model requirements
         reqs["model"] = self.ml_model_inst.requires(self)
 
         return reqs
 
@@ -374,51 +410,63 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # set the sandbox
         self.sandbox = self.ml_model_inst.sandbox(self)
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
-        reqs["models"] = [
-            self.reqs.MLTraining.req(self, branch=f)
-            for f in range(self.ml_model_inst.folds)
-        ]
+        reqs["models"] = self.reqs.MLTraining.req_different_branching(
+            self,
+            configs=(self.config_inst.name,),
+            calibrators=(self.calibrators,),
+            selectors=(self.selector,),
+            producers=(self.producers,),
+        )
+
+        reqs["events"] = self.reqs.MergeReducedEvents.req_different_branching(self)
 
-        reqs["events"] = self.reqs.MergeReducedEvents.req(self, _exclude={"branches"})
         if not self.pilot and self.producers:
             reqs["producers"] = [
                 self.reqs.ProduceColumns.req(self, producer=p)
                 for p in self.producers
             ]
 
         return reqs
 
     def requires(self):
-        reqs = {"models": [
-            self.reqs.MLTraining.req(self, branch=f)
-            for f in range(self.ml_model_inst.folds)
-        ]}
+        reqs = {
+            "models": self.reqs.MLTraining.req_different_branching(
+                self,
+                configs=(self.config_inst.name,),
+                calibrators=(self.calibrators,),
+                selectors=(self.selector,),
+                producers=(self.producers,),
+                branch=-1,
+            ),
+            "events": self.reqs.MergeReducedEvents.req_different_branching(
+                self,
+                tree_index=self.branch,
+                branch=-1,
+            ),
+        }
 
-        reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"})
         if self.producers:
             reqs["producers"] = [
                 self.reqs.ProduceColumns.req(self, producer=p)
                 for p in self.producers
             ]
 
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return self.target(f"mlcols_{self.branch}.pickle")
+        return {"mlcolumns": self.target(f"mlcolumns_{self.branch}.pickle")}
 
     @law.decorator.log
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, sorted_ak_to_parquet, update_ak_array, add_ak_aliases,
@@ -430,37 +478,42 @@
         output_chunks = {}
 
         # create a temp dir for saving intermediate files
         tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
         tmp_dir.touch()
 
         # open all model files
-        models = [self.ml_model_inst.open_model(inp) for inp in inputs["models"]]
+        models = [
+            self.ml_model_inst.open_model(inp)
+            for inp in inputs["models"]["collection"].targets.values()
+        ]
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # check once if the events were used during trainig
         events_used_in_training = self.events_used_in_training(
+            self.config_inst,
             self.dataset_inst,
             self.global_shift_inst,
         )
 
         # define columns that need to be read
-        read_columns = self.ml_model_inst.used_columns | {"deterministic_seed"} | set(aliases.values())
+        read_columns = {"deterministic_seed"} | set(aliases.values())
+        read_columns |= set.union(*self.ml_model_inst.used_columns.values())
         read_columns = {Route(c) for c in read_columns}
 
         # define columns that will be written
-        write_columns = self.ml_model_inst.produced_columns
+        write_columns = set.union(*self.ml_model_inst.produced_columns.values())
         route_filter = RouteFilter(write_columns)
 
         # iterate over chunks of events and diffs
-        files = [inputs["events"]["collection"][0].path]
+        files = [inputs["events"]["collection"][0]["events"].path]
         if self.producers:
-            files.extend([inp.path for inp in inputs["producers"]])
+            files.extend([inp["columns"].path for inp in inputs["producers"]])
         for (events, *columns), pos in self.iter_chunked_io(
             files,
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             # add additional columns
             events = update_ak_array(events, *columns)
@@ -490,15 +543,15 @@
             # save as parquet via a thread in the same pool
             chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
             output_chunks[pos.index] = chunk
             self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
 
         # merge output files
         sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
-        law.pyarrow.merge_parquet_task(self, sorted_chunks, output, local=True)
+        law.pyarrow.merge_parquet_task(self, sorted_chunks, output["mlcolumns"], local=True)
 
 
 # overwrite class defaults
 MLEvaluation.check_finite = ChunkedIOMixin.check_finite.copy(
     default=MLEvaluation.task_family in check_finite_tasks,
     add_default_to_description=True,
 )
```

### Comparing `columnflow-0.2.0/columnflow/tasks/plotting.py` & `columnflow-0.2.1/columnflow/tasks/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,16 @@
     def create_branch_map(self):
         return [
             DotDict({"category": cat_name, "variable": var_name})
             for cat_name in sorted(self.categories)
             for var_name in sorted(self.variables)
         ]
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["merged_hists"] = self.requires_from_branch()
 
         return reqs
 
     @abstractmethod
     def get_plot_shifts(self):
@@ -94,15 +92,15 @@
 
         # histogram data per process
         hists = {}
 
         with self.publish_step(f"plotting {self.branch_data.variable} in {category_inst.name}"):
             for dataset, inp in self.input().items():
                 dataset_inst = self.config_inst.get_dataset(dataset)
-                h_in = inp["collection"][0].targets[self.branch_data.variable].load(formatter="pickle")
+                h_in = inp["collection"][0]["hists"].targets[self.branch_data.variable].load(formatter="pickle")
 
                 # loop and extract one histogram per process
                 for process_inst in process_insts:
                     # skip when the dataset is already known to not contain any sub process
                     if not any(map(dataset_inst.has_process, sub_process_insts[process_inst])):
                         continue
 
@@ -135,15 +133,19 @@
                     if process_inst in hists:
                         hists[process_inst] += h
                     else:
                         hists[process_inst] = h
 
             # there should be hists to plot
             if not hists:
-                raise Exception("no histograms found to plot")
+                raise Exception(
+                    "no histograms found to plot; possible reasons:\n" +
+                    "  - requested variable requires columns that were missing during histogramming\n" +
+                    "  - selected --processes did not match any value on the process axis of the input histogram",
+                )
 
             # sort hists by process order
             hists = OrderedDict(
                 (process_inst.copy_shallow(), hists[process_inst])
                 for process_inst in sorted(hists, key=process_insts.index)
             )
 
@@ -154,15 +156,15 @@
                 config_inst=self.config_inst,
                 category_inst=category_inst.copy_shallow(),
                 variable_insts=[var_inst.copy_shallow() for var_inst in variable_insts],
                 **self.get_plot_parameters(),
             )
 
             # save the plot
-            for outp in self.output():
+            for outp in self.output()["plots"]:
                 outp.dump(fig, formatter="mpl")
 
 
 class PlotVariablesBaseSingleShift(
     PlotVariablesBase,
     ShiftTask,
 ):
@@ -191,18 +193,18 @@
                 _prefer_cli={"variables"},
             )
             for d in self.datasets
         }
 
     def output(self):
         b = self.branch_data
-        return [
+        return {"plots": [
             self.target(name)
             for name in self.get_plot_names(f"plot__proc_{self.processes_repr}__cat_{b.category}__var_{b.variable}")
-        ]
+        ]}
 
     def get_plot_shifts(self):
         return [self.global_shift_inst]
 
 
 class PlotVariables1D(
     PlotVariablesBaseSingleShift,
@@ -275,20 +277,20 @@
                 _prefer_cli={"variables"},
             )
             for d in self.datasets
         }
 
     def output(self):
         b = self.branch_data
-        return [
+        return {"plots": [
             self.target(name)
             for name in self.get_plot_names(
                 f"plot__proc_{self.processes_repr}__unc_{b.shift_source}__cat_{b.category}__var_{b.variable}",
             )
-        ]
+        ]}
 
     def get_plot_shifts(self):
         return [
             self.config_inst.get_shift(s) for s in [
                 "nominal",
                 f"{self.branch_data.shift_source}_up",
                 f"{self.branch_data.shift_source}_down",
```

### Comparing `columnflow-0.2.0/columnflow/tasks/production.py` & `columnflow-0.2.1/columnflow/tasks/production.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,16 @@
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
     )
 
     register_producer_shifts = True
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         # add producer dependent requirements
         reqs["producer"] = self.producer_inst.run_requires()
 
@@ -53,15 +51,15 @@
         return {
             "events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"}),
             "producer": self.producer_inst.run_requires(),
         }
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return self.target(f"columns_{self.branch}.parquet")
+        return {"columns": self.target(f"columns_{self.branch}.parquet")}
 
     @law.decorator.log
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, mandatory_coffea_columns, add_ak_aliases, sorted_ak_to_parquet,
@@ -89,15 +87,15 @@
 
         # define columns that will be written
         write_columns = self.producer_inst.produced_columns
         route_filter = RouteFilter(write_columns)
 
         # iterate over chunks of events and diffs
         for events, pos in self.iter_chunked_io(
-            inputs["events"]["collection"][0].path,
+            inputs["events"]["collection"][0]["events"].path,
             source_type="awkward_parquet",
             read_columns=read_columns,
         ):
             # add aliases
             events = add_ak_aliases(events, aliases, remove_src=True)
 
             # invoke the producer
@@ -114,15 +112,15 @@
             # save as parquet via a thread in the same pool
             chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
             output_chunks[pos.index] = chunk
             self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
 
         # merge output files
         sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
-        law.pyarrow.merge_parquet_task(self, sorted_chunks, output, local=True)
+        law.pyarrow.merge_parquet_task(self, sorted_chunks, output["columns"], local=True)
 
 
 # overwrite class defaults
 check_finite_tasks = law.config.get_expanded("analysis", "check_finite_output", [], split_csv=True)
 ProduceColumns.check_finite = ChunkedIOMixin.check_finite.copy(
     default=ProduceColumns.task_family in check_finite_tasks,
     add_default_to_description=True,
```

### Comparing `columnflow-0.2.0/columnflow/tasks/reduction.py` & `columnflow-0.2.1/columnflow/tasks/reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Tasks related to reducing events for use on further tasks.
 """
 
 import math
 import functools
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
 
 import law
 import luigi
 
 from columnflow.tasks.framework.base import Requirements, AnalysisTask, DatasetTask, wrapper_factory
 from columnflow.tasks.framework.mixins import (
     CalibratorsMixin, SelectorStepsMixin, ChunkedIOMixin,
@@ -38,18 +38,16 @@
     reqs = Requirements(
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
         CalibrateEvents=CalibrateEvents,
         SelectEvents=SelectEvents,
     )
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         if not self.pilot:
             reqs["calibrations"] = [
                 self.reqs.CalibrateEvents.req(self, calibrator=c)
                 for c in self.calibrators
@@ -69,15 +67,15 @@
                 self.reqs.CalibrateEvents.req(self, calibrator=c)
                 for c in self.calibrators
             ],
             "selection": self.reqs.SelectEvents.req(self),
         }
 
     def output(self):
-        return self.target(f"events_{self.branch}.parquet")
+        return {"events": self.target(f"events_{self.branch}.parquet")}
 
     @ensure_proxy
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, mandatory_coffea_columns, update_ak_array, add_ak_aliases,
@@ -94,34 +92,52 @@
         tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
         tmp_dir.touch()
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # define columns that will be written
-        write_columns = set(self.config_inst.x.keep_columns.get(self.task_family, ["*"]))
+        write_columns = {
+            Route(c)
+            for c in self.config_inst.x.keep_columns.get(self.task_family, ["*"])
+        }
         route_filter = RouteFilter(write_columns)
 
+        # map routes to write to their top level column
+        write_columns_groups = defaultdict(set)
+        for route in write_columns:
+            if len(route) > 1:
+                write_columns_groups[route[0]].add(route)
+
         # define columns that need to be read
         read_columns = write_columns | set(mandatory_coffea_columns) | set(aliases.values())
         read_columns = {Route(c) for c in read_columns}
 
         # define columns to read for the differently structured selection masks
         read_sel_columns = set()
         # open either selector steps of the full event selection mask
         read_sel_columns.add(Route("steps.*" if self.selector_steps else "event"))
         # add object masks, depending on the columns to write
         # (as object masks are dynamic and deeply nested, preload the meta info to access fields)
-        write_columns_toplevel = {Route(r)[0] for r in write_columns}
         sel_results = inputs["selection"]["results"].load(formatter="dask_awkward")
         if "objects" in sel_results.fields:
             for src_field in sel_results.objects.fields:
                 for dst_field in sel_results.objects[src_field].fields:
-                    if law.util.multi_match(dst_field, write_columns_toplevel):
-                        read_sel_columns.add(Route(f"objects.{src_field}.{dst_field}"))
+                    # nothing to do in case the top level column does not need to be loaded
+                    if not law.util.multi_match(dst_field, write_columns_groups.keys()):
+                        continue
+                    # register the object masks
+                    read_sel_columns.add(Route(f"objects.{src_field}.{dst_field}"))
+                    # in case new collections are created and configured to be written, make sure
+                    # that the corresponding columns of the source collection are loaded
+                    if src_field != dst_field:
+                        read_columns |= {
+                            src_field + route[1:]
+                            for route in write_columns_groups[dst_field]
+                        }
         del sel_results
 
         # event counters
         n_all = 0
         n_reduced = 0
 
         # let the lfn_task prepare the nano file (basically determine a good pfn)
@@ -130,15 +146,15 @@
         # open the input file with uproot
         with self.publish_step("load and open ..."):
             nano_file = input_file.load(formatter="uproot")
 
         # collect input paths
         input_paths = [nano_file]
         input_paths.append(inputs["selection"]["results"].path)
-        input_paths.extend([inp.path for inp in inputs["calibrations"]])
+        input_paths.extend([inp["columns"].path for inp in inputs["calibrations"]])
         if self.selector_inst.produced_columns:
             input_paths.append(inputs["selection"]["columns"].path)
 
         # iterate over chunks of events and diffs
         for (events, sel, *diffs), pos in self.iter_chunked_io(
             input_paths,
             source_type=["coffea_root"] + (len(input_paths) - 1) * ["awkward_parquet"],
@@ -198,15 +214,15 @@
         # some logs
         self.publish_message(
             f"reduced {n_all} to {n_reduced} events ({safe_div(n_reduced, n_all) * 100:.2f}%)",
         )
 
         # merge output files
         sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
-        law.pyarrow.merge_parquet_task(self, sorted_chunks, output, local=True)
+        law.pyarrow.merge_parquet_task(self, sorted_chunks, output["events"], local=True)
 
 
 ReduceEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=ReduceEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
 )
@@ -250,23 +266,23 @@
 
         return params
 
     def requires(self):
         return self.reqs.ReduceEvents.req(self, branches=((0, self.n_inputs),))
 
     def output(self):
-        return self.target(f"stats_n{self.n_inputs}.json")
+        return {"stats": self.target(f"stats_n{self.n_inputs}.json")}
 
     @law.decorator.safe_output
     def run(self):
         # get all file sizes in bytes
         coll = self.input()["collection"]
         n = len(coll)
         sizes = [
-            inp.stat().st_size
+            inp["events"].stat().st_size
             for inp in self.iter_progress(coll.targets.values(), n, msg=f"loading {n} stats ...")
         ]
 
         # helpers for avg and mean computation
         def get_avg_std(values):
             n = len(values)
             if n < 1:
@@ -291,15 +307,15 @@
             ("n_test_files", n),
             ("tot_size", tot_size),
             ("avg_size", avg_size),
             ("std_size", std_size),
             ("max_size_merged", max_size_merged),
             ("merge_factor", merge_factor),
         ])
-        self.output().dump(stats, indent=4, formatter="json")
+        self.output()["stats"].dump(stats, indent=4, formatter="json")
 
         # print them
         self.publish_message(f" stats of {n} input files ".center(40, "-"))
         self.publish_message(f"tot. size: {law.util.human_bytes(tot_size, fmt=True)}")
         self.publish_message(f"avg. size: {law.util.human_bytes(avg_size, fmt=True)}")
         self.publish_message(f"std. size: {law.util.human_bytes(std_size, fmt=True)}")
         self.publish_message(" merging info ".center(40, "-"))
@@ -341,16 +357,16 @@
     def file_merging(self):
         """
         Needed by DatasetTask to define the default branch map.
         """
         if self._cached_file_merging < 0:
             # check of the merging stats is present and of so, set the cached file merging value
             output = self.reqs.MergeReductionStats.req(self).output()
-            if output.exists():
-                self._cached_file_merging = output.load(formatter="json")["merge_factor"]
+            if output["stats"].exists():
+                self._cached_file_merging = output["stats"].load(formatter="json")["merge_factor"]
                 self._cache_branches = True
 
         return self._cached_file_merging
 
     @property
     def merging_stats_exist(self):
         return self.file_merging >= 1
@@ -358,15 +374,15 @@
     def reduced_dummy_output(self):
         # dummy output to be returned in case the merging stats are not present yet
         return self.target("DUMMY_UNTIL_REDUCED_MERGING_STATS_EXIST")
 
     @classmethod
     def maybe_dummy(cls, func):
         # meant to wrap output methods of tasks depending on merging stats
-        # to inject a dummy output in case the status are not there yet
+        # to inject a dummy output in case the stats are not there yet
         @functools.wraps(func)
         def wrapper(self):
             # when the merging stats do not exist yet, return a dummy target
             if not self.merging_stats_exist:
                 return self.reduced_dummy_output()
 
             # otherwise, bind the wrapped function and call it
@@ -419,33 +435,35 @@
             ),
         }
 
     def trace_merge_workflow_inputs(self, inputs):
         return super().trace_merge_workflow_inputs(inputs["events"])
 
     def trace_merge_inputs(self, inputs):
-        return super().trace_merge_inputs(inputs["events"]["collection"].targets.values())
+        return super().trace_merge_inputs([
+            inp["events"] for inp in inputs["events"]["collection"].targets.values()
+        ])
 
     def reduced_dummy_output(self):
         # mark the dummy output as a placeholder for the ForestMerge task
         dummy = super().reduced_dummy_output()
         self._mark_merge_output_placeholder(dummy)
         return dummy
 
     @MergeReducedEventsUser.maybe_dummy
     def merge_output(self):
         # use the branch_map defined in DatasetTask to compute the number of files after merging
         n_merged = len(DatasetTask.create_branch_map(self))
         return law.SiblingFileCollection([
-            self.target(f"events_{i}.parquet")
+            {"events": self.target(f"events_{i}.parquet")}
             for i in range(n_merged)
         ])
 
     def merge(self, inputs, output):
-        law.pyarrow.merge_parquet_task(self, inputs, output)
+        law.pyarrow.merge_parquet_task(self, inputs, output["events"])
 
 
 MergeReducedEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=MergeReducedEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
 )
```

### Comparing `columnflow-0.2.0/columnflow/tasks/selection.py` & `columnflow-0.2.1/columnflow/tasks/selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from columnflow.tasks.framework.remote import RemoteWorkflow
 from columnflow.tasks.external import GetDatasetLFNs
 from columnflow.tasks.calibration import CalibrateEvents
 from columnflow.production import Producer
 from columnflow.util import maybe_import, ensure_proxy, dev_sandbox, safe_div
 
 
+np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 class SelectEvents(
     SelectorMixin,
     CalibratorsMixin,
     ChunkedIOMixin,
@@ -36,18 +37,16 @@
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
         CalibrateEvents=CalibrateEvents,
     )
 
     register_selector_shifts = True
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         if not self.pilot:
             reqs["calib"] = [
                 self.reqs.CalibrateEvents.req(self, calibrator=c)
                 for c in self.calibrators
@@ -118,28 +117,28 @@
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # define columns that need to be read
         read_columns = mandatory_coffea_columns | self.selector_inst.used_columns | set(aliases.values())
         read_columns = {Route(c) for c in read_columns}
 
         # define columns that will be written
-        write_columns = self.selector_inst.produced_columns
+        write_columns = mandatory_coffea_columns | self.selector_inst.produced_columns
         route_filter = RouteFilter(write_columns)
 
         # let the lfn_task prepare the nano file (basically determine a good pfn)
         [(lfn_index, input_file)] = lfn_task.iter_nano_files(self)
 
         # open the input file with uproot
         with self.publish_step("load and open ..."):
             nano_file = input_file.load(formatter="uproot")
 
         # iterate over chunks of events and diffs
         n_calib = len(inputs["calibrations"])
         for (events, *diffs), pos in self.iter_chunked_io(
-            [nano_file] + [inp.path for inp in inputs["calibrations"]],
+            [nano_file] + [inp["columns"].path for inp in inputs["calibrations"]],
             source_type=["coffea_root"] + n_calib * ["awkward_parquet"],
             read_columns=(1 + n_calib) * [read_columns],
         ):
             # apply the calibrated diffs
             events = update_ak_array(events, *diffs)
 
             # add aliases
@@ -216,61 +215,56 @@
     CalibratorsMixin,
     DatasetTask,
     law.tasks.ForestMerge,
 ):
     # recursively merge 20 files into one
     merge_factor = 20
 
-    # default upstream dependency task classes
-    dep_SelectEvents = SelectEvents
-
     # skip receiving some parameters via req
     exclude_params_req_get = {"workflow"}
 
     # upstream requirements
     reqs = Requirements(
         SelectEvents=SelectEvents,
     )
 
     def create_branch_map(self):
         # DatasetTask implements a custom branch map, but we want to use the one in ForestMerge
         return law.tasks.ForestMerge.create_branch_map(self)
 
     def merge_workflow_requires(self):
-        return self.reqs.SelectEvents.req(self, _exclude={"branches"}, _prefer_cli={"workflow"})
+        return self.reqs.SelectEvents.req(self, _exclude={"branches"})
 
     def merge_requires(self, start_branch, end_branch):
         return self.reqs.SelectEvents.req(
             self,
             branches=((start_branch, end_branch),),
             workflow="local",
             _exclude={"branch"},
         )
 
     def merge_output(self):
-        return self.target("stats.json")
+        return {"stats": self.target("stats.json")}
 
     def trace_merge_inputs(self, inputs):
-        return super().trace_merge_inputs(
-            inp["stats"] for inp in inputs["collection"].targets.values()
-        )
+        return super().trace_merge_inputs(inputs["collection"].targets.values())
 
     @law.decorator.log
     def run(self):
         return super().run()
 
     def merge(self, inputs, output):
         # merge input stats
         merged_stats = defaultdict(float)
         for inp in inputs:
-            stats = inp.load(formatter="json", cache=False)
+            stats = inp["stats"].load(formatter="json", cache=False)
             self.merge_counts(merged_stats, stats)
 
         # write the output
-        output.dump(merged_stats, indent=4, formatter="json", cache=False)
+        output["stats"].dump(merged_stats, indent=4, formatter="json", cache=False)
 
     @classmethod
     def merge_counts(cls, dst: dict, src: dict) -> dict:
         """
         Adds counts (integers or floats) in a *src* dictionary recursively into a *dst* dictionary.
         *dst* is updated in-place and also returned.
         """
@@ -308,79 +302,92 @@
         RemoteWorkflow.reqs,
         SelectEvents=SelectEvents,
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # store the normalization weight producer
-        self.norm_weight_producer = Producer.get_cls("normalization_weights")(
-            inst_dict=self.get_producer_kwargs(self),
-        )
+        # store the normalization weight producer for MC
+        self.norm_weight_producer = None
+        if self.dataset_inst.is_mc:
+            self.norm_weight_producer = Producer.get_cls("normalization_weights")(
+                inst_dict=self.get_producer_kwargs(self),
+            )
 
     def create_branch_map(self):
         # DatasetTask implements a custom branch map, but we want to use the one in ForestMerge
         return law.tasks.ForestMerge.create_branch_map(self)
 
     def merge_workflow_requires(self):
-        return {
+        reqs = {
             "selection": self.reqs.SelectEvents.req(self, _exclude={"branches"}),
-            "normalization": self.norm_weight_producer.run_requires(),
         }
 
+        if self.dataset_inst.is_mc:
+            reqs["normalization"] = self.norm_weight_producer.run_requires()
+
+        return reqs
+
     def merge_requires(self, start_branch, end_branch):
-        return {
+        reqs = {
             "selection": [
                 self.reqs.SelectEvents.req(self, branch=b)
                 for b in range(start_branch, end_branch)
             ],
-            "normalization": self.norm_weight_producer.run_requires(),
         }
 
+        if self.dataset_inst.is_mc:
+            reqs["normalization"] = self.norm_weight_producer.run_requires()
+
+        return reqs
+
     def trace_merge_workflow_inputs(self, inputs):
         return super().trace_merge_workflow_inputs(inputs["selection"])
 
     def trace_merge_inputs(self, inputs):
         return super().trace_merge_inputs(inputs["selection"])
 
     def merge_output(self):
-        return self.target("masks.parquet")
+        return {"masks": self.target("masks.parquet")}
 
     def merge(self, inputs, output):
         # in the lowest (leaf) stage, zip selection results with additional columns first
         if self.is_leaf():
             # create a temp dir for saving intermediate files
             tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
             tmp_dir.touch()
             inputs = self.zip_results_and_columns(inputs, tmp_dir)
+        else:
+            inputs = [inp["masks"] for inp in inputs]
 
-        law.pyarrow.merge_parquet_task(self, inputs, output)
+        law.pyarrow.merge_parquet_task(self, inputs, output["masks"])
 
     def zip_results_and_columns(self, inputs, tmp_dir):
-        import awkward as ak
-        from columnflow.columnar_util import RouteFilter, sorted_ak_to_parquet
+        from columnflow.columnar_util import RouteFilter, sorted_ak_to_parquet, mandatory_coffea_columns
 
         chunks = []
 
         # setup the normalization weights producer
-        self.norm_weight_producer.run_setup(
-            self.requires()["forest_merge"]["normalization"],
-            self.input()["forest_merge"]["normalization"],
-        )
+        if self.dataset_inst.is_mc:
+            self.norm_weight_producer.run_setup(
+                self.requires()["forest_merge"]["normalization"],
+                self.input()["forest_merge"]["normalization"],
+            )
 
         # define columns that will be written
-        write_columns = set(self.config_inst.x.keep_columns[self.task_family])
+        write_columns = mandatory_coffea_columns | set(self.config_inst.x.keep_columns[self.task_family])
         route_filter = RouteFilter(write_columns)
 
         for inp in inputs:
             events = inp["columns"].load(formatter="awkward")
             steps = inp["results"].load(formatter="awkward").steps
 
             # add normalization weight
-            events = self.norm_weight_producer(events)
+            if self.dataset_inst.is_mc:
+                events = self.norm_weight_producer(events)
 
             # remove columns
             events = route_filter(events)
 
             # zip them
             out = ak.zip({"steps": steps, "events": events})
```

### Comparing `columnflow-0.2.0/columnflow/tasks/union.py` & `columnflow-0.2.1/columnflow/tasks/union.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,16 @@
         MergeReducedEvents.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
         MLEvaluation=MLEvaluation,
     )
 
-    def workflow_requires(self, only_super: bool = False):
+    def workflow_requires(self):
         reqs = super().workflow_requires()
-        if only_super:
-            return reqs
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot:
             if self.producers:
                 reqs["producers"] = [
@@ -76,15 +74,15 @@
                 for m in self.ml_models
             ]
 
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return self.target(f"data_{self.branch}.parquet")
+        return {"columns": self.target(f"data_{self.branch}.parquet")}
 
     @law.decorator.log
     @law.decorator.localize(input=True, output=False)
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, mandatory_coffea_columns, update_ak_array, sorted_ak_to_parquet,
@@ -104,19 +102,19 @@
         route_filter = RouteFilter(write_columns)
 
         # define columns that need to be read
         read_columns = write_columns | set(mandatory_coffea_columns)
         read_columns = {Route(c) for c in read_columns}
 
         # iterate over chunks of events and diffs
-        files = [inputs["events"]["collection"][0].path]
+        files = [inputs["events"]["collection"][0]["events"].path]
         if self.producers:
-            files.extend([inp.path for inp in inputs["producers"]])
+            files.extend([inp["columns"].path for inp in inputs["producers"]])
         if self.ml_models:
-            files.extend([inp.path for inp in inputs["ml"]])
+            files.extend([inp["mlcolumns"].path for inp in inputs["ml"]])
         for (events, *columns), pos in self.iter_chunked_io(
             files,
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             # add additional columns
             events = update_ak_array(events, *columns)
@@ -131,15 +129,15 @@
             # save as parquet via a thread in the same pool
             chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
             output_chunks[pos.index] = chunk
             self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
 
         # merge output files
         sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
-        law.pyarrow.merge_parquet_task(self, sorted_chunks, output, local=True)
+        law.pyarrow.merge_parquet_task(self, sorted_chunks, output["columns"], local=True)
 
 
 # overwrite class defaults
 check_finite_tasks = law.config.get_expanded("analysis", "check_finite_output", [], split_csv=True)
 UniteColumns.check_finite = ChunkedIOMixin.check_finite.copy(
     default=UniteColumns.task_family in check_finite_tasks,
     add_default_to_description=True,
```

### Comparing `columnflow-0.2.0/columnflow/util.py` & `columnflow-0.2.1/columnflow/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 from __future__ import annotations
 
 __all__ = [
     "UNSET", "env_is_remote", "env_is_dev", "primes",
     "maybe_import", "import_plt", "import_ROOT", "import_file", "create_random_name", "expand_path",
     "real_path", "ensure_dir", "wget", "call_thread", "call_proc", "ensure_proxy", "dev_sandbox",
-    "safe_div", "test_float", "is_pattern", "is_regex", "pattern_matcher",
+    "safe_div", "test_float", "test_int", "is_pattern", "is_regex", "pattern_matcher",
     "dict_add_strict", "get_source_code",
     "DotDict", "MockModule", "FunctionArgs", "ClassPropertyDescriptor", "classproperty",
     "DerivableMeta", "Derivable",
 ]
 
 import os
+import abc
 import uuid
 import queue
 import threading
 import subprocess
 import importlib
 import fnmatch
 import re
@@ -163,16 +164,15 @@
         path = os.path.expandvars(os.path.expanduser(path))
 
     return path
 
 
 def real_path(*path: str) -> str:
     """
-    Takes *path* fragments and returns the joined,  real and absolute location with all variables
-    expanded.
+    Takes *path* fragments and returns the real, absolute location with all variables expanded.
     """
     return os.path.realpath(expand_path(*path))
 
 
 def ensure_dir(path: str) -> str:
     """
     Ensures that a directory at *path* (and its subdirectories) exists and returns the full,
@@ -391,23 +391,34 @@
     Returns *a* divided by *b* if *b* is not zero, and zero otherwise.
     """
     return (a / b) if b else 0.0
 
 
 def test_float(f: Any) -> bool:
     """
-    Tests whether a value *i* can be converted to a float.
+    Tests whether a value *f* can be converted to a float.
     """
     try:
         float(f)
         return True
     except (ValueError, TypeError):
         return False
 
 
+def test_int(i: Any) -> bool:
+    """
+    Tests whether a value *i* can be converted to an integer.
+    """
+    try:
+        int(i)
+        return True
+    except (ValueError, TypeError):
+        return False
+
+
 def is_pattern(s: str) -> bool:
     """
     Returns *True* if a string *s* contains pattern characters such as "*" or "?", and *False*
     otherwise.
     """
     return "*" in s or "?" in s
 
@@ -653,15 +664,15 @@
     """
     if not isinstance(func, (classmethod, staticmethod)):
         func = classmethod(func)
 
     return ClassPropertyDescriptor(func)
 
 
-class DerivableMeta(type):
+class DerivableMeta(abc.ABCMeta):
     """
     Meta class for :py:class:`Derivable` objects providing class-level features such as improved
     tracing and lookup of subclasses, and single-line subclassing for partial-like overwriting of
     class-level attributes.
     """
 
     _classes = {}
```

### Comparing `columnflow-0.2.0/columnflow.egg-info/PKG-INFO` & `columnflow-0.2.1/columnflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: columnflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: columnflow
-Home-page: https://github.com/uhh-cms/columnflow
-Author: The Columnflow Team
-Author-email: todo@uni-hamburg.de
+Home-page: https://github.com/columnflow/columnflow
+Author: The columnflow team
+Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,28 +20,28 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <center>
-  <a href="https://github.com/uhh-cms/columnflow">
-    <img src="https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/logo_dark.png" width="480" />
+  <a href="https://github.com/columnflow/columnflow">
+    <img src="https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/logo_dark.png" width="480" />
   </a>
 </center>
 
 
 <!-- marker-after-logo -->
 
 
-[![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/workflows/lint_and_test.yaml)
+[![Build status](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/actions/workflows/lint_and_test.yaml)
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
-[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=master)](http://columnflow.readthedocs.io)
-[![Code coverge](https://codecov.io/gh/uhh-cms/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow)
-[![License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https://github.com/uhh-cms/columnflow/blob/master/LICENSE)
+[![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
+[![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
+[![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
 
 <!-- marker-after-header -->
 
 
@@ -49,24 +49,24 @@
 
 This project is currently in a beta phase.
 The project setup, suggested workflows, definitions of particular tasks, and the signatures of various helper classes and functions are mostly frozen but could still be subject to changes in the near future.
 At this point (December 2022), four large-scale analyses based upon columnflow are being developed, and in the process, help test and verify various aspects of its core.
 The first released version is expected in early 2023.
 However, if you would like to join early on, contribute or just give it a spin, feel free to get in touch!
 
-![Columnflow analytics](https://repobeats.axiom.co/api/embed/bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics")
+![Columnflow analytics](https://repobeats.axiom.co/api/embed/b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics")
 
 
 ## Quickstart
 
-To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/uhh-cms/columnflow/tree/master/analysis_templates).
+To create an analysis using columnflow, it is recommended to start from a predefined template (located in [analysis_templates](https://github.com/columnflow/columnflow/tree/master/analysis_templates)).
 The following command (no previous git clone required) interactively asks for a handful of names and settings, and creates a minimal, yet fully functioning project structure for you!
 
 ```shell
-bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/columnflow/master/create_analysis.sh)"
+bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/columnflow/master/create_analysis.sh)"
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
@@ -76,15 +76,15 @@
   2. Run local tests & linting checks to verify that the analysis is setup correctly.
     > ./tests/run_all
 
   3. Create a GRID proxy if you intend to run tasks that need one
     > voms-proxy-init -voms cms -rfc -valid 196:00
 
   4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/master/start.html
+    https://columnflow.readthedocs.io/en/stable/start.html
 
     Suggestions for tasks to run:
 
     a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
        default dataset using the default calibrator and default selector
        (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
@@ -95,15 +95,15 @@
     c) Include the ttbar dataset and also plot jet1_eta:
       > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 
     d) Create cms-style datacards for the example model in hgg/inference/example.py:
       > law run cf.CreateDatacards --version dev1 --inference-model example
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
@@ -115,36 +115,36 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/uhh-cms/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=kramerto" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/riga"><img src="https://avatars.githubusercontent.com/u/1908734?v=4?s=100" width="100px;" alt="Marcel Rieger"/><br /><sub><b>Marcel Rieger</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Ariga" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Documentation">📖</a> <a href="https://github.com/columnflow/columnflow/commits?author=riga" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mafrahm"><img src="https://avatars.githubusercontent.com/u/49306645?v=4?s=100" width="100px;" alt="Mathis Frahm"/><br /><sub><b>Mathis Frahm</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mafrahm" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Amafrahm" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=dsavoiu" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Adsavoiu" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkausw"><img src="https://avatars.githubusercontent.com/u/26219567?v=4?s=100" width="100px;" alt="pkausw"/><br /><sub><b>pkausw</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=pkausw" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/pulls?q=is%3Apr+reviewed-by%3Apkausw" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nprouvost"><img src="https://avatars.githubusercontent.com/u/49162277?v=4?s=100" width="100px;" alt="nprouvost"/><br /><sub><b>nprouvost</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=nprouvost" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Bogdan-Wiederspan"><img src="https://avatars.githubusercontent.com/u/79155113?v=4?s=100" width="100px;" alt="Bogdan-Wiederspan"/><br /><sub><b>Bogdan-Wiederspan</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Code">💻</a> <a href="https://github.com/columnflow/columnflow/commits?author=Bogdan-Wiederspan" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kramerto"><img src="https://avatars.githubusercontent.com/u/18616159?v=4?s=100" width="100px;" alt="Tobias Kramer"/><br /><sub><b>Tobias Kramer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=kramerto" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=mschrode" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=jolange" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/uhh-cms/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mschrode"><img src="https://avatars.githubusercontent.com/u/5065234?v=4?s=100" width="100px;" alt="Matthias Schroeder"/><br /><sub><b>Matthias Schroeder</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=mschrode" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jolange"><img src="https://avatars.githubusercontent.com/u/6584443?v=4" width="100px;" alt="Johannes Lange"/><br /><sub><b>Johannes Lange</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=jolange" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BalduinLetzer"><img src="https://avatars.githubusercontent.com/u/70058868?v=4?s=100" width="100px;" alt="BalduinLetzer"/><br /><sub><b>BalduinLetzer</b></sub></a><br /><a href="https://github.com/columnflow/columnflow/commits?author=BalduinLetzer" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
 
 
 ## Development
 
-- Source hosted at [GitHub](https://github.com/uhh-cms/columnflow)
-- Report issues, questions, feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/issues)
+- Source hosted at [GitHub](https://github.com/columnflow/columnflow)
+- Report issues, questions, feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/issues)
 
 
 <!-- marker-after-body -->
```

#### html2text {}

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1 Name: columnflow Version: 0.2.0 Summary: columnflow Home-
-page: https://github.com/uhh-cms/columnflow Author: The Columnflow Team Author-
-email: todo@uni-hamburg.de License: BSD-3-Clause Keywords:
+Metadata-Version: 2.1 Name: columnflow Version: 0.2.1 Summary: columnflow Home-
+page: https://github.com/columnflow/columnflow Author: The columnflow team
+Author-email: github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Development Status :: 4 - Beta Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology Requires-Python: >=3.7,
 <4 Description-Content-Type: text/markdown License-File: LICENSE
- [https://media.githubusercontent.com/media/uhh-cms/columnflow/master/assets/
+[https://media.githubusercontent.com/media/columnflow/columnflow/master/assets/
                                 logo_dark.png]
- [![Build status](https://github.com/uhh-cms/columnflow/actions/workflows/
-lint_and_test.yaml/badge.svg)](https://github.com/uhh-cms/columnflow/actions/
-workflows/lint_and_test.yaml) [![Package version](https://img.shields.io/pypi/
-v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow) [!
-[Documentation status](https://readthedocs.org/projects/columnflow/badge/
-?version=master)](http://columnflow.readthedocs.io) [![Code coverge](https://
-codecov.io/gh/uhh-cms/columnflow/branch/master/graph/
-badge.svg?token=33FLINPXFP)](https://codecov.io/gh/uhh-cms/columnflow) [!
-[License](https://img.shields.io/github/license/uhh-cms/columnflow.svg)](https:
-//github.com/uhh-cms/columnflow/blob/master/LICENSE) Backend for columnar,
-fully orchestrated HEP analyses with pure Python, [law](https://github.com/
-riga/law) and [order](https://github.com/riga/order).  ## Note on current
-development This project is currently in a beta phase. The project setup,
-suggested workflows, definitions of particular tasks, and the signatures of
-various helper classes and functions are mostly frozen but could still be
+ [![Build status](https://github.com/columnflow/columnflow/actions/workflows/
+lint_and_test.yaml/badge.svg)](https://github.com/columnflow/columnflow/
+actions/workflows/lint_and_test.yaml) [![Package version](https://
+img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/
+columnflow) [![Documentation status](https://readthedocs.org/projects/
+columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
+coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
+badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
+[License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
+(https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
+columnar, fully orchestrated HEP analyses with pure Python, [law](https://
+github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
+current development This project is currently in a beta phase. The project
+setup, suggested workflows, definitions of particular tasks, and the signatures
+of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
 analytics](https://repobeats.axiom.co/api/embed/
-bb5150c6a379b852d6c8f9eca3e2620bbcb23c4b.svg "Columnflow analytics") ##
+b6ebc5ba41019de55eb48e195eecb438890442c8.svg "Columnflow analytics") ##
 Quickstart To create an analysis using columnflow, it is recommended to start
 from a predefined template (located in [analysis_templates](https://github.com/
-uhh-cms/columnflow/tree/master/analysis_templates). The following command (no
-previous git clone required) interactively asks for a handful of names and
+columnflow/columnflow/tree/master/analysis_templates)). The following command
+(no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
-you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/uhh-cms/
+you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
 repository and install the environment. > source setup.sh [optional_setup_name]
 2. Run local tests & linting checks to verify that the analysis is setup
 correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
 that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
 'Getting started' guide to run your first tasks. https://
-columnflow.readthedocs.io/en/master/start.html Suggestions for tasks to run: a)
+columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
 law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
 distribution for the single top dataset: > law run cf.PlotVariables1D --version
 dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
 plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
 --variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
 model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
 --inference-model example ``` For a better overview of the tasks that are
 triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/uhh-cms/columnflow/issues/25#issue-1258137827). ##
+graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
 Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
 hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
 github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
 /github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
 (https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
 events with CMS. - [analysis playground](https://github.com/uhh-cms/
 analysis_playground): A testing playground for HEP analyses. ## Contributors
@@ -75,10 +75,10 @@
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
                       ð»                ð»          ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. ## Development - Source hosted at
-[GitHub](https://github.com/uhh-cms/columnflow) - Report issues, questions,
-feature requests on [GitHub Issues](https://github.com/uhh-cms/columnflow/
+[GitHub](https://github.com/columnflow/columnflow) - Report issues, questions,
+feature requests on [GitHub Issues](https://github.com/columnflow/columnflow/
 issues)
```

### Comparing `columnflow-0.2.0/columnflow.egg-info/SOURCES.txt` & `columnflow-0.2.1/columnflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,29 @@
 columnflow/production/cms/muon.py
 columnflow/production/cms/pdf.py
 columnflow/production/cms/pileup.py
 columnflow/production/cms/scale.py
 columnflow/production/cms/seeds.py
 columnflow/selection/__init__.py
 columnflow/selection/matching.py
+columnflow/selection/cms/__init__.py
+columnflow/selection/cms/json_filter.py
+columnflow/selection/cms/met_filters.py
 columnflow/tasks/__init__.py
 columnflow/tasks/calibration.py
 columnflow/tasks/cutflow.py
 columnflow/tasks/external.py
 columnflow/tasks/histograms.py
 columnflow/tasks/ml.py
 columnflow/tasks/plotting.py
 columnflow/tasks/production.py
 columnflow/tasks/reduction.py
 columnflow/tasks/selection.py
 columnflow/tasks/union.py
+columnflow/tasks/yields.py
 columnflow/tasks/cms/__init__.py
 columnflow/tasks/cms/external.py
 columnflow/tasks/cms/inference.py
 columnflow/tasks/framework/__init__.py
 columnflow/tasks/framework/base.py
 columnflow/tasks/framework/decorators.py
 columnflow/tasks/framework/mixins.py
```

### Comparing `columnflow-0.2.0/setup.py` & `columnflow-0.2.1/setup.py`

 * *Files identical despite different names*

