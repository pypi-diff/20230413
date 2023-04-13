# Comparing `tmp/gmltools-0.0.47.tar.gz` & `tmp/gmltools-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.47.tar", last modified: Wed Apr 12 11:18:57 2023, max compression
+gzip compressed data, was "gmltools-0.0.48.tar", last modified: Thu Apr 13 10:45:14 2023, max compression
```

## Comparing `gmltools-0.0.47.tar` & `gmltools-0.0.48.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.858407 gmltools-0.0.47/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.47/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.47/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-12 11:18:57.857402 gmltools-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.47/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.785427 gmltools-0.0.47/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.47/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.47/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.47/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.47/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.47/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.47/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-12 11:18:37.000000 gmltools-0.0.47/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 11:18:57.858407 gmltools-0.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-12 11:18:23.000000 gmltools-0.0.47/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.753131 gmltools-0.0.47/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.788073 gmltools-0.0.47/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.47/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.47/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.816420 gmltools-0.0.47/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.47/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.47/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.844938 gmltools-0.0.47/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.47/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.47/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.47/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0   118400 2023-04-12 11:18:07.000000 gmltools-0.0.47/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.47/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.47/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.849351 gmltools-0.0.47/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.47/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 10:42:46.000000 gmltools-0.0.47/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.47/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.855905 gmltools-0.0.47/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.47/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.47/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.47/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.47/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:18:57.813263 gmltools-0.0.47/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-12 11:18:57.000000 gmltools-0.0.47/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 11:18:57.000000 gmltools-0.0.47/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 11:18:57.000000 gmltools-0.0.47/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-12 11:18:57.000000 gmltools-0.0.47/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 11:18:57.000000 gmltools-0.0.47/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.321137 gmltools-0.0.48/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.48/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.48/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-13 10:45:14.320141 gmltools-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.48/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.108501 gmltools-0.0.48/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.48/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.48/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.48/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.48/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.48/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.48/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-13 10:44:42.000000 gmltools-0.0.48/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:45:14.321137 gmltools-0.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-13 10:44:23.000000 gmltools-0.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.046151 gmltools-0.0.48/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.126424 gmltools-0.0.48/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.48/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.48/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.181850 gmltools-0.0.48/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.48/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.48/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.237890 gmltools-0.0.48/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.48/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.48/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.48/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.48/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.48/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     9157 2023-04-13 10:43:05.000000 gmltools-0.0.48/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.275435 gmltools-0.0.48/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.48/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.48/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.48/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.317184 gmltools-0.0.48/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.48/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.48/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.48/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.48/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.166217 gmltools-0.0.48/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.47/LICENSE` & `gmltools-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/Models.ipynb` & `gmltools-0.0.48/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/PKG-INFO` & `gmltools-0.0.48/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.47
+Version: 0.0.48
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.47/README.md` & `gmltools-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.48/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.48/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.48/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.48/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/gmltools.yml` & `gmltools-0.0.48/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/mltools.yml` & `gmltools-0.0.48/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/pyproject.toml` & `gmltools-0.0.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.47"
+version = "0.0.48"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.47/setup.py` & `gmltools-0.0.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.47',
+    'version': '0.0.48',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.47/src/gmltools/To_Do.txt` & `gmltools-0.0.48/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/eda/eda.py` & `gmltools-0.0.48/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/models/bayes.py` & `gmltools-0.0.48/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.48/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/models/model.py` & `gmltools-0.0.48/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1257,14 +1257,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
 
     
     def XGB_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
@@ -1359,14 +1360,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
 
 
     
     def Linear_Regression(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
@@ -1457,14 +1459,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
 
     
     def KNN_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
@@ -1556,14 +1559,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
     
 
 
     
     def DecisionTree_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
@@ -1657,14 +1661,15 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
 
     
     def MLP_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
@@ -1761,14 +1766,16 @@
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+        
+            print(self.model.best_params_)
 
     
 
     def save(self,return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
@@ -1811,14 +1818,15 @@
                 df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
                 df_summary = pd.concat([df_summary, df_best], axis=0,ignore_index=True)
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
             else:
                 df_best.to_excel(file_path, index=False, sheet_name='Sheet2')
             if return_best_metrics:
                 return df_best
+            
 
     def load(self):
 
         """
         Loads a model from a file.
 
         Parameters
```

### Comparing `gmltools-0.0.47/src/gmltools/models/models_info.py` & `gmltools-0.0.48/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.48/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.48/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.48/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.48/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.48/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.47/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.48/src/gmltools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.47
+Version: 0.0.48
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.47/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.48/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

