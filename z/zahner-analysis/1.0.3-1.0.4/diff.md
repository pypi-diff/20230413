# Comparing `tmp/zahner_analysis-1.0.3.tar.gz` & `tmp/zahner_analysis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zahner_analysis-1.0.3.tar", last modified: Mon Jan 16 15:03:30 2023, max compression
+gzip compressed data, was "zahner_analysis-1.0.4.tar", last modified: Thu Apr 13 11:03:47 2023, max compression
```

## Comparing `zahner_analysis-1.0.3.tar` & `zahner_analysis-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     7119 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5840 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1665 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.166333 zahner_analysis-1.0.3/zahner_analysis/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/zahner_analysis/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9132 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/analysis_tools/analysis_connection.py
--rw-r--r--   0 runner    (1001) docker     (116)    26939 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/analysis_tools/eis_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/zahner_analysis/file_import/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13651 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/impedance_model_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     7096 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/isc_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     8764 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/ism_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     6933 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/iss_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     3310 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/file_import/thales_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.170333 zahner_analysis-1.0.3/zahner_analysis/plotting/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14910 2023-01-16 15:03:17.000000 zahner_analysis-1.0.3/zahner_analysis/plotting/impedance_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 15:03:30.166333 zahner_analysis-1.0.3/zahner_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7119 2023-01-16 15:03:30.000000 zahner_analysis-1.0.3/zahner_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-01-16 15:03:30.000000 zahner_analysis-1.0.3/zahner_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-16 15:03:30.000000 zahner_analysis-1.0.3/zahner_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       26 2023-01-16 15:03:30.000000 zahner_analysis-1.0.3/zahner_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-01-16 15:03:30.000000 zahner_analysis-1.0.3/zahner_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.089647 zahner_analysis-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/BasicIntroduction/
+-rw-r--r--   0 runner    (1001) docker     (123)   459849 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/AnalysisScreenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   152479 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/
+-rw-r--r--   0 runner    (1001) docker     (123)   105801 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100508 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-data.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)   374829 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    89466 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132610 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79494 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)    45584 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-battery.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    61065 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/Examples/ZHIT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/RC-R-L.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)   434541 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/drift.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/jupyter
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/matplotlib
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/numpy
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/requests
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/scipy
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/analysis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29914 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/eis_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/zahner_analysis/file_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/impedance_model_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/isc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/ism_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/iss_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/seqtxt_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/thales_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/zahner_analysis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/plotting/impedance_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/top_level.txt
```

### Comparing `zahner_analysis-1.0.3/LICENSE` & `zahner_analysis-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/PKG-INFO` & `zahner_analysis-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 Metadata-Version: 2.1
 Name: zahner_analysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for the analysis of electrochemical impedance spectra.
-Home-page: https://zahner.de/
-Author: Maximilian Krapp
-Author-email: maximilian.krapp@zahner.de
-License: MIT
+Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
+License: MIT License
+        
+        Copyright (c) 2022 Zahner-Elektrik
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Project-URL: Documentation, https://doc.zahner.de/zahner_analysis
 Project-URL: Examples, https://github.com/Zahner-elektrik/Zahner-Analysis-Python/tree/main/Examples
 Project-URL: Source Code, https://github.com/Zahner-elektrik/Zahner-Analysis-Python
 Project-URL: Bug Tracker, https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues
-Keywords: potentiostat, electrochemistry, chemistry, eis, cyclic voltammetry, fuel-cell, battery
-Platform: any
+Project-URL: Homepage, https://zahner.de/
+Keywords: potentiostat,electrochemistry,chemistry,eis,cyclic voltammetry,fuel-cell,battery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Zahner-Analysis-Python](https://doc.zahner.de/github_resources/zahner_analysis.png)
 
 [zahner_analysis](zahner_analysis) is a Python package which uses the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) to evaluate measured electrochemical data.
 
@@ -113,23 +134,30 @@
 
 ## [ImpedanceVsVoltageSeriesFit.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb)
 
 * EIS series fit
 * Load all files from a directory
 * Plot circuit element vs series parameter
 
+## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
+
+* Fit the model to the data
+* Load the data and the model
+* Perform ZHIT evaluation
+* Plot the result
+
 # 📧 Haveing a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
 
 # ✅ Requirements
 
 Programming is done with the latest Python version at the time of commit.
 
-If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
+If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis Software](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
 
 The packages [matplotlib](https://matplotlib.org/), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) are used to display the measurement results. The [requests package](https://pypi.org/project/requests/) is necessary to communicate with the Zahner Analysis. Jupyter is not necessary, each example is also available as a Python file.
```

### Comparing `zahner_analysis-1.0.3/README.md` & `zahner_analysis-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,30 @@
 
 ## [ImpedanceVsVoltageSeriesFit.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb)
 
 * EIS series fit
 * Load all files from a directory
 * Plot circuit element vs series parameter
 
+## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
+
+* Fit the model to the data
+* Load the data and the model
+* Perform ZHIT evaluation
+* Plot the result
+
 # 📧 Haveing a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
 
 # ✅ Requirements
 
 Programming is done with the latest Python version at the time of commit.
 
-If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
+If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis Software](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
 
 The packages [matplotlib](https://matplotlib.org/), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) are used to display the measurement results. The [requests package](https://pypi.org/project/requests/) is necessary to communicate with the Zahner Analysis. Jupyter is not necessary, each example is also available as a Python file.
```

### Comparing `zahner_analysis-1.0.3/zahner_analysis/analysis_tools/analysis_connection.py` & `zahner_analysis-1.0.4/zahner_analysis/analysis_tools/analysis_connection.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/zahner_analysis/analysis_tools/eis_fitting.py` & `zahner_analysis-1.0.4/zahner_analysis/analysis_tools/eis_fitting.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,49 @@
 from zahner_analysis.file_import.impedance_model_import import (
     IsfxModelImport,
     IsfxModelElement,
     IsfxModelElementParameter,
 )
 from zahner_analysis.plotting.impedance_plot import bodePlotter, nyquistPlotter
 from zahner_analysis.analysis_tools.analysis_connection import AnalysisConnection
+from zahner_analysis.analysis_tools.error import ZahnerAnalysisError
 
 import os
 import json
 import io
 import logging
 import time
 
+DUMMY_MODEL = """<?xml version="1.0" encoding="UTF-8"?>
+<zahner-impedance-model name="New Model">
+    <zahner-fileinfo>
+        <type>zahner-impedance-model</type>
+        <file-version>3.0</file-version>
+        <created>2023-04-13T07:51:22+02:00</created>
+        <generator>Zahner Analysis</generator>
+        <generator-version>3.3.5</generator-version>
+        <comment></comment>
+        <app-session>cef8c2e3-250d-47ff-9638-ef58933d107e</app-session>
+        <file-id>e0e0c2a4-296f-40d0-9937-58cad6e47464</file-id>
+    </zahner-fileinfo>
+    <parsed-tree>
+        <serial-connect>
+            <resistor name="R0">
+                <parameter index="0" value="100" fitterFixed="1"/>
+            </resistor>
+        </serial-connect>
+    </parsed-tree>
+    <schematics-graph>
+        <node pos-x="0" type="1" name="R0" node-id="0" pos-y="-64">
+            <parameter value="100" fitterFixed="1" index="0"/>
+        </node>
+    </schematics-graph>
+</zahner-impedance-model>
+"""
+
 
 class EisFittingResult:
     """This class contains the results of the fit.
 
     The constructor of this class is called by the fit method.
 
     :param fitResult: Fit result as JSON string.
@@ -297,35 +325,78 @@
 
             fitting = ImpedanceFitting(conn)
 
     :param analysisConnection: Optional connection object to the Zahner Analysis.
         Not needed if Zahner Analysis is installed locally.
     """
 
-    classAnalysisConnection = None
+    classAnalysisConnection: AnalysisConnection = None
 
     def __init__(self, analysisConnection: AnalysisConnection = None):
         self._analysisConnection = analysisConnection
 
         if self._analysisConnection is None:
             if EisFitting.classAnalysisConnection is None:
                 EisFitting.classAnalysisConnection = AnalysisConnection()
 
             self._analysisConnection = EisFitting.classAnalysisConnection
         return
 
+    def zhit(
+        self,
+        data: IsmImport = None,
+        parameters: dict = {},
+        timeout: float = None,
+    ) -> IsmImport:
+        """
+        Performs the ZHIT evaluation.
+
+        ZHIT is a software tool that uses measured phase data to reconstruct the impedance spectrum.
+        The reconstructed impedance spectrum is then compared to the measured impedance spectrum to validate the measurement and identify any artifacts.
+
+        Links to the topic ZHIT:
+         * https://en.wikipedia.org/wiki/Z-HIT
+         * https://doc.zahner.de/manuals/zahner_analysis.pdf
+
+        Parameter dictionary for optional parameters:
+
+        .. csv-table::
+            :header-rows: 1
+
+            Key , Description
+            Smoothness , Factor with which smoothed. This must be determined empirically in the GUI.
+            NumberOfSamples , Number of samples used for the data. Default all samples.
+
+        .. code-block:: python
+
+            parameters = {
+                "Smoothness": 0.0002,
+                "NumberOfSamples": 20
+            }
+
+        :param data: Data to which the ZHIT is applied.
+        :param parameters: Optional parameters for the ZHIT.
+        :param timeout: Timeout for the caculation.
+        """
+        model = IsfxModelImport(xmlString=DUMMY_MODEL)
+        parameters["DataSource"] = "zhit"
+        # A fit is performed and then everything is discarded except the data used for the fit.
+        fitResult = self.fit(model, data, parameters, timeout=timeout)
+        return fitResult.getFitInputData()
+
     def fit(
         self,
         model: IsfxModelImport,
         data: IsmImport = None,
         fitParams: dict = {},
         simulationParams: dict = {},
         timeout: float = None,
     ) -> EisFittingResult:
-        """Performing the fit.
+        """
+        Performing the fit.
 
         With this method the model is fitted to the data.
         The initial values and the model can be easily developed using the Zahner Analysis GUI.
 
         The parameters are optional. You can also use only some optional parameters and omit others.
         Parameter dictionary for optional fit parameters:
 
@@ -378,24 +449,27 @@
         paramsDict["job"] = "EvalEis.Fit"
         paramsDict["parameters"] = {"Fit": fitParams, "Simulation": simulationParams}
         paramsDict["mode"] = "queued"
 
         jobId = self._startFit(model, data, paramsDict)
         logging.debug("Zahner Analysis job-id: " + jobId)
         fitResult = self._waitForJob(jobId, timeout)
+        if fitResult is None:
+            raise ZahnerAnalysisError("Operation in Zahner Analysis Server failed")
         fittedModel = self._readFittedModel(jobId)
         fittedSimulatedSamples = self._readSimulatedData(jobId)
         fitInputSamples = self._readFitInputData(jobId)
 
         return EisFittingResult(
             fitResult, fittedModel, fittedSimulatedSamples, fitInputSamples
         )
 
     def _startFit(self, model: IsfxModelImport, data: IsmImport, params: dict) -> str:
-        """Function which starts the fit.
+        """
+        Function which starts the fit.
 
         This function sends the model, data and parameters to the Zahner Analysis via HTTP post request.
         The JobId assigned by Zahner Analysis is returned.
 
         :param model: Model which is fitted to the data.
         :param data: Data to which the model is fitted.
         :param dict: Dictionary {"Fit":fitParams, "Simulation":simulationParams}.
@@ -408,29 +482,29 @@
                 (model.getFileName(), io.BytesIO(model.getBinaryFileContent())),
             ),
             ("job", (None, json.dumps(params).encode("utf-8"))),
         ]
         reply = self._analysisConnection.post("/job/start", files=files)
 
         if reply.status_code == 200:
-
             replyContent = json.loads(reply.content)
             jobId = replyContent["job-id"]
 
             if replyContent["status"] in ["failed", "error"]:
                 logging.error("Zahner Analysis reply: " + str(replyContent))
         else:
             logging.error("Zahner Analysis reply: " + str(replyContent))
 
         return jobId
 
     def simulate(
         self, model: IsfxModelImport, simulationParams: dict, timeout: float = None
     ) -> IsmImport:
-        """Simulate the model.
+        """
+        Simulate the model.
 
         With this method, an impedance spectrum is generated from the model.
 
         Parameter dictionary for simulation parameters:
 
         .. csv-table::
             :header-rows: 1
@@ -461,15 +535,16 @@
         jobId = self._startSimulation(model, paramsDict)
         logging.debug("Zahner Analysis job-id: " + jobId)
         self._waitForJob(jobId, timeout)
 
         return self._readSimulatedData(jobId)
 
     def _startSimulation(self, model: IsfxModelImport, params: dict) -> str:
-        """Function which starts the simulation.
+        """
+        Function which starts the simulation.
 
         This function sends the model and parameters to the Zahner Analysis via HTTP post request.
         The JobId assigned by Zahner Analysis is returned.
 
         :param model: Model to be simulated.
         :param dict: Dictionary {"Simulation":simulationParams}.
         :returns: JobId
@@ -480,27 +555,27 @@
                 (model.getFileName(), io.BytesIO(model.getBinaryFileContent())),
             ),
             ("job", (None, json.dumps(params).encode("utf-8"))),
         ]
         reply = self._analysisConnection.post("/job/start", files=files)
 
         if reply.status_code == 200:
-
             replyContent = json.loads(reply.content)
             jobId = replyContent.get("job-id")
 
             if replyContent["status"] in ["failed", "error"]:
                 logging.error("Zahner Analysis reply: " + str(replyContent))
         else:
             logging.error("Zahner Analysis reply: " + str(replyContent))
 
         return jobId
 
     def _waitForJob(self, jobId: str, timeout: float = None):
-        """Function which is waiting for the fit.
+        """
+        Function which is waiting for the fit result.
 
         This function polls the status of the fit operation and reads the fit result as JSON.
 
         :param jobId: JobId.
         :param timeout: Time for which polling should be done in seconds, or None for infinite.
         :returns: Fit result as JSON string.
         """
@@ -514,15 +589,17 @@
             if reply.status_code == 200:
                 replyContent = json.loads(reply.content)
                 jobStatus = replyContent["status"]
 
                 if jobStatus == "done":
                     continueWait = False
                     result = replyContent.get("result")
-
+                elif jobStatus == "failed":
+                    continueWait = False
+                    logging.error("Zahner Analysis fitting failed")
                 else:
                     diffTime = time.time() - startTime
                     if timeout is not None:
                         if diffTime > timeout:
                             logging.error("Zahner Analysis fitting timeout")
                             continueWait = False
                     if continueWait == True:
@@ -533,26 +610,28 @@
                 logging.error(
                     "Zahner Analysis reply: " + str(json.loads(reply.content))
                 )
 
         return result
 
     def _readFittedModel(self, jobId) -> IsfxModelImport:
-        """Reading the fitted model from the Zahner Analysis.
+        """
+        Reading the fitted model from the Zahner Analysis.
 
         Reading is done via http get request.
 
         :param jobId: JobId.
         :returns: Object from received data.
         """
         reply = self._analysisConnection.get(f"/job/{jobId}/model")
         return IsfxModelImport(xmlString=reply.content.decode("utf-8"))
 
     def _readFitInputData(self, jobId) -> IsmImport:
-        """Reading the Samples used for fit from the Zahner Analysis.
+        """
+        Reading the Samples used for fit from the Zahner Analysis.
 
         Reading is done via http get request.
 
         :param jobId: JobId.
         :returns: Object from received data.
         """
         reply = self._analysisConnection.get(f"/job/{jobId}/samples")
@@ -567,15 +646,16 @@
         :returns: Object from received data.
         """
         reply = self._analysisConnection.get(f"/job/{jobId}/simulation")
         return IsmImport(reply.content)
 
 
 class EisFittingPlotter:
-    """Class with utility Nyquist and Bode plotting methods.
+    """
+    Class with utility Nyquist and Bode plotting methods.
 
     This class contains methods to display the fit results in the style of Zahner Analysis.
     """
 
     @staticmethod
     def plotBode(
         fittingResult: EisFittingResult,
@@ -655,15 +735,16 @@
     def plotNyquist(
         fittingResult: EisFittingResult,
         impedanceData: IsmImport = None,
         ax=None,
         minusNyquist=True,
         maximumAbsImpedance: float = None,
     ):
-        """Plotting the data in the Nyquist plot.
+        """
+        Plotting the data in the Nyquist plot.
 
         For plotting matplotlib is used with the function :meth:`zahner_analysis.plotting.impedance_plot.nyquistPlot`.
         With this function or also only with matplotlib the plot can be represented adapted.
         This method displays the plot in the standard Zahner Analysis design.
 
         Either axes can be passed on which will be plotted, or a new figure with axes will be created
         automatically. The figure and the axes are always returned.
```

### Comparing `zahner_analysis-1.0.3/zahner_analysis/file_import/impedance_model_import.py` & `zahner_analysis-1.0.4/zahner_analysis/file_import/impedance_model_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Either you pass the filename of the model you want to open or you pass the content of the file as a string.
 
     :param xmlFilePath: The file path of the isfx model file.
     :param xmlString: The model as a string or the content of an isfx file.
     """
 
     def __init__(self, xmlFilePath=None, xmlString=None):
-        self._filename = None
+        self._filename = "FromString.isfx"
         if xmlString is not None:
             self._xmlString = xmlString
             self._completeXmlTree = et.fromstring(xmlString)
         elif xmlFilePath is not None:
             (_, self._filename) = os.path.split(xmlFilePath)
             with open(xmlFilePath, "r", encoding="utf-8") as filename:
                 self._xmlString = filename.read()
@@ -167,21 +167,15 @@
 
         If the model was created from the disk, then the filename is returned,
         otherwise the name attribute from the xml is returned.
         If the xml name attribute is an empty string "FromString.isfx" is returned.
 
         :returns: The name.
         """
-        if self._filename is None:
-            if self._completeXmlTree.attrib["name"] == "":
-                return "FromString.isfx"
-            else:
-                return self._completeXmlTree.attrib["name"]
-        else:
-            return self._filename
+        return self._filename
 
     def getBinaryFileContent(self):
         """Get the content of the file binary.
 
         Returns the file contents as a binary byte array.
 
         :returns: bytearray with the file content.
```

### Comparing `zahner_analysis-1.0.3/zahner_analysis/file_import/isc_import.py` & `zahner_analysis-1.0.4/zahner_analysis/file_import/isc_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/zahner_analysis/file_import/ism_import.py` & `zahner_analysis-1.0.4/zahner_analysis/file_import/ism_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
 THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import numpy as np
 import datetime
 import io
 import os
+from typing import Union
 
 from zahner_analysis.file_import.thales_file_utils import *
 
 
 class IsmImport:
     """Class to be able to read ism files (EIS data).
 
     This class extracts the data from the ism files.
     It returns the data for the frequency range between the reversal frequency and the end frequency.
 
     :param file: The path to the ism file, or the ism file as bytes or bytearray.
     :type file: str, bytes, bytearray
     """
 
-    def __init__(self, filename):
+    def __init__(self, filename: Union[str, bytes, bytearray]):
         self._filename = "FromBytes.ism"
         if isinstance(filename, bytes) or isinstance(filename, bytearray):
             self._binaryFileContent = filename
             ismFile = io.BytesIO(filename)
         else:
             (_, self._filename) = os.path.split(filename)
             with open(filename, "rb") as f:
```

### Comparing `zahner_analysis-1.0.3/zahner_analysis/file_import/iss_import.py` & `zahner_analysis-1.0.4/zahner_analysis/file_import/iss_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/zahner_analysis/file_import/thales_file_utils.py` & `zahner_analysis-1.0.4/zahner_analysis/file_import/thales_file_utils.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/zahner_analysis/plotting/impedance_plot.py` & `zahner_analysis-1.0.4/zahner_analysis/plotting/impedance_plot.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.3/zahner_analysis.egg-info/PKG-INFO` & `zahner_analysis-1.0.4/zahner_analysis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 Metadata-Version: 2.1
 Name: zahner-analysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for the analysis of electrochemical impedance spectra.
-Home-page: https://zahner.de/
-Author: Maximilian Krapp
-Author-email: maximilian.krapp@zahner.de
-License: MIT
+Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
+License: MIT License
+        
+        Copyright (c) 2022 Zahner-Elektrik
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Project-URL: Documentation, https://doc.zahner.de/zahner_analysis
 Project-URL: Examples, https://github.com/Zahner-elektrik/Zahner-Analysis-Python/tree/main/Examples
 Project-URL: Source Code, https://github.com/Zahner-elektrik/Zahner-Analysis-Python
 Project-URL: Bug Tracker, https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues
-Keywords: potentiostat, electrochemistry, chemistry, eis, cyclic voltammetry, fuel-cell, battery
-Platform: any
+Project-URL: Homepage, https://zahner.de/
+Keywords: potentiostat,electrochemistry,chemistry,eis,cyclic voltammetry,fuel-cell,battery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Zahner-Analysis-Python](https://doc.zahner.de/github_resources/zahner_analysis.png)
 
 [zahner_analysis](zahner_analysis) is a Python package which uses the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) to evaluate measured electrochemical data.
 
@@ -113,23 +134,30 @@
 
 ## [ImpedanceVsVoltageSeriesFit.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb)
 
 * EIS series fit
 * Load all files from a directory
 * Plot circuit element vs series parameter
 
+## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
+
+* Fit the model to the data
+* Load the data and the model
+* Perform ZHIT evaluation
+* Plot the result
+
 # 📧 Haveing a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
 
 # ✅ Requirements
 
 Programming is done with the latest Python version at the time of commit.
 
-If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
+If you work with equivalent circuits and you need the fit and simulate functions, you need the [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with its REST interface. To use the REST interface, you need a licensed [Zahner Analysis](https://zahner.de/products-details/software/Zahner-Analysis) with at least version **3.2.1**. The [Zahner Analysis Software](https://zahner.de/products-details/software/Zahner-Analysis) is **not required for importing and plotting** data.
 
 The packages [matplotlib](https://matplotlib.org/), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) are used to display the measurement results. The [requests package](https://pypi.org/project/requests/) is necessary to communicate with the Zahner Analysis. Jupyter is not necessary, each example is also available as a Python file.
```

