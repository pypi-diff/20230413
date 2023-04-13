# Comparing `tmp/ProcessOptimizer-0.7.7.tar.gz` & `tmp/ProcessOptimizer-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessOptimizer-0.7.7.tar", last modified: Fri Nov 18 13:41:07 2022, max compression
+gzip compressed data, was "ProcessOptimizer-0.7.8.tar", last modified: Tue Feb 14 09:47:43 2023, max compression
```

## Comparing `ProcessOptimizer-0.7.7.tar` & `ProcessOptimizer-0.7.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.741204 ProcessOptimizer-0.7.7/
--rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/AUTHORS_scikit_optimize.md
--rw-rw-rw-   0        0        0     1597 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.7/LICENSE.md
--rw-rw-rw-   0        0        0    10763 2022-11-18 13:41:07.739215 ProcessOptimizer-0.7.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.379671 ProcessOptimizer-0.7.7/ProcessOptimizer/
--rw-rw-rw-   0        0        0     1821 2022-11-18 13:29:16.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/__init__.py
--rw-rw-rw-   0        0        0    11574 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/acquisition.py
--rw-rw-rw-   0        0        0    29142 2022-03-10 13:53:50.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/bokeh_plot.py
--rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/callbacks.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.444675 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/
--rw-rw-rw-   0        0        0      425 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/__init__.py
--rw-rw-rw-   0        0        0    18673 2021-09-23 13:20:36.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/forest.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.499677 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/
--rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/__init__.py
--rw-rw-rw-   0        0        0    17518 2022-11-18 13:15:59.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/gpr.py
--rw-rw-rw-   0        0        0    15219 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/kernels.py
--rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gbrt.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.629199 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/
--rw-rw-rw-   0        0        0        0 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/__init__.py
--rw-rw-rw-   0        0        0     3586 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/benchmarks.py
--rw-rw-rw-   0        0        0      605 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/branin_hoo.py
--rw-rw-rw-   0        0        0     2563 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/model_system.py
--rw-rw-rw-   0        0        0     1359 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.696200 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/
--rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/_NSGA2.py
--rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/__init__.py
--rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/base.py
--rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/dummy.py
--rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/forest.py
--rw-rw-rw-   0        0        0     6836 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/gbrt.py
--rw-rw-rw-   0        0        0    10782 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/gp.py
--rw-rw-rw-   0        0        0    46582 2022-03-02 12:49:46.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/optimizer.py
--rw-rw-rw-   0        0        0    90067 2022-11-18 13:15:43.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/plots.py
--rw-rw-rw-   0        0        0    28205 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/searchcv.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.733202 ProcessOptimizer-0.7.7/ProcessOptimizer/space/
--rw-rw-rw-   0        0        0       71 2021-07-29 06:17:13.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/space/__init__.py
--rw-rw-rw-   0        0        0    30019 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/space/constraints.py
--rw-rw-rw-   0        0        0    29945 2022-03-10 13:55:31.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/space/space.py
--rw-rw-rw-   0        0        0     5265 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/space/transformers.py
--rw-rw-rw-   0        0        0    33016 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.7/ProcessOptimizer/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-18 13:41:07.403671 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/
--rw-rw-rw-   0        0        0    10763 2022-11-18 13:41:05.000000 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1402 2022-11-18 13:41:05.000000 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 13:41:05.000000 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2022-11-18 13:41:05.000000 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-11-18 13:41:05.000000 ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10315 2022-03-01 09:52:04.000000 ProcessOptimizer-0.7.7/README.md
--rw-rw-rw-   0        0        0       42 2022-11-18 13:41:07.741204 ProcessOptimizer-0.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1580 2022-11-18 13:29:49.000000 ProcessOptimizer-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:43.233762 ProcessOptimizer-0.7.8/
+-rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/AUTHORS_scikit_optimize.md
+-rw-rw-rw-   0        0        0     1598 2023-02-14 09:41:21.000000 ProcessOptimizer-0.7.8/LICENSE.md
+-rw-rw-rw-   0        0        0    10763 2023-02-14 09:47:43.232828 ProcessOptimizer-0.7.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:42.890030 ProcessOptimizer-0.7.8/ProcessOptimizer/
+-rw-rw-rw-   0        0        0     1821 2023-02-14 09:43:42.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/__init__.py
+-rw-rw-rw-   0        0        0    11574 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/acquisition.py
+-rw-rw-rw-   0        0        0    29142 2022-03-10 13:53:50.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/bokeh_plot.py
+-rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:42.960270 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/
+-rw-rw-rw-   0        0        0      425 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/__init__.py
+-rw-rw-rw-   0        0        0    18835 2023-01-26 13:09:11.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/forest.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:43.002265 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/
+-rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/__init__.py
+-rw-rw-rw-   0        0        0    17518 2022-11-18 13:15:59.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/gpr.py
+-rw-rw-rw-   0        0        0    15219 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/kernels.py
+-rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gbrt.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:43.075301 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/
+-rw-rw-rw-   0        0        0        0 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/__init__.py
+-rw-rw-rw-   0        0        0     3586 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/benchmarks.py
+-rw-rw-rw-   0        0        0      605 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/branin_hoo.py
+-rw-rw-rw-   0        0        0     2563 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/model_system.py
+-rw-rw-rw-   0        0        0     1359 2022-11-09 08:13:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:43.177355 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/
+-rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/_NSGA2.py
+-rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/__init__.py
+-rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/base.py
+-rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/dummy.py
+-rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/forest.py
+-rw-rw-rw-   0        0        0     6836 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/gbrt.py
+-rw-rw-rw-   0        0        0    10782 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/gp.py
+-rw-rw-rw-   0        0        0    46582 2022-03-02 12:49:46.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0    89998 2023-02-14 09:41:21.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/plots.py
+-rw-rw-rw-   0        0        0    28205 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/searchcv.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:43.226827 ProcessOptimizer-0.7.8/ProcessOptimizer/space/
+-rw-rw-rw-   0        0        0       71 2021-07-29 06:17:13.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/space/__init__.py
+-rw-rw-rw-   0        0        0    30019 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/space/constraints.py
+-rw-rw-rw-   0        0        0    29945 2022-03-10 13:55:31.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/space/space.py
+-rw-rw-rw-   0        0        0     5265 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/space/transformers.py
+-rw-rw-rw-   0        0        0    33016 2022-01-13 12:11:20.000000 ProcessOptimizer-0.7.8/ProcessOptimizer/utils.py
+drwxrwxrwx   0        0        0        0 2023-02-14 09:47:42.923148 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/
+-rw-rw-rw-   0        0        0    10763 2023-02-14 09:47:41.000000 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1402 2023-02-14 09:47:41.000000 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-14 09:47:41.000000 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-02-14 09:47:41.000000 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-02-14 09:47:41.000000 ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10315 2022-03-01 09:52:04.000000 ProcessOptimizer-0.7.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-02-14 09:47:43.233762 ProcessOptimizer-0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-02-14 09:43:33.000000 ProcessOptimizer-0.7.8/setup.py
```

### Comparing `ProcessOptimizer-0.7.7/AUTHORS_scikit_optimize.md` & `ProcessOptimizer-0.7.8/AUTHORS_scikit_optimize.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/LICENSE.md` & `ProcessOptimizer-0.7.8/LICENSE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 New BSD License
 
-Copyright (c) 2016 - scikit-optimize developers.
+Copyright (c) 2023 - ProcessOptimizer developers.
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
   a. Redistributions of source code must retain the above copyright notice,
```

### Comparing `ProcessOptimizer-0.7.7/PKG-INFO` & `ProcessOptimizer-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.7.7
+Version: 0.7.8
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: browniebee
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.7.7 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.7.8 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Platform: UNKNOWN Description-
 Content-Type: text/markdown Provides-Extra: browniebee License-File: LICENSE.md
 License-File: AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
```

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/__init__.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .utils import expected_minimum_random_sampling
 from .utils import load
 from .utils import cook_estimator, create_result, y_coverage
 from .plots import plot_objective, plot_objectives
 from .plots import plot_evaluations, plot_convergence
 from .plots import plot_Pareto, plot_expected_minimum_convergence
 
-__version__ = "0.7.7"
+__version__ = "0.7.8"
 
 
 __all__ = (
     "acquisition",
     "benchmarks",
     "callbacks",
     "learning",
```

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/acquisition.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/acquisition.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/bokeh_plot.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/callbacks.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/callbacks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/learning/forest.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/learning/forest.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Prediction of each data point as returned by RandomForestRegressor
         or ExtraTreesRegressor.
 
     Returns
     -------
     * `std` [array-like, shape=(n_samples,)]:
         Standard deviation of `y` at `X`. If criterion
-        is set to "mse", then `std[i] ~= std(y | X[i])`.
+        is set to "squared_error", then `std[i] ~= std(y | X[i])`.
     """
     # This derives std(y | x) as described in 4.3.2 of arXiv:1211.0906
     std = np.zeros(len(X))
 
     for tree in trees:
         var_tree = tree.tree_.impurity[tree.apply(X)]
 
@@ -56,18 +56,18 @@
     RandomForestRegressor that supports conditional std computation.
 
     Parameters
     ----------
     n_estimators : integer, optional (default=10)
         The number of trees in the forest.
 
-    criterion : string, optional (default="mse")
+    criterion : string, optional (default="squared_error")
         The function to measure the quality of a split. Supported criteria
-        are "mse" for the mean squared error, which is equal to variance
-        reduction as feature selection criterion, and "mae" for the mean
+        are "squared_error" for the mean squared error, which is equal to variance
+        reduction as feature selection criterion, and "absolute_error" for the
         absolute error.
 
     max_features : int, float, string or None, optional (default="auto")
         The number of features to consider when looking for the best split:
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a percentage and
           `int(max_features * n_features)` features are considered at each
@@ -181,15 +181,15 @@
     fitting, ``random_state`` has to be fixed.
 
     References
     ----------
     .. [1] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
     """
 
-    def __init__(self, n_estimators=10, criterion='mse', max_depth=None,
+    def __init__(self, n_estimators=10, criterion='squared_error', max_depth=None,
                  min_samples_split=2, min_samples_leaf=1,
                  min_weight_fraction_leaf=0.0, max_features='auto',
                  max_leaf_nodes=None, bootstrap=True, oob_score=False,
                  n_jobs=1, random_state=None, verbose=0, warm_start=False,
                  min_variance=0.0):
         self.min_variance = min_variance
         super(RandomForestRegressor, self).__init__(
@@ -213,27 +213,27 @@
 
         return_std : boolean
             Whether or not to return the standard deviation.
 
         Returns
         -------
         predictions : array-like of shape = (n_samples,)
-            Predicted values for X. If criterion is set to "mse",
+            Predicted values for X. If criterion is set to "squared_error",
             then `predictions[i] ~= mean(y | X[i])`.
 
         std : array-like of shape=(n_samples,)
             Standard deviation of `y` at `X`. If criterion
-            is set to "mse", then `std[i] ~= std(y | X[i])`.
+            is set to "squared_error", then `std[i] ~= std(y | X[i])`.
         """
         mean = super(RandomForestRegressor, self).predict(X)
 
         if return_std:
-            if self.criterion != "mse":
+            if self.criterion != "squared_error":
                 raise ValueError(
-                    "Expected impurity to be 'mse', got %s instead"
+                    "Expected impurity to be 'squared_error', got %s instead"
                     % self.criterion)
             std = _return_std(X, self.estimators_, mean, self.min_variance)
             return mean, std
         return mean
 
 
 class ExtraTreesRegressor(_sk_ExtraTreesRegressor):
@@ -241,18 +241,18 @@
     ExtraTreesRegressor that supports conditional standard deviation.
 
     Parameters
     ----------
     n_estimators : integer, optional (default=10)
         The number of trees in the forest.
 
-    criterion : string, optional (default="mse")
+    criterion : string, optional (default="squared_error")
         The function to measure the quality of a split. Supported criteria
-        are "mse" for the mean squared error, which is equal to variance
-        reduction as feature selection criterion, and "mae" for the mean
+        are "squared_error" for the mean squared error, which is equal to variance
+        reduction as feature selection criterion, and "absolute_error" for the
         absolute error.
 
     max_features : int, float, string or None, optional (default="auto")
         The number of features to consider when looking for the best split:
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a percentage and
           `int(max_features * n_features)` features are considered at each
@@ -366,15 +366,15 @@
     fitting, ``random_state`` has to be fixed.
 
     References
     ----------
     .. [1] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
     """
 
-    def __init__(self, n_estimators=10, criterion='mse', max_depth=None,
+    def __init__(self, n_estimators=10, criterion='squared_error', max_depth=None,
                  min_samples_split=2, min_samples_leaf=1,
                  min_weight_fraction_leaf=0.0, max_features='auto',
                  max_leaf_nodes=None, bootstrap=False, oob_score=False,
                  n_jobs=1, random_state=None, verbose=0, warm_start=False,
                  min_variance=0.0):
         self.min_variance = min_variance
         super(ExtraTreesRegressor, self).__init__(
@@ -399,25 +399,25 @@
 
         return_std : boolean
             Whether or not to return the standard deviation.
 
         Returns
         -------
         predictions : array-like of shape=(n_samples,)
-            Predicted values for X. If criterion is set to "mse",
+            Predicted values for X. If criterion is set to "squared_error",
             then `predictions[i] ~= mean(y | X[i])`.
 
         std : array-like of shape=(n_samples,)
             Standard deviation of `y` at `X`. If criterion
-            is set to "mse", then `std[i] ~= std(y | X[i])`.
+            is set to "squared_error", then `std[i] ~= std(y | X[i])`.
         """
         mean = super(ExtraTreesRegressor, self).predict(X)
 
         if return_std:
-            if self.criterion != "mse":
+            if self.criterion != "squared_error":
                 raise ValueError(
-                    "Expected impurity to be 'mse', got %s instead"
+                    "Expected impurity to be 'squared_error', got %s instead"
                     % self.criterion)
             std = _return_std(X, self.estimators_, mean, self.min_variance)
             return mean, std
 
         return mean
```

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/gpr.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gaussian_process/kernels.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gaussian_process/kernels.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/learning/gbrt.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/learning/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/benchmarks.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/branin_hoo.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/branin_hoo.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/model_system.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/model_system.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/model_systems/second_order_polynomial_2d.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/model_systems/second_order_polynomial_2d.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/_NSGA2.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/_NSGA2.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/base.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/dummy.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/dummy.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/forest.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/gbrt.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/gp.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/gp.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/optimizer/optimizer.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/plots.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -2249,30 +2249,29 @@
                      obj2: [i[1] for i in optimizer.yi]}
     
     for i, dim in enumerate(dimensions):
         data_observed_dict[dim] =  [x[i] for x in optimizer.Xi]
 
     data_calculated_dict = {
         'front_x': np.unique(front, axis=0)[:,0].tolist(),
-        'front_y': np.unique(front, axis=0)[:,1].tolist(),
-        'recipe_x': pop[np.unique(front, axis=0, return_index=True)[1],0].tolist(),
-        'recipe_y': pop[np.unique(front, axis=0, return_index=True)[1],1].tolist(),
-    }
+        'front_y': np.unique(front, axis=0)[:,1].tolist()}
+    for i, dim in enumerate(dimensions):
+        data_calculated_dict[dim] = pop[np.unique(front, axis=0, return_index=True)[1],i].tolist()
     
     # Create Tooltip strings for the observed data points
     Tooltips_observed = '''<div><font size="2"><b>Settings for this point are:</b></font></div>'''
     for dim in dimensions:
         Tooltips_observed += '''<div><font size="2">'''+dim+''' = @{'''+dim+'''}{0.0}</font></div>'''
     Tooltips_observed += '''<div><font size="2"><b>Scores for this point are:</b></font></div>'''
     Tooltips_observed += '''<div><font size="2">[ @{'''+obj1+'''}{0.00} , @{'''+obj2+'''}{0.00} ]</font></div>'''
     
     # Create Tooltip strings for calculated points on the Pareto-front
     Tooltips_recipe = '''<div><font size="2"><b>Settings for this point are:</b></font></div>'''
-    for dim, rec in zip(dimensions,['recipe_x','recipe_y']):
-        Tooltips_recipe += '''<div><font size="2">'''+dim+''' = @{'''+rec+'''}{0.0}</font></div>'''
+    for dim in dimensions:
+        Tooltips_recipe += '''<div><font size="2">'''+dim+''' = @{'''+dim+'''}{0.0}</font></div>'''
     Tooltips_recipe += '''<div><font size="2"><b>Predicted scores for this point are:</b></font></div>'''
     Tooltips_recipe += '''<div><font size="2">[ @{front_x}{0.00} , @{front_y}{0.00} ]</font></div>'''
     
     # Load data into bokeh object
     source_observed = bh_models.ColumnDataSource(data_observed_dict)
     source_calculated = bh_models.ColumnDataSource(data_calculated_dict)
```

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/searchcv.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/searchcv.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/space/constraints.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/space/constraints.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/space/space.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/space/space.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/space/transformers.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/space/transformers.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer/utils.py` & `ProcessOptimizer-0.7.8/ProcessOptimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/PKG-INFO` & `ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.7.7
+Version: 0.7.8
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: browniebee
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.7.7 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.7.8 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Platform: UNKNOWN Description-
 Content-Type: text/markdown Provides-Extra: browniebee License-File: LICENSE.md
 License-File: AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
```

### Comparing `ProcessOptimizer-0.7.7/ProcessOptimizer.egg-info/SOURCES.txt` & `ProcessOptimizer-0.7.8/ProcessOptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/README.md` & `ProcessOptimizer-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.7.7/setup.py` & `ProcessOptimizer-0.7.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ProcessOptimizer',
-      version='0.7.7',
+      version='0.7.8',
       description='Sequential model-based optimization toolbox \
     (forked from scikit-optimize)',
       url='https://github.com/novonordisk-research/ProcessOptimizer',
       license='BSD',
       author='Novo Nordisk, Research & Early Development',
       packages=[
           'ProcessOptimizer',
```

