# Comparing `tmp/bimmm-0.0.2.tar.gz` & `tmp/bimmm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bimmm-0.0.2.tar", last modified: Thu Apr 13 09:19:57 2023, max compression
+gzip compressed data, was "dist/bimmm-0.0.3.tar", last modified: Thu Apr 13 09:36:01 2023, max compression
```

## Comparing `bimmm-0.0.2.tar` & `bimmm-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.787352 bimmm-0.0.2/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:19:57.787213 bimmm-0.0.2/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     2315 2023-04-13 09:16:57.000000 bimmm-0.0.2/README.md
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.786408 bimmm-0.0.2/bimmm/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 bimmm-0.0.2/bimmm/__init__.py
--rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 bimmm-0.0.2/bimmm/analyse_mmm_models.py
-drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:19:57.787020 bimmm-0.0.2/bimmm.egg-info/
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     3255 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/PKG-INFO
--rw-r--r--   0 simonteggelaar   (501) staff       (20)      208 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/SOURCES.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/dependency_links.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       52 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/requires.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)        6 2023-04-13 09:19:57.000000 bimmm-0.0.2/bimmm.egg-info/top_level.txt
--rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-04-13 09:19:57.787394 bimmm-0.0.2/setup.cfg
--rw-r--r--   0 simonteggelaar   (501) staff       (20)     1486 2023-04-13 09:19:29.000000 bimmm-0.0.2/setup.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:36:01.013773 bimmm-0.0.3/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     3433 2023-04-13 09:36:01.013630 bimmm-0.0.3/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     2429 2023-04-13 09:35:58.000000 bimmm-0.0.3/README.md
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:36:01.012794 bimmm-0.0.3/bimmm/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        0 2023-02-26 09:19:56.000000 bimmm-0.0.3/bimmm/__init__.py
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)    21775 2023-04-07 12:26:23.000000 bimmm-0.0.3/bimmm/analyse_mmm_models.py
+drwxr-xr-x   0 simonteggelaar   (501) staff       (20)        0 2023-04-13 09:36:01.013427 bimmm-0.0.3/bimmm.egg-info/
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     3433 2023-04-13 09:36:00.000000 bimmm-0.0.3/bimmm.egg-info/PKG-INFO
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)      208 2023-04-13 09:36:00.000000 bimmm-0.0.3/bimmm.egg-info/SOURCES.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        1 2023-04-13 09:36:00.000000 bimmm-0.0.3/bimmm.egg-info/dependency_links.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       57 2023-04-13 09:36:00.000000 bimmm-0.0.3/bimmm.egg-info/requires.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)        6 2023-04-13 09:36:00.000000 bimmm-0.0.3/bimmm.egg-info/top_level.txt
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)       38 2023-04-13 09:36:01.013813 bimmm-0.0.3/setup.cfg
+-rw-r--r--   0 simonteggelaar   (501) staff       (20)     1494 2023-04-13 09:33:19.000000 bimmm-0.0.3/setup.py
```

### Comparing `bimmm-0.0.2/PKG-INFO` & `bimmm-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: bimmm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package that makes it a bit easier to visualize and analyse Marketing Mix Models
 Home-page: UNKNOWN
 Author: Simon Teggelaar
 Author-email: simonteggelaar@gmail.com
 License: MIT
 Description: # `bimmm`
         
         The `bimmm` is a package to analyse MMM models and visualize them
         
         ## Installation
         
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
+        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bimmm.
         
         ```bash
         pip install bimmm
         ```
         
         ## 1. Usage Decomposition for logistic regressions over time
         
@@ -43,25 +43,33 @@
         df_forecast = df_example.iloc[26:]
         
         # Make your model
         formule = 'sales ~ s_curve(decay(tv, 0.3), 3) + s_curve(decay(radio, 0.2), 7) + jackpot + jan + apr + dec + ' \
                   'sunday_near_drawing + event + competitor + consumer_trust'
         model = smf.ols(formula=formule, data=df_train)
         
+        # mmm object maken
         analyse_model = mmm(model=model, var_date=df_train.maand_jaar, df=df_train)
-        analyse_model.actual_vs_fit_graph()
-        analyse_model.decomposition_graph()
+        
+        # Actual vs fit
+        analyse_model.actual_vs_fit_graph().show()
+        
+        # Decompositie
+        analyse_model.decomposition_graph().show()
         analyse_model.decompositie_sum()
         
         # Kosten van de kanalen waarvan je de ROI wilt weten
         media_dict = {'tv': 10, 'radio': 5}
         analyse_model.roi(media_dict, 'sales')
         
+        # Model results
         analyse_model.model_characteristics()
         analyse_model.VIF()
+        
+        # Analyse for adding variables
         analyse_model.select_n_largest_outliers(5)
         analyse_model.check_variables_to_add()
         ``` 
         
         ## License
         
         Copyright (c) 2023 Rumiko
```

### Comparing `bimmm-0.0.2/README.md` & `bimmm-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # `bimmm`
 
 The `bimmm` is a package to analyse MMM models and visualize them
 
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bimmm.
 
 ```bash
 pip install bimmm
 ```
 
 ## 1. Usage Decomposition for logistic regressions over time
 
@@ -35,25 +35,33 @@
 df_forecast = df_example.iloc[26:]
 
 # Make your model
 formule = 'sales ~ s_curve(decay(tv, 0.3), 3) + s_curve(decay(radio, 0.2), 7) + jackpot + jan + apr + dec + ' \
           'sunday_near_drawing + event + competitor + consumer_trust'
 model = smf.ols(formula=formule, data=df_train)
 
+# mmm object maken
 analyse_model = mmm(model=model, var_date=df_train.maand_jaar, df=df_train)
-analyse_model.actual_vs_fit_graph()
-analyse_model.decomposition_graph()
+
+# Actual vs fit
+analyse_model.actual_vs_fit_graph().show()
+
+# Decompositie
+analyse_model.decomposition_graph().show()
 analyse_model.decompositie_sum()
 
 # Kosten van de kanalen waarvan je de ROI wilt weten
 media_dict = {'tv': 10, 'radio': 5}
 analyse_model.roi(media_dict, 'sales')
 
+# Model results
 analyse_model.model_characteristics()
 analyse_model.VIF()
+
+# Analyse for adding variables
 analyse_model.select_n_largest_outliers(5)
 analyse_model.check_variables_to_add()
 ``` 
 
 ## License
 
 Copyright (c) 2023 Rumiko
```

### Comparing `bimmm-0.0.2/bimmm/analyse_mmm_models.py` & `bimmm-0.0.3/bimmm/analyse_mmm_models.py`

 * *Files identical despite different names*

### Comparing `bimmm-0.0.2/bimmm.egg-info/PKG-INFO` & `bimmm-0.0.3/bimmm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: bimmm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package that makes it a bit easier to visualize and analyse Marketing Mix Models
 Home-page: UNKNOWN
 Author: Simon Teggelaar
 Author-email: simonteggelaar@gmail.com
 License: MIT
 Description: # `bimmm`
         
         The `bimmm` is a package to analyse MMM models and visualize them
         
         ## Installation
         
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bixai.
+        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install bimmm.
         
         ```bash
         pip install bimmm
         ```
         
         ## 1. Usage Decomposition for logistic regressions over time
         
@@ -43,25 +43,33 @@
         df_forecast = df_example.iloc[26:]
         
         # Make your model
         formule = 'sales ~ s_curve(decay(tv, 0.3), 3) + s_curve(decay(radio, 0.2), 7) + jackpot + jan + apr + dec + ' \
                   'sunday_near_drawing + event + competitor + consumer_trust'
         model = smf.ols(formula=formule, data=df_train)
         
+        # mmm object maken
         analyse_model = mmm(model=model, var_date=df_train.maand_jaar, df=df_train)
-        analyse_model.actual_vs_fit_graph()
-        analyse_model.decomposition_graph()
+        
+        # Actual vs fit
+        analyse_model.actual_vs_fit_graph().show()
+        
+        # Decompositie
+        analyse_model.decomposition_graph().show()
         analyse_model.decompositie_sum()
         
         # Kosten van de kanalen waarvan je de ROI wilt weten
         media_dict = {'tv': 10, 'radio': 5}
         analyse_model.roi(media_dict, 'sales')
         
+        # Model results
         analyse_model.model_characteristics()
         analyse_model.VIF()
+        
+        # Analyse for adding variables
         analyse_model.select_n_largest_outliers(5)
         analyse_model.check_variables_to_add()
         ``` 
         
         ## License
         
         Copyright (c) 2023 Rumiko
```

### Comparing `bimmm-0.0.2/setup.py` & `bimmm-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="bimmm",
 
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
 
     # Name of Author
     author="Simon Teggelaar",
 
     # your Email address
     author_email="simonteggelaar@gmail.com",
 
@@ -31,15 +31,15 @@
     # url="https://github.com/username/",
     packages=setuptools.find_packages(),
 
     # if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-         "pandas", "numpy", "scipy", "plotly", "statsmodels", "tqdm", "requests"
+         "pandas", "numpy", "scipy", "plotly", "statsmodels", "tqdm", "requests", "lxml"
        ],
 
     license="MIT",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
         "Programming Language :: Python :: 3",
```

