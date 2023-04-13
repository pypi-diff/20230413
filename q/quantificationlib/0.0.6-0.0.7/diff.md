# Comparing `tmp/quantificationlib-0.0.6.tar.gz` & `tmp/quantificationlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantificationlib-0.0.6.tar", last modified: Fri Mar 31 11:38:32 2023, max compression
+gzip compressed data, was "quantificationlib-0.0.7.tar", last modified: Thu Apr 13 14:19:29 2023, max compression
```

## Comparing `quantificationlib-0.0.6.tar` & `quantificationlib-0.0.7.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.014513 quantificationlib-0.0.6/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-03-31 08:18:56.000000 quantificationlib-0.0.6/LICENCE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1759 2023-03-31 11:38:32.014513 quantificationlib-0.0.6/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      605 2023-03-31 11:38:13.000000 quantificationlib-0.0.6/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.002513 quantificationlib-0.0.6/quantificationlib/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      821 2023-03-31 11:38:09.000000 quantificationlib-0.0.6/quantificationlib/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    21959 2023-03-31 11:16:32.000000 quantificationlib-0.0.6/quantificationlib/bag_generator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    14309 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/base.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.006513 quantificationlib-0.0.6/quantificationlib/baselines/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/baselines/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    23684 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/baselines/ac.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9902 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/baselines/cc.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.006513 quantificationlib-0.0.6/quantificationlib/binary/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/binary/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7489 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/binary/debias.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    10493 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/binary/emd.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11269 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/binary/quantiles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       86 2023-03-29 12:43:43.000000 quantificationlib-0.0.6/quantificationlib/cvxpy_installed_solvers.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      626 2023-03-31 08:24:16.000000 quantificationlib-0.0.6/quantificationlib/data_utils.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.006513 quantificationlib-0.0.6/quantificationlib/decomposition/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/decomposition/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9147 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/decomposition/multiclass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15664 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/decomposition/ordinal.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.006513 quantificationlib-0.0.6/quantificationlib/ensembles/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/ensembles/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    28508 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/ensembles/eoq.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.006513 quantificationlib-0.0.6/quantificationlib/estimators/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/estimators/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12799 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/estimators/cross_validation.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6707 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/estimators/ensembles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    42851 2023-03-31 11:31:31.000000 quantificationlib-0.0.6/quantificationlib/estimators/frank_and_hall.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    16148 2023-03-31 11:31:29.000000 quantificationlib-0.0.6/quantificationlib/estimators/ordinal_ddag.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6239 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/estimators/weighted_knn.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.010513 quantificationlib-0.0.6/quantificationlib/metrics/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/metrics/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5832 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/metrics/binary.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11844 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/metrics/multiclass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2684 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/metrics/ordinal.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.010513 quantificationlib-0.0.6/quantificationlib/multiclass/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/multiclass/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    34737 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/multiclass/df.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9077 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/multiclass/em.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    25478 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/multiclass/energy.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12964 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/multiclass/friedman.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7483 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/multiclass/knn.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    29130 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/multiclass/regression.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    19390 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/optimization.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.010513 quantificationlib-0.0.6/quantificationlib/ordinal/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.6/quantificationlib/ordinal/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9803 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/ordinal/ac_ordinal.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    13836 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/ordinal/pdf.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1972 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/ordinal/trees.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15685 2023-03-31 11:16:33.000000 quantificationlib-0.0.6/quantificationlib/search.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.002513 quantificationlib-0.0.6/quantificationlib.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1759 2023-03-31 11:38:31.000000 quantificationlib-0.0.6/quantificationlib.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1932 2023-03-31 11:38:31.000000 quantificationlib-0.0.6/quantificationlib.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-03-31 11:38:31.000000 quantificationlib-0.0.6/quantificationlib.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       64 2023-03-31 11:38:31.000000 quantificationlib-0.0.6/quantificationlib.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       18 2023-03-31 11:38:31.000000 quantificationlib-0.0.6/quantificationlib.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2023-03-31 11:38:32.014513 quantificationlib-0.0.6/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6536 2023-03-31 11:38:04.000000 quantificationlib-0.0.6/setup.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-03-31 11:38:32.014513 quantificationlib-0.0.6/tests/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7564 2023-03-31 08:19:06.000000 quantificationlib-0.0.6/tests/test_binary_quantifiers.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3041 2023-03-31 11:37:23.000000 quantificationlib-0.0.6/tests/test_cv_estimator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5138 2023-03-31 09:53:47.000000 quantificationlib-0.0.6/tests/test_decomposition.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3461 2023-03-31 09:48:33.000000 quantificationlib-0.0.6/tests/test_ensembles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1953 2023-03-31 10:26:42.000000 quantificationlib-0.0.6/tests/test_metrics.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5896 2023-03-31 11:04:10.000000 quantificationlib-0.0.6/tests/test_ordinal_quantifiers.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-03-31 08:18:56.000000 quantificationlib-0.0.7/LICENCE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2108 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      955 2023-04-13 14:17:52.000000 quantificationlib-0.0.7/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      821 2023-04-13 14:18:10.000000 quantificationlib-0.0.7/quantificationlib/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    21959 2023-03-31 11:16:32.000000 quantificationlib-0.0.7/quantificationlib/bag_generator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    14309 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/base.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib/baselines/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/baselines/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    23752 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/baselines/ac.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9902 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/baselines/cc.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/binary/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/binary/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7489 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/binary/debias.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    10493 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/binary/emd.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11269 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/binary/quantiles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       86 2023-03-29 12:43:43.000000 quantificationlib-0.0.7/quantificationlib/cvxpy_installed_solvers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      626 2023-03-31 08:24:16.000000 quantificationlib-0.0.7/quantificationlib/data_utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/decomposition/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/decomposition/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9147 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/decomposition/multiclass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15664 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/decomposition/ordinal.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/ensembles/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ensembles/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    28508 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ensembles/eoq.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/estimators/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/estimators/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12799 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/cross_validation.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6707 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/ensembles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    42851 2023-03-31 11:31:31.000000 quantificationlib-0.0.7/quantificationlib/estimators/frank_and_hall.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    16148 2023-03-31 11:31:29.000000 quantificationlib-0.0.7/quantificationlib/estimators/ordinal_ddag.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6239 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/weighted_knn.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.905383 quantificationlib-0.0.7/quantificationlib/metrics/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/metrics/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5832 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/binary.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11844 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/multiclass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2684 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/ordinal.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.905383 quantificationlib-0.0.7/quantificationlib/multiclass/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    34737 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/df.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9077 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/em.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    25478 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/energy.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12964 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/friedman.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7483 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/knn.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    29130 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/regression.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    19390 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/optimization.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/quantificationlib/ordinal/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ordinal/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9803 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/ac_ordinal.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    13836 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/pdf.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1972 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/trees.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/quantificationlib/plot/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/plot/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2832 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/plot/qlplot.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15685 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/search.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2108 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2029 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       75 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       18 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6550 2023-04-13 14:18:04.000000 quantificationlib-0.0.7/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/tests/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3038 2023-03-31 12:04:50.000000 quantificationlib-0.0.7/tests/test_bag_generators.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7575 2023-04-10 13:16:55.000000 quantificationlib-0.0.7/tests/test_binary_quantifiers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3041 2023-03-31 11:37:23.000000 quantificationlib-0.0.7/tests/test_cv_estimator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5084 2023-04-10 13:38:50.000000 quantificationlib-0.0.7/tests/test_decomposition.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3372 2023-04-10 13:34:32.000000 quantificationlib-0.0.7/tests/test_ensembles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1953 2023-03-31 10:26:42.000000 quantificationlib-0.0.7/tests/test_metrics.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5896 2023-03-31 11:04:10.000000 quantificationlib-0.0.7/tests/test_ordinal_quantifiers.py
```

### Comparing `quantificationlib-0.0.6/LICENCE` & `quantificationlib-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/PKG-INFO` & `quantificationlib-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quantificationlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: quantificationlib: A library for Quantification Learning
 Home-page: https://github.com/AICGijon/quantificationlib
-Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz
 Author: Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz
 Author-email: bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es
 Keywords: quantification,label shift,prevalence estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -18,21 +18,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ![cibadge](https://github.com/aicgijon/quantificationlib/actions/workflows/quantificationlib.yml/badge.svg)
+[![docs](https://img.shields.io/badge/docs-sphinx-blue)](https://aicgijon.github.io/quantificationlib/)
 [![codecov](https://codecov.io/github/AICGijon/quantificationlib/branch/main/graph/badge.svg?token=6Y3SMCVWCD)](https://app.codecov.io/github/AICGijon/quantificationlib)
+[![Downloads PyPI](https://static.pepy.tech/personalized-badge/quantificationlib?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=pypi)](https://pypi.org/project/quantificationlib/)
 
 
 # QuantificationLib
 
 QuantificationLib is an open-source library for quantification learning. 
 
 ### Last updates:
-
+- Adding plots [0.0.7]
 - Initial version of the library released [0.0.6].
 
 ### Installation and documentation
 
 The installation, quick-start guide and documentation are available [here](https://aicgijon.github.io/quantificationlib/).
```

### Comparing `quantificationlib-0.0.6/quantificationlib/__init__.py` & `quantificationlib-0.0.7/quantificationlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # from quantificationlib import ensembles
 # from quantificationlib import estimators
 # from quantificationlib import examples
 # from quantificationlib import metrics
 # from quantificationlib import multiclass
 # from quantificationlib import ordinal
 #
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 # __all__ = [
 #     'baselines',
 #     'binary',
 #     'datasets',
 #     'decomposition',
 #     'ensembles',
```

### Comparing `quantificationlib-0.0.6/quantificationlib/bag_generator.py` & `quantificationlib-0.0.7/quantificationlib/bag_generator.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/base.py` & `quantificationlib-0.0.7/quantificationlib/base.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/baselines/ac.py` & `quantificationlib-0.0.7/quantificationlib/baselines/ac.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,16 @@
         else:
             try:
                 inv_cm = linalg.inv(self.cm_.T)
                 prevalences = inv_cm.dot(prevalences_0)
 
                 prevalences[prevalences < 0] = 0
                 prevalences = prevalences / sum(prevalences)
-
+                prevalences = prevalences.squeeze()
+                
             except np.linalg.LinAlgError:
                 #  inversion fails, looking for a solution that optimizes the selected distance
                 if self.distance == 'HD':
                     self.problem_, prevalences = solve_hd(train_distrib=self.cm_.T, test_distrib=prevalences_0,
                                                           n_classes=n_classes, problem=self.problem_)
                 elif self.distance == 'L2':
                     prevalences = solve_l2(train_distrib=self.cm_.T, test_distrib=prevalences_0,
```

### Comparing `quantificationlib-0.0.6/quantificationlib/baselines/cc.py` & `quantificationlib-0.0.7/quantificationlib/baselines/cc.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/binary/debias.py` & `quantificationlib-0.0.7/quantificationlib/binary/debias.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/binary/emd.py` & `quantificationlib-0.0.7/quantificationlib/binary/emd.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/binary/quantiles.py` & `quantificationlib-0.0.7/quantificationlib/binary/quantiles.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/data_utils.py` & `quantificationlib-0.0.7/quantificationlib/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/decomposition/multiclass.py` & `quantificationlib-0.0.7/quantificationlib/decomposition/multiclass.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/decomposition/ordinal.py` & `quantificationlib-0.0.7/quantificationlib/decomposition/ordinal.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/ensembles/eoq.py` & `quantificationlib-0.0.7/quantificationlib/ensembles/eoq.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/estimators/cross_validation.py` & `quantificationlib-0.0.7/quantificationlib/estimators/cross_validation.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/estimators/ensembles.py` & `quantificationlib-0.0.7/quantificationlib/estimators/ensembles.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/estimators/frank_and_hall.py` & `quantificationlib-0.0.7/quantificationlib/estimators/frank_and_hall.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/estimators/ordinal_ddag.py` & `quantificationlib-0.0.7/quantificationlib/estimators/ordinal_ddag.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/estimators/weighted_knn.py` & `quantificationlib-0.0.7/quantificationlib/estimators/weighted_knn.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/metrics/binary.py` & `quantificationlib-0.0.7/quantificationlib/metrics/binary.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/metrics/multiclass.py` & `quantificationlib-0.0.7/quantificationlib/metrics/multiclass.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/metrics/ordinal.py` & `quantificationlib-0.0.7/quantificationlib/metrics/ordinal.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/df.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/df.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/em.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/em.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/energy.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/energy.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/friedman.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/friedman.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/knn.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/knn.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/multiclass/regression.py` & `quantificationlib-0.0.7/quantificationlib/multiclass/regression.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/optimization.py` & `quantificationlib-0.0.7/quantificationlib/optimization.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/ordinal/ac_ordinal.py` & `quantificationlib-0.0.7/quantificationlib/ordinal/ac_ordinal.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/ordinal/pdf.py` & `quantificationlib-0.0.7/quantificationlib/ordinal/pdf.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/ordinal/trees.py` & `quantificationlib-0.0.7/quantificationlib/ordinal/trees.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib/search.py` & `quantificationlib-0.0.7/quantificationlib/search.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/quantificationlib.egg-info/PKG-INFO` & `quantificationlib-0.0.7/quantificationlib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quantificationlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: quantificationlib: A library for Quantification Learning
 Home-page: https://github.com/AICGijon/quantificationlib
-Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz
 Author: Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz
 Author-email: bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es
 Keywords: quantification,label shift,prevalence estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -18,21 +18,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ![cibadge](https://github.com/aicgijon/quantificationlib/actions/workflows/quantificationlib.yml/badge.svg)
+[![docs](https://img.shields.io/badge/docs-sphinx-blue)](https://aicgijon.github.io/quantificationlib/)
 [![codecov](https://codecov.io/github/AICGijon/quantificationlib/branch/main/graph/badge.svg?token=6Y3SMCVWCD)](https://app.codecov.io/github/AICGijon/quantificationlib)
+[![Downloads PyPI](https://static.pepy.tech/personalized-badge/quantificationlib?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=pypi)](https://pypi.org/project/quantificationlib/)
 
 
 # QuantificationLib
 
 QuantificationLib is an open-source library for quantification learning. 
 
 ### Last updates:
-
+- Adding plots [0.0.7]
 - Initial version of the library released [0.0.6].
 
 ### Installation and documentation
 
 The installation, quick-start guide and documentation are available [here](https://aicgijon.github.io/quantificationlib/).
```

### Comparing `quantificationlib-0.0.6/quantificationlib.egg-info/SOURCES.txt` & `quantificationlib-0.0.7/quantificationlib.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,13 +43,16 @@
 quantificationlib/multiclass/friedman.py
 quantificationlib/multiclass/knn.py
 quantificationlib/multiclass/regression.py
 quantificationlib/ordinal/__init__.py
 quantificationlib/ordinal/ac_ordinal.py
 quantificationlib/ordinal/pdf.py
 quantificationlib/ordinal/trees.py
+quantificationlib/plot/__init__.py
+quantificationlib/plot/qlplot.py
+tests/test_bag_generators.py
 tests/test_binary_quantifiers.py
 tests/test_cv_estimator.py
 tests/test_decomposition.py
 tests/test_ensembles.py
 tests/test_metrics.py
 tests/test_ordinal_quantifiers.py
```

### Comparing `quantificationlib-0.0.6/setup.py` & `quantificationlib-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     long_description_content_type='text/markdown',  # Optional (see note above)
 
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url='https://github.com/AICGijon/quantificationlib',  # Optional
-    download_url='https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.6.tar.gz',
+    download_url='https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz',
 
     author='Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz',
 
     author_email='bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -106,15 +106,15 @@
     #
     #   py_modules=["my_module"],
     #
     packages=find_packages(include=['quantificationlib', 'quantificationlib.*']),  # Required
 
     python_requires='>=3.6',
 
-    install_requires=['scikit-learn', 'cvxpy', 'quadprog', 'scipy', 'numpy', 'ecos', 'statsmodels', 'pandas'],
+    install_requires=['scikit-learn', 'cvxpy', 'quadprog', 'scipy', 'numpy', 'ecos', 'statsmodels', 'pandas', 'matplotlib'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

### Comparing `quantificationlib-0.0.6/tests/test_binary_quantifiers.py` & `quantificationlib-0.0.7/tests/test_binary_quantifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     X_train, X_test = normalize(X_train, X_test)
 
     # classifiers are fitted by each object (all methods will use exactly the same predictions)
     # but they checked whether the estimator is already fitted (by a previous object) or not
     estimator = RandomForestClassifier(n_estimators=100, random_state=master_seed, class_weight='balanced')
 
     #  AC
-    ac = AC(estimator_train=estimator, estimator_test=estimator)
+    ac = AC(estimator_train=estimator, estimator_test=estimator, verbose=1)
     ac.fit(X_train, y_train)
     #  CC
     cc = CC(estimator_test=estimator)
     cc.fit(X_train, y_train)
     #  PCC
     pcc = PCC(estimator_test=estimator)
     pcc.fit(X_train, y_train)
```

### Comparing `quantificationlib-0.0.6/tests/test_cv_estimator.py` & `quantificationlib-0.0.7/tests/test_cv_estimator.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/tests/test_decomposition.py` & `quantificationlib-0.0.7/tests/test_decomposition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import numpy as np
-import os
-import warnings
 
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.multiclass import OneVsRestClassifier
 
 from quantificationlib.baselines.ac import AC
-from quantificationlib.baselines.cc import CC
+from quantificationlib.multiclass.df import HDX
 
 from quantificationlib.decomposition.multiclass import OneVsRestQuantifier
 
+from quantificationlib.metrics.ordinal import emd, emd_score
+
+from quantificationlib.estimators.frank_and_hall import FrankAndHallClassifier
+from quantificationlib.decomposition.ordinal import FrankAndHallQuantifier
+
 from quantificationlib.estimators.cross_validation import CV_estimator
 from quantificationlib.bag_generator import PriorShift_BagGenerator
 from quantificationlib.metrics.multiclass import mean_absolute_error
 
 from quantificationlib.data_utils import load_data, normalize
 
 
 def test_decomposition_multiclass():
 
     dataset='examples/datasets/multiclass/iris.csv'
     n_bags=5
     master_seed=2032
 
-    method_name = ['OVR-CC', 'OVR-AC']
+    method_name = ['OVR-HDX', 'OVR-AC']
 
     results = np.zeros((n_bags, len(method_name)))
 
     X, y = load_data(dataset)
 
 
     current_seed = master_seed
@@ -44,67 +47,48 @@
     ovr_estimator = OneVsRestClassifier(estimator, n_jobs=-1)
 
     #  AC
     ovr_ac = OneVsRestQuantifier(base_quantifier=AC(),
                                     estimator_train=ovr_estimator, estimator_test=ovr_estimator)
     ovr_ac.fit(X_train, y_train)
     #  CC
-    ovr_cc = OneVsRestQuantifier(base_quantifier=CC(), estimator_test=ovr_estimator)
-    ovr_cc.fit(X_train, y_train)
+    ovr_hdx = OneVsRestQuantifier(base_quantifier=HDX())
+    ovr_hdx.fit(X_train, y_train)
     
 
     #  Testing bags
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
 
         prev_preds = [
-            ovr_cc.predict(X_test[indexes[:, n_bag], :]),
+            ovr_hdx.predict(X_test[indexes[:, n_bag], :]),
             ovr_ac.predict(X_test[indexes[:, n_bag], :]),
         ]
 
         for n_method, prev_pred in enumerate(prev_preds):
             results[n_bag, n_method] = mean_absolute_error(prev_true[:, n_bag], prev_pred)
 
     #  printing and saving results
     avg = np.mean(results, axis=0)
     for name, result in zip(method_name,avg):
-        assert result >= 0 and result <= 0.02, "Error in method %s " % name
-
-
-import numpy as np
-import os
-import warnings
-
-from sklearn.model_selection import train_test_split
-from sklearn.ensemble import RandomForestClassifier
-
-from quantificationlib.baselines.ac import AC
-from quantificationlib.baselines.cc import CC
-
-from quantificationlib.estimators.frank_and_hall import FrankAndHallClassifier
-from quantificationlib.decomposition.ordinal import FrankAndHallQuantifier
-
-from quantificationlib.bag_generator import PriorShift_BagGenerator
-from quantificationlib.metrics.ordinal import emd
-
-from quantificationlib.data_utils import load_data, normalize
-
+        assert result >= 0 and result <= 0.026, "Error in method %s " % name
 
 def test_decomposition_ordinal():
 
     dataset='examples/datasets/ordinal/ESL.csv'
     n_bags=5
     master_seed=2032
 
     method_name = ['FH-CC', 'FH-AC']
 
-    results = np.zeros((n_bags, len(method_name)))
+    results_emd = np.zeros((n_bags, len(method_name)))
+    results_emd_score = np.zeros((n_bags, len(method_name)))
 
     X, y = load_data(dataset)
 
     current_seed = master_seed
 
     # generating training-test partition
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, stratify=y, random_state=current_seed)
@@ -116,27 +100,32 @@
                                                                     random_state=master_seed,
                                                                     class_weight='balanced'), n_jobs=-1)
 
     #  AC_HD
     fh_ac = FrankAndHallQuantifier(quantifier=AC(), estimator_train=fh, estimator_test=fh)
     fh_ac.fit(X_train, y_train)
     #  CC
-    fh_cc = FrankAndHallQuantifier(quantifier=CC(), estimator_train=None, estimator_test=fh)
-    fh_cc.fit(X_train, y_train)
+    fh_hdx = FrankAndHallQuantifier(quantifier=HDX(), estimator_train=None, estimator_test=None)
+    fh_hdx.fit(X_train, y_train)
     
 
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
         prev_preds = [
-            fh_cc.predict(X_test[indexes[:, n_bag], :]),
+            fh_hdx.predict(X_test[indexes[:, n_bag], :]),
             fh_ac.predict(X_test[indexes[:, n_bag], :]),
         ]
 
     for n_method, prev_pred in enumerate(prev_preds):
-        results[n_bag, n_method] = emd(prev_true[:, n_bag], prev_pred)
+        results_emd[n_bag, n_method] = emd(prev_true[:, n_bag], prev_pred)
+        results_emd_score[n_bag, n_method] = emd_score(prev_true[:, n_bag], prev_pred)
 
-    avg = np.mean(results, axis=0)
-    for name, result in zip(method_name,avg):
-        assert result >= 0 and result <= 0.05, "Error in method %s " % name
+    avg_emd = np.mean(results_emd, axis=0)
+    avg_emd_score = np.mean(results_emd_score, axis=0)
+    for name, result in zip(method_name,avg_emd):
+        assert result >= 0 and result <= 0.05, "Error in method %s " % name
+
+    for name, result in zip(method_name,avg_emd_score):
+        assert result >= 0 and result <= 0.2, "Error in method %s " % name
```

### Comparing `quantificationlib-0.0.6/tests/test_ensembles.py` & `quantificationlib-0.0.7/tests/test_ensembles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import os
 
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 
 from quantificationlib.baselines.ac import PAC
-from quantificationlib.baselines.cc import PCC
+from quantificationlib.multiclass.df import HDX
 
 
 from quantificationlib.multiclass.em import EM
 
 
 from quantificationlib.estimators.ensembles import EnsembleOfClassifiers
 from quantificationlib.ensembles.eoq import EoQ
@@ -22,15 +22,15 @@
 
 def test_ensembles():
 
     dataset = 'examples/datasets/binary/iris.3.csv'
     master_seed = 2032
     n_bags = 5
 
-    method_name = ['EOQ-PCC', 'EOQ-PAC', 'EOQ-EM']
+    method_name = ['EOQ-HDX', 'EOQ-PAC', 'EOQ-EM']
 
     results = np.zeros((n_bags, len(method_name)))
    
     X, y = load_data(dataset)
 
     current_seed = master_seed
 
@@ -45,24 +45,23 @@
     estimator = RandomForestClassifier(n_estimators=100, random_state=master_seed, class_weight='balanced')
 
     ensemble_estimator = EnsembleOfClassifiers(base_estimator=estimator)
 
     bag_generator_eoq = PriorShift_BagGenerator(n_bags=100, bag_size=len(X_train),
                                                 min_prevalence=0.05, random_state=current_seed)
 
-    #  PCC
-    eoq_pcc = EoQ(base_quantifier=PCC(),
+    #  HDX
+    eoq_hdx = EoQ(base_quantifier=HDX(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
-                    combination_strategy='mean',
-                    ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator)
-    eoq_pcc.fit(X_train, y_train)
+                    combination_strategy='prevalence_similarity')
+    eoq_hdx.fit(X_train, y_train)
     #  PAC
     eoq_pac = EoQ(base_quantifier=PAC(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
-                    combination_strategy='mean',
+                    combination_strategy='median',
                     ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator)
     eoq_pac.fit(X_train, y_train)
 
     # EM
     eoq_em = EoQ(base_quantifier=EM(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
                     combination_strategy='mean',
@@ -73,15 +72,15 @@
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
 
         prev_preds = [
-            eoq_pcc.predict(X_test[indexes[:, n_bag], :]),
+            eoq_hdx.predict(X_test[indexes[:, n_bag], :]),
             eoq_pac.predict(X_test[indexes[:, n_bag], :]),
             eoq_em.predict(X_test[indexes[:, n_bag], :]),
         ]
 
         for n_method, prev_pred in enumerate(prev_preds):
             results[n_bag, n_method] = mean_absolute_error(prev_true[:, n_bag], prev_pred)
```

### Comparing `quantificationlib-0.0.6/tests/test_metrics.py` & `quantificationlib-0.0.7/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.6/tests/test_ordinal_quantifiers.py` & `quantificationlib-0.0.7/tests/test_ordinal_quantifiers.py`

 * *Files identical despite different names*

