# Comparing `tmp/blinpy-0.1.6.tar.gz` & `tmp/blinpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blinpy-0.1.6.tar", last modified: Sat Mar  4 09:21:35 2023, max compression
+gzip compressed data, was "blinpy-0.1.7.tar", last modified: Thu Apr 13 10:00:11 2023, max compression
```

## Comparing `blinpy-0.1.6.tar` & `blinpy-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-03-04 09:21:35.866458 blinpy-0.1.6/
--rw-rw-r--   0 solant    (1000) solant    (1000)    12056 2023-03-04 09:21:35.866458 blinpy-0.1.6/PKG-INFO
--rw-rw-r--   0 solant    (1000) solant    (1000)     9370 2021-06-22 10:00:59.000000 blinpy-0.1.6/README.md
-drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-03-04 09:21:35.865458 blinpy-0.1.6/blinpy/
--rw-rw-r--   0 solant    (1000) solant    (1000)       21 2021-05-23 02:35:31.000000 blinpy-0.1.6/blinpy/__init__.py
--rw-rw-r--   0 solant    (1000) solant    (1000)     8979 2021-06-30 07:27:57.000000 blinpy-0.1.6/blinpy/models.py
--rw-rw-r--   0 solant    (1000) solant    (1000)    19745 2021-06-30 07:25:25.000000 blinpy-0.1.6/blinpy/utils.py
-drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-03-04 09:21:35.866458 blinpy-0.1.6/blinpy.egg-info/
--rw-rw-r--   0 solant    (1000) solant    (1000)    12056 2023-03-04 09:21:35.000000 blinpy-0.1.6/blinpy.egg-info/PKG-INFO
--rw-rw-r--   0 solant    (1000) solant    (1000)      229 2023-03-04 09:21:35.000000 blinpy-0.1.6/blinpy.egg-info/SOURCES.txt
--rw-rw-r--   0 solant    (1000) solant    (1000)        1 2023-03-04 09:21:35.000000 blinpy-0.1.6/blinpy.egg-info/dependency_links.txt
--rw-rw-r--   0 solant    (1000) solant    (1000)       53 2023-03-04 09:21:35.000000 blinpy-0.1.6/blinpy.egg-info/requires.txt
--rw-rw-r--   0 solant    (1000) solant    (1000)        7 2023-03-04 09:21:35.000000 blinpy-0.1.6/blinpy.egg-info/top_level.txt
--rw-r--r--   0 solant    (1000) solant    (1000)       79 2023-03-04 09:21:35.866458 blinpy-0.1.6/setup.cfg
--rw-rw-r--   0 solant    (1000) solant    (1000)     1038 2023-03-04 09:12:52.000000 blinpy-0.1.6/setup.py
+drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-04-13 10:00:11.158592 blinpy-0.1.7/
+-rw-rw-r--   0 solant    (1000) solant    (1000)    12056 2023-04-13 10:00:11.158592 blinpy-0.1.7/PKG-INFO
+-rw-rw-r--   0 solant    (1000) solant    (1000)     9370 2021-06-22 10:00:59.000000 blinpy-0.1.7/README.md
+drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-04-13 10:00:11.157592 blinpy-0.1.7/blinpy/
+-rw-rw-r--   0 solant    (1000) solant    (1000)       21 2021-05-23 02:35:31.000000 blinpy-0.1.7/blinpy/__init__.py
+-rw-rw-r--   0 solant    (1000) solant    (1000)    10132 2023-04-13 09:47:04.000000 blinpy-0.1.7/blinpy/models.py
+-rw-rw-r--   0 solant    (1000) solant    (1000)    19745 2021-06-30 07:25:25.000000 blinpy-0.1.7/blinpy/utils.py
+drwxrwxr-x   0 solant    (1000) solant    (1000)        0 2023-04-13 10:00:11.158592 blinpy-0.1.7/blinpy.egg-info/
+-rw-rw-r--   0 solant    (1000) solant    (1000)    12056 2023-04-13 10:00:11.000000 blinpy-0.1.7/blinpy.egg-info/PKG-INFO
+-rw-rw-r--   0 solant    (1000) solant    (1000)      229 2023-04-13 10:00:11.000000 blinpy-0.1.7/blinpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 solant    (1000) solant    (1000)        1 2023-04-13 10:00:11.000000 blinpy-0.1.7/blinpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 solant    (1000) solant    (1000)       53 2023-04-13 10:00:11.000000 blinpy-0.1.7/blinpy.egg-info/requires.txt
+-rw-rw-r--   0 solant    (1000) solant    (1000)        7 2023-04-13 10:00:11.000000 blinpy-0.1.7/blinpy.egg-info/top_level.txt
+-rw-r--r--   0 solant    (1000) solant    (1000)       79 2023-04-13 10:00:11.158592 blinpy-0.1.7/setup.cfg
+-rw-rw-r--   0 solant    (1000) solant    (1000)     1038 2023-04-13 09:57:08.000000 blinpy-0.1.7/setup.py
```

### Comparing `blinpy-0.1.6/PKG-INFO` & `blinpy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blinpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bayesian Linear Models in Python
 Home-page: https://github.com/solbes/blinpy
 Author: Antti Solonen
 Author-email: antti.solonen@gmail.com
 License: MIT
-Download-URL: https://github.com/solbes/blinpy/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/solbes/blinpy/archive/refs/tags/0.1.7.tar.gz
 Description: # blinpy - Bayesian LINear models in PYthon
         
         When applying linear regression models in practice, one often ends up going  
         back to the basic formulas to figure out how things work, especially if 
         Gaussian priors are applied. This package is built for this (almost trivial) 
         task of fitting linear-Gaussian models. The package includes a basic numpy 
         engine for fitting a general linear-Gaussian model, plus some model classes
```

### Comparing `blinpy-0.1.6/README.md` & `blinpy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `blinpy-0.1.6/blinpy/models.py` & `blinpy-0.1.7/blinpy/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,25 +42,36 @@
 
         self.pri_cols = pri_cols if pri_cols is not None else self.theta_names
 
         self.post_mu = np.nan * np.zeros(len(self.theta_names))
         self.post_icov = None
         self.boot_samples = None
         self.post_samples = None
+        self.obs_cov = None
 
         # TODO: check system validity
 
     @property
     def _prior_sys(self):
 
         _pri_inds = [self.theta_names.index(col) for col in self.pri_cols]
         pri_sys = np.eye(len(self.input_cols))[_pri_inds, :]
 
         return pri_sys
 
+    def _build_system_matrix(self, data):
+
+        # add intercept if needed
+        _data = data.copy()
+        if self.bias:
+            _data['bias'] = 1.0
+
+        # construct system matrix
+        return np.stack([_data.eval(col).values for col in self.input_cols]).T
+
     def fit(self, data, obs_cov=1.0, pri_mu=None, pri_cov=1.0):
         """Feed data (observation data and possible prior specs) and fit the
         model.
 
         Parameters
         ----------
         data : pd.DataFrame giving both input and output data
@@ -74,27 +85,37 @@
         The model can be used to make predictions and plot validation figs.
 
         """
 
         # TODO: check data validity
         assert isinstance(data, pd.DataFrame), "Data must be pd.DataFrame"
 
-        # add intercept if needed
-        _data = data.copy()
-        if self.bias:
-            _data['bias'] = 1.0
-
         # construct system matrix and obs vector
-        A = np.stack([_data.eval(col).values for col in self.input_cols]).T
-        obs = _data.eval(self.output_col).values
+        A = self._build_system_matrix(data)
+        obs = data.eval(self.output_col).values
+
+        # if MSE requested, fit a model with constant variance first
+        if obs_cov == 'mse':
+            post_mu, _, _ = linfit(
+                obs, A,
+                obs_cov=1.0,
+                pri_mu=pri_mu,
+                B=self._prior_sys,
+                pri_cov=pri_cov,
+            )
+            ypred = A.dot(post_mu[:, np.newaxis])[:, 0]
+            rss = np.sum((obs-ypred)**2)
+            self.obs_cov = rss/(len(obs)-len(post_mu))
+        else:
+            self.obs_cov = obs_cov
 
         # fit the linear gaussian models
         self.post_mu, self.post_icov, _ = linfit(
             obs, A,
-            obs_cov=obs_cov,
+            obs_cov=self.obs_cov,
             pri_mu=pri_mu,
             B=self._prior_sys,
             pri_cov=pri_cov
         )
 
         return self
 
@@ -107,42 +128,63 @@
 
         Returns
         -------
         Returns the posterior predictive mean as numpy vector
 
         """
 
-        # add bias to data if needed
-        _data = data.copy()
-        if self.bias:
-            _data['bias'] = 1.0
-
         # build system matrix
-        A = np.stack([_data.eval(col).values for col in self.input_cols]).T
+        A = self._build_system_matrix(data)
 
         return A.dot(self.post_mu[:, np.newaxis])[:, 0]
 
+    def predict_cov(self, data):
+        """Predictive covariance with a fitted linear model.
+
+        Parameters
+        ----------
+        data: input data as pd.DataFrame
+
+        Returns
+        -------
+        Posterior predictive covariance as numpy array
+        """
+
+        A = self._build_system_matrix(data)
+        return A.dot(np.linalg.solve(self.post_icov, A.T))
+
+    def predict_var(self, data):
+        """Predictive variance with a fitted linear model.
+
+        Parameters
+        ----------
+        data: input data as pd.DataFrame
+
+        Returns
+        -------
+        Posterior predictive variance as a numpy vector
+        """
+
+        A = self._build_system_matrix(data)
+        icov_At = np.linalg.solve(self.post_icov, A.T)
+        return np.sum(A*icov_At.T, axis=1)
+
     @property
     def theta(self):
         return dict(zip(self.theta_names, self.post_mu))
 
     def bootstrap(self, data, obs_cov=1.0, pri_mu=None, pri_cov=1.0,
                   boot_size=None, nsamples=500):
 
         ny = len(data)
         boot_size = boot_size if boot_size is not None else ny
 
-        # add intercept if needed
-        _data = data.copy()
-        if self.bias:
-            _data['bias'] = 1.0
-
         # construct system matrix and obs vector
-        A = np.stack([_data.eval(col).values for col in self.input_cols]).T
-        obs = _data.eval(self.output_col).values
+        A = self._build_system_matrix(data)
+        obs = data.eval(self.output_col).values
 
         # fit in a loop
         samples = np.zeros((len(self.post_mu), nsamples)) * np.nan
         linalg_errors = 0
         for i in range(nsamples):
             try:
                 ii = np.random.randint(ny, size=boot_size)
```

### Comparing `blinpy-0.1.6/blinpy/utils.py` & `blinpy-0.1.7/blinpy/utils.py`

 * *Files identical despite different names*

### Comparing `blinpy-0.1.6/blinpy.egg-info/PKG-INFO` & `blinpy-0.1.7/blinpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blinpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bayesian Linear Models in Python
 Home-page: https://github.com/solbes/blinpy
 Author: Antti Solonen
 Author-email: antti.solonen@gmail.com
 License: MIT
-Download-URL: https://github.com/solbes/blinpy/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/solbes/blinpy/archive/refs/tags/0.1.7.tar.gz
 Description: # blinpy - Bayesian LINear models in PYthon
         
         When applying linear regression models in practice, one often ends up going  
         back to the basic formulas to figure out how things work, especially if 
         Gaussian priors are applied. This package is built for this (almost trivial) 
         task of fitting linear-Gaussian models. The package includes a basic numpy 
         engine for fitting a general linear-Gaussian model, plus some model classes
```

### Comparing `blinpy-0.1.6/setup.py` & `blinpy-0.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fh:
     long_description = fh.read()
 
 setup(
     name='blinpy',
-    version='0.1.6',
+    version='0.1.7',
     packages=['blinpy'],
     url='https://github.com/solbes/blinpy',
-    download_url = 'https://github.com/solbes/blinpy/archive/refs/tags/0.1.6.tar.gz',
+    download_url = 'https://github.com/solbes/blinpy/archive/refs/tags/0.1.7.tar.gz',
     license='MIT',
     author='Antti Solonen',
     author_email='antti.solonen@gmail.com',
     description='Bayesian Linear Models in Python',
     keywords=['bayes', 'linear', 'gam'],
     install_requires=['numpy', 'pandas', 'jsonpickle', 'scipy', 'quadprog'],
     extras_require={
```

