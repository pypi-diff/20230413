# Comparing `tmp/cyclic-boosting-0.0.5.tar.gz` & `tmp/cyclic_boosting-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclic-boosting-0.0.5.tar", last modified: Thu Apr 13 11:01:53 2023, max compression
+gzip compressed data, was "cyclic_boosting-0.1.0.tar", max compression
```

## Comparing `cyclic-boosting-0.0.5.tar` & `cyclic_boosting-0.1.0.tar`

### file list

```diff
@@ -1,87 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.104747 cyclic-boosting-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.108747 cyclic-boosting-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting/
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/GBSregression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45795 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting/binning/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/bin_number_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/binning/ecdf_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/common_smoothers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/nbinom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.120747 cyclic-boosting-0.0.5/cyclic_boosting/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/_1dplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/_2dplots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.120747 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/extrapolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/meta_smoother.py
--rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/multidim.py
--rw-r--r--   0 runner    (1001) docker     (123)    26512 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/onedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/smoothing/orthofit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30604 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/cyclic_boosting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.116747 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:01:53.000000 cyclic-boosting-0.0.5/cyclic_boosting.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.124748 cyclic-boosting-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.128748 cyclic-boosting-0.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.binning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/cyclic_boosting.smoothing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:01:53.132748 cyclic-boosting-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)  2526940 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/integration_test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_multidim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_onedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_smoothing_ortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 11:01:39.000000 cyclic-boosting-0.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0    14197 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1268 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/README.md
+-rw-r--r--   0        0        0     3489 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/GBSregression.py
+-rw-r--r--   0        0        0     1943 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/__init__.py
+-rw-r--r--   0        0        0    44776 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/base.py
+-rw-r--r--   0        0        0      719 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/__init__.py
+-rw-r--r--   0        0        0    10628 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/_binary_search.py
+-rw-r--r--   0        0        0     2953 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/_utils.py
+-rw-r--r--   0        0        0     8282 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/bin_number_transformer.py
+-rw-r--r--   0        0        0    19266 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/ecdf_transformer.py
+-rw-r--r--   0        0        0     4896 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/classification.py
+-rw-r--r--   0        0        0    12955 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/common_smoothers.py
+-rw-r--r--   0        0        0    11607 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/features.py
+-rw-r--r--   0        0        0    13132 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/flags.py
+-rw-r--r--   0        0        0     2308 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/learning_rate.py
+-rw-r--r--   0        0        0     2383 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/link.py
+-rw-r--r--   0        0        0     8943 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/location.py
+-rw-r--r--   0        0        0     8331 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/nbinom.py
+-rw-r--r--   0        0        0     6831 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/observers.py
+-rw-r--r--   0        0        0     6108 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/pipelines.py
+-rw-r--r--   0        0        0    11070 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/_1dplots.py
+-rw-r--r--   0        0        0     7517 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/_2dplots.py
+-rw-r--r--   0        0        0    10899 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/__init__.py
+-rw-r--r--   0        0        0     7497 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/plot_utils.py
+-rw-r--r--   0        0        0    15702 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/price.py
+-rw-r--r--   0        0        0     6953 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/regression.py
+-rw-r--r--   0        0        0      529 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/base.py
+-rw-r--r--   0        0        0     4737 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/extrapolate.py
+-rw-r--r--   0        0        0    10724 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/meta_smoother.py
+-rw-r--r--   0        0        0    14258 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/multidim.py
+-rw-r--r--   0        0        0    26024 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/onedim.py
+-rw-r--r--   0        0        0     4940 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/orthofit.py
+-rw-r--r--   0        0        0    30546 2023-04-13 16:16:00.147156 cyclic_boosting-0.1.0/cyclic_boosting/utils.py
+-rw-r--r--   0        0        0     1394 2023-04-13 16:16:00.147156 cyclic_boosting-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 cyclic_boosting-0.1.0/PKG-INFO
```

### Comparing `cyclic-boosting-0.0.5/LICENSE` & `cyclic_boosting-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.5/PKG-INFO` & `cyclic_boosting-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: cyclic-boosting
-Version: 0.0.5
-Author: Blue Yonder GmbH
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
 
 ## Documentation
 
 The documentation can be found [here](https://cyclic-boosting.readthedocs.io/en/latest/).
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/GBSregression.py` & `cyclic_boosting-0.1.0/cyclic_boosting/GBSregression.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         observers=None,
         smoother_choice=None,
         output_column=None,
         learn_rate=None,
         regalpha=0.0,
         aggregate=True,
     ):
-
         CyclicBoostingBase.__init__(
             self,
             feature_groups=feature_groups,
             feature_properties=feature_properties,
             weight_column=weight_column,
             minimal_loss_change=minimal_loss_change,
             minimal_factor_change=minimal_factor_change,
@@ -80,20 +79,18 @@
         sum_nd = np.bincount(lex_binnumbers, weights=n * d, minlength=minlength)
 
         sum_n2 = np.bincount(lex_binnumbers, weights=n * n, minlength=minlength)
 
         sum_d2 = np.bincount(lex_binnumbers, weights=d * d, minlength=minlength)
 
         sum_d += 1
-        sum_d2 += 1 ** 2
+        sum_d2 += 1**2
 
         summand = sum_n / sum_d
-        variance_summand = (
-            sum_d ** 2 * sum_n2 - 2.0 * sum_n * sum_d * sum_nd + sum_n ** 2 * sum_d2
-        ) / sum_d ** 4
+        variance_summand = (sum_d**2 * sum_n2 - 2.0 * sum_n * sum_d * sum_nd + sum_n**2 * sum_d2) / sum_d**4
 
         return summand, np.sqrt(variance_summand)
 
     def _check_y(self, y):
         pass
 
     def _init_global_scale(self, X, y):
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/__init__.py` & `cyclic_boosting-0.1.0/cyclic_boosting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,35 @@
 Background Subtraction
 
 - :class:`~.CBGBSRegressor`
 """
 
 from __future__ import division, print_function
 
+
 from cyclic_boosting.base import CyclicBoostingBase
 from cyclic_boosting.regression import CBNBinomRegressor, CBPoissonRegressor
 from cyclic_boosting.price import CBExponential
 from cyclic_boosting.location import CBLocationRegressor, CBLocPoissonRegressor
 from cyclic_boosting.nbinom import CBNBinomC
 from cyclic_boosting.classification import CBClassifier
 from cyclic_boosting.GBSregression import CBGBSRegressor
-from cyclic_boosting.pipelines import pipeline_CBPoissonRegressor, pipeline_CBNBinomRegressor, \
-        pipeline_CBClassifier, pipeline_CBLocationRegressor, pipeline_CBExponential, \
-        pipeline_CBLocPoissonRegressor, pipeline_CBNBinomC, pipeline_CBGBSRegressor
+from cyclic_boosting.pipelines import (
+    pipeline_CBPoissonRegressor,
+    pipeline_CBNBinomRegressor,
+    pipeline_CBClassifier,
+    pipeline_CBLocationRegressor,
+    pipeline_CBExponential,
+    pipeline_CBLocPoissonRegressor,
+    pipeline_CBNBinomC,
+    pipeline_CBGBSRegressor,
+)
 
 __all__ = [
+    "CyclicBoostingBase",
     "CBPoissonRegressor",
     "CBNBinomRegressor",
     "CBExponential",
     "CBLocationRegressor",
     "CBLocPoissonRegressor",
     "CBNBinomC",
     "CBClassifier",
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/base.py` & `cyclic_boosting-0.1.0/cyclic_boosting/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,15 @@
         return np.repeat(0.0, len(X))
 
 
 def predict_factors(feature, X_for_smoother, neutral_factor):
     prediction_smoother = utils.nans(len(X_for_smoother))
     isfinite_all = utils.slice_finite_semi_positive(X_for_smoother)
     if isfinite_all.any() and (feature.smoother is not None):
-        prediction_smoother[
-            isfinite_all
-        ] = feature.learn_rate * feature.smoother.predict(X_for_smoother[isfinite_all])
+        prediction_smoother[isfinite_all] = feature.learn_rate * feature.smoother.predict(X_for_smoother[isfinite_all])
 
     prediction_smoother[~isfinite_all] = feature.factors_link[-1]
     prediction_smoother[~np.isfinite(prediction_smoother)] = neutral_factor
 
     return prediction_smoother
 
 
@@ -49,18 +47,15 @@
 
     Parameters
     ----------
 
     features: :class:`~cyclic_boosting.base.FeatureList`
         Collection of all features.
     """
-    mean_factor_devs = [
-        np.mean(np.abs(feature.factors_link - feature.factors_link_old))
-        for feature in features
-    ]
+    mean_factor_devs = [np.mean(np.abs(feature.factors_link - feature.factors_link_old)) for feature in features]
     return np.mean(mean_factor_devs)
 
 
 @six.add_metaclass(abc.ABCMeta)
 class CyclicBoostingBase(
     link.LinkFunction,
     sklearnb.BaseEstimator,
@@ -224,17 +219,15 @@
             self.learn_rate = learn_rate
         self._init_features()
 
     def loss(self, prediction, y, weights):
         if not len(y) > 0:
             raise ValueError("Loss cannot be computed on empty data")
         else:
-            sum_weighted_error = numexpr.evaluate(
-                "sum((prediction - y) * (prediction - y) * weights)"
-            )
+            sum_weighted_error = numexpr.evaluate("sum((prediction - y) * (prediction - y) * weights)")
             sum_weights = numexpr.evaluate("sum(weights)")
             return sum_weighted_error / sum_weights
 
     @property
     def global_scale_(self):
         """
         Obtain the global scale in the space of the original target ``y``.
@@ -283,53 +276,45 @@
         """
         exclude_columns = []
         if self.prior_prediction_column is not None:
             exclude_columns.append(self.prior_prediction_column)
         if self.weight_column is not None:
             exclude_columns.append(self.weight_column)
 
-        self.feature_groups = utils.get_feature_column_names(
-            X, exclude_columns=exclude_columns
-        )
+        self.feature_groups = utils.get_feature_column_names(X, exclude_columns=exclude_columns)
 
     def _init_global_scale(self, X, y):
         """
         Initializes the ``global_scale_link_`` and the
         ``prior_pred_link_offset_``. The ``global_scale_link_`` is set to the
         weighted mean of the target ``y`` transformed into the link space.
         The ``prior_pred_link_offset_`` is the difference between the
         ``global_scale_link_`` and the weighted mean of the prior prediction
         transformed to the link space.
         """
         if self.weights is None:
             raise RuntimeError("The weights have to be initialized.")
         minimal_prediction = 0.001
-        self.global_scale_link_ = self.link_func(
-            np.sum(y * self.weights) / np.sum(self.weights) + minimal_prediction
-        )
+        self.global_scale_link_ = self.link_func(np.sum(y * self.weights) / np.sum(self.weights) + minimal_prediction)
         if self.prior_prediction_column is not None:
             prior_pred = utils.get_X_column(X, self.prior_prediction_column)
             finite = np.isfinite(prior_pred)
             if not np.all(finite):
                 _logger.warning(
                     "Found a total number of {} non-finite values in the prior prediction column".format(
                         np.sum(~finite)
                     )
                 )
 
-            prior_pred_mean = np.sum(
-                prior_pred[finite] * self.weights[finite]
-            ) / np.sum(self.weights[finite])
+            prior_pred_mean = np.sum(prior_pred[finite] * self.weights[finite]) / np.sum(self.weights[finite])
 
             prior_pred_link_mean = self.link_func(prior_pred_mean)
 
             if np.isfinite(prior_pred_link_mean):
-                self.prior_pred_link_offset_ = (
-                    self.global_scale_link_ - prior_pred_link_mean
-                )
+                self.prior_pred_link_offset_ = self.global_scale_link_ - prior_pred_link_mean
             else:
                 warnings.warn(
                     "The mean prior prediction in link-space is not finite. "
                     "Therefore no indiviualization is done "
                     "and no prior mean substraction is necessary."
                 )
                 self.prior_pred_link_offset_ = float(self.global_scale_link_)
@@ -339,26 +324,22 @@
             raise RuntimeError("The weights have to be initialized.")
 
     def _init_features(self):
         """
         Initializes the ``features`` and binds the data belonging to a feature
         to it.
         """
-        self.features = create_features(
-            self.feature_groups, self.feature_properties, self.smoother_choice
-        )
+        self.features = create_features(self.feature_groups, self.feature_properties, self.smoother_choice)
 
     def _get_prior_predictions(self, X):
         if self.prior_prediction_column is None:
             prior_prediction_link = np.repeat(self.global_scale_link_, X.shape[0])
         else:
             prior_pred = utils.get_X_column(X, self.prior_prediction_column)
-            prior_prediction_link = (
-                self.link_func(prior_pred) + self.prior_pred_link_offset_
-            )
+            prior_prediction_link = self.link_func(prior_pred) + self.prior_pred_link_offset_
             finite = np.isfinite(prior_prediction_link)
             prior_prediction_link[~finite] = self.global_scale_link_
 
         return prior_prediction_link
 
     def _feature_contribution(self, feature, contribution):
         """The contribution of a feature group to the full model in link space.
@@ -384,23 +365,20 @@
         """
         return contribution
 
     def is_diverged(self, loss):
         return loss > self.initial_loss_ * 2
 
     def _check_convergence(self):
-
         msg = (
             "Your cyclic boosting training seems to be "
             "diverging. In the {0}. iteration the "
             "current loss: {1}, is greater "
             "than the trivial loss with just mean "
-            "predictions: {2}.".format(
-                self.iteration_ + 1, self.insample_loss_, self.initial_loss_
-            )
+            "predictions: {2}.".format(self.iteration_ + 1, self.insample_loss_, self.initial_loss_)
         )
 
         if self.is_diverged(self.insample_loss_):
             self.is_diverging = True
             self.diverging += 1
             warnings.warn(msg)
             if self.diverging >= 5:
@@ -434,23 +412,19 @@
                     loss_change=loss_change,
                     deviation=deviation,
                 )
             )
 
     def _call_observe_feature_iterations(self, iteration, i, X, y, prediction):
         for observer in self.observers:
-            observer.observe_feature_iterations(
-                iteration, i, X, y, prediction, self.weights, self.get_state()
-            )
+            observer.observe_feature_iterations(iteration, i, X, y, prediction, self.weights, self.get_state())
 
     def _call_observe_iterations(self, iteration, X, y, prediction, delta):
         for observer in self.observers:
-            observer.observe_iterations(
-                iteration, X, y, prediction, self.weights, self.get_state(), delta
-            )
+            observer.observe_iterations(iteration, X, y, prediction, self.weights, self.get_state(), delta)
 
     def get_state(self):
         return {
             "link_function": self,
             "features": self.features,
             "globale_scale": self.global_scale_,
             "insample_loss": self.insample_loss_,
@@ -468,17 +442,15 @@
             feature.fitted_aggregated -= feature.factors_link
             feature.unbind_data()
 
     def visit_factors(self, feature, unfitted_factors, X, y, pred):
         clip = isinstance(self, LogLinkMixin)
         if clip and self.aggregate:
             # Maximal/Minimal updates
-            feature.factors_link = np.clip(
-                feature.factors_link, np.log(0.5), np.log(2), out=feature.factors_link
-            )
+            feature.factors_link = np.clip(feature.factors_link, np.log(0.5), np.log(2), out=feature.factors_link)
 
             # Absolute size of factors/exponents per feature
             if feature.is_fitted:
                 if feature.feature_type is not None:
                     if len(feature.feature_group) == 1:
                         min_f = 0.05
                         max_f = 20
@@ -514,17 +486,15 @@
                         msg = "Feature factors for {} will be ignored due to diverging loss".format(
                             feature.feature_group
                         )
                         warnings.warn(msg)
                         feature.factors_link = -feature.fitted_aggregated
                         feature.smoother = ZeroSmoother()
                 elif check_diverged():
-                    msg = "Feature factors for {} will be clipped due to diverging loss".format(
-                        feature.feature_group
-                    )
+                    msg = "Feature factors for {} will be clipped due to diverging loss".format(feature.feature_group)
                     warnings.warn(msg)
                     np.clip(
                         feature.factors_link,
                         unfitted_factors + np.log(0.8),
                         unfitted_factors + np.log(1.2),
                         out=feature.factors_link,
                     )
@@ -539,17 +509,15 @@
             feature.is_fitted = True
 
     def feature_iteration(self, X, y, feature, pred, prefit_data):
         if not self.aggregate:
             feature_predictions = self._pred_feature(X, feature, True)
             pred.remove_predictions(feature_predictions, feature)
 
-        factors_link, uncertainties_link = self.calc_parameters(
-            feature, y, pred, prefit_data=prefit_data
-        )
+        factors_link, uncertainties_link = self.calc_parameters(feature, y, pred, prefit_data=prefit_data)
 
         X_for_smoother = feature.update_factors(
             factors_link.copy(),
             uncertainties_link,
             self.neutral_factor_link,
             self.learning_rate(feature),
         )
@@ -572,17 +540,15 @@
         for i, feature in enumerate(self.features):
             if feature.feature_type is None:
                 weights = self.weights
             else:
                 weights = self.weights_external
             if self.iteration_ == 0:
                 feature.bind_data(X, weights, True)
-                feature.factors_link = (
-                    np.ones(feature.n_bins) * self.neutral_factor_link
-                )
+                feature.factors_link = np.ones(feature.n_bins) * self.neutral_factor_link
                 if prefit_data is not None:
                     prefit_data[i] = self.precalc_parameters(feature, y, pred)
             else:
                 feature.bind_data(X, weights, False)
             yield i, feature, prefit_data[i]
             feature.unbind_data()
 
@@ -615,25 +581,21 @@
         self.initial_loss_ = self.insample_loss_
         self.initial_msd_ = self.insample_loss_
         loss_change = 1e20
         delta = 100.0
 
         self.iteration_ = 0
 
-        while (
-            not self._check_stop_criteria(self.iteration_, delta, loss_change)
-        ) or self.is_diverging:
+        while (not self._check_stop_criteria(self.iteration_, delta, loss_change)) or self.is_diverging:
             self._call_observe_iterations(self.iteration_, X, y, prediction, delta)
 
             self._log_iteration_info(delta, loss_change)
             for i, feature, pf_data in self.cb_features(X, y, pred, prefit_data):
                 pred = self.feature_iteration(X, y, feature, pred, pf_data)
-                self._call_observe_feature_iterations(
-                    self.iteration_, i, X, y, prediction
-                )
+                self._call_observe_feature_iterations(self.iteration_, i, X, y, prediction)
                 if feature.factor_sum is None:
                     feature.factor_sum = [np.sum(np.abs(feature.fitted_aggregated))]
                 else:
                     feature.factor_sum.append(np.sum(np.abs(feature.fitted_aggregated)))
             prediction = self.unlink_func(pred.predict_link())
             loss_change = self._update_loss(prediction, y)
             delta = factors_deviation(self.features)
@@ -652,17 +614,15 @@
 
         if len(self.observers) > 0:
             self.prepare_plots(X, y, prediction)
 
         self._call_observe_iterations(-1, X, y, prediction, delta)
         self._check_convergence()
 
-        _logger.info(
-            "Cyclic Boosting, final global scale {}".format(self.global_scale_)
-        )
+        _logger.info("Cyclic Boosting, final global scale {}".format(self.global_scale_))
 
         for feature in self.features:
             feature.factors_link = feature.fitted_aggregated
             feature.unbind_data()
             if len(self.observers) == 0:
                 feature.bin_weightsums = None
             feature.unbind_factor_data()
@@ -671,20 +631,16 @@
     def prepare_plots(self, X, y, prediction):
         for feature in self.features:
             if feature.feature_type is None:
                 weights = self.weights
             else:
                 weights = self.weights_external
             feature.bind_data(X, weights, True)
-            sum_w = np.bincount(
-                feature.lex_binned_data, weights=weights, minlength=feature.n_bins
-            )
-            sum_yw = np.bincount(
-                feature.lex_binned_data, weights=weights * y, minlength=feature.n_bins
-            )
+            sum_w = np.bincount(feature.lex_binned_data, weights=weights, minlength=feature.n_bins)
+            sum_yw = np.bincount(feature.lex_binned_data, weights=weights * y, minlength=feature.n_bins)
             mean_target_binned = (sum_yw + 1) / (sum_w + 1)
             sum_pw = np.bincount(
                 feature.lex_binned_data,
                 weights=weights * prediction,
                 minlength=feature.n_bins,
             )
             if feature.n_bins > 1:
@@ -697,21 +653,17 @@
             mean_prediction_binned = (sum_pw + 1) / (sum_w + 1)
             feature.unbind_data()
             if isinstance(self, IdentityLinkMixin):
                 feature.mean_dev = mean_prediction_binned - mean_target_binned
                 feature.y = mean_target_binned - mean_y_finite
                 feature.prediction = mean_prediction_binned - mean_prediction_finite
             else:
-                feature.mean_dev = np.log(mean_prediction_binned + 1e-12) - np.log(
-                    mean_target_binned + 1e-12
-                )
+                feature.mean_dev = np.log(mean_prediction_binned + 1e-12) - np.log(mean_target_binned + 1e-12)
                 feature.y = np.log(mean_target_binned / mean_y_finite + 1e-12)
-                feature.prediction = np.log(
-                    mean_prediction_binned / mean_y_finite + 1e-12
-                )
+                feature.prediction = np.log(mean_prediction_binned / mean_y_finite + 1e-12)
             feature.y_finite = mean_y_finite
             feature.p_finite = mean_prediction_finite
 
             feature.learn_rate = 1.0
 
     def _fit_predict(self, X, y=None, fit_mode=0):
         """Fit the estimator to the training samples.
@@ -726,17 +678,15 @@
 
         return prediction
 
     def _pred_feature(self, X, feature, is_fit):
         if is_fit:
             return feature.factors_link[feature.lex_binned_data]
         else:
-            X_for_predict = utils.get_X_column(
-                X, feature.feature_group, array_for_1_dim=False
-            )
+            X_for_predict = utils.get_X_column(X, feature.feature_group, array_for_1_dim=False)
             pred = predict_factors(feature, X_for_predict, self.neutral_factor_link)
             return pred
 
     def predict(self, X, y=None, fit_mode=0, actions=None):
         pred = self.predict_extended(X, None)
         return self.unlink_func(pred.predict_link())
 
@@ -754,39 +704,31 @@
         return pred
 
     def fit_transform(self, X, y=None, fit_mode=0):
         if not self.output_column:
             raise KeyError("output_column not defined")
         try:
             if self.output_column in X.columns:
-                raise KeyError(
-                    """output_column "{}" exists already""".format(self.output_column)
-                )
+                raise KeyError("""output_column "{}" exists already""".format(self.output_column))
         except AttributeError:
-            raise TypeError(
-                "data needs to be a dataframe for the usage as a fit_transformer"
-            )
+            raise TypeError("data needs to be a dataframe for the usage as a fit_transformer")
         if fit_mode != 1:
             X[self.output_column] = self._fit_predict(X, y, fit_mode)
         else:
             X[self.output_column] = self.predict(X=X, y=y, fit_mode=fit_mode)
         return X
 
     def transform(self, X, y=None, fit_mode=0):
         if not self.output_column:
             raise KeyError("output_column not defined")
         try:
             if self.output_column in X.columns:
-                raise KeyError(
-                    """output_column "{}" exists already""".format(self.output_column)
-                )
+                raise KeyError("""output_column "{}" exists already""".format(self.output_column))
         except AttributeError:
-            raise TypeError(
-                "data needs to be a dataframe for the usage as a transformer"
-            )
+            raise TypeError("data needs to be a dataframe for the usage as a transformer")
         X[self.output_column] = self.predict(X=X, y=y, fit_mode=fit_mode)
         return X
 
     def _check_stop_criteria(self, iterations, delta, loss_change):
         """
         Checks the stop criteria and returns True if none are satisfied.
 
@@ -814,17 +756,15 @@
             )
             stop_factor_change = True
 
         if abs(loss_change) <= self.minimal_loss_change:
             _logger.info(
                 "Cyclic Boosting stopped because the change of "
                 "the loss {0} was lower "
-                "than the required minimum {1}.".format(
-                    loss_change, self.minimal_loss_change
-                )
+                "than the required minimum {1}.".format(loss_change, self.minimal_loss_change)
             )
             stop_loss_change = True
 
         if loss_change < 0:
             _logger.warning(
                 "Encountered negative change of loss. "
                 "This might not be a problem, as long as the "
@@ -850,16 +790,15 @@
             raise ValueError("Estimator should be applied on non-empty data")
 
     def _check_y(self, y):
         """Check that y has the correct values. Has to be
         implemented by the child class.
         """
         raise NotImplementedError(
-            "You have to implement the function _check_y"
-            " to ensure your target has correct values."
+            "You have to implement the function _check_y" " to ensure your target has correct values."
         )
 
     def get_subestimators_as_items(self, prototypes=True):
         """
         For prototypes=False, the clones are indexed by the column name
         or index.
         """
@@ -1031,17 +970,15 @@
 
     sigma = (quant1_link - quant2_link) / (a1 - a2)
     mu = quant1_link - sigma * a1
 
     return mu, sigma
 
 
-def calc_factors_generic(
-    lex_binnumbers, w_x, w, w_x2, external_weights, minlength, x0, w0
-):
+def calc_factors_generic(lex_binnumbers, w_x, w, w_x2, external_weights, minlength, x0, w0):
     r"""Generic calculation of factors and uncertainties
 
     It is always possible to reparametrise :math:`\chi^2`
     of the different cyclic boosting models to the following standard form
 
     .. math::
         \chi^2 =\sum_i w_i \cdot (x_i - \hat{x})^2
@@ -1205,27 +1142,25 @@
         A tuple of ``factors`` and ``uncertainties``
         in the original space.
     """
     sum_w_x = np.bincount(lex_binnumbers, weights=w_x, minlength=minlength)
 
     sum_w = np.bincount(lex_binnumbers, weights=w, minlength=minlength)
 
-    sum_vw = np.bincount(
-        lex_binnumbers, weights=external_weights * w, minlength=minlength
-    )
+    sum_vw = np.bincount(lex_binnumbers, weights=external_weights * w, minlength=minlength)
 
     sum_w_x2 = np.bincount(lex_binnumbers, weights=w_x2, minlength=minlength)
 
     sum_w_x += w0 * x0
     sum_w += w0
-    sum_w_x2 += w0 * x0 ** 2
+    sum_w_x2 += w0 * x0**2
     sum_vw += w0
 
     weighted_mean = sum_w_x / sum_w
-    variance_weighted_mean = sum_vw / sum_w ** 2
+    variance_weighted_mean = sum_vw / sum_w**2
 
     return weighted_mean, np.sqrt(variance_weighted_mean)
 
 
 class UpdateMixin(object):
     def include_price_contrib(self, pred):
         self.df["exponents"] += pred
@@ -1250,25 +1185,21 @@
             else:
                 self.df[influence_category] = pred
 
     def update_predictions(self, pred, feature, influence_categories=None):
         if feature.feature_type == FeatureTypes.external:
             self.include_price_contrib(pred)
         else:
-            self.include_factor_contrib(
-                pred, get_influence_category(feature, influence_categories)
-            )
+            self.include_factor_contrib(pred, get_influence_category(feature, influence_categories))
 
     def remove_predictions(self, pred, feature, influence_categories=None):
         if feature.feature_type == FeatureTypes.external:
             self.remove_price_contrib(pred)
         else:
-            self.remove_factor_contrib(
-                pred, get_influence_category(feature, influence_categories)
-            )
+            self.remove_factor_contrib(pred, get_influence_category(feature, influence_categories))
 
 
 class CBLinkPredictionsFactors(UpdateMixin):
     """Support for prediction of type log(p) = factors"""
 
     def __init__(self, predictions):
         self.df = pd.DataFrame({"factors": predictions})
@@ -1287,17 +1218,15 @@
         if (
             influence_category is None
         ):  # this is due to the flaws in create features, i would propose to only allow tuple
             if len(feature.feature_group) == 1:
                 fg = feature.feature_group[0]
                 influence_category = influence_categories.get(fg, None)
         if influence_category is None:
-            raise KeyError(
-                f"Please add {feature.feature_group} to influence_categories"
-            )
+            raise KeyError(f"Please add {feature.feature_group} to influence_categories")
     return influence_category
 
 
 __all__ = [
     "factors_deviation",
     "CyclicBoostingBase",
     "gaussian_matching_by_quantiles",
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/binning/__init__.py` & `cyclic_boosting-0.1.0/cyclic_boosting/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/binning/_binary_search.py` & `cyclic_boosting-0.1.0/cyclic_boosting/binning/_binary_search.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/binning/_utils.py` & `cyclic_boosting-0.1.0/cyclic_boosting/binning/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     if feature_properties is None:
         return flags.IS_CONTINUOUS
     else:
         try:
             fprop = feature_properties[col]
             flags.check_flags_consistency(fprop)
         except KeyError:
-            _logger.warning(
-                "Column '%s' not found in " "feature_properties dict." % col
-            )
+            _logger.warning("Column '%s' not found in " "feature_properties dict." % col)
             fprop = None
         return fprop
 
 
 def minimal_difference(values):
     """Minimal difference of consecutive array values
     excluding zero differences.
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/binning/bin_number_transformer.py` & `cyclic_boosting-0.1.0/cyclic_boosting/binning/bin_number_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,15 @@
 
         for col, epsilon, bins_and_cdfs in self.bins_and_cdfs_:
             feature_prop = _read_feature_property(col, self.feature_properties)
 
             if feature_prop is None:
                 pass
             else:
-                xt = self._transform_one_feature(
-                    X, feature_prop, col, epsilon, bins_and_cdfs
-                )
+                xt = self._transform_one_feature(X, feature_prop, col, epsilon, bins_and_cdfs)
                 column_setter(X, col, xt)
 
         if not isinstance(X, pd.DataFrame) and n_transformed_features == X.shape[1]:
             X = _as_int_array_of_minimum_dtype(X)
         return X
 
     def get_feature_bin_boundaries(self):
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/binning/ecdf_transformer.py` & `cyclic_boosting-0.1.0/cyclic_boosting/binning/ecdf_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,39 +206,33 @@
     def fit(self, X, y=None, fit_mode=0):
         self._nbins_per_feature = self._normalize_bins(self.n_bins)
         self.bins_and_cdfs_ = []
 
         if check_frame_empty(X):
             raise ValueError("Your input matrix for the binning is empty.")
 
-        feature_columns = get_feature_column_names_or_indices(
-            X, exclude_columns=[self.weight_column]
-        )
+        feature_columns = get_feature_column_names_or_indices(X, exclude_columns=[self.weight_column])
         weights = get_weight_column(X, self.weight_column)
 
         for col in feature_columns:
             _logger.info("{0} column: {1}".format(self.__class__.__name__, col))
             x_col = get_X_column(X, col)
 
             feature_prop = _read_feature_property(col, self.feature_properties)
 
             if feature_prop is None:
                 continue
 
-            bins_x, cdf_x, _wsum, _n_nan = calculate_cdf_from_weighted_data(
-                x_col.astype(float), weights
-            )
+            bins_x, cdf_x, _wsum, _n_nan = calculate_cdf_from_weighted_data(x_col.astype(float), weights)
 
             if len(bins_x) == 0 or len(cdf_x) == 0:
                 self.bins_and_cdfs_.append((col, self.epsilon, None))
                 continue
 
-            if flags.is_ordered_set(feature_prop) or flags.is_unordered_set(
-                feature_prop
-            ):
+            if flags.is_ordered_set(feature_prop) or flags.is_unordered_set(feature_prop):
                 bin_boundaries = np.r_[bins_x[0], bins_x]
                 cdf = np.r_[0.0, cdf_x]
             else:
                 bin_boundaries, cdf = reduce_cdf_and_boundaries_to_nbins(
                     bins_x,
                     cdf_x,
                     self._nbins_per_feature[col],
@@ -256,17 +250,15 @@
             self.bins_and_cdfs_.append((col, epsilon, bins_and_cdfs))
         return self
 
     def _check_input_for_transform(self, X):
         if self.bins_and_cdfs_ is None:
             raise RuntimeError("Fit was not called before.")
 
-        columns = get_feature_column_names_or_indices(
-            X, exclude_columns=[self.weight_column]
-        )
+        columns = get_feature_column_names_or_indices(X, exclude_columns=[self.weight_column])
         if self.feature_properties is not None:
             columns = [col for col in columns if col in self.feature_properties]
         n_cols = len(columns)
         if n_cols != len(self.bins_and_cdfs_):
             raise ValueError(
                 "Input Matrix X has not the same number"
                 " of feature columns (%s) as "
@@ -395,26 +387,20 @@
     array([ 1.,  0.])
     """
     if weight_column is not None:
         if isinstance(X, pd.DataFrame):
             try:
                 return np.asarray(X[weight_column])
             except:
-                raise ValueError(
-                    "Weight column {} not found in X.".format(str(weight_column))
-                )
+                raise ValueError("Weight column {} not found in X.".format(str(weight_column)))
         else:
             try:
                 return X[:, weight_column]
             except:
-                raise ValueError(
-                    "Index {} defining weight column not found in X.".format(
-                        str(weight_column)
-                    )
-                )
+                raise ValueError("Index {} defining weight column not found in X.".format(str(weight_column)))
     else:
         return np.ones(X.shape[0], dtype=np.float64)
 
 
 def reduce_cdf_and_boundaries_to_nbins(bins_x, cdf_x, n_bins, epsilon, tolerance):
     """
     Section the cdf spectrum into `n_bin` parts of equal statistics, and find
@@ -567,15 +553,13 @@
 
     n_nan = np.count_nonzero(np.isnan(z))
     z_unique = np.unique(z[~np.isnan(z)])
 
     wsum = np.nansum(w[~np.isnan(z)])
 
     # Accumulate the weights for the unique values.
-    uniques = (
-        pd.DataFrame({"z": z, "w": w}).groupby(["z"]).agg({"w": "sum"}).reset_index()
-    )
+    uniques = pd.DataFrame({"z": z, "w": w}).groupby(["z"]).agg({"w": "sum"}).reset_index()
     uniques = uniques.loc[uniques["w"] != 0]
 
     cdf = np.nancumsum(uniques["w"]) / wsum
 
     return z_unique, cdf, wsum, n_nan
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/classification.py` & `cyclic_boosting-0.1.0/cyclic_boosting/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,30 +50,27 @@
     """
     epsilon = 1e-12
     prediction = np.where(prediction == 0.0, epsilon, prediction)
     prediction = np.where(prediction == 1.0, 1 - epsilon, prediction)
     return np.where(y, 1 - prediction, prediction)
 
 
-class CBClassifier(
-    sklearn.base.ClassifierMixin, CyclicBoostingBase, LogitLinkMixin
-):
+class CBClassifier(sklearn.base.ClassifierMixin, CyclicBoostingBase, LogitLinkMixin):
     """This regressor is the cyclic boosting core algorithm for classifications
 
     Its interface, methods and arguments are described in
     :class:`~CyclicBoostingBase`.
     """
+
     def _check_y(self, y):
         """Check that y has only values 0 or 1"""
         if not ((y == 0.0) | (y == 1.0)).all():
             raise ValueError(
                 "The target y must be either 0 or 1 "
-                "and not NAN. y[(y != 0) & (y != 1)] = {0}".format(
-                    y[(y != 0) & (y != 1)]
-                )
+                "and not NAN. y[(y != 0) & (y != 1)] = {0}".format(y[(y != 0) & (y != 1)])
             )
 
     def precalc_parameters(self, feature, y, pred):
         return None
 
     def calc_parameters(self, feature, y, pred, prefit_data):
         lex_binnumbers = feature.lex_binned_data
@@ -82,23 +79,19 @@
         event_weights = self.weights
         boosting_weights = boost_weights(y, prediction)
         weights = event_weights * boosting_weights
         alpha_prior, beta_prior = get_beta_priors()
 
         wsum = np.bincount(lex_binnumbers, weights=weights, minlength=minlength)
 
-        w2sum = np.bincount(
-            lex_binnumbers, weights=weights * boosting_weights, minlength=minlength
-        )
+        w2sum = np.bincount(lex_binnumbers, weights=weights * boosting_weights, minlength=minlength)
 
         alpha = np.bincount(lex_binnumbers, weights=weights * y, minlength=minlength)
 
-        beta = np.bincount(
-            lex_binnumbers, weights=weights * (1 - y), minlength=minlength
-        )
+        beta = np.bincount(lex_binnumbers, weights=weights * (1 - y), minlength=minlength)
 
         weight_factor = np.ones_like(wsum)
         np.true_divide(wsum, w2sum, out=weight_factor, where=wsum != 0)
         alpha *= weight_factor
         alpha = np.where(alpha < 0, 0, alpha)
         beta *= weight_factor
         beta = np.where(beta < 0, 0, beta)
@@ -122,27 +115,21 @@
         perc1 = 0.75 - shift
         perc2 = 0.25 - shift
 
         # * the actual Gaussian matching
         (
             factors_link,
             uncertainties_l,
-        ) = cyclic_boosting_base.gaussian_matching_by_quantiles(
-            posterior, self.link_func, perc1, perc2
-        )
+        ) = cyclic_boosting_base.gaussian_matching_by_quantiles(posterior, self.link_func, perc1, perc2)
 
         return factors_link, uncertainties_l
 
     def predict_proba(self, X, y=None, fit_mode=0):
-        probability_signal = super(CBClassifier, self).predict(
-            X, y=y, fit_mode=fit_mode, actions=None
-        )
+        probability_signal = super(CBClassifier, self).predict(X, y=y, fit_mode=fit_mode, actions=None)
         return np.c_[1 - probability_signal, probability_signal]
 
     def predict(self, X, y=None, fit_mode=0, actions=None):
-        probability_signal = super(CBClassifier, self).predict(
-            X, y=y, fit_mode=fit_mode, actions=None
-        )
+        probability_signal = super(CBClassifier, self).predict(X, y=y, fit_mode=fit_mode, actions=None)
         return np.asarray(probability_signal > 0.5, dtype=np.float64)
 
 
 __all__ = ["CBClassifier", "boost_weights", "get_beta_priors"]
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/common_smoothers.py` & `cyclic_boosting-0.1.0/cyclic_boosting/common_smoothers.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,50 +50,40 @@
         return flags.IS_UNORDERED
     else:
         features = ""
         if feature_group is not None:
             features = "for feature {}".format(feature_group)
         _logger.warning(
             "Feature property {0} is not known {1}."
-            " Thus it is converted to IS_UNORDERED!".format(
-                flags.flags_to_string(feature_property), features
-            )
+            " Thus it is converted to IS_UNORDERED!".format(flags.flags_to_string(feature_property), features)
         )
         return flags.IS_UNORDERED
 
 
 def _choice_fct_svd(feature_group, feature_prop, feature_type=None):
     if isinstance(feature_prop, tuple):
-        feature_prop = tuple(
-            [_simplify_flags(fp, feature_group) for fp in feature_prop]
-        )
+        feature_prop = tuple([_simplify_flags(fp, feature_group) for fp in feature_prop])
         return feature_prop
     else:
         return (_simplify_flags(feature_prop),)
 
 
 def _default_smoother_types(neutral_factor_link=0, use_normalization=True):
     smoother_types = {
-        flags.IS_UNORDERED: smoothing.onedim.WeightedMeanSmoother(
-            prior_prediction=neutral_factor_link
-        ),
-        flags.IS_ORDERED: smoothing.onedim.WeightedMeanSmoother(
-            prior_prediction=neutral_factor_link
-        ),
+        flags.IS_UNORDERED: smoothing.onedim.WeightedMeanSmoother(prior_prediction=neutral_factor_link),
+        flags.IS_ORDERED: smoothing.onedim.WeightedMeanSmoother(prior_prediction=neutral_factor_link),
         flags.IS_CONTINUOUS: smoothing.onedim.OrthogonalPolynomialSmoother(),
         flags.IS_LINEAR: smoothing.extrapolate.LinearExtrapolator(),
         flags.IS_SEASONAL:
         # the seasonal smoother does not work with offset_tozero
         # when the normalization is done within the smoother
         smoothing.onedim.SeasonalSmoother(offset_tozero=not use_normalization),
         flags.IS_MONOTONIC: smoothing.onedim.IsotonicRegressor(increasing="auto"),
-        flags.IS_MONOTONIC
-        | flags.INCREASING: smoothing.onedim.IsotonicRegressor(increasing=True),
-        flags.IS_MONOTONIC
-        | flags.DECREASING: smoothing.onedim.IsotonicRegressor(increasing=False),
+        flags.IS_MONOTONIC | flags.INCREASING: smoothing.onedim.IsotonicRegressor(increasing=True),
+        flags.IS_MONOTONIC | flags.DECREASING: smoothing.onedim.IsotonicRegressor(increasing=False),
     }
     return smoother_types
 
 
 def determine_reg_type(feature_group, feature_property, feature_type):
     """Function to determine the RegressionType of a feature.
 
@@ -108,25 +98,20 @@
 
     feature_type:
         Type of the feature.
     """
     if not isinstance(feature_property, tuple):
         if flags.is_linear_set(feature_property):
             return RegressionType.extrapolating
-        elif flags.is_seasonal_set(feature_property) or flags.is_continuous_set(
-            feature_property
-        ):
+        elif flags.is_seasonal_set(feature_property) or flags.is_continuous_set(feature_property):
             return RegressionType.interpolating
         else:
             return RegressionType.discontinuous
     else:
-        reg_types = [
-            determine_reg_type(fg, fp, feature_type)
-            for fg, fp in zip(feature_group, feature_property)
-        ]
+        reg_types = [determine_reg_type(fg, fp, feature_type) for fg, fp in zip(feature_group, feature_property)]
         if RegressionType.discontinuous in reg_types:
             return RegressionType.discontinuous
         elif RegressionType.interpolating in reg_types:
             return RegressionType.interpolating
         else:
             return RegressionType.extrapolating
 
@@ -182,50 +167,37 @@
         where feature_group is a tuple of strings and smoother is
         and instance of AbstractBinSmoother.
         (default = None)
 
     """
     neutral_factor_link = 0
 
-    def __init__(
-        self, use_regression_type=True, use_normalization=True, explicit_smoothers=None
-    ):
+    def __init__(self, use_regression_type=True, use_normalization=True, explicit_smoothers=None):
         self.use_regression_type = use_regression_type
         self.use_normalization = use_normalization
         self.explicit_smoothers = self._validate_explicit_smoothers(explicit_smoothers)
-        self.onedim_smoothers = _default_smoother_types(
-            self.neutral_factor_link, use_normalization
-        )
+        self.onedim_smoothers = _default_smoother_types(self.neutral_factor_link, use_normalization)
 
     @staticmethod
     def _validate_explicit_smoothers(explicit_smoothers):
-
         if explicit_smoothers is None:
             return {}
 
         def is_tuple_of_strings(x):
-            return isinstance(x, tuple) and all(
-                isinstance(s, six.string_types) for s in x
-            )
+            return isinstance(x, tuple) and all(isinstance(s, six.string_types) for s in x)
 
-        if not all(
-            is_tuple_of_strings(feature_group)
-            for feature_group in explicit_smoothers.keys()
-        ):
+        if not all(is_tuple_of_strings(feature_group) for feature_group in explicit_smoothers.keys()):
             raise ValueError(
                 "All explicit smoothers passed to the SmootherChoice"
                 " need to have a tuple of strings as a feature group key."
             )
 
-        if not all(
-            isinstance(sm, AbstractBinSmoother) for sm in explicit_smoothers.values()
-        ):
+        if not all(isinstance(sm, AbstractBinSmoother) for sm in explicit_smoothers.values()):
             raise ValueError(
-                "All explicit smoothers passed to the SmootherChoice"
-                " need to be instances of AbstractBinSmoother."
+                "All explicit smoothers passed to the SmootherChoice" " need to be instances of AbstractBinSmoother."
             )
 
         return explicit_smoothers
 
     def choice_fct(self, feature_group, feature_property, feature_type=None):
         """
         Returns the smoother specified by the `get_raw_smoother` method
@@ -248,21 +220,17 @@
         """
 
         explicit_smoother = self.explicit_smoothers.get(feature_group)
 
         if explicit_smoother is not None:
             smoother = explicit_smoother
         else:
-            smoother = self.get_raw_smoother(
-                feature_group, feature_property, feature_type
-            )
+            smoother = self.get_raw_smoother(feature_group, feature_property, feature_type)
 
-        return self.wrap_smoother(
-            smoother, feature_group, feature_property, feature_type
-        )
+        return self.wrap_smoother(smoother, feature_group, feature_property, feature_type)
 
     def get_onedim_smoother(self, feature_property, feature_name=None):
         """
         Returns the standard one-dimensional smoother to be used for a
         specific feature.
         If an explicit 1D-smoother for the feature is defined, it is returned,
         otherwise the default smoother for the feature property is chosen.
@@ -335,46 +303,38 @@
     r"""Weighted mean smoothing for multi-dimensional feature groups.
 
     This defines a set of common smoothers where
     choose_smoothers_for_factor_model selects from.
     """
 
     def get_raw_smoother(self, feature_group, feature_prop, feature_type=None):
-
         if len(feature_group) > 1:
-            smoother = smoothing.multidim.WeightedMeanSmoother(
-                prior_prediction=self.neutral_factor_link
-            )
+            smoother = smoothing.multidim.WeightedMeanSmoother(prior_prediction=self.neutral_factor_link)
         else:
             smoother = self.get_onedim_smoother(feature_prop[0], feature_group[0])
         return smoother
 
 
 class SmootherChoiceGroupBy(SmootherChoice):
     """
     Groupby smoothing for multi-dimensional feature groups.
     """
 
-    def wrap_smoother(
-        self, smoother, feature_group, feature_property, feature_type=None
-    ):
-
+    def wrap_smoother(self, smoother, feature_group, feature_property, feature_type=None):
         # only the properties of the innermost feature should
         # determine the regression type of the groupby smoother:
         if not isinstance(smoother, smoothing.multidim.GroupBySmootherCB):
             return super(self.__class__, self).wrap_smoother(
                 smoother, feature_group, feature_property[-1], feature_type
             )
         else:
             return smoother
 
     def get_raw_smoother(self, feature_group, feature_prop, feature_type=None):
-        innermost_smoother = self.get_onedim_smoother(
-            feature_prop[-1], feature_group[-1]
-        )
+        innermost_smoother = self.get_onedim_smoother(feature_prop[-1], feature_group[-1])
         if len(feature_group) > 1:
             return smoothing.multidim.GroupBySmootherCB(
                 self.wrap_smoother(innermost_smoother, feature_group, feature_prop),
                 n_dim=len(feature_group),
             )
         else:
             return innermost_smoother
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/features.py` & `cyclic_boosting-0.1.0/cyclic_boosting/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 
     Note
     ----
 
     The suffix ``_link`` in attributes refers to values valid in link space.
     """
 
-    def __init__(
-        self, feature_id, feature_property, smoother, minimal_factor_change=1e-4
-    ):
+    def __init__(self, feature_id, feature_property, smoother, minimal_factor_change=1e-4):
         self.feature_id = feature_id
         self.feature_group = feature_id.feature_group
         if len(self.feature_group) < 2:
             self.smootherb = onedim.BinValuesSmoother()
         else:
             self.smootherb = multidim.BinValuesSmoother()
         self.is_fitted = False
@@ -89,18 +87,15 @@
         return self.dim == 1
 
     @property
     def missing_not_learned(self):
         """
         True if ``flags.MISSING_NOT_LEARNED`` can be found in feature property.
         """
-        return any(
-            flags.missing_not_learned_set(feature_prop)
-            for feature_prop in self.feature_property
-        )
+        return any(flags.missing_not_learned_set(feature_prop) for feature_prop in self.feature_property)
 
     @property
     def n_bins(self):
         """Number of bins, including the extra bin for missing and infinite
         values
         """
         return self.n_bins_finite + 1
@@ -142,20 +137,16 @@
         * nan_bin_weightsum: The sum of weights for the nan-bin.
         * bin_centers: Array containing the center of each bin.
         """
         binnumbers = get_X_column(X, self.feature_group, array_for_1_dim=False)
         (
             self.lex_binned_data,
             self.n_multi_bins_finite,
-        ) = multidim_binnos_to_lexicographic_binnos(
-            binnumbers, self.n_multi_bins_finite
-        )
-        self.bin_weightsums = np.bincount(
-            self.lex_binned_data, weights=weights, minlength=self.n_bins
-        )
+        ) = multidim_binnos_to_lexicographic_binnos(binnumbers, self.n_multi_bins_finite)
+        self.bin_weightsums = np.bincount(self.lex_binned_data, weights=weights, minlength=self.n_bins)
 
     @property
     def unfitted_factor_link_nan_bin(self):
         return self.unfitted_factors_link[-1]
 
     @property
     def factor_link_nan_bin(self):
@@ -185,17 +176,15 @@
 
         X_for_smoother[:n_bins, :n_bin_dims] = self.bin_centers
         X_for_smoother[n_bins, :n_bin_dims] = np.nan
         X_for_smoother[:, n_bin_dims] = self.bin_weightsums
         X_for_smoother[:, -1] = uncertainties_link
         return X_for_smoother
 
-    def update_factors(
-        self, unfitted_factors, unfitted_uncertainties, neutral_factor_link, learn_rate
-    ):
+    def update_factors(self, unfitted_factors, unfitted_uncertainties, neutral_factor_link, learn_rate):
         """Call the smoother on the bin results if necessary.
 
         Parameters
         ----------
 
         unfitted_factors: ndarray
             bin means in link space as returned by the method
@@ -238,17 +227,15 @@
     into :class:`FeatureID`s
     """
     if isinstance(feature_group_or_id, FeatureID):
         return feature_group_or_id
     elif isinstance(feature_group_or_id, tuple):
         return FeatureID(feature_group=feature_group_or_id, feature_type=default_type)
     else:
-        return FeatureID(
-            feature_group=(feature_group_or_id,), feature_type=default_type
-        )
+        return FeatureID(feature_group=(feature_group_or_id,), feature_type=default_type)
 
 
 def create_features(feature_groups_or_ids, feature_properties, smoother_choice):
     """
     Parameters
     ----------
 
@@ -266,23 +253,18 @@
 
     def make_feature_for_group_or_id(feature_group_or_id):
         feature_id = create_feature_id(feature_group_or_id)
 
         feature_property = flags.read_feature_property(
             feature_properties, feature_id.feature_group, default=flags.HAS_MISSING
         )
-        smoother = smoother_choice.choice_fct(
-            feature_id.feature_group, feature_property, feature_id.feature_type
-        )
+        smoother = smoother_choice.choice_fct(feature_id.feature_group, feature_property, feature_id.feature_type)
         return Feature(feature_id, feature_property, clone(smoother))
 
-    features = [
-        make_feature_for_group_or_id(feature_group_or_id)
-        for feature_group_or_id in feature_groups_or_ids
-    ]
+    features = [make_feature_for_group_or_id(feature_group_or_id) for feature_group_or_id in feature_groups_or_ids]
 
     return FeatureList(features)
 
 
 class FeatureList(object):
     """Iterable providing the information about a list of features in the
     form of :class:`Feature` objects
@@ -343,17 +325,15 @@
            Feature instance
         """
         feature_id = create_feature_id(feature_group_or_id)
 
         for feature in self.features:
             if feature.feature_id == feature_id:
                 return feature
-        raise KeyError(
-            "Feature {0} is not known in {1}".format(feature_id, self.feature_ids)
-        )
+        raise KeyError("Feature {0} is not known in {1}".format(feature_id, self.feature_ids))
 
     def get_feature(self, feature_group, feature_type=None):
         """Selects feature specified by ``feature_group`` and ``feature_type``
 
         Parameters
         ----------
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/flags.py` & `cyclic_boosting-0.1.0/cyclic_boosting/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,20 +284,15 @@
     Traceback (most recent call last):
     ValueError: Exactly one of IS_CONTINUOUS, IS_ORDERED, IS_UNORDERED ...
 
     >>> check_flags_consistency(flags.DECREASING | flags.INCREASING)
     Traceback (most recent call last):
     ValueError: One feature can either be ...
     """
-    if (
-        int(is_continuous_set(flags_value))
-        + int(is_ordered_set(flags_value))
-        + int(is_unordered_set(flags_value))
-        != 1
-    ):
+    if int(is_continuous_set(flags_value)) + int(is_ordered_set(flags_value)) + int(is_unordered_set(flags_value)) != 1:
         raise ValueError(
             "Exactly one of IS_CONTINUOUS, IS_ORDERED, "
             "IS_UNORDERED must be set in a "
             "flags value for the feature properties."
         )
     if int(increasing_set(flags_value)) + int(decreasing_set(flags_value)) == 2:
         raise ValueError("One feature can either be INCREASING" " or DECREASING")
@@ -352,17 +347,15 @@
     """
     if isinstance(flags_value, tuple):
         return tuple(_convert_flags_to_string(flags_val) for flags_val in flags_value)
     else:
         return _convert_flags_to_string(flags_value)
 
 
-def _convert_flags_to_string(
-    flags_value, alternative_flag_list=None, alternative_flags=None
-):
+def _convert_flags_to_string(flags_value, alternative_flag_list=None, alternative_flags=None):
     """
     This function converts the numeric flags to the corresponding strings
     that are defined in the flag list.
 
     Parameters
     ----------
 
@@ -416,18 +409,15 @@
     >>> feature_properties = {'a': flags.IS_ORDERED, 'b': flags.IS_UNORDERED}
     >>> flags_to_string(read_feature_property(feature_properties, 'b', flags.HAS_MISSING))
     'IS_UNORDERED'
     >>> flags_to_string(read_feature_property(feature_properties, 'c', flags.HAS_MISSING))
     'HAS_MISSING'
     """
     if isinstance(feature_group, tuple):
-        return tuple(
-            read_feature_property(feature_properties, col, default=default)
-            for col in feature_group
-        )
+        return tuple(read_feature_property(feature_properties, col, default=default) for col in feature_group)
     else:
         feature_prop = None
         if feature_properties is not None:
             feature_prop = feature_properties.get(feature_group)
         if feature_prop is None:
             feature_prop = default
         return feature_prop
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/learning_rate.py` & `cyclic_boosting-0.1.0/cyclic_boosting/learning_rate.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,10 +78,8 @@
 
     maximal_iteration: int
         Maximal cyclic boosting iteration.
 
     feature: :class:`cyclic_boosting.base.Feature`
         Feature
     """
-    return np.minimum(
-        linear_learn_rate(iteration, maximal_iteration * 0.5, feature), 1.0
-    )
+    return np.minimum(linear_learn_rate(iteration, maximal_iteration * 0.5, feature), 1.0)
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/link.py` & `cyclic_boosting-0.1.0/cyclic_boosting/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 import numexpr
 import numpy as np
 import six
 
 
 @six.add_metaclass(abc.ABCMeta)
 class LinkFunction(object):
-    r"""Abstract base class for link function computations.
-    """
+    r"""Abstract base class for link function computations."""
 
     @abc.abstractmethod
     def is_in_range(self, values):
         "Check if values can be transformed by the link function."
         pass
 
     @abc.abstractmethod
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/location.py` & `cyclic_boosting-0.1.0/cyclic_boosting/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 from cyclic_boosting.base import CyclicBoostingBase, calc_factors_generic
 from cyclic_boosting.link import IdentityLinkMixin
 from cyclic_boosting.utils import weighted_stddev
 
 _logger = logging.getLogger(__name__)
 
 
-class CBLocPoissonRegressor(
-    CyclicBoostingBase, sklearn.base.RegressorMixin, IdentityLinkMixin
-):
+class CBLocPoissonRegressor(CyclicBoostingBase, sklearn.base.RegressorMixin, IdentityLinkMixin):
     def precalc_parameters(self, feature, y, pred):
         lex_binnumbers = feature.lex_binned_data
         minlength = feature.n_bins
         weights = self.weights
 
         global_std = weighted_stddev(y, weights)
         y_sum = np.bincount(lex_binnumbers, weights=y * weights, minlength=minlength)
@@ -41,16 +39,16 @@
 
         :math:`\mu_n = \sigma_{n}^{2} \left(\frac{\mu_0}{sigma_{0}^{2}} +
             \frac{n \bar{x}}{\sigma_{x}^{2}}`
         """
         prior_mean = 0.0
         reg_mean = (
             1.0
-            / (bincount / uncertainties ** 2 + 1.0 / global_std ** 2)
-            * (bincount * summands / uncertainties ** 2 + prior_mean / global_std ** 2)
+            / (bincount / uncertainties**2 + 1.0 / global_std**2)
+            * (bincount * summands / uncertainties**2 + prior_mean / global_std**2)
         )
         return reg_mean
 
     def calc_parameters(self, feature, y, pred, prefit_data=None):
         lex_binnumbers = feature.lex_binned_data
         minlength = feature.n_bins
         prediction = self.unlink_func(pred.predict_link())
@@ -61,35 +59,27 @@
         variance = numexpr.evaluate("where(prediction <= 0., 1, prediction)")
 
         factor_numerator = np.bincount(
             lex_binnumbers,
             weights=weights * (y - prediction) / variance,
             minlength=minlength,
         )
-        denominator = np.bincount(
-            lex_binnumbers, weights=weights / variance, minlength=minlength
-        )
-        uncertainty_numerator = np.bincount(
-            lex_binnumbers, weights=weights ** 2 / variance, minlength=minlength
-        )
+        denominator = np.bincount(lex_binnumbers, weights=weights / variance, minlength=minlength)
+        uncertainty_numerator = np.bincount(lex_binnumbers, weights=weights**2 / variance, minlength=minlength)
 
         denominator = np.where(denominator > 0, denominator, 1)
         summands = factor_numerator / denominator
         uncertainties = uncertainty_numerator / denominator
         uncertainties = np.where(uncertainties > 0, uncertainties, global_std)
 
-        summands = self._regularize_summands(
-            bincount, summands, uncertainties, global_std
-        )
+        summands = self._regularize_summands(bincount, summands, uncertainties, global_std)
         return summands, uncertainties
 
     def predict(self, X, y=None, fit_mode=0, actions=None):
-        result = super(CBLocPoissonRegressor, self).predict(
-            X, y=y, fit_mode=fit_mode, actions=actions
-        )
+        result = super(CBLocPoissonRegressor, self).predict(X, y=y, fit_mode=fit_mode, actions=actions)
         return np.where(result > 0, result, 0)
 
 
 def precalc_variance_y(feature, y, weights, n_prior=1):
     """Calculate expected value of posterior of variance parameter for a gaussian
     with a gamma distributed prior Gamma(a_0, b_0) and known mean for each bin.
 
@@ -115,17 +105,15 @@
     ndarray
         The estimated variance of y for each bin
     """
     lex_binnumbers = feature.lex_binned_data
     minlength = feature.n_bins
 
     weighted_mean_y = np.sum(y * weights) / np.sum(weights)
-    variance_prior = np.sum(
-        (y - weighted_mean_y) * (y - weighted_mean_y) * weights
-    ) / np.sum(weights)
+    variance_prior = np.sum((y - weighted_mean_y) * (y - weighted_mean_y) * weights) / np.sum(weights)
     if variance_prior <= 1e-9:  # No variation in y; happens only in tests
         variance_prior = 1.0
 
     sum_y = np.bincount(lex_binnumbers, weights=weights * y, minlength=minlength)
     sum_weights = np.bincount(lex_binnumbers, weights=weights, minlength=minlength)
     mean_y = sum_y[lex_binnumbers] / sum_weights[lex_binnumbers]
     weighted_squared_residual_sum = np.bincount(
@@ -135,17 +123,15 @@
     a_0 = 0.5 * n_prior
     b_0 = a_0 * variance_prior
     a = a_0 + 0.5 * sum_weights
     b = b_0 + 0.5 * weighted_squared_residual_sum
     return b / a
 
 
-def calc_parameters_intercept(
-    lex_binnumbers, prediction, minlength, y, variance_y, weights
-):
+def calc_parameters_intercept(lex_binnumbers, prediction, minlength, y, variance_y, weights):
     """Calculates intercepts and uncertainties for each bin of a feature group.
 
     Parameters
     ----------
     lex_binnumbers: :class:`numpy.ndarray` (float64, ndims=1)
         1-dimensional numpy array containing the bin numbers.
     prediction: :class:`numpy.ndarray` (float64, ndims=1)
@@ -167,22 +153,18 @@
         ``intercepts`` and ``uncertainties``.
     """
     w = weights / variance_y
     w_x = w * (y - prediction)
     w_x2 = w * (y - prediction) ** 2
     x0 = 0
     w0 = 1e-2
-    return calc_factors_generic(
-        lex_binnumbers, w_x, w, w_x2, weights, minlength, x0, w0
-    )
+    return calc_factors_generic(lex_binnumbers, w_x, w, w_x2, weights, minlength, x0, w0)
 
 
-class CBLocationRegressor(
-    sklearn.base.RegressorMixin, CyclicBoostingBase, IdentityLinkMixin
-):
+class CBLocationRegressor(sklearn.base.RegressorMixin, CyclicBoostingBase, IdentityLinkMixin):
     def _check_y(self, y):
         """Check that y has no negative values."""
         if not np.isfinite(y).all():
             raise ValueError("The target y must be real value and not NAN.")
 
     def precalc_parameters(self, feature, y, pred):
         """Calculations that are not  dependent on intermediate predictions. If
@@ -227,31 +209,25 @@
         tuple
             This method must return a tuple of ``factors`` and
             ``uncertainties`` in the **link space**.
         """
         lex_binnumbers = feature.lex_binned_data
         minlength = feature.n_bins
         variance_y = prefit_data[lex_binnumbers]
-        return calc_parameters_intercept(
-            lex_binnumbers, pred.predict_link(), minlength, y, variance_y, self.weights
-        )
+        return calc_parameters_intercept(lex_binnumbers, pred.predict_link(), minlength, y, variance_y, self.weights)
 
     def calibrate_to_weighted_mean(self, feature):
         if feature.missing_not_learned:
             calibrated_factors_link = (
                 feature.factors_link[:-1]
-                - (feature.factors_link[:-1] * feature.bin_weightsums[:-1]).sum()
-                / feature.bin_weightsums[:-1].sum()
-            )
-            calibrated_factors_link = np.append(
-                calibrated_factors_link, self.neutral_factor_link
+                - (feature.factors_link[:-1] * feature.bin_weightsums[:-1]).sum() / feature.bin_weightsums[:-1].sum()
             )
+            calibrated_factors_link = np.append(calibrated_factors_link, self.neutral_factor_link)
         else:
             calibrated_factors_link = (
                 feature.factors_link
-                - (feature.factors_link * feature.bin_weightsums).sum()
-                / feature.bin_weightsums.sum()
+                - (feature.factors_link * feature.bin_weightsums).sum() / feature.bin_weightsums.sum()
             )
         return calibrated_factors_link
 
 
 __all__ = ["CBLocationRegressor", "CBLocPoissonRegressor"]
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/nbinom.py` & `cyclic_boosting-0.1.0/cyclic_boosting/nbinom.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,20 @@
 def _try_compile_parallel_func(**targetoptions):
     """
     Decorator that tries to compile a wrapped function in numba parallel mode. If that
     fails it will compile the function in non-parallel mode.
     """
 
     def wrapper(f):
-
         try:
             wrapper = nb.jit(**targetoptions, parallel=True)
             func = wrapper(f)
 
         except:  # noqa
-            _logger.warning(
-                f"Could not compile function {f} in parallel mode, falling back to"
-                f"non-parallel mode."
-            )
+            _logger.warning(f"Could not compile function {f} in parallel mode, falling back to" f"non-parallel mode.")
             wrapper = nb.jit(**targetoptions, parallel=False)
             func = wrapper(f)
 
         return func
 
     return wrapper
 
@@ -102,16 +98,15 @@
         self.bayes = bayes
         self.n_steps = n_steps
 
     def _check_y(self, y):
         """Check that y has no negative values."""
         if not (y >= 0.0).all():
             raise ValueError(
-                "The target y must be positive semi-definite "
-                "and not NAN. y[~(y>=0)] = {0}".format(y[~(y >= 0)])
+                "The target y must be positive semi-definite " "and not NAN. y[~(y>=0)] = {0}".format(y[~(y >= 0)])
             )
 
     def precalc_parameters(self, feature, y, pred):
         return None
 
     def calc_parameters(self, feature, y, pred, prefit_data):
         c_link = pred.predict_link()
@@ -181,17 +176,15 @@
     return coeff + n * np.log(p) + x * np.log(1 - p)
 
 
 @_try_compile_parallel_func(
     nogil=True,
     nopython=True,
 )
-def loss_nbinom_c(
-    y: nb.float64[:], mu: nb.float64[:], c: nb.float64[:], gamma: nb.float64
-) -> nb.float64:
+def loss_nbinom_c(y: nb.float64[:], mu: nb.float64[:], c: nb.float64[:], gamma: nb.float64) -> nb.float64:
     n_samples = len(y)
 
     p = np.minimum(1.0 / (1 + c * mu), 1.0 - 1e-8)
     n = mu * p / (1 - p)
 
     loss = np.zeros(n_samples)
     for i in nb.prange(n_samples):
@@ -244,42 +237,35 @@
     gamma: nb.float64,
     new_c_link: nb.float64[:],
 ) -> nb.float64[:, :]:
     n_new_c = len(new_c_link)
     loss = np.empty((n_new_c, minlength), dtype=np.float64)
 
     for i in nb.prange(n_new_c):
-        loss[i] = binned_loss_nbinom_c(
-            y.astype(np.float64), mu, c_link, binnumbers, minlength, gamma,
-            new_c_link[i]
-        )
+        loss[i] = binned_loss_nbinom_c(y.astype(np.float64), mu, c_link, binnumbers, minlength, gamma, new_c_link[i])
 
     return loss
 
 
 @nb.njit(nogil=True)
-def bayes_result(
-    loss: nb.float64[:, :], minlength: nb.int64, new_c_link: nb.float64[:]
-) -> nb.float64[:]:
+def bayes_result(loss: nb.float64[:, :], minlength: nb.int64, new_c_link: nb.float64[:]) -> nb.float64[:]:
     result = np.zeros(minlength)
 
     for j in range(minlength):
         l = -loss[:, j]
         l -= l.max()
         l = np.exp(l)
         l[~np.isfinite(l)] = 0.0
         l /= np.sum(l)
         result[j] = np.sum(l * new_c_link)
 
     return result
 
 
-def calc_parameters_nbinom_c(
-    y, mu, c_link, binnumbers, minlength, gamma, bayes, new_c_link
-):
+def calc_parameters_nbinom_c(y, mu, c_link, binnumbers, minlength, gamma, bayes, new_c_link):
     loss = compute_2d_loss(y, mu, c_link, binnumbers, minlength, gamma, new_c_link)
 
     if bayes:
         result = bayes_result(loss, minlength, new_c_link)
 
     else:
         result = new_c_link[np.argmin(loss, axis=0)]
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/observers.py` & `cyclic_boosting-0.1.0/cyclic_boosting/observers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         estimator_state : dict
             state of the estimator. See
             :meth:`cyclic_boosting.base.CyclicBoostingBase.get_state` for
             information on what will be passed here
 
         """
 
-    def observe_feature_iterations(
-        self, iteration, feature_i, X, y, prediction, weights, estimator_state
-    ):
+    def observe_feature_iterations(self, iteration, feature_i, X, y, prediction, weights, estimator_state):
         """
         Called after each feature has been processed as part of a full
         iteration of the algorithm.
 
         Parameters
         ----------
         iteration : int
@@ -100,31 +98,27 @@
         after the given iteration has been calculated.
         Default is `-1`, which signifies the last iteration.
 
     """
 
     def __init__(self, iteration=-1):
         if iteration == 0:
-            raise ValueError(
-                "This plotting observer only makes sense with iterations >= 1."
-            )
+            raise ValueError("This plotting observer only makes sense with iterations >= 1.")
         self.iteration = iteration
 
         self.features = None
         self.link_function = None
         self.n_feature_bins = None
         self.loss = list()
         self.factor_change = list()
         self.histograms = None
 
         self._fitted = False
 
-    def observe_iterations(
-        self, iteration, X, y, prediction, weights, estimator_state, delta=None
-    ):
+    def observe_iterations(self, iteration, X, y, prediction, weights, estimator_state, delta=None):
         """Observe iterations in cyclic_boosting estimator to collect information for
         necessary for plots. This function is called in each major loop and once in the
         end.
 
         Parameters
         ----------
 
@@ -153,24 +147,19 @@
             if iteration != 0:
                 # for iteration 0 there are no old fators to compare with
                 self.factor_change.append(delta)
 
         if iteration == self.iteration:
             self._fitted = True
             self.features = copy.deepcopy(features)
-            self.n_feature_bins = {
-                feature.feature_group: feature.n_multi_bins_finite
-                for feature in self.features
-            }
+            self.n_feature_bins = {feature.feature_group: feature.n_multi_bins_finite for feature in self.features}
             self.link_function = estimator_state["link_function"]
             self.histograms = calc_in_sample_histograms(y, prediction, weights)
 
-    def observe_feature_iterations(
-        self, iteration, feature_i, X, y, prediction, weights, estimator_state
-    ):
+    def observe_feature_iterations(self, iteration, feature_i, X, y, prediction, weights, estimator_state):
         """Observe iterations in cyclic_boosting estimator to collect information for
         necessary for plots. This function is called in each feature/minor loop.
 
         Parameters
         ----------
 
         iteration: int
@@ -226,17 +215,15 @@
         * errors
         * counts
     """
     nbins = 100
     bin_boundaries, bin_centers = utils.calc_linear_bins(pred, nbins)
     bin_numbers = utils.digitize(pred, bin_boundaries)
     means, _, counts, errors = utils.calc_means_medians(bin_numbers, y, weights)
-    bin_centers = bin_centers[
-        np.where(~np.isnan(means.reindex(np.arange(1, nbins + 1))))
-    ]
+    bin_centers = bin_centers[np.where(~np.isnan(means.reindex(np.arange(1, nbins + 1))))]
     # quantiles do not work for classification mode
     if np.isin(y, [0, 1]).all():
         return means, bin_centers, None, counts
     else:
         return means, bin_centers, errors, counts
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/pipelines.py` & `cyclic_boosting-0.1.0/cyclic_boosting/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-from cyclic_boosting import CBLocationRegressor, CBExponential, \
-    CBNBinomRegressor, CBPoissonRegressor,  CBLocPoissonRegressor, CBNBinomC, \
-    CBClassifier, CBGBSRegressor, binning
+from cyclic_boosting import (
+    CBLocationRegressor,
+    CBExponential,
+    CBNBinomRegressor,
+    CBPoissonRegressor,
+    CBLocPoissonRegressor,
+    CBNBinomC,
+    CBClassifier,
+    CBGBSRegressor,
+    binning,
+)
 
 from sklearn.pipeline import Pipeline
 
 
 def pipeline_CB(
-        estimator=None,
-        feature_groups=None,
-        feature_properties=None,
-        weight_column=None,
-        prior_prediction_column=None,
-        minimal_loss_change=1e-3,
-        minimal_factor_change=1e-3,
-        maximal_iterations=10,
-        observers=None,
-        smoother_choice=None,
-        output_column=None,
-        learn_rate=None,
-        number_of_bins=100,
-        aggregate=True,
-        a=1.0,
-        c=0.0,
-        external_colname=None,
-        standard_feature_groups=None,
-        external_feature_groups=None,
-        var_prior_exponent=0.1,
-        prior_exponent_colname=None,
-        mean_prediction_column=None,
-        gamma=0.0,
-        bayes=False,
-        n_steps=15,
-        regalpha=0.0,
-    ):
-
-    if estimator in [CBPoissonRegressor, CBLocPoissonRegressor,
-                     CBLocationRegressor, CBClassifier]:
+    estimator=None,
+    feature_groups=None,
+    feature_properties=None,
+    weight_column=None,
+    prior_prediction_column=None,
+    minimal_loss_change=1e-3,
+    minimal_factor_change=1e-3,
+    maximal_iterations=10,
+    observers=None,
+    smoother_choice=None,
+    output_column=None,
+    learn_rate=None,
+    number_of_bins=100,
+    aggregate=True,
+    a=1.0,
+    c=0.0,
+    external_colname=None,
+    standard_feature_groups=None,
+    external_feature_groups=None,
+    var_prior_exponent=0.1,
+    prior_exponent_colname=None,
+    mean_prediction_column=None,
+    gamma=0.0,
+    bayes=False,
+    n_steps=15,
+    regalpha=0.0,
+):
+    if estimator in [CBPoissonRegressor, CBLocPoissonRegressor, CBLocationRegressor, CBClassifier]:
         estimatorCB = estimator(
             feature_groups=feature_groups,
             feature_properties=feature_properties,
             weight_column=weight_column,
             prior_prediction_column=prior_prediction_column,
             minimal_loss_change=minimal_loss_change,
             minimal_factor_change=minimal_factor_change,
@@ -127,48 +133,55 @@
 
 def pipeline_CBPoissonRegressor(**kwargs):
     """
     Convenience function containing CBPoissonRegressor (estimator) + binning.
     """
     return pipeline_CB(CBPoissonRegressor, **kwargs)
 
+
 def pipeline_CBNBinomRegressor(**kwargs):
     """
     Convenience function containing CBNBinomRegressor (estimator) + binning.
     """
     return pipeline_CB(CBNBinomRegressor, **kwargs)
 
+
 def pipeline_CBClassifier(**kwargs):
     """
     Convenience function containing CBClassifier (estimator) + binning.
     """
     return pipeline_CB(CBClassifier, **kwargs)
 
+
 def pipeline_CBLocationRegressor(**kwargs):
     """
     Convenience function containing CBLocationRegressor (estimator) + binning.
     """
     return pipeline_CB(CBLocationRegressor, **kwargs)
 
+
 def pipeline_CBExponential(**kwargs):
     """
     Convenience function containing CBExponential (estimator) + binning.
     """
-    return pipeline_CB(CBExponential,**kwargs)
+    return pipeline_CB(CBExponential, **kwargs)
+
 
 def pipeline_CBLocPoissonRegressor(**kwargs):
     """
     Convenience function containing CBLocPoissonRegressor (estimator) + binning.
     """
-    return pipeline_CB(CBLocPoissonRegressor,**kwargs)
+    return pipeline_CB(CBLocPoissonRegressor, **kwargs)
+
 
 def pipeline_CBNBinomC(**kwargs):
     """
     Convenience function containing CBNBinomC (estimator) + binning.
     """
-    return pipeline_CB(CBNBinomC,**kwargs)
+    return pipeline_CB(CBNBinomC, **kwargs)
+
 
 def pipeline_CBGBSRegressor(**kwargs):
     """
     Convenience function containing CBGBSRegressor (estimator) + binning.
     """
-    return pipeline_CB(CBGBSRegressor,**kwargs)
+    return pipeline_CB(CBGBSRegressor, **kwargs)
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/plots/_1dplots.py` & `cyclic_boosting-0.1.0/cyclic_boosting/plots/_1dplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-
 import matplotlib.pyplot as plt
 import numpy as np
 from six.moves import map
 
 from cyclic_boosting import flags
-from cyclic_boosting.link import IdentityLinkMixin, LogitLinkMixin,\
-    LogLinkMixin
+from cyclic_boosting.link import IdentityLinkMixin, LogitLinkMixin, LogLinkMixin
 
 
 def _format_tick(tick, precision=1e-2):
     """Returns a suitable string representation for a
     factor, when it is given a tick position in linear space.
 
     A "suitable" string reprentation is (in this order):
@@ -89,17 +87,15 @@
 
 
 def _plot_factors(factors, x_axis_range, label, uncertainties=None):
     """
     Plot unsmoothed factors in given range with errobars if uncertainties are provided
     """
     if uncertainties is not None:
-        unsmoothed_style = dict(
-            capsize=2.5, markersize=2, fmt="o", color="k", alpha=0.6
-        )
+        unsmoothed_style = dict(capsize=2.5, markersize=2, fmt="o", color="k", alpha=0.6)
         unsmoothed_style["label"] = label
         plt.errorbar(x_axis_range, factors, yerr=uncertainties, **unsmoothed_style)
     else:
         unsmoothed_style = dict(markersize=2, marker="o", color="k", alpha=0.6)
         unsmoothed_style["label"] = label
         plt.plot(x_axis_range, factors, **unsmoothed_style)
 
@@ -118,20 +114,15 @@
             markersize=5.0,
             linestyle="none",
             fillstyle="none",
             color="r",
         )
     smoothed_style["label"] = "smoothed factors"
     if uncertainties is not None:
-        plt.errorbar(
-            x_axis_range,
-            factors,
-            yerr=[uncertainties[0], uncertainties[1]],
-            **smoothed_style
-        )
+        plt.errorbar(x_axis_range, factors, yerr=[uncertainties[0], uncertainties[1]], **smoothed_style)
     else:
         plt.plot(x_axis_range, factors, **smoothed_style)
 
 
 def _plot_missing_factor(factors, x_axis_range, y_axis_range):
     """
     Plot the factor which was calculated for missing values and mark the region in an orange color
@@ -223,21 +214,15 @@
         uncertainties = [uncertainties, uncertainties]
     else:
         uncertainties = [
             feature.unfitted_uncertainties_link,
             feature.unfitted_uncertainties_link,
         ]
 
-    assert (
-        len(factors)
-        == len(smoothed_factors)
-        == len(uncertainties[0])
-        == len(uncertainties[1])
-        > 0
-    )
+    assert len(factors) == len(smoothed_factors) == len(uncertainties[0]) == len(uncertainties[1]) > 0
     number_of_factors = len(factors)
 
     if isinstance(link_function, IdentityLinkMixin):
         plt.axhline(0, color="gray")
         plt.ylabel("Summand")
 
     elif isinstance(link_function, LogLinkMixin):
@@ -246,32 +231,25 @@
         if plot_yp:
             y = link_function.unlink_func(y)
             p = link_function.unlink_func(p)
         plt.axhline(1, color="gray")
         plt.ylabel("Factor")
 
     elif isinstance(link_function, LogitLinkMixin):
-        lower = np.abs(
-            link_function.unlink_func(factors - uncertainties[0])
-            - link_function.unlink_func(factors)
-        )
-        upper = np.abs(
-            link_function.unlink_func(factors + uncertainties[1])
-            - link_function.unlink_func(factors)
-        )
+        lower = np.abs(link_function.unlink_func(factors - uncertainties[0]) - link_function.unlink_func(factors))
+        upper = np.abs(link_function.unlink_func(factors + uncertainties[1]) - link_function.unlink_func(factors))
         factors = link_function.unlink_func(factors)
         smoothed_factors = link_function.unlink_func(smoothed_factors)
         uncertainties = [
             np.where(lower < 0.0, 0.0, lower),
             np.where(upper > 1.0, 1.0, upper),
         ]
         if plot_yp:
             # do not unlink for nbinom width mode
-            if ((link_function.unlink_func(y) >= 0).all()) and \
-                    ((link_function.unlink_func(y) <= 1).all()):
+            if ((link_function.unlink_func(y) >= 0).all()) and ((link_function.unlink_func(y) <= 1).all()):
                 y = link_function.unlink_func(y)
             p = link_function.unlink_func(p)
         plt.axhline(0.5, color="gray")
         plt.ylabel("Probability")
 
     else:
         plt.ylabel("Unkown")
@@ -281,17 +259,15 @@
     if number_of_factors > 400:
         from cyclic_boosting.plots import plot_factor_histogram
 
         plot_factor_histogram(feature)
         return
 
     feature_property = _ensure_tuple(feature.feature_property)
-    is_continuous = flags.is_continuous_set(feature_property[0]) | flags.is_linear_set(
-        feature_property[0]
-    )
+    is_continuous = flags.is_continuous_set(feature_property[0]) | flags.is_linear_set(feature_property[0])
     if plot_yp:
         minmax = np.r_[
             np.min(np.r_[factors, smoothed_factors, y, p]),
             np.max(np.r_[factors, smoothed_factors, y, p]),
         ]
     else:
         minmax = np.r_[
@@ -302,17 +278,15 @@
     if len(f) > 1:
         f[:2] = minmax
         u = uncertainties
     else:
         f = minmax
         u = np.c_[uncertainties, uncertainties]
 
-    y_axis_range, y_axis_labels = _get_y_axis(
-        f, u if ylimits_include_errors else None
-    )
+    y_axis_range, y_axis_labels = _get_y_axis(f, u if ylimits_include_errors else None)
     x_axis_range, x_axis_labels = _get_x_axis(factors, bin_bounds, is_continuous)
 
     if "MISSING" in flags._convert_flags_to_string(feature.feature_property[0]):
         _plot_missing_factor(smoothed_factors, x_axis_range, y_axis_range)
     elif len(factors) > 1:
         factors = factors[:-1]
         uncertainties = [uncertainties[0][:-1], uncertainties[1][:-1]]
@@ -322,31 +296,27 @@
 
     _plot_smoothed_factors(smoothed_factors, x_axis_range, is_continuous, None)
 
     if not plot_yp:
         label = "factors"
         if is_continuous:
             x_axis_range = (x_axis_range + np.append(x_axis_range, x_axis_range[-1] + 1)[1:]) / 2
-        _plot_factors(
-            factors, x_axis_range, label, uncertainties if with_errorbars else None
-        )
+        _plot_factors(factors, x_axis_range, label, uncertainties if with_errorbars else None)
 
     try:
         if len(factors) > 1:
             plt.plot(p[:-1], ".-", label="prediction", alpha=0.5)
             plt.plot(y[:-1], ".-", label="truth", alpha=0.5)
         else:
             plt.plot(p, ".-", label="prediction", alpha=0.5)
             plt.plot(y, ".-", label="truth", alpha=0.5)
     except:
         pass
 
     from cyclic_boosting.plots import _format_groupname_with_type
 
-    feature_group = _format_groupname_with_type(
-        feature.feature_group, feature.feature_type
-    )
+    feature_group = _format_groupname_with_type(feature.feature_group, feature.feature_type)
     plt.xlabel(feature_group)
     plt.legend()
 
 
 __all__ = []
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/plots/_2dplots.py` & `cyclic_boosting-0.1.0/cyclic_boosting/plots/_2dplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
         "No finite samples to plot",
         horizontalalignment="center",
         verticalalignment="center",
         transform=ax.transAxes,
     )
 
 
-def _imshow_factors_2d(
-    ax, factors, nan_factor, nan_uncertainty, title, clim, feature, nan_count
-):
+def _imshow_factors_2d(ax, factors, nan_factor, nan_uncertainty, title, clim, feature, nan_count):
     """Factor plots for unsmoothed and smoothed 2d factors.
     Parameters
     ----------
     ax
         Matplotlib axis where drawing takes place
     factors
         numpy ndarray (two-dimensional) with factor data
@@ -75,24 +73,20 @@
     if n_bins % 2 == 0:
         n_bins += 1
     return np.linspace(-extremal_absolute_factor, extremal_absolute_factor, n_bins + 1)
 
 
 def _plot_factors_histogram(ax, factors, extremal_absolute_factor):
     plt.sca(ax)
-    bin_boundaries = bin_boundaries_for_factor_histograms(
-        len(factors), extremal_absolute_factor
-    )
-    freq, bin_borders = colorful_histogram(
-        ax, factors, bin_boundaries=bin_boundaries, cmap=blue_cyan_green_cmap()
-    )
+    bin_boundaries = bin_boundaries_for_factor_histograms(len(factors), extremal_absolute_factor)
+    freq, bin_borders = colorful_histogram(ax, factors, bin_boundaries=bin_boundaries, cmap=blue_cyan_green_cmap())
     ax.set_title("histogram of smoothed factors")
     plt.xlabel("Factor")
     ticks = 0.5 * bin_borders[1:] + 0.5 * bin_borders[:-1]
-    plt.xticks(ticks, ["{:.1f}".format(x) for x in 2 ** ticks])
+    plt.xticks(ticks, ["{:.1f}".format(x) for x in 2**ticks])
 
 
 def plot_factor_2d(n_bins_finite, feature, grid_item=None):
     """
     Plots a single two dimensional factor plot. For an example see the
     :ref:`cyclic_boosting_analysis_plots`
 
@@ -206,23 +200,17 @@
                 marginal_p,
                 marginal_y,
                 smoothed2d.flatten(),
             ]
         else:
             all_arrays = np.r_[marginal_smoothed, marginal_dev, smoothed2d.flatten()]
         minmax = np.r_[np.min(all_arrays), np.max(all_arrays)]
-        y_axis_range, y_axis_labels = _get_y_axis(
-            np.r_[minmax, marginal_smoothed]
-        )
+        y_axis_range, y_axis_labels = _get_y_axis(np.r_[minmax, marginal_smoothed])
         plt.yticks(y_axis_range, y_axis_labels)
-        plt.title(
-            "Marginal Distribution: {}".format(
-                feature.feature_group[0 if axis == 1 else 1]
-            )
-        )
+        plt.title("Marginal Distribution: {}".format(feature.feature_group[0 if axis == 1 else 1]))
         plt.legend()
 
     plt.sca(plt.subplot(gs[0, 1]))
     if len(factors2d) == 0:
         _no_finite_samples(plt.gca())
     else:
         plot_marginal(1)
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/plots/__init__.py` & `cyclic_boosting-0.1.0/cyclic_boosting/plots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     """
     Guesses a suitable number of histograms for a given number of samples.
     """
     sturges = int(np.ceil(np.log(n) / np.log(2) + 1))
     return np.clip(sturges, 5, 30)
 
 
-def _factor_plots_y_limits(
-    factor_arr, uncert_arr=None, percentage=0.05, ymin_for_zero=1e-3
-):
+def _factor_plots_y_limits(factor_arr, uncert_arr=None, percentage=0.05, ymin_for_zero=1e-3):
     """
     >>> y = np.array([0, 1e-5, 0.1, 0.5, 1, 2, 10, 100, 1e5])
     >>> np.allclose(_factor_plots_y_limits(y), (-1e-3, 1e5 * 1.05))
     True
 
     >>> y = np.array([1e-5, 10])
     >>> np.allclose(_factor_plots_y_limits(y), (1e-5 * 0.95, 10 * 1.05))
@@ -184,15 +182,14 @@
         A tuple with length containing the width and height of the figures.
     use_tightlayout: bool
         If true the tightlayout option of matplotlib is used.
     """
     filepath_or_object = append_extension(file_obj, ".pdf")
     dpi = 200
     with contextlib.closing(PdfPages(filepath_or_object)) as pdf_pages:
-
         plot_observer.check_fitted()
         means, bin_centers, errors, _ = plot_observer.histograms
 
         # do not show for nbinom width mode
         if plot_observer.link_function.__class__ != CBNBinomC:
             plt.figure(figsize=figsize)
             plot_in_sample_diagonal_plot(plot_observer)
@@ -261,40 +258,33 @@
     use_tightlayout: bool
         If true the tightlayout option of matplotlib is used.
     """
     plot_observer.check_fitted()
     if feature_groups_or_ids is None:
         features = plot_observer.features
     else:
-        feature_ids = [
-            create_feature_id(feature_group_or_id)
-            for feature_group_or_id in feature_groups_or_ids
-        ]
+        feature_ids = [create_feature_id(feature_group_or_id) for feature_group_or_id in feature_groups_or_ids]
         features = [plot_observer.features[feature_id] for feature_id in feature_ids]
 
     n_plots = len(features)
     grid = gridspec.GridSpec(int(np.ceil(n_plots / features_per_row)), features_per_row)
 
     for i, feature in enumerate(features):
-        _plot_one_feature_group(
-            plot_observer, grid[i], feature, binners, use_tightlayout, plot_yp=plot_yp
-        )
+        _plot_one_feature_group(plot_observer, grid[i], feature, binners, use_tightlayout, plot_yp=plot_yp)
 
 
 def _format_groupname_with_type(feature_group, feature_type):
     name = ", ".join(feature_group)
     if feature_type is None:
         return name
     else:
         return "{0} ({1})".format(name, feature_type)
 
 
-def _plot_one_feature_group(
-    plot_observer, grid_item, feature, binners=None, use_tightlayout=True, plot_yp=True
-):
+def _plot_one_feature_group(plot_observer, grid_item, feature, binners=None, use_tightlayout=True, plot_yp=True):
     if len(feature.feature_group) == 1:
         # treatment of one-dimensional features
         plt.subplot(grid_item)
         plot_factor_1d(
             feature,
             bin_bounds=get_bin_bounds(binners, feature.feature_group[0]),
             link_function=plot_observer.link_function,
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/plots/plot_utils.py` & `cyclic_boosting-0.1.0/cyclic_boosting/plots/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     rcParams["font.size"] = 20
     rcParams["legend.fontsize"] = "small"
     rcParams["axes.labelsize"] = "small"
     rcParams["axes.titlesize"] = "medium"
     rcParams["xtick.labelsize"] = "small"
     rcParams["ytick.labelsize"] = "small"
 
-    rcParams["image.interpolation"] = 'antialiased'
+    rcParams["image.interpolation"] = "antialiased"
 
     with mpl.rc_context(rcParams):
         yield
 
 
 nbpy_style = utils.generator_to_decorator(_nbpy_style)
 nbpy_style_context = contextlib.contextmanager(_nbpy_style)
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/price.py` & `cyclic_boosting-0.1.0/cyclic_boosting/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     one list of feature_ids.
     """
     if standard_feature_groups is None:
         raise ValueError("Pass at least one feature in `standard_feature_groups`.")
     standard_feature_groups = [create_feature_id(fg) for fg in standard_feature_groups]
     if external_feature_groups is not None:
         external_feature_groups = [
-            create_feature_id(exfg, default_type=FeatureTypes.external)
-            for exfg in external_feature_groups
+            create_feature_id(exfg, default_type=FeatureTypes.external) for exfg in external_feature_groups
         ]
         _check_feature_groups(standard_feature_groups, external_feature_groups)
         return standard_feature_groups + external_feature_groups
     else:
         _check_feature_groups(standard_feature_groups, external_feature_groups)
         return standard_feature_groups
 
@@ -139,20 +138,15 @@
     else:
         l = start_values
 
     for i in range(maximal_iterations):
         l_new, jac, hess = newton_step(l, *args)
         finite = np.isfinite(jac) & np.isfinite(hess) & np.isfinite(l_new)
         valid = valid & finite
-        converged = (
-            (np.abs(jac) < epsilon)
-            | (np.abs(l - x_l) < epsilon)
-            | (np.abs(x_r - l) < epsilon)
-            | (~valid)
-        )
+        converged = (np.abs(jac) < epsilon) | (np.abs(l - x_l) < epsilon) | (np.abs(x_r - l) < epsilon) | (~valid)
         if np.all(converged):
             break
         x_l[valid & (jac < 0)] = l[valid & (jac < 0)]
         x_r[valid & (jac >= 0)] = l[valid & (jac >= 0)]
 
         index = np.full_like(valid, False)
         index[valid] = (l_new[valid] > x_r[valid]) | (l_new[valid] < x_l[valid])
@@ -191,41 +185,31 @@
     l1_ = l1_[lex_binnumbers, :]  # noqa
     l1 = l1_[:, 0]  # noqa
     log_l1 = l1_[:, 1]  # noqa
 
     mu = evaluate("p * exp((k * l1) * log_x)")  # noqa
     w = k * log_x  # noqa
 
-    bin_counts = np.bincount(lex_binnumbers, minlength=minlength)[  # noqa
-        lex_binnumbers
-    ]
+    bin_counts = np.bincount(lex_binnumbers, minlength=minlength)[lex_binnumbers]  # noqa
     # wolfram alpha: jacobian matrix ((y - p * x ** (l * k))^2 * s + ((l*k - c)^2 +
     # (l - 1)^2 + log(l)^2 + log(l*k / c)^2) / v) with respect to (l)
-    jac_prior = evaluate(
-        "2 * (k * (k * l1 - prior) + l1 - 1 + (log_k_prior + 2 * log_l1) / l1) / var_l / bin_counts"
-    )
+    jac_prior = evaluate("2 * (k * (k * l1 - prior) + l1 - 1 + (log_k_prior + 2 * log_l1) / l1) / var_l / bin_counts")
 
     jac_data = evaluate("- (2 * w * mu * (y - mu)) * s")
-    jacobian = np.bincount(
-        lex_binnumbers, weights=jac_data + jac_prior, minlength=minlength
-    )
+    jacobian = np.bincount(lex_binnumbers, weights=jac_data + jac_prior, minlength=minlength)
 
     if only_jac:
         return jacobian
 
     # wolfram alpha: hessian matrix ((y - p * x ** (l * k))^2 * s + ((l*k - c)^2 +
     # (l - 1)^2 + log(l)^2 + log(l*k / c)^2) / v) with respect to (l)
-    hess_prior = evaluate(
-        "2 * (k * k + 1 + (2 - (log_k_prior + 2 * log_l1) ) / l1 / l1) / var_l / bin_counts"
-    )
+    hess_prior = evaluate("2 * (k * k + 1 + (2 - (log_k_prior + 2 * log_l1) ) / l1 / l1) / var_l / bin_counts")
 
     hess_data = evaluate("(2 * w * w * mu * mu) * s + w * jac_data")
-    hessian = np.bincount(
-        lex_binnumbers, weights=hess_data + hess_prior, minlength=minlength
-    )
+    hessian = np.bincount(lex_binnumbers, weights=hess_data + hess_prior, minlength=minlength)
 
     lnew = np.full_like(l, np.nan)
     m_non_zero = hessian != 0
     lnew[m_non_zero] = l[m_non_zero] - jacobian[m_non_zero] / hessian[m_non_zero]
 
     return lnew, jacobian, hessian
 
@@ -251,17 +235,15 @@
         a=1.0,
         c=0.0,
     ):
         self.standard_feature_groups = standard_feature_groups
         self.external_feature_groups = external_feature_groups
         self.prior_exponent_colname = prior_exponent_colname
 
-        feature_id_list = combine_lists_of_feature_groups(
-            standard_feature_groups, external_feature_groups
-        )
+        feature_id_list = combine_lists_of_feature_groups(standard_feature_groups, external_feature_groups)
 
         self.external_colname = external_colname
 
         CBNBinomRegressor.__init__(
             self,
             feature_groups=feature_id_list,
             feature_properties=feature_properties,
@@ -352,17 +334,15 @@
         """
         if feature.feature_type == FeatureTypes.external:
             _logger.debug("Price Feature {}".format(feature.feature_group))
             expo, variance = self._calc_parameters_exponent(feature, y, pred)
             return expo, variance
         else:
             _logger.debug("Demand Feature {}".format(feature.feature_group))
-            return CBNBinomRegressor.calc_parameters(
-                self, feature, y, pred, None
-            )
+            return CBNBinomRegressor.calc_parameters(self, feature, y, pred, None)
 
     def _calc_parameters_exponent(self, feature, y, pred):
         """Calculates exponents and uncertainties
         for each bin of a feature group.
 
         Parameters
         ----------
@@ -382,17 +362,15 @@
         lex_binnumbers = feature.lex_binned_data
         pred_factors = self.unlink_func(pred.factors())
         pred_expos = pred.exponents()
         base = pred.base()
         prior_exponents = pred.prior_exponents()
 
         bounds_l = np.zeros(feature.n_bins, dtype=np.float64)
-        feature.bounds_r = self.starting_bound_bisect * np.ones(
-            feature.n_bins, dtype=np.float64
-        )
+        feature.bounds_r = self.starting_bound_bisect * np.ones(feature.n_bins, dtype=np.float64)
         start_values = np.ones(feature.n_bins, dtype=np.float64)
 
         p = self.unlink_func(pred.predict_link())
 
         log_k_prior = evaluate("log(pred_expos / prior_exponents)")
         a = self.a
         c = self.c
@@ -425,17 +403,15 @@
         return self.unlink_func(pred.predict_link())
 
     def predict_extended(self, X, influence_categories):
         self._check_fitted()
         self._init_external_column(X, False)
 
         prediction_link = self._get_prior_predictions(X)
-        pred = CBLinkPredictions(
-            prediction_link, self._get_prior_exponent(X), self.external_col
-        )
+        pred = CBLinkPredictions(prediction_link, self._get_prior_exponent(X), self.external_col)
 
         for feature in self.features:
             feature_predictions = self._pred_feature(X, feature, is_fit=False)
             pred.update_predictions(feature_predictions, feature, influence_categories)
         return pred
 
     def fit(self, X, y=None, fit_mode=0):
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/regression.py` & `cyclic_boosting-0.1.0/cyclic_boosting/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     # beta_posterior. Therefore we omit calculating the median and take the
     # mean instead (since mean -> median for large values of alpha_posterior
     # and beta_posterior).
 
     noncritical_posterior = (alpha_posterior <= 1e12) & (beta_posterior <= 1e12)
     # Median of the gamma distribution
     posterior_gamma = (
-        scipy.special.gammaincinv(alpha_posterior[noncritical_posterior], 0.5)
-        / beta_posterior[noncritical_posterior]
+        scipy.special.gammaincinv(alpha_posterior[noncritical_posterior], 0.5) / beta_posterior[noncritical_posterior]
     )
 
     factors = alpha_posterior / beta_posterior
     factors[noncritical_posterior] = posterior_gamma
     return np.log(factors)
 
 
@@ -64,16 +63,15 @@
     for regression problems with a target range of: :math:`0 \leq y < \infty`.
     """
 
     def _check_y(self, y):
         """Check that y has no negative values."""
         if not (y >= 0.0).all():
             raise ValueError(
-                "The target y must be positive semi-definite "
-                "and not NAN. y[~(y>=0)] = {0}".format(y[~(y >= 0)])
+                "The target y must be positive semi-definite " "and not NAN. y[~(y>=0)] = {0}".format(y[~(y >= 0)])
             )
 
     @abc.abstractmethod
     def calc_parameters(self, feature, y, pred, prefit_data):
         raise NotImplementedError("implement in subclass")
 
     @abc.abstractmethod
@@ -115,15 +113,14 @@
         smoother_choice=None,
         output_column=None,
         learn_rate=None,
         a=1.0,
         c=0.0,
         aggregate=True,
     ):
-
         CyclicBoostingBase.__init__(
             self,
             feature_groups=feature_groups,
             feature_properties=feature_properties,
             weight_column=weight_column,
             prior_prediction_column=prior_prediction_column,
             minimal_loss_change=minimal_loss_change,
@@ -139,20 +136,20 @@
         self.c = c
 
     def precalc_parameters(self, feature, y, pred):
         pass
 
     def calc_parameters(self, feature, y, pred, prefit_data):
         prediction_link = pred.predict_link()
-        weights = self.weights
+        weights = self.weights  # noqa: F841
         lex_binnumbers = feature.lex_binned_data
         minlength = feature.n_bins
-        prediction = self.unlink_func(prediction_link)
-        a = self.a
-        c = self.c
+        prediction = self.unlink_func(prediction_link)  # noqa: F841
+        a = self.a  # noqa: F841
+        c = self.c  # noqa: F841
 
         w = numexpr.evaluate("weights * y / (a + c * prediction)")
         alpha = np.bincount(lex_binnumbers, weights=w, minlength=minlength)
 
         w = numexpr.evaluate("weights * prediction / (a + c * prediction)")
         beta = np.bincount(lex_binnumbers, weights=w, minlength=minlength)
 
@@ -165,26 +162,22 @@
 
     As Poisson regressor, it is a special case of the more general negative
     binomial regressor :class:`~.CBNBinomRegressor`, assuming *purely*
     Poisson-distributed target values.
     """
 
     def precalc_parameters(self, feature, y, pred):
-        return np.bincount(
-            feature.lex_binned_data, weights=y * self.weights, minlength=feature.n_bins
-        )
+        return np.bincount(feature.lex_binned_data, weights=y * self.weights, minlength=feature.n_bins)
 
     def calc_parameters(self, feature, y, pred, prefit_data):
         prediction = self.unlink_func(pred.predict_link())
 
         prediction_sum_of_bins = np.bincount(
             feature.lex_binned_data,
             weights=self.weights * prediction,
             minlength=feature.n_bins,
         )
 
-        return _calc_factors_and_uncertainties(
-            alpha=prefit_data, beta=prediction_sum_of_bins, link_func=self.link_func
-        )
+        return _calc_factors_and_uncertainties(alpha=prefit_data, beta=prediction_sum_of_bins, link_func=self.link_func)
 
 
 __all__ = ["get_gamma_priors", "CBPoissonRegressor", "CBNBinomRegressor"]
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/base.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/base.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/extrapolate.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/extrapolate.py`

 * *Files identical despite different names*

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/meta_smoother.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/meta_smoother.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,15 @@
             self.norm_ = np.sum(y * w) / weightsum
         else:
             self.norm_ = 0
 
         if not np.isfinite(self.norm_):
             _logger.info(
                 "The norm in smoother {0} is not finite: "
-                "norm= {1}; weights= {2}; target= {3}".format(
-                    self.__class__.__name__, self.norm_, X_for_smoother, y
-                )
+                "norm= {1}; weights= {2}; target= {3}".format(self.__class__.__name__, self.norm_, X_for_smoother, y)
             )
             self.norm_ = 0.0
 
     def fit(self, X_for_smoother, y):
         self.calc_norm(X_for_smoother, y)
         self.smoother.fit(X_for_smoother, y - self.norm_)
 
@@ -168,21 +166,17 @@
             The ``k + 1`` column are the weights of these x-values, while
             the ``k + 2`` column contains the uncertainties.
 
         smoothed_y: :class:`numpy.ndarray`
              Array that contains the result of the subsmoother.
         """
         if not_interpolating(self.reg_type):
-            selected_events = utils.not_seen_events(
-                X_for_smoother[:, : self.ndim_], self.bin_weights_, self.n_bins_
-            )
+            selected_events = utils.not_seen_events(X_for_smoother[:, : self.ndim_], self.bin_weights_, self.n_bins_)
         elif not_extrapolating(self.reg_type):
-            selected_events = _selected_events_interpolating(
-                X_for_smoother, self.ndim_, self.n_bins_
-            )
+            selected_events = _selected_events_interpolating(X_for_smoother, self.ndim_, self.n_bins_)
         else:
             return smoothed_y
 
         smoothed_y = np.asarray(smoothed_y, dtype=np.float64)
         smoothed_y[selected_events] = np.nan
         return smoothed_y
 
@@ -191,17 +185,15 @@
         self.smoother.fit(X_for_smoother, y)
 
     def predict(self, X_for_smoother):
         smoothed_y = self.smoother.predict(X_for_smoother)
         return self.apply_cut(X_for_smoother, smoothed_y)
 
 
-class NormalizationRegressionTypeSmoother(
-    NormalizationSmoother, RegressionTypeSmoother
-):
+class NormalizationRegressionTypeSmoother(NormalizationSmoother, RegressionTypeSmoother):
     """Meta-smoother to constrain all values according to their
     :class:`~cyclic_boosting.smoothing.RegressionType` from the ``predict`` method
     of the subsmoother.
 
     Parameters
     ----------
 
@@ -291,17 +283,15 @@
         if np.sum(~cond_lower) > 0:
             self.smoother_upper.fit(X_for_smoother[~cond_lower], y[~cond_lower])
             self.smoother_upper_fitted = True
         assert self.smoother_upper_fitted or self.smoother_lower_fitted
 
     def predict(self, X_for_smoother):
         if not self.smoother_upper_fitted and not self.smoother_lower_fitted:
-            raise ValueError(
-                "The {} has not been fitted!".format(self.__class__.__name__)
-            )
+            raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
 
         cond_lower = self._split_condition(X_for_smoother)
         pred = np.ones(len(X_for_smoother)) * self.nan_representation
         if self.smoother_lower_fitted and np.sum(cond_lower) > 0:
             pred[cond_lower] = self.smoother_lower.predict(X_for_smoother[cond_lower])
         if self.smoother_upper_fitted and np.sum(~cond_lower) > 0:
             pred[~cond_lower] = self.smoother_upper.predict(X_for_smoother[~cond_lower])
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/multidim.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/multidim.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,36 +36,29 @@
     :type `n_bins_`: :class:`numpy.ndarray` (int64, shape `(n_dims + x,)`)
 
     For examples, see the subclass :class:`BinValuesSmoother`.
     """
 
     def predict(self, X):
         if not hasattr(self, "n_bins_"):
-            raise ValueError(
-                'Please call the method "fit" before "predict" and '
-                '"set_n_bins" in your "fit" method'
-            )
+            raise ValueError('Please call the method "fit" before "predict" and ' '"set_n_bins" in your "fit" method')
 
         if self._bin_steps is None:
             self.n_bins_ = self.n_bins_[: X.shape[1]]
             self._bin_steps = utils.bin_steps(self.n_bins_)
 
         binnos = X
         binnos_round = np.asarray(np.floor(X), dtype=int)
         is_valid = np.all(
-            np.isfinite(binnos)
-            & (binnos >= 0)
-            & (binnos_round < (self.n_bins_[None, :])),
+            np.isfinite(binnos) & (binnos >= 0) & (binnos_round < (self.n_bins_[None, :])),
             axis=1,
         )
 
         pred = utils.nans(len(binnos))
-        pred[is_valid] = self.smoothed_y_[
-            np.dot(binnos_round[is_valid], self._bin_steps[1:])
-        ]
+        pred[is_valid] = self.smoothed_y_[np.dot(binnos_round[is_valid], self._bin_steps[1:])]
 
         return pred
 
 
 class BinValuesSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     """Smoother of multidimensional bins that outputs the saved bin values of
     y (as received from the profile function in the fit) as the prediction.
@@ -118,17 +111,15 @@
         """Restore state from the unpickled state values."""
         for elem in self.elems:
             if elem in state and state[elem] is not None:
                 state[elem] = state[elem].toarray()[0, :]
         self.__dict__.update(state)
 
 
-class RegularizeToPriorExpectationSmoother(
-    AbstractBinSmoother, PredictingBinValueMixin
-):
+class RegularizeToPriorExpectationSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     r"""Smoother of multidimensional bins regularizing values with uncertainties
     to a prior expectation.
 
     For details, see :func:`cyclic_boosting.utils.regularize_to_prior_expectation`.
 
     :param prior_expectation: The prior dominate the regularized value if the
         uncertainties are large.
@@ -200,17 +191,15 @@
         is below the threshold, the global measurement replaces the factor.
         Internally :func:`cyclic_boosting.utils.regularize_to_prior_expectation`
         is used.
     :type threshold: float
     """
 
     def __init__(self, threshold=2.5):
-        RegularizeToPriorExpectationSmoother.__init__(
-            self, prior_expectation=1, threshold=threshold
-        )
+        RegularizeToPriorExpectationSmoother.__init__(self, prior_expectation=1, threshold=threshold)
 
 
 class WeightedMeanSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     r"""Smoother for multidimensional bins regularizing values with
     uncertainties to the weighted mean.
 
     For details see :func:`cyclic_boosting.utils.regularize_to_error_weighted_mean`.
@@ -235,17 +224,15 @@
     """
 
     def __init__(self, prior_prediction=None):
         self.prior_prediction = prior_prediction
 
     def fit(self, X_for_smoother, y):
         self.set_n_bins(X_for_smoother)
-        self.smoothed_y_ = utils.regularize_to_error_weighted_mean(
-            y, X_for_smoother[:, -1], self.prior_prediction
-        )
+        self.smoothed_y_ = utils.regularize_to_error_weighted_mean(y, X_for_smoother[:, -1], self.prior_prediction)
 
 
 class PriorExpectationMetaSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     """Meta-Smoother that takes another multi-dimensional smoother which
     results are addionally smoothed using
     :func:`cyclic_boosting.utils.regularize_to_prior_expectation`.
 
@@ -338,17 +325,15 @@
             gb = Xp.groupby(gb_cols)[self.n_dim].sum()
             Xp = Xp[gb_cols].merge(gb.reset_index(), how="left", on=gb_cols)
             mask = Xp[self.n_dim].values > 0
             X_for_smoother = X_for_smoother[mask]
             y = y[mask]
         X = pd.DataFrame(np.c_[X_for_smoother, y])
         self.group_cols = list(range(self.n_group_columns))
-        self.gb = X.groupby(self.group_cols, sort=False).apply(
-            _fit_est_on_group, self.n_group_columns, self.est
-        )
+        self.gb = X.groupby(self.group_cols, sort=False).apply(_fit_est_on_group, self.n_group_columns, self.est)
 
     def predict(self, X):
         X = pd.DataFrame(X)
         pred = X.groupby(self.group_cols, sort=False)[X.columns[-1]].transform(
             _predict_groups, self.gb, self.n_group_columns
         )
         return pred.values
@@ -377,16 +362,15 @@
     :func:`cyclic_boosting.utils.neutralize_one_dim_influence`.
     """
 
     def __init__(self, est):
         self.est = est
 
     def fit(self, X_for_smoother, y):
-        """Fit the transformer to training samples.
-        """
+        """Fit the transformer to training samples."""
         d = X_for_smoother.shape[1] - 2
         if d < 2:
             raise ValueError("You need at least 4 columns for multidim smoothing.")
 
         # We get the y values as 1d array, hence we have to reshape it into
         # the correct 2d array
         new_shape = np.max(X_for_smoother[:, :2], axis=0).astype(np.int64) + 1
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/onedim.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/onedim.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,18 @@
 
     For examples, see the subclasses :class:`BinValuesSmoother` and
     :class:`BinKernelSmoother`.
     """
 
     def predict(self, X):
         if not hasattr(self, "smoothed_y_"):
-            raise ValueError(
-                "The {} has not been fitted!".format(self.__class__.__name__)
-            )
+            raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
         binnos = X[:, 0]
         binnos_round = np.asarray(np.rint(binnos), dtype=np.int64)
-        is_valid = (
-            np.isfinite(binnos)
-            & (binnos >= 0)
-            & (binnos_round < (len(self.smoothed_y_)))
-        )
+        is_valid = np.isfinite(binnos) & (binnos >= 0) & (binnos_round < (len(self.smoothed_y_)))
 
         pred = utils.nans(len(binnos))
         pred[is_valid] = self.smoothed_y_[binnos_round[is_valid]]
         return pred
 
 
 class BinValuesSmoother(AbstractBinSmoother, PredictingBinValueMixin):
@@ -104,17 +98,15 @@
     def __setstate__(self, state):
         """Restore state from the unpickled state values."""
         if self.elem in state and state[self.elem] is not None:
             state[self.elem] = state[self.elem].toarray()[0, :]
         self.__dict__.update(state)
 
 
-class RegularizeToPriorExpectationSmoother(
-    AbstractBinSmoother, PredictingBinValueMixin
-):
+class RegularizeToPriorExpectationSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     r"""Smoother of one-dimensional bins regularizing values with uncertainties
     to a prior expectation.
 
     :param prior_expectation: The prior dominate the regularized value if the
         uncertainties are large.
     :type prior_expectation: :class:`numpy.ndarray` (float64, dim=1) or float
 
@@ -174,17 +166,15 @@
     :param threshold: threshold in terms of sigma.
         If the significance of a factor is below the threshold, the global
         measurement replaces the factor.
     :type threshold: float
     """
 
     def __init__(self, threshold=2.5):
-        RegularizeToPriorExpectationSmoother.__init__(
-            self, prior_expectation=1, threshold=threshold
-        )
+        RegularizeToPriorExpectationSmoother.__init__(self, prior_expectation=1, threshold=threshold)
 
 
 class WeightedMeanSmoother(AbstractBinSmoother, PredictingBinValueMixin):
     r"""Smoother for one-dimensional bins regularizing values with
     uncertainties to the weighted mean or a user defined value.
 
     :param prior_prediction: If the `prior_prediction` is specified, all values
@@ -223,17 +213,15 @@
 
     """
 
     def __init__(self, prior_prediction=None):
         self.prior_prediction = prior_prediction
 
     def fit(self, X_for_smoother, y):
-        self.smoothed_y_ = utils.regularize_to_error_weighted_mean(
-            y, X_for_smoother[:, 2], self.prior_prediction
-        )
+        self.smoothed_y_ = utils.regularize_to_error_weighted_mean(y, X_for_smoother[:, 2], self.prior_prediction)
 
 
 class OrthogonalPolynomialSmoother(AbstractBinSmoother):
     """A polynomial fit that uses orthogonal polynomials as basis functions.
 
     Ansatz, see Blobel (http://www.desy.de/~blobel/eBuch.pdf)
     """
@@ -250,17 +238,15 @@
         )
 
         return self
 
     def predict(self, X):
         assert X.ndim == 2
         if not hasattr(self, "pp_"):
-            raise ValueError(
-                "The {} has not been fitted!".format(self.__class__.__name__)
-            )
+            raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
         x = np.ascontiguousarray(X[:, 0], dtype=np.float64)
         x[x < self.minimal_x] = self.minimal_x
         x[x > self.maximal_x] = self.maximal_x
         y = cy_apply_orthogonal_poly_fit_equidistant(x, self.pp_, self.n_degrees_)
         return y
 
 
@@ -280,26 +266,18 @@
 
 
 def _seasonality_first_order(x, c_const, c_sin, c_cos):
     return c_const + c_sin * np.sin(x) + c_cos * np.cos(x)
 
 
 def _seasonality_second_order(x, c_const, c_sin_1x, c_cos_1x, c_sin_2x, c_cos_2x):
-    return (
-        c_const
-        + c_sin_1x * np.sin(x)
-        + c_cos_1x * np.cos(x)
-        + c_sin_2x * np.sin(2 * x)
-        + c_cos_2x * np.cos(2 * x)
-    )
+    return c_const + c_sin_1x * np.sin(x) + c_cos_1x * np.cos(x) + c_sin_2x * np.sin(2 * x) + c_cos_2x * np.cos(2 * x)
 
 
-def _seasonality_third_order(
-    x, c_const, c_sin_1x, c_cos_1x, c_sin_2x, c_cos_2x, c_sin_3x, c_cos_3x
-):
+def _seasonality_third_order(x, c_const, c_sin_1x, c_cos_1x, c_sin_2x, c_cos_2x, c_sin_3x, c_cos_3x):
     return (
         c_const
         + c_sin_1x * np.sin(x)
         + c_cos_1x * np.cos(x)
         + c_sin_2x * np.sin(2 * x)
         + c_cos_2x * np.cos(2 * x)
         + c_sin_3x * np.sin(3 * x)
@@ -360,58 +338,49 @@
     frequency_: float
         Frequency calculated from the maximum binnumber.
 
     par_: numpy.ndarray
         Parameters from the fit.
     """
 
-    def __init__(
-        self, offset_tozero=True, order=1, custom_fit_function=None, fallback_value=0.0
-    ):
+    def __init__(self, offset_tozero=True, order=1, custom_fit_function=None, fallback_value=0.0):
         self.offset_tozero = offset_tozero
         self.order = order
         self.custom_fit_function = custom_fit_function
         if custom_fit_function is None:
             self.fit_function = _choose_default_fit_function(order)
         else:
             self.fit_function = custom_fit_function
             if order != 1:
-                warnings.warn(
-                    "You specified a `custom_fit_function` thus "
-                    "the `order` parameter will be ignored!"
-                )
+                warnings.warn("You specified a `custom_fit_function` thus " "the `order` parameter will be ignored!")
         self.converged = None
         self.fallback_value = fallback_value
 
     def transform_X(self, X):
         return 2 * np.pi * X[:, 0] * self.frequency_
 
     def fit(self, X_for_smoother, y):
         self.frequency_ = 1.0 / len(X_for_smoother)
         xdata = self.transform_X(X_for_smoother)
         try:
-            self.par_, _ = scipy.optimize.curve_fit(
-                self.fit_function, xdata=xdata, ydata=y, sigma=X_for_smoother[:, 2]
-            )
+            self.par_, _ = scipy.optimize.curve_fit(self.fit_function, xdata=xdata, ydata=y, sigma=X_for_smoother[:, 2])
             if self.offset_tozero:
                 self.par_[0] = 0.0
         except TypeError:
             warnings.warn("Seasonal Smoother did not converge. Fallback value is used")
             self.converged = False
         else:
             self.converged = True
 
         return self
 
     def predict(self, X):
         if self.converged or self.converged is None:
             if not hasattr(self, "par_"):
-                raise ValueError(
-                    "The {} has not been fitted!".format(self.__class__.__name__)
-                )
+                raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
             return self.fit_function(self.transform_X(X), *self.par_)
         else:
             return np.ones(len(X), dtype=np.float64) * self.fallback_value
 
 
 class SeasonalLassoSmoother(AbstractBinSmoother):
     """
@@ -464,17 +433,15 @@
 
     def _fallback_predict(self, X):
         return np.zeros(len(X), dtype=np.float64)
 
     def predict(self, X):
         if not self.fallback_mode:
             if not self.est:
-                raise ValueError(
-                    "The {} has not been fitted!".format(self.__class__.__name__)
-                )
+                raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
             Xt = self.prepare_X(X[:, 0])
             return self.est.predict(Xt)
         else:
             return self._fallback_predict(X)
 
     def fit(self, X_for_smoother, y):
         self.max_bin = X_for_smoother[-1, 0]
@@ -584,17 +551,15 @@
             s=self.s,
         )
 
         return self
 
     def predict(self, X):
         if not hasattr(self, "spline_"):
-            raise ValueError(
-                "The {} has not been fitted!".format(self.__class__.__name__)
-            )
+            raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
         return self.spline_(np.asarray(X[:, 0], dtype=np.float64))
 
 
 class PolynomialSmoother(AbstractBinSmoother):
     r"""Least squares polynomial fit.
 
     Fit a polynomial ``p(x) = p[0] * x**deg + ... + p[deg]`` of degree `deg`
@@ -635,17 +600,15 @@
             self.k,
             w=w,
         )
         return self
 
     def predict(self, X):
         if not hasattr(self, "coefficients_"):
-            raise ValueError(
-                "The {} has not been fitted!".format(self.__class__.__name__)
-            )
+            raise ValueError("The {} has not been fitted!".format(self.__class__.__name__))
         x = np.asarray(X[:, 0], dtype=np.float64)
         return np.polyval(self.coefficients_, x)
 
 
 class LinearSmoother(PolynomialSmoother):
     r"""Least squares linear fit (special case of PolynomialSmoother).
 
@@ -723,16 +686,15 @@
             y = y.astype(np.float64)
             t = np.asanyarray(self.interior_knots, dtype=np.float64)
             w = X[:, 1]
             k = self.degree
             self.fitted_spline = scipy.interpolate.LSQUnivariateSpline(x, y, t, w, k=k)
         else:
             raise ValueError(
-                "Spline degree equals {}. Must be <= 5 and less"
-                " than the available data points".format(self.degree)
+                "Spline degree equals {}. Must be <= 5 and less" " than the available data points".format(self.degree)
             )
         return self
 
     def predict(self, X):
         if self.fitted_spline is None:
             raise ValueError("LSQUnivariateSpline has not been fitted!")
         return self.fitted_spline(X.astype(np.float64)[:, 0])
@@ -772,17 +734,15 @@
         self.increasing = increasing
 
     def fit(self, X_for_smoother, y):
         X = X_for_smoother.astype(np.float64)
         sigma = X[:, 2]
         sigma = np.where(sigma > 0, sigma, 1e12)
         w = 1.0 / (sigma * sigma)
-        self.est_ = sklearn.isotonic.IsotonicRegression(
-            increasing=self.increasing, out_of_bounds="clip"
-        )
+        self.est_ = sklearn.isotonic.IsotonicRegression(increasing=self.increasing, out_of_bounds="clip")
         self.est_.fit(X[:, 0], y.astype(np.float64), sample_weight=w)
         return self
 
     def predict(self, X):
         if self.est_ is None:
             raise ValueError("IsotonicRegressor has not been fitted!")
         return self.est_.predict(X.astype(np.float64)[:, 0])
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/smoothing/orthofit.py` & `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/orthofit.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,35 @@
 import numpy as np
 
 N_COEFFICIENTS = 5
 N_PARAMETERS = 21
 
 
 @nb.njit()
-def cy_orthogonal_poly_fit_equidistant(
-    binnos: nb.float64[:], y_values: nb.float64[:], y_errors: nb.float64[:]
-):
+def cy_orthogonal_poly_fit_equidistant(binnos: nb.float64[:], y_values: nb.float64[:], y_errors: nb.float64[:]):
     weights = np.empty(y_errors.shape[0])
     parameters = np.empty((N_PARAMETERS, N_COEFFICIENTS))
 
     for j in range(y_errors.shape[0]):
         weights[j] = 1.0 / (y_errors[j] * y_errors[j])
 
     n_degrees = fit_orthogonal_poly_(binnos, y_values, weights, parameters)
 
-    n_significant_parameters = significant_parameters_(
-        parameters, n_degrees, len(y_values)
-    )
-    n_degrees = reduce_to_signifcant_parameters(
-        n_significant_parameters, parameters, n_degrees, len(y_values)
-    )
+    n_significant_parameters = significant_parameters_(parameters, n_degrees, len(y_values))
+    n_degrees = reduce_to_signifcant_parameters(n_significant_parameters, parameters, n_degrees, len(y_values))
     return parameters, n_degrees
 
 
 @nb.njit()
 def fit_orthogonal_poly_(
     x: nb.float64[:],
     y: nb.float64[:],
     weights: nb.float64[:],
     parameters: nb.float64[:],
 ) -> nb.float64:
-
     n_supporting_points = x.shape[0]
     alpha = 0.0
     beta = 0.0
     gamma = 0.0
     delta = 0.0
     scratch = np.empty((2, x.shape[0]))
 
@@ -76,17 +69,15 @@
         beta = 0.0
         for j in range(0, n_supporting_points):
             alpha += weights[j] * x[j] * scratch[3 - ii - 1, j] * scratch[3 - ii - 1, j]
             beta += weights[j] * x[j] * scratch[ii - 1, j] * scratch[3 - ii - 1, j]
 
         gamma = 0.0
         for j in range(0, n_supporting_points):
-            scratch[ii - 1, j] = (x[j] - alpha) * scratch[
-                3 - ii - 1, j
-            ] - beta * scratch[ii - 1, j]
+            scratch[ii - 1, j] = (x[j] - alpha) * scratch[3 - ii - 1, j] - beta * scratch[ii - 1, j]
             gamma += weights[j] * scratch[ii - 1, j] * scratch[ii - 1, j]
 
         if gamma != 0.0:
             gamma = 1.0 / np.sqrt(gamma)
 
         delta = 0.0
         for j in range(0, n_supporting_points):
@@ -135,18 +126,15 @@
     elif value < lower:
         return lower
     elif value > upper:
         return upper
 
 
 @nb.njit()
-def reduce_to_signifcant_parameters(
-    n_signi_par, parameters, n_degrees, n_supporting_points
-):
-
+def reduce_to_signifcant_parameters(n_signi_par, parameters, n_degrees, n_supporting_points):
     n_degrees = min(n_degrees, n_signi_par)
     if n_degrees == n_supporting_points:
         if n_supporting_points > 2:
             n_degrees = custom_clip(int(n_supporting_points * 0.2), 2, N_PARAMETERS)
         else:
             n_degrees = 1
 
@@ -169,13 +157,12 @@
         values[0] = parameters[0, 2]
         values[1] = 0.0
         y_estimate = parameters[0, 2] * parameters[0, 3]
         j = 1
         for k in range(1, n_degrees):
             j = 3 - j
             values[j - 1] = (
-                (binnos[i] - parameters[k, 0]) * values[2 - j]
-                - parameters[k, 1] * values[j - 1]
+                (binnos[i] - parameters[k, 0]) * values[2 - j] - parameters[k, 1] * values[j - 1]
             ) * parameters[k, 2]
             y_estimate += parameters[k, 3] * values[j - 1]
         result[i] = y_estimate
     return result
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting/utils.py` & `cyclic_boosting-0.1.0/cyclic_boosting/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,32 +232,28 @@
         else:
             n_bins = np.max(finite_bins, axis=0).astype(np.int64) + 1
 
     if binsteps is None:
         binsteps = bin_steps(n_bins)
 
     is_valid = np.isfinite(binnos).all(axis=1)
-    is_valid[is_valid] &= (
-        (binnos[is_valid] >= 0) & (binnos[is_valid] < n_bins[None, :])
-    ).all(axis=1)
+    is_valid[is_valid] &= ((binnos[is_valid] >= 0) & (binnos[is_valid] < n_bins[None, :])).all(axis=1)
 
     if not np.any(is_valid):
         result = np.repeat(0, len(binnos))
     else:
         result = np.repeat(np.product(n_bins), len(binnos))
 
     result[is_valid] = np.dot(np.floor(binnos[is_valid]), binsteps[1:])
 
     if n_bins.prod() >= np.iinfo(np.int32).max:
         _logger.warning(
             "Enumerating multidimensional bins: A multidimensional feature of "
             "shape {n_bins} requires {total_bins} unique bins in total. "
-            "Please consider whether this is what you want.".format(
-                n_bins=n_bins, total_bins=n_bins.prod()
-            )
+            "Please consider whether this is what you want.".format(n_bins=n_bins, total_bins=n_bins.prod())
         )
     result = result.astype(np.int64)
     return result, n_bins
 
 
 @nb.njit()
 def bin_steps(n_bins: nb.int64[:]):
@@ -684,16 +680,15 @@
     elif not hasattr(estimator, "get_params"):
         if not safe:
             return copy.deepcopy(estimator)
         else:
             raise TypeError(
                 "Cannot clone object '%s' (type %s): "
                 "it does not seem to be a scikit-learn estimator as "
-                "it does not implement a 'get_params' methods."
-                % (repr(estimator), type(estimator))
+                "it does not implement a 'get_params' methods." % (repr(estimator), type(estimator))
             )
     klass = estimator.__class__
     new_object_params = estimator.get_params(deep=False)
 
     if hasattr(estimator, "no_deepcopy"):
         no_deepcopy = estimator.no_deepcopy
         for name, param in six.iteritems(new_object_params):
@@ -704,17 +699,15 @@
             new_object_params[name] = clone(param, safe=False)
 
     new_object = klass(**new_object_params)
 
     return new_object
 
 
-def regularize_to_prior_expectation(
-    values, uncertainties, prior_expectation, threshold=2.5
-):
+def regularize_to_prior_expectation(values, uncertainties, prior_expectation, threshold=2.5):
     r"""Regularize values with uncertainties to a prior expectation.
 
     :param values: measured values
     :type values: :class:`numpy.ndarray` (float64, dim=1)
 
     :param uncertainties: uncertainties for the values.
     :type uncertainties: :class:`numpy.ndarray` (float64, dim=1)
@@ -750,15 +743,15 @@
     >>> np.allclose(1 + np.sqrt(((values[-1] - 1) / 0.1)**2 - 2.5**2) * 0.1,
     ...     regularized_values[-1])
     True
     """
     significance = (values - prior_expectation) / uncertainties
     return prior_expectation + uncertainties * np.where(
         np.abs(significance) > threshold,
-        np.sign(significance) * np.sqrt(significance ** 2.0 - threshold ** 2.0),
+        np.sign(significance) * np.sqrt(significance**2.0 - threshold**2.0),
         0,
     )
 
 
 def regularize_to_error_weighted_mean(values, uncertainties, prior_prediction=None):
     r"""Regularize values with uncertainties to the error weighted mean.
 
@@ -974,9 +967,10 @@
     beta = (s_w * s_wxy - s_wx * s_wy) / det
     return alpha, beta
 
 
 def get_feature_column_names(X, exclude_columns=[]):
     features = list(X.columns)
     for col in exclude_columns:
-        if col in features: features.remove(col)
+        if col in features:
+            features.remove(col)
     return features
```

### Comparing `cyclic-boosting-0.0.5/cyclic_boosting.egg-info/PKG-INFO` & `cyclic_boosting-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 Metadata-Version: 2.1
 Name: cyclic-boosting
-Version: 0.0.5
+Version: 0.1.0
+Summary: Implementation of Cyclic Boosting machine learning algorithms
 Author: Blue Yonder GmbH
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: decorator (>=5.1.1,<6.0.0)
+Requires-Dist: hypothesis (>=6.70.0,<7.0.0)
+Requires-Dist: matplotlib (>=1.5.1)
+Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numba-scipy (>=0.3.1,<0.4.0)
+Requires-Dist: numexpr (>=2.5.2)
+Requires-Dist: numpy (>=1.12.1)
+Requires-Dist: pandas (>=0.20.3)
+Requires-Dist: scikit-learn (>=0.18.2)
+Requires-Dist: scipy (==1.7.2) ; python_version < "3.10"
+Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
 
 ## Documentation
 
@@ -26,7 +46,8 @@
 CB_est.fit(X_train, y)
 yhat = CB_est.predict(X_test)
 ```
 
 ## Usage
 
 It can be used in a [scikit-learn](https://scikit-learn.org/stable/)-like fashion, combining a binning method (e.g., [BinNumberTransformer](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/binning/bin_number_transformer.py)) with a Cyclic Boosting estimator (find all estimators in the [init](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/cyclic_boosting/__init__.py)). Usage examples can be found in the [integration tests](https://github.com/Blue-Yonder-OSS/cyclic-boosting/blob/main/tests/test_integration.py).
+
```

