# Comparing `tmp/sklearn_quantile-0.0.21.tar.gz` & `tmp/sklearn_quantile-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_quantile-0.0.21.tar", last modified: Thu Apr 13 13:25:19 2023, max compression
+gzip compressed data, was "sklearn_quantile-0.0.3.tar", last modified: Fri Feb  4 17:31:28 2022, max compression
```

## Comparing `sklearn_quantile-0.0.21.tar` & `sklearn_quantile-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,32 @@
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.257120 sklearn_quantile-0.0.21/
--rw-r--r--   0 jroebroek   (501) staff       (20)     1515 2022-01-18 08:10:04.000000 sklearn_quantile-0.0.21/LICENSE
--rw-r--r--   0 jroebroek   (501) staff       (20)       72 2023-04-13 13:25:17.000000 sklearn_quantile-0.0.21/MANIFEST.in
--rw-r--r--   0 jroebroek   (501) staff       (20)     3510 2023-04-13 13:25:19.257303 sklearn_quantile-0.0.21/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)     3214 2022-02-28 07:49:20.000000 sklearn_quantile-0.0.21/README.md
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.242073 sklearn_quantile-0.0.21/dist/
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.242196 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.242487 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.246530 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/
--rw-r--r--   0 jroebroek   (501) staff       (20)     6006 2023-04-13 08:40:08.000000 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/maximum.pyx
--rw-r--r--   0 jroebroek   (501) staff       (20)    57611 2023-04-13 08:40:08.000000 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/quantile.pyx
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.247544 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/
--rw-r--r--   0 jroebroek   (501) staff       (20)      685 2021-06-10 12:55:07.000000 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pxd
--rw-r--r--   0 jroebroek   (501) staff       (20)    12224 2022-02-04 11:36:30.000000 sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pyx
--rw-r--r--   0 jroebroek   (501) staff       (20)       79 2023-04-13 13:25:19.257958 sklearn_quantile-0.0.21/setup.cfg
--rw-r--r--   0 jroebroek   (501) staff       (20)     1341 2023-04-13 13:23:46.000000 sklearn_quantile-0.0.21/setup.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.248371 sklearn_quantile-0.0.21/sklearn_quantile/
--rw-r--r--   0 jroebroek   (501) staff       (20)      290 2022-02-03 17:30:06.000000 sklearn_quantile-0.0.21/sklearn_quantile/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     1366 2023-04-13 07:26:40.000000 sklearn_quantile-0.0.21/sklearn_quantile/base.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.251947 sklearn_quantile-0.0.21/sklearn_quantile/ensemble/
--rw-r--r--   0 jroebroek   (501) staff       (20)      273 2023-04-13 13:11:21.000000 sklearn_quantile-0.0.21/sklearn_quantile/ensemble/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     6006 2023-04-13 08:40:08.000000 sklearn_quantile-0.0.21/sklearn_quantile/ensemble/maximum.pyx
--rw-r--r--   0 jroebroek   (501) staff       (20)    57611 2023-04-13 08:40:08.000000 sklearn_quantile-0.0.21/sklearn_quantile/ensemble/quantile.pyx
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.253342 sklearn_quantile-0.0.21/sklearn_quantile/neighbors/
--rw-r--r--   0 jroebroek   (501) staff       (20)       76 2023-04-13 13:11:22.000000 sklearn_quantile-0.0.21/sklearn_quantile/neighbors/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     7220 2022-02-04 11:44:21.000000 sklearn_quantile-0.0.21/sklearn_quantile/neighbors/quantile.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.255332 sklearn_quantile-0.0.21/sklearn_quantile/utils/
--rw-r--r--   0 jroebroek   (501) staff       (20)       71 2023-04-13 13:11:22.000000 sklearn_quantile-0.0.21/sklearn_quantile/utils/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)      355 2023-04-13 08:04:46.000000 sklearn_quantile-0.0.21/sklearn_quantile/utils/utils.py
--rw-r--r--   0 jroebroek   (501) staff       (20)      685 2021-06-10 12:55:07.000000 sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pxd
--rw-r--r--   0 jroebroek   (501) staff       (20)    12224 2022-02-04 11:36:30.000000 sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pyx
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.250654 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/
--rw-r--r--   0 jroebroek   (501) staff       (20)     3510 2023-04-13 13:25:19.000000 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)     1019 2023-04-13 13:25:19.000000 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/SOURCES.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        1 2023-04-13 13:25:19.000000 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/dependency_links.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)      129 2023-04-13 13:25:19.000000 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/requires.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       17 2023-04-13 13:25:19.000000 sklearn_quantile-0.0.21/sklearn_quantile.egg-info/top_level.txt
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-04-13 13:25:19.256688 sklearn_quantile-0.0.21/tests/
--rw-r--r--   0 jroebroek   (501) staff       (20)     2368 2022-02-04 16:03:51.000000 sklearn_quantile-0.0.21/tests/test_quantile_KNN.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     5569 2022-02-04 16:08:21.000000 sklearn_quantile-0.0.21/tests/test_quantile_RF.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     3987 2022-02-04 11:40:57.000000 sklearn_quantile-0.0.21/tests/test_weighted_quantile.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.577214 sklearn_quantile-0.0.3/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1515 2022-01-18 08:10:04.000000 sklearn_quantile-0.0.3/LICENSE
+-rw-r--r--   0 jroebroek   (501) staff       (20)       42 2022-02-04 17:05:29.000000 sklearn_quantile-0.0.3/MANIFEST.in
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2784 2022-02-04 17:31:28.577307 sklearn_quantile-0.0.3/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2452 2022-02-04 17:30:34.000000 sklearn_quantile-0.0.3/README.md
+-rw-r--r--   0 jroebroek   (501) staff       (20)       79 2022-02-04 17:31:28.577714 sklearn_quantile-0.0.3/setup.cfg
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1282 2022-02-04 17:31:23.000000 sklearn_quantile-0.0.3/setup.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.567810 sklearn_quantile-0.0.3/sklearn_quantile/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      290 2022-02-03 17:30:06.000000 sklearn_quantile-0.0.3/sklearn_quantile/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1367 2022-02-03 18:27:39.000000 sklearn_quantile-0.0.3/sklearn_quantile/base.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.573440 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      223 2022-02-03 17:29:39.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)  1150275 2022-02-04 14:41:20.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.c
+-rw-r--r--   0 jroebroek   (501) staff       (20)     5873 2022-02-04 14:41:17.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.pyx
+-rw-r--r--   0 jroebroek   (501) staff       (20)  1523734 2022-02-04 15:19:36.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.c
+-rw-r--r--   0 jroebroek   (501) staff       (20)    52546 2022-02-04 15:19:33.000000 sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.pyx
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.573955 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/
+-rw-r--r--   0 jroebroek   (501) staff       (20)       50 2022-02-04 09:23:10.000000 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7220 2022-02-04 11:44:21.000000 sklearn_quantile-0.0.3/sklearn_quantile/neighbors/quantile.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.576811 sklearn_quantile-0.0.3/sklearn_quantile/utils/
+-rw-r--r--   0 jroebroek   (501) staff       (20)       49 2022-01-17 17:41:49.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)  1066554 2022-02-04 11:36:32.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.c
+-rw-r--r--   0 jroebroek   (501) staff       (20)      685 2021-06-10 12:55:07.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pxd
+-rw-r--r--   0 jroebroek   (501) staff       (20)    12224 2022-02-04 11:36:30.000000 sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pyx
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.568901 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2784 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      767 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/SOURCES.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        1 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/dependency_links.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       91 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/requires.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       17 2022-02-04 17:31:28.000000 sklearn_quantile-0.0.3/sklearn_quantile.egg-info/top_level.txt
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2022-02-04 17:31:28.577029 sklearn_quantile-0.0.3/tests/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3987 2022-02-04 11:40:57.000000 sklearn_quantile-0.0.3/tests/test_weighted_quantile.py
```

### Comparing `sklearn_quantile-0.0.21/LICENSE` & `sklearn_quantile-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.21/PKG-INFO` & `sklearn_quantile-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: sklearn_quantile
-Version: 0.0.21
-Home-page: https://github.com/jasperroebroek/sklearn-quantile
-Author: Jasper Roebroek
-Author-email: roebroek.jasper@gmail.com
-License: BSD 3 clause
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/sklearn-quantile/badge/?version=latest)](https://sklearn-quantile.readthedocs.io/en/latest/?badge=latest)
 
 This module provides quantile machine learning models for python, in a plug-and-play fashion in the sklearn environment. This means that practically the only dependency is sklearn and all its functionality is applicable to the here provided models without code changes.
 
 The models implemented here share the trait that they are trained in exactly the same way as their non-quantile counterpart. The quantile information is only used in the prediction phase. The advantage of this (over for example Gradient Boosting Quantile Regression) is that several quantiles can be predicted at once without the need for retraining the model, which overall leads to a significantly faster workflow. Note that accuracy of doing this depends on the data. As can be seen in the example in the documentation: with certain data characteristics different quantiles might require different parameter optimisation for optimal performance. This is obviously possible with the implemented models here, but this requires the use of a single quantile during prediction, thus losing the speed advantage described above.
 
 For guidance see docs (through the link in the badge). They include an example that for quantile regression forests in exactly the same template as used for Gradient Boosting Quantile Regression in sklearn for comparability.
@@ -27,42 +16,18 @@
   - ExtraTreesQuantileRegressor: the main implementation
   - SampleExtraTreesQuantileRegressor: an approximation, that is much faster than the main implementation.
 
 - Quantile K-nearest neighbors (KNeighborsQuantileRegressor)
 
 # Installation
 
-The package can be installed with conda:
+The package can be installed with pip (when cython and scikit-learn are already installed):
 
 ```
-conda install --channel conda-forge sklearn-quantile
+pip install sklearn-quantile
 ```
 
 # Example
 
 An example of Random Forest Quantile Regression in action (both the main implementation and its approximation):
 
-<img src="https://github.com/jasperroebroek/sklearn-quantile/raw/master/docs/source/notebooks/example.png"/>
-
-# Usage example
-
-Random Forest Quantile Regressor predicting the 5th, 50th and 95th percentile of the California housing dataset.
-
-```
-from sklearn.datasets import fetch_california_housing
-from sklearn.model_selection import train_test_split
-from sklearn_quantile import RandomForestQuantileRegressor
-
-X, y = fetch_california_housing(return_X_y=True)
-X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.5, random_state=0)
-
-qrf = RandomForestQuantileRegressor(q=[0.05, 0.50, 0.95])
-qrf.fit(X_train, y_train)
-
-y_pred_5, y_pred_median, y_pred_95 = qrf.predict(X_test)
-qrf.score(X_test, y_test)
-```
-
-# Important links
-
-- API reference: https://sklearn-quantile.readthedocs.io/en/latest/api.html
-- Documentation: https://sklearn-quantile.readthedocs.io/en/latest/index.html
+<img src="https://github.com/jasperroebroek/sklearn-quantile/raw/master/tests/examples/readme_example.png"/>
```

### Comparing `sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/maximum.pyx` & `sklearn_quantile-0.0.3/sklearn_quantile/ensemble/maximum.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 It only has a single implementation called RandomForestMaxRegression, which has the
 same parameters as the regular RandomForestRegressor
 """
 import threading
 
 import joblib
 from cython.parallel cimport prange
+cimport openmp
 cimport numpy as np
 from joblib import Parallel
 
 import numpy as np
 from sklearn.tree import DecisionTreeRegressor
-from sklearn.utils.fixes import delayed
+from sklearn.utils.fixes import delayed, _joblib_parallel_args
 from sklearn.utils.validation import check_is_fitted, check_X_y
 from sklearn.ensemble._base import _partition_estimators
-from sklearn.ensemble._forest import _generate_sample_indices, RandomForestRegressor
+from sklearn.ensemble._forest import _generate_sample_indices
 
 from sklearn_quantile.ensemble.quantile import BaseForestQuantileRegressor
-from sklearn_quantile.utils.utils import create_keyword_dict
 
 
 ctypedef np.npy_intp SIZE_t              # Type for indices and counters
 
 
 __all__ = ["RandomForestMaximumRegressor"]
 
@@ -89,56 +89,49 @@
     A random forest regressor predicting conditional maxima
 
     Implementation is equivalent to Random Forest Quantile Regressor,
     but calculation is much faster. For other quantiles revert to the
     original predictor.
     """
     def __init__(self,
-                 n_estimators=100,
-                 *,
-                 criterion='squared_error',
+                 n_estimators=10,
+                 criterion='mse',
                  max_depth=None,
                  min_samples_split=2,
                  min_samples_leaf=1,
                  min_weight_fraction_leaf=0.0,
-                 max_features=1.0,
+                 max_features='auto',
                  max_leaf_nodes=None,
-                 min_impurity_decrease=0.0,
                  bootstrap=True,
+                 oob_score=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0,
-                 warm_start=False,
-                 ccp_alpha=0.0,
-                 max_samples=None):
-
-        estimator_params = RandomForestRegressor().estimator_params
-
+                 warm_start=False):
         super(BaseForestQuantileRegressor, self).__init__(
-            **create_keyword_dict(
-                estimator=DecisionTreeRegressor(),
-                n_estimators=n_estimators,
-                estimator_params=estimator_params,
-                bootstrap=bootstrap,
-                n_jobs=n_jobs,
-                random_state=random_state,
-                verbose=verbose,
-                warm_start=warm_start,
-                max_samples=max_samples)
-        )
+            base_estimator=DecisionTreeRegressor(),
+            n_estimators=n_estimators,
+            estimator_params=("criterion", "max_depth", "min_samples_split",
+                              "min_samples_leaf", "min_weight_fraction_leaf",
+                              "max_features", "max_leaf_nodes",
+                              "random_state"),
+            bootstrap=bootstrap,
+            oob_score=oob_score,
+            n_jobs=n_jobs,
+            random_state=random_state,
+            verbose=verbose,
+            warm_start=warm_start)
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
-        self.min_impurity_decrease = min_impurity_decrease
-        self.ccp_alpha = ccp_alpha
         self.q = 1
 
     def fit(self, X, y, sample_weight=None):
         super(RandomForestMaximumRegressor, self).fit(X, y, sample_weight)
 
         for i, est in enumerate(self.estimators_):
             if self.verbose:
@@ -169,12 +162,13 @@
         # Assign chunk of trees to jobs
         n_jobs, _, _ = _partition_estimators(self.n_estimators, self.n_jobs)
 
         y_hat = np.zeros(X.shape[0], dtype=np.float64)
 
         # Parallel loop
         lock = threading.Lock()
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,
+                 **_joblib_parallel_args(require="sharedmem"))(
             delayed(_accumulate_prediction)(e.predict, X, y_hat, lock)
             for e in self.estimators_)
 
         return y_hat
```

### Comparing `sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/quantile.pyx` & `sklearn_quantile-0.0.3/sklearn_quantile/ensemble/quantile.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 This module is inspired on the skgarden implementation of Forest Quantile Regression,
 based on the following paper:
 
 Nicolai Meinshausen, Quantile Regression Forests
 http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 """
 from cython.parallel cimport prange
+cimport openmp
 cimport numpy as np
 from numpy cimport ndarray
 
 from sklearn_quantile.utils.weighted_quantile cimport _weighted_quantile_presorted_1D, \
     _weighted_quantile_unchecked_1D, Interpolation
 
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
+from numpy.lib.function_base import _quantile_is_valid
 import threading
 import joblib
 from joblib import Parallel
 
-from sklearn.ensemble._forest import ForestRegressor, _accumulate_prediction, _generate_sample_indices, \
-    RandomForestRegressor, ExtraTreesRegressor
+from sklearn.ensemble._forest import ForestRegressor, _accumulate_prediction, _generate_sample_indices
 from sklearn.ensemble._base import _partition_estimators
 from sklearn.utils.fixes import delayed
+from sklearn.utils.fixes import _joblib_parallel_args
 from sklearn.tree import DecisionTreeRegressor, ExtraTreeRegressor
 from sklearn.utils import check_array, check_X_y, check_random_state
 from sklearn.utils.validation import check_is_fitted
+from sklearn.metrics import mean_pinball_loss
 from sklearn_quantile.base import QuantileRegressorMixin
-from sklearn_quantile.utils.utils import create_keyword_dict
 
 ctypedef np.npy_intp SIZE_t              # Type for indices and counters
 
 
 __all__ = ["RandomForestQuantileRegressor", "ExtraTreesQuantileRegressor", "SampleRandomForestQuantileRegressor",
            "SampleExtraTreesQuantileRegressor"]
 
@@ -58,15 +60,14 @@
     y_train_leaves : (n_estimators, n_samples)
     y_weights : (n_estimators, n_samples)
     q : (n_q)
     quantiles : output array (n_q, n_test_samples, n_outputs)
     start, stop : indices to break up computation across threads (used in range)
     """
     # todo; this does not compile with function cdef, only with cpdef
-    # todo; remove option for having more than one output variable
 
     cdef:
         int n_estimators = X_leaves.shape[0]
         int n_outputs = y_train.shape[1]
         int n_q = q.shape[0]
         int n_samples = y_train.shape[0]
         int n_test_samples = X_leaves.shape[1]
@@ -191,15 +192,16 @@
         -------
         self : object
             Returns self.
         """
         # apply method requires X to be of dtype np.float32
         # multi-output should likely work, but tests need to be written first.
         #   known case of error: maximum regressor
-        X, y = check_X_y(X, y, accept_sparse="csc", dtype=np.float32, multi_output=False)
+        X, y = check_X_y(
+            X, y, accept_sparse="csc", dtype=np.float32, multi_output=False)
         super(BaseForestQuantileRegressor, self).fit(X, y, sample_weight=sample_weight)
 
         self.n_samples_ = len(y)
         self.y_train_ = y.reshape((-1, self.n_outputs_)).astype(np.float32)
         self.y_train_leaves_ = self.apply(X).T
         self.y_weights_ = np.zeros_like(self.y_train_leaves_, dtype=np.float32)
 
@@ -280,15 +282,16 @@
 
         chunks = np.full(n_jobs, n_test_samples//n_jobs)
         chunks[:n_test_samples % n_jobs] +=1
         chunks = np.cumsum(np.insert(chunks, 0, 0))
 
         quantiles = np.empty((q.size, n_test_samples, self.n_outputs_), dtype=np.float32)
 
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,
+                 **_joblib_parallel_args(require="sharedmem"))(
             delayed(_quantile_forest_predict)(X_leaves, self.y_train_, self.y_train_leaves_, self.y_weights_, q,
                                               quantiles, chunks[i], chunks[i+1])
             for i in range(n_jobs))
 
         if q.size == 1:
             quantiles = quantiles[0]
         if self.n_outputs_ == 1:
@@ -339,15 +342,16 @@
 
         # apply method requires X to be of dtype np.float32
         X = check_array(X, dtype=np.float32, accept_sparse="csc")
 
         predictions = np.empty((len(X), self.n_outputs_, self.n_estimators))
 
         lock = threading.Lock()
-        Parallel(n_jobs=n_jobs, verbose=self.verbose,require="sharedmem")(
+        Parallel(n_jobs=n_jobs, verbose=self.verbose,
+                 **_joblib_parallel_args(require="sharedmem"))(
             delayed(_accumulate_prediction)(est.predict, X, i, predictions, lock)
             for i, est in enumerate(self.estimators_))
 
         quantiles = np.quantile(predictions, q=q, axis=-1)
         if q.size == 1:
             quantiles = quantiles[0]
         if self.n_outputs_ == 1:
@@ -361,270 +365,164 @@
     """
     A random forest regressor providing quantile estimates.
 
     Note that this implementation is rather slow for large datasets. Above 10000 samples
     it is recommended to use func:`sklearn_quantile.SampleRandomForestQuantileRegressor`,
     which is a model approximating the true conditional quantile.
 
-	Parameters
+    Parameters
     ----------
     q : float or array-like, optional
         Quantiles used for prediction (values ranging from 0 to 1)
 
-    n_estimators : int, default=100
+    n_estimators : integer, optional (default=10)
         The number of trees in the forest.
 
-        .. versionchanged:: 0.22
-           The default value of ``n_estimators`` changed from 10 to 100
-           in 0.22.
-
-    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
-            default="squared_error"
+    criterion : string, optional (default="mse")
         The function to measure the quality of a split. Supported criteria
-        are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion and minimizes the L2
-        loss using the mean of each terminal node, "friedman_mse", which uses
-        mean squared error with Friedman's improvement score for potential
-        splits, "absolute_error" for the mean absolute error, which minimizes
-        the L1 loss using the median of each terminal node, and "poisson" which
-        uses reduction in Poisson deviance to find splits.
-        Training using "absolute_error" is significantly slower
-        than when using "squared_error".
-
+        are "mse" for the mean squared error, which is equal to variance
+        reduction as feature selection criterion, and "mae" for the mean
+        absolute error.
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-        .. versionadded:: 1.0
-           Poisson criterion.
+    max_features : int, float, string or None, optional (default="auto")
+        The number of features to consider when looking for the best split:
+        - If int, then consider `max_features` features at each split.
+        - If float, then `max_features` is a percentage and
+          `int(max_features * n_features)` features are considered at each
+          split.
+        - If "auto", then `max_features=n_features`.
+        - If "sqrt", then `max_features=sqrt(n_features)`.
+        - If "log2", then `max_features=log2(n_features)`.
+        - If None, then `max_features=n_features`.
+        Note: the search for a split does not stop until at least one
+        valid partition of the node samples is found, even if it requires to
+        effectively inspect more than ``max_features`` features.
 
-    max_depth : int, default=None
+    max_depth : integer or None, optional (default=None)
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
-    min_samples_split : int or float, default=2
+    min_samples_split : int, float, optional (default=2)
         The minimum number of samples required to split an internal node:
-
         - If int, then consider `min_samples_split` as the minimum number.
-        - If float, then `min_samples_split` is a fraction and
+        - If float, then `min_samples_split` is a percentage and
           `ceil(min_samples_split * n_samples)` are the minimum
           number of samples for each split.
-
         .. versionchanged:: 0.18
-           Added float values for fractions.
-
-    min_samples_leaf : int or float, default=1
-        The minimum number of samples required to be at a leaf node.
-        A split point at any depth will only be considered if it leaves at
-        least ``min_samples_leaf`` training samples in each of the left and
-        right branches.  This may have the effect of smoothing the model,
-        especially in regression.
+           Added float values for percentages.
 
+    min_samples_leaf : int, float, optional (default=1)
+        The minimum number of samples required to be at a leaf node:
         - If int, then consider `min_samples_leaf` as the minimum number.
-        - If float, then `min_samples_leaf` is a fraction and
+        - If float, then `min_samples_leaf` is a percentage and
           `ceil(min_samples_leaf * n_samples)` are the minimum
           number of samples for each node.
-
         .. versionchanged:: 0.18
-           Added float values for fractions.
+           Added float values for percentages.
 
-    min_weight_fraction_leaf : float, default=0.0
+    min_weight_fraction_leaf : float, optional (default=0.)
         The minimum weighted fraction of the sum total of weights (of all
         the input samples) required to be at a leaf node. Samples have
         equal weight when sample_weight is not provided.
 
-    max_features : {"sqrt", "log2", None}, int or float, default=1.0
-        The number of features to consider when looking for the best split:
-
-        - If int, then consider `max_features` features at each split.
-        - If float, then `max_features` is a fraction and
-          `max(1, int(max_features * n_features_in_))` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
-        - If "sqrt", then `max_features=sqrt(n_features)`.
-        - If "log2", then `max_features=log2(n_features)`.
-        - If None or 1.0, then `max_features=n_features`.
-
-        .. note::
-            The default of 1.0 is equivalent to bagged trees and more
-            randomness can be achieved by setting smaller values, e.g. 0.3.
-
-        .. versionchanged:: 1.1
-            The default of `max_features` changed from `"auto"` to 1.0.
-
-        .. deprecated:: 1.1
-            The `"auto"` option was deprecated in 1.1 and will be removed
-            in 1.3.
-
-        Note: the search for a split does not stop until at least one
-        valid partition of the node samples is found, even if it requires to
-        effectively inspect more than ``max_features`` features.
-
-    max_leaf_nodes : int, default=None
+    max_leaf_nodes : int or None, optional (default=None)
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
-    min_impurity_decrease : float, default=0.0
-        A node will be split if this split induces a decrease of the impurity
-        greater than or equal to this value.
+    bootstrap : boolean, optional (default=True)
+        Whether bootstrap samples are used when building trees.
 
-        The weighted impurity decrease equation is the following::
+    oob_score : bool, optional (default=False)
+        whether to use out-of-bag samples to estimate
+        the R^2 on unseen data.
+
+    n_jobs : integer, optional (default=1)
+        The number of jobs to run in parallel for both `fit` and `predict`.
+        If -1, then the number of jobs is set to the number of cores.
+
+    random_state : int, RandomState instance or None, optional (default=None)
+        If int, random_state is the seed used by the random number generator;
+        If RandomState instance, random_state is the random number generator;
+        If None, the random number generator is the RandomState instance used
+        by `np.random`.
 
-            N_t / N * (impurity - N_t_R / N_t * right_impurity
-                                - N_t_L / N_t * left_impurity)
+    verbose : int, optional (default=0)
+        Controls the verbosity of the tree building process.
 
-        where ``N`` is the total number of samples, ``N_t`` is the number of
-        samples at the current node, ``N_t_L`` is the number of samples in the
-        left child, and ``N_t_R`` is the number of samples in the right child.
-
-        ``N``, ``N_t``, ``N_t_R`` and ``N_t_L`` all refer to the weighted sum,
-        if ``sample_weight`` is passed.
-
-        .. versionadded:: 0.19
-
-    bootstrap : bool, default=True
-        Whether bootstrap samples are used when building trees. If False, the
-        whole dataset is used to build each tree.
-
-    n_jobs : int, default=None
-        The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
-        :meth:`decision_path` and :meth:`apply` are all parallelized over the
-        trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
-        context. ``-1`` means using all processors. See :term:`Glossary
-        <n_jobs>` for more details.
-
-    random_state : int, RandomState instance or None, default=None
-        Controls both the randomness of the bootstrapping of the samples used
-        when building trees (if ``bootstrap=True``) and the sampling of the
-        features to consider when looking for the best split at each node
-        (if ``max_features < n_features``).
-        See :term:`Glossary <random_state>` for details.
-
-    verbose : int, default=0
-        Controls the verbosity when fitting and predicting.
-
-    warm_start : bool, default=False
+    warm_start : bool, optional (default=False)
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`Glossary <warm_start>` and
-        :ref:`gradient_boosting_warm_start` for details.
-
-    ccp_alpha : non-negative float, default=0.0
-        Complexity parameter used for Minimal Cost-Complexity Pruning. The
-        subtree with the largest cost complexity that is smaller than
-        ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
-        :ref:`minimal_cost_complexity_pruning` for details.
-
-        .. versionadded:: 0.22
-
-    max_samples : int or float, default=None
-        If bootstrap is True, the number of samples to draw from X
-        to train each base estimator.
-
-        - If None (default), then draw `X.shape[0]` samples.
-        - If int, then draw `max_samples` samples.
-        - If float, then draw `max_samples * X.shape[0]` samples. Thus,
-          `max_samples` should be in the interval `(0.0, 1.0]`.
-
-        .. versionadded:: 0.22
+        new forest.
 
     Attributes
     ----------
-    estimator_ : :class:`~sklearn.tree.DecisionTreeRegressor`
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. versionadded:: 1.2
-           `base_estimator_` was renamed to `estimator_`.
-
-    base_estimator_ : DecisionTreeRegressor
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. deprecated:: 1.2
-            `base_estimator_` is deprecated and will be removed in 1.4.
-            Use `estimator_` instead.
-
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
-    feature_importances_ : ndarray of shape (n_features,)
-        The impurity-based feature importances.
-        The higher, the more important the feature.
-        The importance of a feature is computed as the (normalized)
-        total reduction of the criterion brought by that feature.  It is also
-        known as the Gini importance.
-        Warning: impurity-based feature importances can be misleading for
-        high cardinality features (many unique values). See
-        :func:`sklearn.inspection.permutation_importance` as an alternative.
-
-    n_features_in_ : int
-        Number of features seen during :term:`fit`.
-
-        .. versionadded:: 0.24
+    feature_importances_ : array of shape = [n_features]
+        The feature importances (the higher, the more important the feature).
 
-    feature_names_in_ : ndarray of shape (`n_features_in_`,)
-        Names of features seen during :term:`fit`. Defined only when `X`
-        has feature names that are all strings.
-
-        .. versionadded:: 1.0
+    n_features_ : int
+        The number of features when ``fit`` is performed.
 
     n_outputs_ : int
         The number of outputs when ``fit`` is performed.
 
-	References
+    oob_score_ : float
+        Score of the training dataset obtained using an out-of-bag estimate.
+
+    oob_prediction_ : array of shape = [n_samples]
+        Prediction computed with out-of-bag estimate on the training set.
+
+    References
     ----------
     .. [1] Nicolai Meinshausen, Quantile Regression Forests
         http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
     """
     def __init__(self,
                  q=None,
-                 n_estimators=100,
-                 *,
-                 criterion='squared_error',
+                 n_estimators=10,
+                 criterion='mse',
                  max_depth=None,
                  min_samples_split=2,
                  min_samples_leaf=1,
                  min_weight_fraction_leaf=0.0,
-                 max_features=1.0,
+                 max_features='auto',
                  max_leaf_nodes=None,
-                 min_impurity_decrease=0.0,
                  bootstrap=True,
+                 oob_score=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0,
-                 warm_start=False,
-                 ccp_alpha=0.0,
-                 max_samples=None):
-
-        estimator_params = RandomForestRegressor().estimator_params
-
+                 warm_start=False):
         super(BaseForestQuantileRegressor, self).__init__(
-            **create_keyword_dict(
-                estimator=DecisionTreeRegressor(),
-                n_estimators=n_estimators,
-                estimator_params=estimator_params,
-                bootstrap=bootstrap,
-                n_jobs=n_jobs,
-                random_state=random_state,
-                verbose=verbose,
-                warm_start=warm_start,
-                max_samples=max_samples)
-            )
+            base_estimator=DecisionTreeRegressor(),
+            n_estimators=n_estimators,
+            estimator_params=("criterion", "max_depth", "min_samples_split",
+                              "min_samples_leaf", "min_weight_fraction_leaf",
+                              "max_features", "max_leaf_nodes",
+                              "random_state"),
+            bootstrap=bootstrap,
+            oob_score=oob_score,
+            n_jobs=n_jobs,
+            random_state=random_state,
+            verbose=verbose,
+            warm_start=warm_start)
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
-        self.min_impurity_decrease = min_impurity_decrease
-        self.ccp_alpha = ccp_alpha
         self.q = q
 
 
 class ExtraTreesQuantileRegressor(ForestQuantileRegressor):
     """
     A extra trees regressor providing quantile estimates.
 
@@ -640,30 +538,31 @@
     n_estimators : int, default=100
         The number of trees in the forest.
 
         .. versionchanged:: 0.22
            The default value of ``n_estimators`` changed from 10 to 100
            in 0.22.
 
-    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
-            default="squared_error"
+    criterion : {"squared_error", "absolute_error"}, default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion and minimizes the L2
-        loss using the mean of each terminal node, "friedman_mse", which uses
-        mean squared error with Friedman's improvement score for potential
-        splits, "absolute_error" for the mean absolute error, which minimizes
-        the L1 loss using the median of each terminal node, and "poisson" which
-        uses reduction in Poisson deviance to find splits.
-        Training using "absolute_error" is significantly slower
-        than when using "squared_error".
+        variance reduction as feature selection criterion, and "absolute_error"
+        for the mean absolute error.
 
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
+        .. deprecated:: 1.0
+            Criterion "mse" was deprecated in v1.0 and will be removed in
+            version 1.2. Use `criterion="squared_error"` which is equivalent.
+
+        .. deprecated:: 1.0
+            Criterion "mae" was deprecated in v1.0 and will be removed in
+            version 1.2. Use `criterion="absolute_error"` which is equivalent.
+
     max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
     min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
@@ -697,15 +596,15 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `max(1, int(max_features * n_features_in_))` features are considered at each
+          `round(max_features * n_features)` features are considered at each
           split.
         - If "auto", then `max_features=n_features`.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
@@ -746,38 +645,43 @@
 
         .. versionadded:: 0.19
 
     bootstrap : bool, default=False
         Whether bootstrap samples are used when building trees. If False, the
         whole dataset is used to build each tree.
 
+    oob_score : bool, default=False
+        Whether to use out-of-bag samples to estimate the generalization score.
+        Only available if bootstrap=True.
+
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
         :meth:`decision_path` and :meth:`apply` are all parallelized over the
         trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
         context. ``-1`` means using all processors. See :term:`Glossary
         <n_jobs>` for more details.
 
     random_state : int, RandomState instance or None, default=None
         Controls 3 sources of randomness:
+
         - the bootstrapping of the samples used when building trees
           (if ``bootstrap=True``)
         - the sampling of the features to consider when looking for the best
           split at each node (if ``max_features < n_features``)
         - the draw of the splits for each of the `max_features`
+
         See :term:`Glossary <random_state>` for details.
 
     verbose : int, default=0
         Controls the verbosity when fitting and predicting.
 
     warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`Glossary <warm_start>` and
-        :ref:`gradient_boosting_warm_start` for details.
+        new forest. See :term:`the Glossary <warm_start>`.
 
     ccp_alpha : non-negative float, default=0.0
         Complexity parameter used for Minimal Cost-Complexity Pruning. The
         subtree with the largest cost complexity that is smaller than
         ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
         :ref:`minimal_cost_complexity_pruning` for details.
 
@@ -792,89 +696,137 @@
         - If float, then draw `max_samples * X.shape[0]` samples. Thus,
           `max_samples` should be in the interval `(0.0, 1.0]`.
 
         .. versionadded:: 0.22
 
     Attributes
     ----------
-    estimator_ : :class:`~sklearn.tree.ExtraTreeRegressor`
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. versionadded:: 1.2
-           `base_estimator_` was renamed to `estimator_`.
-
     base_estimator_ : ExtraTreeRegressor
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
-        .. deprecated:: 1.2
-            `base_estimator_` is deprecated and will be removed in 1.4.
-            Use `estimator_` instead.
-
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
         total reduction of the criterion brought by that feature.  It is also
         known as the Gini importance.
+
         Warning: impurity-based feature importances can be misleading for
         high cardinality features (many unique values). See
         :func:`sklearn.inspection.permutation_importance` as an alternative.
 
+    n_features_ : int
+        The number of features.
+
+        .. deprecated:: 1.0
+            Attribute `n_features_` was deprecated in version 1.0 and will be
+            removed in 1.2. Use `n_features_in_` instead.
+
     n_features_in_ : int
         Number of features seen during :term:`fit`.
 
         .. versionadded:: 0.24
 
     feature_names_in_ : ndarray of shape (`n_features_in_`,)
         Names of features seen during :term:`fit`. Defined only when `X`
         has feature names that are all strings.
 
         .. versionadded:: 1.0
 
     n_outputs_ : int
         The number of outputs.
-    """
-    def __init__(self,
-                 n_estimators=100,
-                 q=None,
-                 *,
-                 criterion="squared_error",
-                 max_depth=None,
-                 min_samples_split=2,
-                 min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0,
-                 max_features=1.0,
-                 max_leaf_nodes=None,
-                 min_impurity_decrease=0.0,
-                 bootstrap=False,
-                 n_jobs=None,
-                 random_state=None,
-                 verbose=0,
-                 warm_start=False,
-                 ccp_alpha=0.0,
-                 max_samples=None):
 
-        estimator_params = ExtraTreesRegressor().estimator_params
+    oob_score_ : float
+        Score of the training dataset obtained using an out-of-bag estimate.
+        This attribute exists only when ``oob_score`` is True.
+
+    oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
+        Prediction computed with out-of-bag estimate on the training set.
+        This attribute exists only when ``oob_score`` is True.
+
+    See Also
+    --------
+    ExtraTreesClassifier : An extra-trees classifier with random splits.
+    RandomForestClassifier : A random forest classifier with optimal splits.
+    RandomForestRegressor : Ensemble regressor using trees with optimal splits.
+
+    Notes
+    -----
+    The default values for the parameters controlling the size of the trees
+    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
+    unpruned trees which can potentially be very large on some data sets. To
+    reduce memory consumption, the complexity and size of the trees should be
+    controlled by setting those parameter values.
 
+    References
+    ----------
+    .. [1] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized trees",
+           Machine Learning, 63(1), 3-42, 2006.
+
+    Examples
+    --------
+    >>> from sklearn.datasets import load_diabetes
+    >>> from sklearn.model_selection import train_test_split
+    >>> from sklearn.ensemble import ExtraTreesRegressor
+    >>> X, y = load_diabetes(return_X_y=True)
+    >>> X_train, X_test, y_train, y_test = train_test_split(
+    ...     X, y, random_state=0)
+    >>> reg = ExtraTreesRegressor(n_estimators=100, random_state=0).fit(
+    ...    X_train, y_train)
+    >>> reg.score(X_test, y_test)
+    0.2727...
+    """
+    def __init__(
+        self,
+        n_estimators=100,
+        q=None,
+        *,
+        criterion="squared_error",
+        max_depth=None,
+        min_samples_split=2,
+        min_samples_leaf=1,
+        min_weight_fraction_leaf=0.0,
+        max_features=1.0,
+        max_leaf_nodes=None,
+        min_impurity_decrease=0.0,
+        bootstrap=False,
+        oob_score=False,
+        n_jobs=None,
+        random_state=None,
+        verbose=0,
+        warm_start=False,
+        ccp_alpha=0.0,
+        max_samples=None,
+    ):
         super().__init__(
-            **create_keyword_dict(
-                estimator=ExtraTreeRegressor(),
-                n_estimators=n_estimators,
-                estimator_params=estimator_params,
-                bootstrap=bootstrap,
-                n_jobs=n_jobs,
-                random_state=random_state,
-                verbose=verbose,
-                warm_start=warm_start,
-                max_samples=max_samples)
+            base_estimator=ExtraTreeRegressor(),
+            n_estimators=n_estimators,
+            estimator_params=(
+                "criterion",
+                "max_depth",
+                "min_samples_split",
+                "min_samples_leaf",
+                "min_weight_fraction_leaf",
+                "max_features",
+                "max_leaf_nodes",
+                "min_impurity_decrease",
+                "random_state",
+                "ccp_alpha",
+            ),
+            bootstrap=bootstrap,
+            oob_score=oob_score,
+            n_jobs=n_jobs,
+            random_state=random_state,
+            verbose=verbose,
+            warm_start=warm_start,
+            max_samples=max_samples,
         )
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
@@ -894,263 +846,159 @@
     For mathematical accuracy use :func:`sklearn_quantile.RandomForestQuantileRegressor`.
 
     Parameters
     ----------
     q : float or array-like, optional
         Quantiles used for prediction (values ranging from 0 to 1)
 
-    n_estimators : int, default=100
+    n_estimators : integer, optional (default=10)
         The number of trees in the forest.
 
-        .. versionchanged:: 0.22
-           The default value of ``n_estimators`` changed from 10 to 100
-           in 0.22.
-
-    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
-            default="squared_error"
+    criterion : string, optional (default="mse")
         The function to measure the quality of a split. Supported criteria
-        are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion and minimizes the L2
-        loss using the mean of each terminal node, "friedman_mse", which uses
-        mean squared error with Friedman's improvement score for potential
-        splits, "absolute_error" for the mean absolute error, which minimizes
-        the L1 loss using the median of each terminal node, and "poisson" which
-        uses reduction in Poisson deviance to find splits.
-        Training using "absolute_error" is significantly slower
-        than when using "squared_error".
-
+        are "mse" for the mean squared error, which is equal to variance
+        reduction as feature selection criterion, and "mae" for the mean
+        absolute error.
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
-        .. versionadded:: 1.0
-           Poisson criterion.
+    max_features : int, float, string or None, optional (default="auto")
+        The number of features to consider when looking for the best split:
+        - If int, then consider `max_features` features at each split.
+        - If float, then `max_features` is a percentage and
+          `int(max_features * n_features)` features are considered at each
+          split.
+        - If "auto", then `max_features=n_features`.
+        - If "sqrt", then `max_features=sqrt(n_features)`.
+        - If "log2", then `max_features=log2(n_features)`.
+        - If None, then `max_features=n_features`.
+        Note: the search for a split does not stop until at least one
+        valid partition of the node samples is found, even if it requires to
+        effectively inspect more than ``max_features`` features.
 
-    max_depth : int, default=None
+    max_depth : integer or None, optional (default=None)
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
-    min_samples_split : int or float, default=2
+    min_samples_split : int, float, optional (default=2)
         The minimum number of samples required to split an internal node:
-
         - If int, then consider `min_samples_split` as the minimum number.
-        - If float, then `min_samples_split` is a fraction and
+        - If float, then `min_samples_split` is a percentage and
           `ceil(min_samples_split * n_samples)` are the minimum
           number of samples for each split.
-
         .. versionchanged:: 0.18
-           Added float values for fractions.
-
-    min_samples_leaf : int or float, default=1
-        The minimum number of samples required to be at a leaf node.
-        A split point at any depth will only be considered if it leaves at
-        least ``min_samples_leaf`` training samples in each of the left and
-        right branches.  This may have the effect of smoothing the model,
-        especially in regression.
+           Added float values for percentages.
 
+    min_samples_leaf : int, float, optional (default=1)
+        The minimum number of samples required to be at a leaf node:
         - If int, then consider `min_samples_leaf` as the minimum number.
-        - If float, then `min_samples_leaf` is a fraction and
+        - If float, then `min_samples_leaf` is a percentage and
           `ceil(min_samples_leaf * n_samples)` are the minimum
           number of samples for each node.
-
         .. versionchanged:: 0.18
-           Added float values for fractions.
+           Added float values for percentages.
 
-    min_weight_fraction_leaf : float, default=0.0
+    min_weight_fraction_leaf : float, optional (default=0.)
         The minimum weighted fraction of the sum total of weights (of all
         the input samples) required to be at a leaf node. Samples have
         equal weight when sample_weight is not provided.
 
-    max_features : {"sqrt", "log2", None}, int or float, default=1.0
-        The number of features to consider when looking for the best split:
-
-        - If int, then consider `max_features` features at each split.
-        - If float, then `max_features` is a fraction and
-          `max(1, int(max_features * n_features_in_))` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
-        - If "sqrt", then `max_features=sqrt(n_features)`.
-        - If "log2", then `max_features=log2(n_features)`.
-        - If None or 1.0, then `max_features=n_features`.
-
-        .. note::
-            The default of 1.0 is equivalent to bagged trees and more
-            randomness can be achieved by setting smaller values, e.g. 0.3.
-
-        .. versionchanged:: 1.1
-            The default of `max_features` changed from `"auto"` to 1.0.
-
-        .. deprecated:: 1.1
-            The `"auto"` option was deprecated in 1.1 and will be removed
-            in 1.3.
-
-        Note: the search for a split does not stop until at least one
-        valid partition of the node samples is found, even if it requires to
-        effectively inspect more than ``max_features`` features.
-
-    max_leaf_nodes : int, default=None
+    max_leaf_nodes : int or None, optional (default=None)
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
-    min_impurity_decrease : float, default=0.0
-        A node will be split if this split induces a decrease of the impurity
-        greater than or equal to this value.
-
-        The weighted impurity decrease equation is the following::
-
-            N_t / N * (impurity - N_t_R / N_t * right_impurity
-                                - N_t_L / N_t * left_impurity)
-
-        where ``N`` is the total number of samples, ``N_t`` is the number of
-        samples at the current node, ``N_t_L`` is the number of samples in the
-        left child, and ``N_t_R`` is the number of samples in the right child.
-
-        ``N``, ``N_t``, ``N_t_R`` and ``N_t_L`` all refer to the weighted sum,
-        if ``sample_weight`` is passed.
-
-        .. versionadded:: 0.19
-
-    bootstrap : bool, default=True
-        Whether bootstrap samples are used when building trees. If False, the
-        whole dataset is used to build each tree.
-
-    n_jobs : int, default=None
-        The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
-        :meth:`decision_path` and :meth:`apply` are all parallelized over the
-        trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
-        context. ``-1`` means using all processors. See :term:`Glossary
-        <n_jobs>` for more details.
+    bootstrap : boolean, optional (default=True)
+        Whether bootstrap samples are used when building trees.
 
-    random_state : int, RandomState instance or None, default=None
-        Controls both the randomness of the bootstrapping of the samples used
-        when building trees (if ``bootstrap=True``) and the sampling of the
-        features to consider when looking for the best split at each node
-        (if ``max_features < n_features``).
-        See :term:`Glossary <random_state>` for details.
+    oob_score : bool, optional (default=False)
+        whether to use out-of-bag samples to estimate
+        the R^2 on unseen data.
+
+    n_jobs : integer, optional (default=1)
+        The number of jobs to run in parallel for both `fit` and `predict`.
+        If -1, then the number of jobs is set to the number of cores.
+
+    random_state : int, RandomState instance or None, optional (default=None)
+        If int, random_state is the seed used by the random number generator;
+        If RandomState instance, random_state is the random number generator;
+        If None, the random number generator is the RandomState instance used
+        by `np.random`.
 
-    verbose : int, default=0
-        Controls the verbosity when fitting and predicting.
+    verbose : int, optional (default=0)
+        Controls the verbosity of the tree building process.
 
-    warm_start : bool, default=False
+    warm_start : bool, optional (default=False)
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`Glossary <warm_start>` and
-        :ref:`gradient_boosting_warm_start` for details.
-
-    ccp_alpha : non-negative float, default=0.0
-        Complexity parameter used for Minimal Cost-Complexity Pruning. The
-        subtree with the largest cost complexity that is smaller than
-        ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
-        :ref:`minimal_cost_complexity_pruning` for details.
-
-        .. versionadded:: 0.22
-
-    max_samples : int or float, default=None
-        If bootstrap is True, the number of samples to draw from X
-        to train each base estimator.
-        - If None (default), then draw `X.shape[0]` samples.
-        - If int, then draw `max_samples` samples.
-        - If float, then draw `max_samples * X.shape[0]` samples. Thus,
-          `max_samples` should be in the interval `(0.0, 1.0]`.
-
-        .. versionadded:: 0.22
+        new forest.
 
     Attributes
     ----------
-    estimator_ : :class:`~sklearn.tree.DecisionTreeRegressor`
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. versionadded:: 1.2
-           `base_estimator_` was renamed to `estimator_`.
-
-    base_estimator_ : DecisionTreeRegressor
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. deprecated:: 1.2
-            `base_estimator_` is deprecated and will be removed in 1.4.
-            Use `estimator_` instead.
-
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
-    feature_importances_ : ndarray of shape (n_features,)
-        The impurity-based feature importances.
-        The higher, the more important the feature.
-        The importance of a feature is computed as the (normalized)
-        total reduction of the criterion brought by that feature.  It is also
-        known as the Gini importance.
-        Warning: impurity-based feature importances can be misleading for
-        high cardinality features (many unique values). See
-        :func:`sklearn.inspection.permutation_importance` as an alternative.
+    feature_importances_ : array of shape = [n_features]
+        The feature importances (the higher, the more important the feature).
 
-    n_features_in_ : int
-        Number of features seen during :term:`fit`.
-
-        .. versionadded:: 0.24
-
-    feature_names_in_ : ndarray of shape (`n_features_in_`,)
-        Names of features seen during :term:`fit`. Defined only when `X`
-        has feature names that are all strings.
-
-        .. versionadded:: 1.0
+    n_features_ : int
+        The number of features when ``fit`` is performed.
 
     n_outputs_ : int
         The number of outputs when ``fit`` is performed.
 
-	References
+    oob_score_ : float
+        Score of the training dataset obtained using an out-of-bag estimate.
+
+    oob_prediction_ : array of shape = [n_samples]
+        Prediction computed with out-of-bag estimate on the training set.
+
+    References
     ----------
     .. [1] Nicolai Meinshausen, Quantile Regression Forests
         http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
     """
     def __init__(self,
                  q=None,
-                 n_estimators=100,
-                 *,
-                 criterion='squared_error',
+                 n_estimators=10,
+                 criterion='mse',
                  max_depth=None,
                  min_samples_split=2,
                  min_samples_leaf=1,
                  min_weight_fraction_leaf=0.0,
-                 max_features=1.0,
+                 max_features='auto',
                  max_leaf_nodes=None,
-                 min_impurity_decrease=0.0,
                  bootstrap=True,
+                 oob_score=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0,
-                 warm_start=False,
-                 ccp_alpha=0.0,
-                 max_samples=None):
-        estimator_params = RandomForestRegressor().estimator_params
-
+                 warm_start=False):
         super(BaseForestQuantileRegressor, self).__init__(
-            **create_keyword_dict(
-                estimator=DecisionTreeRegressor(),
-                n_estimators=n_estimators,
-                estimator_params=estimator_params,
-                bootstrap=bootstrap,
-                n_jobs=n_jobs,
-                random_state=random_state,
-                verbose=verbose,
-                warm_start=warm_start,
-                max_samples=max_samples)
-        )
+            base_estimator=DecisionTreeRegressor(),
+            n_estimators=n_estimators,
+            estimator_params=("criterion", "max_depth", "min_samples_split",
+                              "min_samples_leaf", "min_weight_fraction_leaf",
+                              "max_features", "max_leaf_nodes",
+                              "random_state"),
+            bootstrap=bootstrap,
+            oob_score=oob_score,
+            n_jobs=n_jobs,
+            random_state=random_state,
+            verbose=verbose,
+            warm_start=warm_start)
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
-        self.min_impurity_decrease = min_impurity_decrease
-        self.ccp_alpha = ccp_alpha
         self.q = q
 
 
 class SampleExtraTreesQuantileRegressor(SampleForestQuantileRegressor):
     """
     An approximation extra trees regressor providing quantile estimates.
 
@@ -1166,30 +1014,31 @@
     n_estimators : int, default=100
         The number of trees in the forest.
 
         .. versionchanged:: 0.22
            The default value of ``n_estimators`` changed from 10 to 100
            in 0.22.
 
-    criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
-            default="squared_error"
+    criterion : {"squared_error", "absolute_error"}, default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
-        variance reduction as feature selection criterion and minimizes the L2
-        loss using the mean of each terminal node, "friedman_mse", which uses
-        mean squared error with Friedman's improvement score for potential
-        splits, "absolute_error" for the mean absolute error, which minimizes
-        the L1 loss using the median of each terminal node, and "poisson" which
-        uses reduction in Poisson deviance to find splits.
-        Training using "absolute_error" is significantly slower
-        than when using "squared_error".
+        variance reduction as feature selection criterion, and "absolute_error"
+        for the mean absolute error.
 
         .. versionadded:: 0.18
            Mean Absolute Error (MAE) criterion.
 
+        .. deprecated:: 1.0
+            Criterion "mse" was deprecated in v1.0 and will be removed in
+            version 1.2. Use `criterion="squared_error"` which is equivalent.
+
+        .. deprecated:: 1.0
+            Criterion "mae" was deprecated in v1.0 and will be removed in
+            version 1.2. Use `criterion="absolute_error"` which is equivalent.
+
     max_depth : int, default=None
         The maximum depth of the tree. If None, then nodes are expanded until
         all leaves are pure or until all leaves contain less than
         min_samples_split samples.
 
     min_samples_split : int or float, default=2
         The minimum number of samples required to split an internal node:
@@ -1223,15 +1072,15 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `max(1, int(max_features * n_features_in_))` features are considered at each
+          `round(max_features * n_features)` features are considered at each
           split.
         - If "auto", then `max_features=n_features`.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
@@ -1272,38 +1121,43 @@
 
         .. versionadded:: 0.19
 
     bootstrap : bool, default=False
         Whether bootstrap samples are used when building trees. If False, the
         whole dataset is used to build each tree.
 
+    oob_score : bool, default=False
+        Whether to use out-of-bag samples to estimate the generalization score.
+        Only available if bootstrap=True.
+
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
         :meth:`decision_path` and :meth:`apply` are all parallelized over the
         trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
         context. ``-1`` means using all processors. See :term:`Glossary
         <n_jobs>` for more details.
 
     random_state : int, RandomState instance or None, default=None
         Controls 3 sources of randomness:
+
         - the bootstrapping of the samples used when building trees
           (if ``bootstrap=True``)
         - the sampling of the features to consider when looking for the best
           split at each node (if ``max_features < n_features``)
         - the draw of the splits for each of the `max_features`
+
         See :term:`Glossary <random_state>` for details.
 
     verbose : int, default=0
         Controls the verbosity when fitting and predicting.
 
     warm_start : bool, default=False
         When set to ``True``, reuse the solution of the previous call to fit
         and add more estimators to the ensemble, otherwise, just fit a whole
-        new forest. See :term:`Glossary <warm_start>` and
-        :ref:`gradient_boosting_warm_start` for details.
+        new forest. See :term:`the Glossary <warm_start>`.
 
     ccp_alpha : non-negative float, default=0.0
         Complexity parameter used for Minimal Cost-Complexity Pruning. The
         subtree with the largest cost complexity that is smaller than
         ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
         :ref:`minimal_cost_complexity_pruning` for details.
 
@@ -1318,88 +1172,137 @@
         - If float, then draw `max_samples * X.shape[0]` samples. Thus,
           `max_samples` should be in the interval `(0.0, 1.0]`.
 
         .. versionadded:: 0.22
 
     Attributes
     ----------
-    estimator_ : :class:`~sklearn.tree.ExtraTreeRegressor`
-        The child estimator template used to create the collection of fitted
-        sub-estimators.
-
-        .. versionadded:: 1.2
-           `base_estimator_` was renamed to `estimator_`.
-
     base_estimator_ : ExtraTreeRegressor
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
-        .. deprecated:: 1.2
-            `base_estimator_` is deprecated and will be removed in 1.4.
-            Use `estimator_` instead.
-
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
         total reduction of the criterion brought by that feature.  It is also
         known as the Gini importance.
+
         Warning: impurity-based feature importances can be misleading for
         high cardinality features (many unique values). See
         :func:`sklearn.inspection.permutation_importance` as an alternative.
 
+    n_features_ : int
+        The number of features.
+
+        .. deprecated:: 1.0
+            Attribute `n_features_` was deprecated in version 1.0 and will be
+            removed in 1.2. Use `n_features_in_` instead.
+
     n_features_in_ : int
         Number of features seen during :term:`fit`.
 
         .. versionadded:: 0.24
 
     feature_names_in_ : ndarray of shape (`n_features_in_`,)
         Names of features seen during :term:`fit`. Defined only when `X`
         has feature names that are all strings.
 
         .. versionadded:: 1.0
 
     n_outputs_ : int
         The number of outputs.
-    """
-    def __init__(self,
-                 n_estimators=100,
-                 q=None,
-                 *,
-                 criterion="squared_error",
-                 max_depth=None,
-                 min_samples_split=2,
-                 min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0,
-                 max_features=1.0,
-                 max_leaf_nodes=None,
-                 min_impurity_decrease=0.0,
-                 bootstrap=False,
-                 n_jobs=None,
-                 random_state=None,
-                 verbose=0,
-                 warm_start=False,
-                 ccp_alpha=0.0,
-                 max_samples=None):
-        estimator_params = ExtraTreesRegressor().estimator_params
 
+    oob_score_ : float
+        Score of the training dataset obtained using an out-of-bag estimate.
+        This attribute exists only when ``oob_score`` is True.
+
+    oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
+        Prediction computed with out-of-bag estimate on the training set.
+        This attribute exists only when ``oob_score`` is True.
+
+    See Also
+    --------
+    ExtraTreesClassifier : An extra-trees classifier with random splits.
+    RandomForestClassifier : A random forest classifier with optimal splits.
+    RandomForestRegressor : Ensemble regressor using trees with optimal splits.
+
+    Notes
+    -----
+    The default values for the parameters controlling the size of the trees
+    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
+    unpruned trees which can potentially be very large on some data sets. To
+    reduce memory consumption, the complexity and size of the trees should be
+    controlled by setting those parameter values.
+
+    References
+    ----------
+    .. [1] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized trees",
+           Machine Learning, 63(1), 3-42, 2006.
+
+    Examples
+    --------
+    >>> from sklearn.datasets import load_diabetes
+    >>> from sklearn.model_selection import train_test_split
+    >>> from sklearn.ensemble import ExtraTreesRegressor
+    >>> X, y = load_diabetes(return_X_y=True)
+    >>> X_train, X_test, y_train, y_test = train_test_split(
+    ...     X, y, random_state=0)
+    >>> reg = ExtraTreesRegressor(n_estimators=100, random_state=0).fit(
+    ...    X_train, y_train)
+    >>> reg.score(X_test, y_test)
+    0.2727...
+    """
+    def __init__(
+        self,
+        n_estimators=100,
+        q=None,
+        *,
+        criterion="squared_error",
+        max_depth=None,
+        min_samples_split=2,
+        min_samples_leaf=1,
+        min_weight_fraction_leaf=0.0,
+        max_features=1.0,
+        max_leaf_nodes=None,
+        min_impurity_decrease=0.0,
+        bootstrap=False,
+        oob_score=False,
+        n_jobs=None,
+        random_state=None,
+        verbose=0,
+        warm_start=False,
+        ccp_alpha=0.0,
+        max_samples=None,
+    ):
         super().__init__(
-            **create_keyword_dict(
-                estimator=ExtraTreeRegressor(),
-                n_estimators=n_estimators,
-                estimator_params=estimator_params,
-                bootstrap=bootstrap,
-                n_jobs=n_jobs,
-                random_state=random_state,
-                verbose=verbose,
-                warm_start=warm_start,
-                max_samples=max_samples)
+            base_estimator=ExtraTreeRegressor(),
+            n_estimators=n_estimators,
+            estimator_params=(
+                "criterion",
+                "max_depth",
+                "min_samples_split",
+                "min_samples_leaf",
+                "min_weight_fraction_leaf",
+                "max_features",
+                "max_leaf_nodes",
+                "min_impurity_decrease",
+                "random_state",
+                "ccp_alpha",
+            ),
+            bootstrap=bootstrap,
+            oob_score=oob_score,
+            n_jobs=n_jobs,
+            random_state=random_state,
+            verbose=verbose,
+            warm_start=warm_start,
+            max_samples=max_samples,
         )
 
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
```

### Comparing `sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pxd` & `sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pxd`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.21/dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pyx` & `sklearn_quantile-0.0.3/sklearn_quantile/utils/weighted_quantile.pyx`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.21/setup.py` & `sklearn_quantile-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
               ["sklearn_quantile/ensemble/quantile.pyx"]),
     Extension("sklearn_quantile.ensemble.maximum",
               ["sklearn_quantile/ensemble/maximum.pyx"])
 ]
 
 setup(
     name='sklearn_quantile',
-    version='0.0.21',
+    version='0.0.3',
     packages=find_packages(),
     url='https://github.com/jasperroebroek/sklearn-quantile',
     license='BSD 3 clause',
     author='Jasper Roebroek',
     author_email='roebroek.jasper@gmail.com',
     ext_modules=cythonize(extensions),
     include_dirs=[numpy.get_include()],
-    setup_requires=['cython', 'numpy', 'setuptools'],
-    install_requires=['scikit-learn>=1.0', 'numpy'],
+    setup_requires=['cython', 'numpy'],
+    install_requires=['sklearn', 'numpy'],
     extras_require={
-        'develop': ['cython', 'scikit-learn>=1.0', 'sphinx', 'sphinx_rtd_theme', 'numpydoc', 'jupyter', 'matplotlib', 'pandas', 'packaging']
+        'develop': ['cython', 'sphinx', 'sphinx_rtd_theme', 'numpydoc', 'jupyter', 'matplotlib', 'pandas']
     },
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
 )
```

### Comparing `sklearn_quantile-0.0.21/sklearn_quantile/base.py` & `sklearn_quantile-0.0.3/sklearn_quantile/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             raise ValueError("Quantiles must be in the range [0, 1]")
 
         return q
 
     def score(self, X, y):
         """
         Mean pinball loss for the quantile regressors.
+
         The average over all quantiles is calculated when more than one is provided.
         """
         q = self.validate_quantiles()
         y_pred = self.predict(X)
         losses = np.empty(q.size)
         for i in range(q.size):
             losses[i] = mean_pinball_loss(y, y_pred[i], alpha=q[i])
```

### Comparing `sklearn_quantile-0.0.21/sklearn_quantile/neighbors/quantile.py` & `sklearn_quantile-0.0.3/sklearn_quantile/neighbors/quantile.py`

 * *Files identical despite different names*

### Comparing `sklearn_quantile-0.0.21/sklearn_quantile.egg-info/SOURCES.txt` & `sklearn_quantile-0.0.3/sklearn_quantile.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/maximum.pyx
-dist/sklearn_quantile-0.0.21/sklearn_quantile/ensemble/quantile.pyx
-dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pxd
-dist/sklearn_quantile-0.0.21/sklearn_quantile/utils/weighted_quantile.pyx
 sklearn_quantile/__init__.py
 sklearn_quantile/base.py
 sklearn_quantile.egg-info/PKG-INFO
 sklearn_quantile.egg-info/SOURCES.txt
 sklearn_quantile.egg-info/dependency_links.txt
 sklearn_quantile.egg-info/requires.txt
 sklearn_quantile.egg-info/top_level.txt
 sklearn_quantile/ensemble/__init__.py
+sklearn_quantile/ensemble/maximum.c
 sklearn_quantile/ensemble/maximum.pyx
+sklearn_quantile/ensemble/quantile.c
 sklearn_quantile/ensemble/quantile.pyx
 sklearn_quantile/neighbors/__init__.py
 sklearn_quantile/neighbors/quantile.py
 sklearn_quantile/utils/__init__.py
-sklearn_quantile/utils/utils.py
+sklearn_quantile/utils/weighted_quantile.c
 sklearn_quantile/utils/weighted_quantile.pxd
 sklearn_quantile/utils/weighted_quantile.pyx
-tests/test_quantile_KNN.py
-tests/test_quantile_RF.py
 tests/test_weighted_quantile.py
```

### Comparing `sklearn_quantile-0.0.21/tests/test_weighted_quantile.py` & `sklearn_quantile-0.0.3/tests/test_weighted_quantile.py`

 * *Files identical despite different names*

