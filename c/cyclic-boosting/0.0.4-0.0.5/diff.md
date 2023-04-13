# Comparing `tmp/cyclic-boosting-0.0.4.tar.gz` & `tmp/cyclic-boosting-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclic-boosting-0.0.4.tar", last modified: Tue Apr  4 11:12:38 2023, max compression
+gzip compressed data, was "cyclic-boosting-0.0.5.tar", last modified: Thu Apr 13 11:01:53 2023, max compression
```

## Comparing `cyclic-boosting-0.0.4.tar` & `cyclic-boosting-0.0.5.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.935792 cyclic-boosting-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.923792 cyclic-boosting-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.923792 cyclic-boosting-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-04 11:12:38.935792 cyclic-boosting-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/cyclic_boosting/
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/GBSregression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45795 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/cyclic_boosting/binning/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/binning/_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/binning/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/binning/bin_number_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/binning/ecdf_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/common_smoothers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/nbinom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/cyclic_boosting/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/plots/_1dplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/plots/_2dplots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/extrapolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/meta_smoother.py
--rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/multidim.py
--rw-r--r--   0 runner    (1001) docker     (123)    26512 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/onedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/smoothing/orthofit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30604 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/cyclic_boosting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-04 11:12:38.000000 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-04 11:12:38.000000 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 11:12:38.000000 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 11:12:38.000000 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 11:12:38.000000 cyclic-boosting-0.0.4/cyclic_boosting.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.927792 cyclic-boosting-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.931792 cyclic-boosting-0.0.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/cyclic_boosting.binning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/cyclic_boosting.plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/cyclic_boosting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/cyclic_boosting.smoothing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 11:12:38.935792 cyclic-boosting-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 11:12:38.935792 cyclic-boosting-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)  2526940 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/integration_test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_smoothing_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_smoothing_multidim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_smoothing_onedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_smoothing_ortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-04 11:12:26.000000 cyclic-boosting-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.104747 cyclic-boosting-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.108747 cyclic-boosting-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting/
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/GBSregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45795 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/bin_number_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/ecdf_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/common_smoothers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/learning_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/nbinom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.120747 cyclic-boosting-0.0.5/cyclic_boosting/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/_1dplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/_2dplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.120747 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/extrapolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/meta_smoother.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/multidim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26512 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/onedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/orthofit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30604 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.124748 cyclic-boosting-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.128748 cyclic-boosting-0.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.binning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.smoothing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)  2526940 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/integration_test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_learning_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_multidim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_onedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_ortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_utils.py
```

### Comparing `cyclic-boosting-0.0.4/.github/workflows/python-publish.yml` & `cyclic-boosting-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/.github/workflows/tests.yaml` & `cyclic-boosting-0.0.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/.gitignore` & `cyclic-boosting-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/.readthedocs.yaml` & `cyclic-boosting-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/LICENSE` & `cyclic-boosting-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/PKG-INFO` & `cyclic-boosting-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: cyclic-boosting
-Version: 0.0.4
+Version: 0.0.5
 Author: Blue Yonder GmbH
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-cyclic-boosting
-===============
+# cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
 
-Documentation
--------------
+## Documentation
 
 The documentation can be found [here](https://cyclic-boosting.readthedocs.io/en/latest/).
 
-Usage
------
+## Quickstart
+
+```
+pip install cyclic-boosting
+```
+
+```python
+from cyclic_boosting.pipelines import pipeline_CBPoissonRegressor
+CB_est = pipeline_CBPoissonRegressor()
+CB_est.fit(X_train, y)
+yhat = CB_est.predict(X_test)
+```
+
+## Usage
 
 It can be used in a [scikit-learn](https://scikit-learn.org/stable/)-like fashion, combining a binning method (e.g., [BinNumberTransformer](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/binning/bin_number_transformer.py)) with a Cyclic Boosting estimator (find all estimators in the [init](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/__init__.py)). Usage examples can be found in the [integration tests](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/tests/test_integration.py).
```

### Comparing `cyclic-boosting-0.0.4/README.md` & `cyclic-boosting-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-cyclic-boosting
-===============
+# cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
 
-Documentation
--------------
+## Documentation
 
 The documentation can be found [here](https://cyclic-boosting.readthedocs.io/en/latest/).
 
-Usage
------
+## Quickstart
+
+```
+pip install cyclic-boosting
+```
+
+```python
+from cyclic_boosting.pipelines import pipeline_CBPoissonRegressor
+CB_est = pipeline_CBPoissonRegressor()
+CB_est.fit(X_train, y)
+yhat = CB_est.predict(X_test)
+```
+
+## Usage
 
 It can be used in a [scikit-learn](https://scikit-learn.org/stable/)-like fashion, combining a binning method (e.g., [BinNumberTransformer](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/binning/bin_number_transformer.py)) with a Cyclic Boosting estimator (find all estimators in the [init](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/__init__.py)). Usage examples can be found in the [integration tests](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/tests/test_integration.py).
```

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/GBSregression.py` & `cyclic-boosting-0.0.5/cyclic_boosting/GBSregression.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/__init__.py` & `cyclic-boosting-0.0.5/cyclic_boosting/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/base.py` & `cyclic-boosting-0.0.5/cyclic_boosting/base.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/binning/__init__.py` & `cyclic-boosting-0.0.5/cyclic_boosting/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/binning/_binary_search.py` & `cyclic-boosting-0.0.5/cyclic_boosting/binning/_binary_search.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/binning/_utils.py` & `cyclic-boosting-0.0.5/cyclic_boosting/binning/_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/binning/bin_number_transformer.py` & `cyclic-boosting-0.0.5/cyclic_boosting/binning/bin_number_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/binning/ecdf_transformer.py` & `cyclic-boosting-0.0.5/cyclic_boosting/binning/ecdf_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/classification.py` & `cyclic-boosting-0.0.5/cyclic_boosting/classification.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/common_smoothers.py` & `cyclic-boosting-0.0.5/cyclic_boosting/common_smoothers.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/features.py` & `cyclic-boosting-0.0.5/cyclic_boosting/features.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/flags.py` & `cyclic-boosting-0.0.5/cyclic_boosting/flags.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/learning_rate.py` & `cyclic-boosting-0.0.5/cyclic_boosting/learning_rate.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/link.py` & `cyclic-boosting-0.0.5/cyclic_boosting/link.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/location.py` & `cyclic-boosting-0.0.5/cyclic_boosting/location.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/nbinom.py` & `cyclic-boosting-0.0.5/cyclic_boosting/nbinom.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/observers.py` & `cyclic-boosting-0.0.5/cyclic_boosting/observers.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/pipelines.py` & `cyclic-boosting-0.0.5/cyclic_boosting/pipelines.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/plots/_1dplots.py` & `cyclic-boosting-0.0.5/cyclic_boosting/plots/_1dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/plots/_2dplots.py` & `cyclic-boosting-0.0.5/cyclic_boosting/plots/_2dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/plots/__init__.py` & `cyclic-boosting-0.0.5/cyclic_boosting/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/plots/plot_utils.py` & `cyclic-boosting-0.0.5/cyclic_boosting/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/price.py` & `cyclic-boosting-0.0.5/cyclic_boosting/price.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/regression.py` & `cyclic-boosting-0.0.5/cyclic_boosting/regression.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/base.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/base.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/extrapolate.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/extrapolate.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/meta_smoother.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/meta_smoother.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/multidim.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/multidim.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/onedim.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/onedim.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/smoothing/orthofit.py` & `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/orthofit.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting/utils.py` & `cyclic-boosting-0.0.5/cyclic_boosting/utils.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting.egg-info/PKG-INFO` & `cyclic-boosting-0.0.5/cyclic_boosting.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: cyclic-boosting
-Version: 0.0.4
+Version: 0.0.5
 Author: Blue Yonder GmbH
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-cyclic-boosting
-===============
+# cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
 
-Documentation
--------------
+## Documentation
 
 The documentation can be found [here](https://cyclic-boosting.readthedocs.io/en/latest/).
 
-Usage
------
+## Quickstart
+
+```
+pip install cyclic-boosting
+```
+
+```python
+from cyclic_boosting.pipelines import pipeline_CBPoissonRegressor
+CB_est = pipeline_CBPoissonRegressor()
+CB_est.fit(X_train, y)
+yhat = CB_est.predict(X_test)
+```
+
+## Usage
 
 It can be used in a [scikit-learn](https://scikit-learn.org/stable/)-like fashion, combining a binning method (e.g., [BinNumberTransformer](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/binning/bin_number_transformer.py)) with a Cyclic Boosting estimator (find all estimators in the [init](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/__init__.py)). Usage examples can be found in the [integration tests](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/tests/test_integration.py).
```

### Comparing `cyclic-boosting-0.0.4/cyclic_boosting.egg-info/SOURCES.txt` & `cyclic-boosting-0.0.5/cyclic_boosting.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .readthedocs.yaml
+CODE_OF_CONDUCT.md
 LICENSE
 README.md
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/python-publish.yml
 .github/workflows/tests.yaml
```

### Comparing `cyclic-boosting-0.0.4/docs/Makefile` & `cyclic-boosting-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/make.bat` & `cyclic-boosting-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/conf.py` & `cyclic-boosting-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/cyclic_boosting.binning.rst` & `cyclic-boosting-0.0.5/docs/source/cyclic_boosting.binning.rst`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/cyclic_boosting.rst` & `cyclic-boosting-0.0.5/docs/source/cyclic_boosting.rst`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/cyclic_boosting.smoothing.rst` & `cyclic-boosting-0.0.5/docs/source/cyclic_boosting.smoothing.rst`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/index.rst` & `cyclic-boosting-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/docs/source/introduction.md` & `cyclic-boosting-0.0.5/docs/source/introduction.md`

 * *Files 25% similar despite different names*

```diff
@@ -10,31 +10,45 @@
 Furthermore, model building with Cyclic Boosting is very convenient:
 * few hyperparameters to be tuned
 * not much data pre-processing needed
 * easily configurable for different data types
 * supporting missing values in input data
 * assisting model development with individual analysis plots for features
 
-...
-[base module](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.base)
+Instead of estimating parameters in the sense of coefficients in linear
+regression or weights in neural networks, Cyclic Boosting estimates factors (or
+summands in additive regression mode) for each bin of the different features.
+This allows a natural interpretation of each individual prediction in terms of
+the different feature values, i.e., individual explainability.
+
+The Cyclic Boosting [base algorithm](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.base)
+is quite generic and can be adapted for both regression (in several modes) and
+classification tasks.
 
 Regression
 ----------
 
-...
-
-[multiplicative regression mode](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.regression)
-
-[additive regression mode](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.location)
+The two main regression modes are [multiplicative regression](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.regression)
+and [additive regression mode](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.location).
+Topology-wise, the first resembles [Poisson regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.PoissonRegressor.html),
+i.e., a Generalized Linear model with a log link function, covering the target
+range $[0, \infty]$ and supporting multiplicative dependencies, while the
+latter is similar to linear regression, covering the target range
+$[-\infty, \infty]$ and supporting additive dependencies. It should be noted
+though that, in contrast to Generalized Linear Models, Cyclic Boosting in
+either mode enables highly non-linear models, similar to
+[Generalized Additive Models](https://en.wikipedia.org/wiki/Generalized_additive_model).
 
 Classification
 --------------
 
-...
-[classification mode](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.classification)
+The [classification mode](https://cyclic-boosting.readthedocs.io/en/latest/cyclic_boosting.html#module-cyclic_boosting.classification)
+resembles logistic regression (Generalized Linear Model with logit link) and
+predicts probabilities, i.e., covering the target range $[0, 1]$. It supports
+multiplicative dependencies between features and target odds.
 
 The Story behind Cyclic Boosting
 --------------------------------
 
 The idea of many of the building blocks of Cyclic Boosting, e.g., binning and
 smoothing, originated from an algorithm called NeuroBayes, a feed-forward
 neural network with lots of pre-processing steps, developed by Professor
@@ -76,8 +90,9 @@
 coupon sending only affects a small portion of customers and the bulk of
 unaffected customers needs to be statistically removed to identify causal
 effects.
 
 There is a bunch of people who contributed to the development of the Cyclic
 Boosting library over the years. Without guarantee of completeness, here is a
 list in alphabetic order: Bruno Daniel, Michael Feindt, Martin Hahn, Uwe Korn,
-Holger Peters, Thomas Pfaff, Jörg Rittinger, Daniel Stemmer, Felix Wick
+Holger Peters, Thomas Pfaff, Jörg Rittinger, Daniel Stemmer, Felix Wick, Moritz
+Wolf
```

### Comparing `cyclic-boosting-0.0.4/setup.py` & `cyclic-boosting-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/integration_test_data.csv` & `cyclic-boosting-0.0.5/tests/integration_test_data.csv`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_binary_search.py` & `cyclic-boosting-0.0.5/tests/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_integration.py` & `cyclic-boosting-0.0.5/tests/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,49 @@
 
     yhat = CB_est.predict(X.copy())
 
     mad = np.nanmean(np.abs(y - yhat))
     np.testing.assert_almost_equal(mad, 1.7185, 3)
 
 
+def test_poisson_regression_default_features_and_properties():
+    np.random.seed(42)
+
+    df = pd.read_csv("./tests/integration_test_data.csv")
+
+    X, y = prepare_data(df)
+    X = X[[
+        'dayofweek',
+        'L_ID',
+        'PG_ID_3',
+        'P_ID',
+        'PROMOTION_TYPE',
+        'price_ratio',
+        'dayofyear'
+    ]]
+
+    plobs = [
+        observers.PlottingObserver(iteration=1),
+        observers.PlottingObserver(iteration=-1),
+    ]
+    CB_est = pipeline_CBPoissonRegressor(
+        observers=plobs,
+    )
+    CB_est.fit(X.copy(), y)
+    # plot_CB('analysis_CB_iterfirst',
+    #         [CB_est[-1].observers[0]], CB_est[-2])
+    # plot_CB('analysis_CB_iterlast',
+    #         [CB_est[-1].observers[-1]], CB_est[-2])
+
+    yhat = CB_est.predict(X.copy())
+
+    mad = np.nanmean(np.abs(y - yhat))
+    np.testing.assert_almost_equal(mad, 1.6982, 3)
+
+
 def test_poisson_regression_default_features_notaggregated():
     np.random.seed(42)
 
     df = pd.read_csv("./tests/integration_test_data.csv")
 
     X, y = prepare_data(df)
     X = X[[
```

### Comparing `cyclic-boosting-0.0.4/tests/test_learning_rate.py` & `cyclic-boosting-0.0.5/tests/test_learning_rate.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_link.py` & `cyclic-boosting-0.0.5/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_plots.py` & `cyclic-boosting-0.0.5/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_smoothing_base.py` & `cyclic-boosting-0.0.5/tests/test_smoothing_base.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_smoothing_multidim.py` & `cyclic-boosting-0.0.5/tests/test_smoothing_multidim.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_smoothing_onedim.py` & `cyclic-boosting-0.0.5/tests/test_smoothing_onedim.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_smoothing_ortho.py` & `cyclic-boosting-0.0.5/tests/test_smoothing_ortho.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.4/tests/test_utils.py` & `cyclic-boosting-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

