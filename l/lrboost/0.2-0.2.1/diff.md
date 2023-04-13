# Comparing `tmp/lrboost-0.2.tar.gz` & `tmp/lrboost-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrboost-0.2.tar", last modified: Thu Mar 30 18:01:15 2023, max compression
+gzip compressed data, was "lrboost-0.2.1.tar", last modified: Thu Apr 13 21:19:16 2023, max compression
```

## Comparing `lrboost-0.2.tar` & `lrboost-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-03-30 18:01:15.952633 lrboost-0.2/
--rw-r--r--   0 andrewpatton   (501) staff       (20)     1529 2022-01-04 18:43:39.000000 lrboost-0.2/LICENSE
--rw-r--r--   0 andrewpatton   (501) staff       (20)       25 2022-01-04 18:43:39.000000 lrboost-0.2/MANIFEST.in
--rw-r--r--   0 andrewpatton   (501) staff       (20)     3044 2023-03-30 18:01:15.952734 lrboost-0.2/PKG-INFO
--rw-r--r--   0 andrewpatton   (501) staff       (20)     2031 2023-03-30 17:56:43.000000 lrboost-0.2/README.md
-drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-03-30 18:01:15.950464 lrboost-0.2/lrboost/
--rw-r--r--   0 andrewpatton   (501) staff       (20)      208 2023-03-30 17:56:43.000000 lrboost-0.2/lrboost/__init__.py
--rw-r--r--   0 andrewpatton   (501) staff       (20)       20 2023-03-30 17:59:58.000000 lrboost-0.2/lrboost/_version.py
--rw-r--r--   0 andrewpatton   (501) staff       (20)     6313 2023-03-30 17:56:43.000000 lrboost-0.2/lrboost/lrboost.py
-drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-03-30 18:01:15.952376 lrboost-0.2/lrboost/tests/
--rw-r--r--   0 andrewpatton   (501) staff       (20)        0 2022-01-04 23:43:23.000000 lrboost-0.2/lrboost/tests/__init__.py
--rw-r--r--   0 andrewpatton   (501) staff       (20)      257 2022-01-07 21:59:30.000000 lrboost-0.2/lrboost/tests/test_common.py
--rw-r--r--   0 andrewpatton   (501) staff       (20)      543 2022-01-07 21:59:30.000000 lrboost-0.2/lrboost/tests/test_template.py
--rw-r--r--   0 andrewpatton   (501) staff       (20)      584 2022-01-08 18:14:20.000000 lrboost-0.2/lrboost/utils.py
-drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-03-30 18:01:15.951816 lrboost-0.2/lrboost.egg-info/
--rw-r--r--   0 andrewpatton   (501) staff       (20)     3044 2023-03-30 18:01:15.000000 lrboost-0.2/lrboost.egg-info/PKG-INFO
--rw-r--r--   0 andrewpatton   (501) staff       (20)      411 2023-03-30 18:01:15.000000 lrboost-0.2/lrboost.egg-info/SOURCES.txt
--rw-r--r--   0 andrewpatton   (501) staff       (20)        1 2023-03-30 18:01:15.000000 lrboost-0.2/lrboost.egg-info/dependency_links.txt
--rw-r--r--   0 andrewpatton   (501) staff       (20)        1 2022-01-07 22:06:02.000000 lrboost-0.2/lrboost.egg-info/not-zip-safe
--rw-r--r--   0 andrewpatton   (501) staff       (20)      127 2023-03-30 18:01:15.000000 lrboost-0.2/lrboost.egg-info/requires.txt
--rw-r--r--   0 andrewpatton   (501) staff       (20)        8 2023-03-30 18:01:15.000000 lrboost-0.2/lrboost.egg-info/top_level.txt
--rw-r--r--   0 andrewpatton   (501) staff       (20)       32 2023-03-10 19:59:42.000000 lrboost-0.2/requirements.txt
--rw-r--r--   0 andrewpatton   (501) staff       (20)      147 2023-03-30 18:01:15.953076 lrboost-0.2/setup.cfg
--rw-r--r--   0 andrewpatton   (501) staff       (20)     2200 2023-03-30 17:56:43.000000 lrboost-0.2/setup.py
+drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-04-13 21:19:16.333110 lrboost-0.2.1/
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     1529 2022-01-04 18:43:39.000000 lrboost-0.2.1/LICENSE
+-rw-r--r--   0 andrewpatton   (501) staff       (20)       25 2022-01-04 18:43:39.000000 lrboost-0.2.1/MANIFEST.in
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     3137 2023-04-13 21:19:16.333220 lrboost-0.2.1/PKG-INFO
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     2122 2023-03-30 18:15:34.000000 lrboost-0.2.1/README.md
+drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-04-13 21:19:16.330808 lrboost-0.2.1/lrboost/
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      208 2023-03-30 17:56:43.000000 lrboost-0.2.1/lrboost/__init__.py
+-rw-r--r--   0 andrewpatton   (501) staff       (20)       22 2023-04-13 21:17:48.000000 lrboost-0.2.1/lrboost/_version.py
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     6307 2023-04-13 21:18:23.000000 lrboost-0.2.1/lrboost/lrboost.py
+drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-04-13 21:19:16.332811 lrboost-0.2.1/lrboost/tests/
+-rw-r--r--   0 andrewpatton   (501) staff       (20)        0 2022-01-04 23:43:23.000000 lrboost-0.2.1/lrboost/tests/__init__.py
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      257 2022-01-07 21:59:30.000000 lrboost-0.2.1/lrboost/tests/test_common.py
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      543 2022-01-07 21:59:30.000000 lrboost-0.2.1/lrboost/tests/test_template.py
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      584 2022-01-08 18:14:20.000000 lrboost-0.2.1/lrboost/utils.py
+drwxr-xr-x   0 andrewpatton   (501) staff       (20)        0 2023-04-13 21:19:16.332148 lrboost-0.2.1/lrboost.egg-info/
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     3137 2023-04-13 21:19:16.000000 lrboost-0.2.1/lrboost.egg-info/PKG-INFO
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      411 2023-04-13 21:19:16.000000 lrboost-0.2.1/lrboost.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewpatton   (501) staff       (20)        1 2023-04-13 21:19:16.000000 lrboost-0.2.1/lrboost.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewpatton   (501) staff       (20)        1 2022-01-07 22:06:02.000000 lrboost-0.2.1/lrboost.egg-info/not-zip-safe
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      127 2023-04-13 21:19:16.000000 lrboost-0.2.1/lrboost.egg-info/requires.txt
+-rw-r--r--   0 andrewpatton   (501) staff       (20)        8 2023-04-13 21:19:16.000000 lrboost-0.2.1/lrboost.egg-info/top_level.txt
+-rw-r--r--   0 andrewpatton   (501) staff       (20)       32 2023-03-10 19:59:42.000000 lrboost-0.2.1/requirements.txt
+-rw-r--r--   0 andrewpatton   (501) staff       (20)      147 2023-04-13 21:19:16.333631 lrboost-0.2.1/setup.cfg
+-rw-r--r--   0 andrewpatton   (501) staff       (20)     2200 2023-03-30 17:56:43.000000 lrboost-0.2.1/setup.py
```

### Comparing `lrboost-0.2/LICENSE` & `lrboost-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lrboost-0.2/PKG-INFO` & `lrboost-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrboost
-Version: 0.2
+Version: 0.2.1
 Summary: Linear Residual Boosting compatible with scikit-learn.
 Home-page: https://github.com/anpatton/lrboost
 Download-URL: https://github.com/anpatton/lrboost
 Maintainer: A. Patton, N. Walker, K. Medvedovsky
 Maintainer-email: anpatt7@gmail.com, bibigon@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -25,14 +25,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src=https://raw.githubusercontent.com/anpatton/lrboost/main/doc/images/lrboost.png width=300>
 
 [![Documentation Status](https://readthedocs.org/projects/lrboost/badge/?version=latest)](https://lrboost.readthedocs.org)
 
+[![PyPI version](https://badge.fury.io/py/lrboost.svg)](https://badge.fury.io/py/lrboost)
+
 lrboost is a [sckit-learn](https://scikit-learn.org/) compatible package for linear residual boosting. lrboost uses a linear estimator to first remove any linear trends from the data, and then uses a separate non-linear estimator to model the remaining non-linear trends. We find that extrapolation tasks or data with linear and non-linear components are the best use cases. Not every modeling task will benefit from lrboost, but we use this in our own work and wanted to share something that made it easy to use.  
 
 For a stable version, install using ``pip``:
 
 ```python
 pip install lrboost
 ```
```

### Comparing `lrboost-0.2/README.md` & `lrboost-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <img src=https://raw.githubusercontent.com/anpatton/lrboost/main/doc/images/lrboost.png width=300>
 
 [![Documentation Status](https://readthedocs.org/projects/lrboost/badge/?version=latest)](https://lrboost.readthedocs.org)
 
+[![PyPI version](https://badge.fury.io/py/lrboost.svg)](https://badge.fury.io/py/lrboost)
+
 lrboost is a [sckit-learn](https://scikit-learn.org/) compatible package for linear residual boosting. lrboost uses a linear estimator to first remove any linear trends from the data, and then uses a separate non-linear estimator to model the remaining non-linear trends. We find that extrapolation tasks or data with linear and non-linear components are the best use cases. Not every modeling task will benefit from lrboost, but we use this in our own work and wanted to share something that made it easy to use.  
 
 For a stable version, install using ``pip``:
 
 ```python
 pip install lrboost
 ```
```

### Comparing `lrboost-0.2/lrboost/lrboost.py` & `lrboost-0.2.1/lrboost/lrboost.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,31 +89,31 @@
 
     def _fit_primary_model(self, X, y, **fit_params):
         self.primary_features_ = fit_params.pop('features', None)
 
         _X = self._validate_primary_X(X)
         self.primary_model.fit(_X, y, **fit_params)
 
-        self.primary_prediction = self.primary_model.predict(_X).reshape(-1,1)
+        self.primary_prediction = self.primary_model.predict(_X).reshape(-1)
         
 
     def _fit_secondary_model(self, X, y, **fit_params):
         self.secondary_features_ = fit_params.pop('features', None)
         
         _X = self._validate_secondary_X(X)
         self.secondary_model.fit(_X, y, **fit_params)
 
     def predict(self, X, detail=False):
         check_is_fitted(self)
 
         primary_X = self._validate_primary_X(X)
         secondary_X = self._validate_secondary_X(X)
 
-        primary_prediction = self.primary_model.predict(primary_X).reshape(-1,1)
-        secondary_prediction = self.secondary_model.predict(secondary_X).reshape(-1,1)
+        primary_prediction = self.primary_model.predict(primary_X).reshape(-1)
+        secondary_prediction = self.secondary_model.predict(secondary_X).reshape(-1)
         final_prediction = primary_prediction + secondary_prediction
         if detail:
             prediction_dict = {
                 "final_prediction": final_prediction,
                 "primary_prediction": primary_prediction,
                 "secondary_prediction": secondary_prediction,
             }
```

### Comparing `lrboost-0.2/lrboost/tests/test_template.py` & `lrboost-0.2.1/lrboost/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `lrboost-0.2/lrboost/utils.py` & `lrboost-0.2.1/lrboost/utils.py`

 * *Files identical despite different names*

### Comparing `lrboost-0.2/lrboost.egg-info/PKG-INFO` & `lrboost-0.2.1/lrboost.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrboost
-Version: 0.2
+Version: 0.2.1
 Summary: Linear Residual Boosting compatible with scikit-learn.
 Home-page: https://github.com/anpatton/lrboost
 Download-URL: https://github.com/anpatton/lrboost
 Maintainer: A. Patton, N. Walker, K. Medvedovsky
 Maintainer-email: anpatt7@gmail.com, bibigon@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -25,14 +25,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src=https://raw.githubusercontent.com/anpatton/lrboost/main/doc/images/lrboost.png width=300>
 
 [![Documentation Status](https://readthedocs.org/projects/lrboost/badge/?version=latest)](https://lrboost.readthedocs.org)
 
+[![PyPI version](https://badge.fury.io/py/lrboost.svg)](https://badge.fury.io/py/lrboost)
+
 lrboost is a [sckit-learn](https://scikit-learn.org/) compatible package for linear residual boosting. lrboost uses a linear estimator to first remove any linear trends from the data, and then uses a separate non-linear estimator to model the remaining non-linear trends. We find that extrapolation tasks or data with linear and non-linear components are the best use cases. Not every modeling task will benefit from lrboost, but we use this in our own work and wanted to share something that made it easy to use.  
 
 For a stable version, install using ``pip``:
 
 ```python
 pip install lrboost
 ```
```

### Comparing `lrboost-0.2/setup.py` & `lrboost-0.2.1/setup.py`

 * *Files identical despite different names*

