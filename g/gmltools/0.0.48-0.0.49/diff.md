# Comparing `tmp/gmltools-0.0.48.tar.gz` & `tmp/gmltools-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.48.tar", last modified: Thu Apr 13 10:45:14 2023, max compression
+gzip compressed data, was "gmltools-0.0.49.tar", last modified: Thu Apr 13 10:48:46 2023, max compression
```

## Comparing `gmltools-0.0.48.tar` & `gmltools-0.0.49.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.321137 gmltools-0.0.48/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.48/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.48/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-13 10:45:14.320141 gmltools-0.0.48/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.48/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.108501 gmltools-0.0.48/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.48/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.48/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.48/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.48/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.48/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.48/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-13 10:44:42.000000 gmltools-0.0.48/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 10:45:14.321137 gmltools-0.0.48/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-13 10:44:23.000000 gmltools-0.0.48/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.046151 gmltools-0.0.48/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.126424 gmltools-0.0.48/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.48/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.48/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.181850 gmltools-0.0.48/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.48/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.48/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.237890 gmltools-0.0.48/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.48/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.48/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.48/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.48/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.48/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     9157 2023-04-13 10:43:05.000000 gmltools-0.0.48/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.275435 gmltools-0.0.48/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.48/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.48/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.48/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.317184 gmltools-0.0.48/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.48/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.48/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.48/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.48/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:45:14.166217 gmltools-0.0.48/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 10:45:13.000000 gmltools-0.0.48/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:46.019483 gmltools-0.0.49/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.49/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.49/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-13 10:48:46.018489 gmltools-0.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.49/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.932256 gmltools-0.0.49/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.49/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.49/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.49/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.49/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.49/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.49/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-13 10:48:16.000000 gmltools-0.0.49/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 10:48:46.019483 gmltools-0.0.49/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-13 10:48:36.000000 gmltools-0.0.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.910354 gmltools-0.0.49/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.934249 gmltools-0.0.49/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.49/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.49/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.972129 gmltools-0.0.49/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.49/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.49/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.997605 gmltools-0.0.49/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.49/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.49/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.49/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.49/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.49/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     9021 2023-04-13 10:47:52.000000 gmltools-0.0.49/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:46.004497 gmltools-0.0.49/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.49/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.49/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.49/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:46.015501 gmltools-0.0.49/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.49/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.49/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.49/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.49/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-13 10:48:45.969178 gmltools-0.0.49/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-13 10:48:45.000000 gmltools-0.0.49/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-13 10:48:45.000000 gmltools-0.0.49/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 10:48:45.000000 gmltools-0.0.49/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-13 10:48:45.000000 gmltools-0.0.49/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 10:48:45.000000 gmltools-0.0.49/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.48/LICENSE` & `gmltools-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/Models.ipynb` & `gmltools-0.0.49/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/PKG-INFO` & `gmltools-0.0.49/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.48
+Version: 0.0.49
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.48/README.md` & `gmltools-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.49/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.49/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.49/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.49/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/gmltools.yml` & `gmltools-0.0.49/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/mltools.yml` & `gmltools-0.0.49/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/pyproject.toml` & `gmltools-0.0.49/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.48"
+version = "0.0.49"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.48/setup.py` & `gmltools-0.0.49/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.48',
+    'version': '0.0.49',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.48/src/gmltools/To_Do.txt` & `gmltools-0.0.49/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/eda/eda.py` & `gmltools-0.0.49/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models/bayes.py` & `gmltools-0.0.49/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.49/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models/model.py` & `gmltools-0.0.49/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models/models_info.py` & `gmltools-0.0.49/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.49/src/gmltools/models/timeseriesplit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import numpy as np
 import matplotlib.pyplot as plt
-from sklearn.model_selection import _BaseKFold
-from sklearn.utils import indexable
-from sklearn.utils.validation import _num_samples
 
 class BlockingTimeSeriesSplit():
 
     """
     BlockingTimeSeriesSplit is a variation of TimeSeriesSplit that splits the data into n_splits blocks of equal size.
     https://towardsdatascience.com/4-things-to-do-when-applying-cross-validation-with-time-series-c6a5674ebf3a
     https://neptune.ai/blog/cross-validation-mistakes
```

### Comparing `gmltools-0.0.48/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.49/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.49/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.49/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.49/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.49/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.48/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.49/src/gmltools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.48
+Version: 0.0.49
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.48/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.49/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

