# Comparing `tmp/mfglib-0.1.0.tar.gz` & `tmp/mfglib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfglib-0.1.0.tar", max compression
+gzip compressed data, was "mfglib-0.1.1.tar", max compression
```

## Comparing `mfglib-0.1.0.tar` & `mfglib-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1126 2023-04-13 16:24:47.753554 mfglib-0.1.0/LICENSE
--rw-r--r--   0        0        0     1704 2023-04-13 16:24:47.753554 mfglib-0.1.0/README.md
--rw-r--r--   0        0        0       72 2023-04-13 16:24:47.753554 mfglib-0.1.0/mfglib/__init__.py
--rw-r--r--   0        0        0      283 2023-04-13 16:24:47.753554 mfglib-0.1.0/mfglib/alg/__init__.py
--rw-r--r--   0        0        0     3121 2023-04-13 16:24:47.753554 mfglib-0.1.0/mfglib/alg/abc.py
--rw-r--r--   0        0        0     7937 2023-04-13 16:24:47.753554 mfglib-0.1.0/mfglib/alg/fictitious_play.py
--rw-r--r--   0        0        0     1093 2023-04-13 16:24:47.753554 mfglib-0.1.0/mfglib/alg/greedy_policy_given_mean_field.py
--rw-r--r--   0        0        0    17088 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo.py
--rw-r--r--   0        0        0     1879 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo_constraints.py
--rw-r--r--   0        0        0     2962 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo_obj.py
--rw-r--r--   0        0        0     1935 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo_params.py
--rw-r--r--   0        0        0     1009 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo_policy_given_mean_field.py
--rw-r--r--   0        0        0     3487 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/mf_omo_residual_balancing.py
--rw-r--r--   0        0        0     6435 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/online_mirror_descent.py
--rw-r--r--   0        0        0     7710 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/prior_descent.py
--rw-r--r--   0        0        0     3630 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/q_fn.py
--rw-r--r--   0        0        0     6330 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/alg/utils.py
--rw-r--r--   0        0        0       74 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/__init__.py
--rw-r--r--   0        0        0    14796 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/environment.py
--rw-r--r--   0        0        0        0 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/__init__.py
--rw-r--r--   0        0        0     1167 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/beach_bar.py
--rw-r--r--   0        0        0     2301 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/building_evacuation.py
--rw-r--r--   0        0        0     1504 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/conservative_treasure_hunting.py
--rw-r--r--   0        0        0     2625 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/crowd_motion.py
--rw-r--r--   0        0        0     1643 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/equilibrium_price.py
--rw-r--r--   0        0        0      688 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/left_right.py
--rw-r--r--   0        0        0     2526 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/linear_quadratic.py
--rw-r--r--   0        0        0      859 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/random_linear.py
--rw-r--r--   0        0        0      762 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/rock_paper_scissors.py
--rw-r--r--   0        0        0      922 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/env/examples/susceptible_infected.py
--rw-r--r--   0        0        0     1177 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/mean_field.py
--rw-r--r--   0        0        0     1305 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/metrics.py
--rw-r--r--   0        0        0     4312 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/policy.py
--rw-r--r--   0        0        0        0 2023-04-13 16:24:47.757554 mfglib-0.1.0/mfglib/py.typed
--rw-r--r--   0        0        0     1315 2023-04-13 16:24:47.757554 mfglib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 mfglib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-04-13 17:00:23.245917 mfglib-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2242 2023-04-13 17:00:23.245917 mfglib-0.1.1/README.md
+-rw-r--r--   0        0        0       72 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/__init__.py
+-rw-r--r--   0        0        0     3121 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/abc.py
+-rw-r--r--   0        0        0     7937 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/fictitious_play.py
+-rw-r--r--   0        0        0     1093 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/greedy_policy_given_mean_field.py
+-rw-r--r--   0        0        0    17088 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo.py
+-rw-r--r--   0        0        0     1879 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo_constraints.py
+-rw-r--r--   0        0        0     2962 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo_obj.py
+-rw-r--r--   0        0        0     1935 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo_params.py
+-rw-r--r--   0        0        0     1009 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo_policy_given_mean_field.py
+-rw-r--r--   0        0        0     3487 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/mf_omo_residual_balancing.py
+-rw-r--r--   0        0        0     6435 2023-04-13 17:00:23.245917 mfglib-0.1.1/mfglib/alg/online_mirror_descent.py
+-rw-r--r--   0        0        0     7710 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/alg/prior_descent.py
+-rw-r--r--   0        0        0     3630 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/alg/q_fn.py
+-rw-r--r--   0        0        0     6330 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/alg/utils.py
+-rw-r--r--   0        0        0       74 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/__init__.py
+-rw-r--r--   0        0        0    14796 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/environment.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/__init__.py
+-rw-r--r--   0        0        0     1167 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/beach_bar.py
+-rw-r--r--   0        0        0     2301 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/building_evacuation.py
+-rw-r--r--   0        0        0     1504 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/conservative_treasure_hunting.py
+-rw-r--r--   0        0        0     2625 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/crowd_motion.py
+-rw-r--r--   0        0        0     1643 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/equilibrium_price.py
+-rw-r--r--   0        0        0      688 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/left_right.py
+-rw-r--r--   0        0        0     2526 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/linear_quadratic.py
+-rw-r--r--   0        0        0      859 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/random_linear.py
+-rw-r--r--   0        0        0      762 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/rock_paper_scissors.py
+-rw-r--r--   0        0        0      922 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/env/examples/susceptible_infected.py
+-rw-r--r--   0        0        0     1177 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/mean_field.py
+-rw-r--r--   0        0        0     1305 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/metrics.py
+-rw-r--r--   0        0        0     4312 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/policy.py
+-rw-r--r--   0        0        0        0 2023-04-13 17:00:23.249917 mfglib-0.1.1/mfglib/py.typed
+-rw-r--r--   0        0        0     1390 2023-04-13 17:00:23.249917 mfglib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 mfglib-0.1.1/PKG-INFO
```

### Comparing `mfglib-0.1.0/LICENSE` & `mfglib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/README.md` & `mfglib-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 <h1 align="center">MFGLib: A Library for Mean-Field Games</h1>
 
 <p align="center">
+    <a href='https://mfglib.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/mfglib/badge/?version=latest' alt='Documentation Status' />
+    </a>
     <a href="http://mypy-lang.org/"><img alt="Checked with mypy" src="http://www.mypy-lang.org/static/mypy_badge.svg"></a>
+    <a href="https://github.com/charliermarsh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&label=linting" alt="Ruff" style="max-width:100%;"></a>
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     <a href="https://pycqa.github.io/isort/"><img alt="Imports: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
     <a href="https://opensource.org/licenses/MIT"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
 </p>
 
 ## Overview
 MFGLib is an open-source Python library dedicated to solving Nash equilibria (NEs) for generic mean-field games (MFGs) with a user-friendly and customizable interface, aiming at promoting both applications and research of MFGs. On one hand, it facilitates the creation and analysis of arbitrary user-defined MFG environments with minimal prior knowledge on MFGs. On the other hand, it serves as a modular and extensible code base
 for the community to easily prototype and implement new algorithms and environments of MFGs as well as their variants and generalizations.
 
 The official documentation for MFGLib is available at https://mfglib.readthedocs.io/en/latest/.
 
+## Installation
+
+MFGLib supports all major platforms and can be installed with `pip`:
+
+```
+$ pip install mfglib
+```
+
 ## Citing
 If you wish to cite `MFGLib`, please use the following:
 ```
 @misc{mfglib_code,
     author       = {Guo, X. and Hu, A. and Santamaria, M. and Tajrobehkar, M. and Zhang, J.},
     title        = {{MFGLib}: A Library for Mean Field Games, version 0.1.0},
     howpublished = {\url{https://github.com/radar-research-lab/MFGLib}},
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
              ****** MFGLib: A Library for Mean-Field Games ******
-    [Checked_with_mypy] [Code_style:_black] [Imports:_isort] [License:_MIT]
+[Documentation_Status] [Checked_with_mypy] [Ruff] [Code_style:_black] [Imports:
+                             isort] [License:_MIT]
 ## Overview MFGLib is an open-source Python library dedicated to solving Nash
 equilibria (NEs) for generic mean-field games (MFGs) with a user-friendly and
 customizable interface, aiming at promoting both applications and research of
 MFGs. On one hand, it facilitates the creation and analysis of arbitrary user-
 defined MFG environments with minimal prior knowledge on MFGs. On the other
 hand, it serves as a modular and extensible code base for the community to
 easily prototype and implement new algorithms and environments of MFGs as well
 as their variants and generalizations. The official documentation for MFGLib is
-available at https://mfglib.readthedocs.io/en/latest/. ## Citing If you wish to
-cite `MFGLib`, please use the following: ``` @misc{mfglib_code, author = {Guo,
-X. and Hu, A. and Santamaria, M. and Tajrobehkar, M. and Zhang, J.}, title = {
-{MFGLib}: A Library for Mean Field Games, version 0.1.0}, howpublished = {\url
-{https://github.com/radar-research-lab/MFGLib}}, year = {2023} } ```
+available at https://mfglib.readthedocs.io/en/latest/. ## Installation MFGLib
+supports all major platforms and can be installed with `pip`: ``` $ pip install
+mfglib ``` ## Citing If you wish to cite `MFGLib`, please use the following:
+``` @misc{mfglib_code, author = {Guo, X. and Hu, A. and Santamaria, M. and
+Tajrobehkar, M. and Zhang, J.}, title = {{MFGLib}: A Library for Mean Field
+Games, version 0.1.0}, howpublished = {\url{https://github.com/radar-research-
+lab/MFGLib}}, year = {2023} } ```
```

### Comparing `mfglib-0.1.0/mfglib/alg/abc.py` & `mfglib-0.1.1/mfglib/alg/abc.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/fictitious_play.py` & `mfglib-0.1.1/mfglib/alg/fictitious_play.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/greedy_policy_given_mean_field.py` & `mfglib-0.1.1/mfglib/alg/greedy_policy_given_mean_field.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo.py` & `mfglib-0.1.1/mfglib/alg/mf_omo.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo_constraints.py` & `mfglib-0.1.1/mfglib/alg/mf_omo_constraints.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo_obj.py` & `mfglib-0.1.1/mfglib/alg/mf_omo_obj.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo_params.py` & `mfglib-0.1.1/mfglib/alg/mf_omo_params.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo_policy_given_mean_field.py` & `mfglib-0.1.1/mfglib/alg/mf_omo_policy_given_mean_field.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/mf_omo_residual_balancing.py` & `mfglib-0.1.1/mfglib/alg/mf_omo_residual_balancing.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/online_mirror_descent.py` & `mfglib-0.1.1/mfglib/alg/online_mirror_descent.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/prior_descent.py` & `mfglib-0.1.1/mfglib/alg/prior_descent.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/q_fn.py` & `mfglib-0.1.1/mfglib/alg/q_fn.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/alg/utils.py` & `mfglib-0.1.1/mfglib/alg/utils.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/environment.py` & `mfglib-0.1.1/mfglib/env/environment.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/beach_bar.py` & `mfglib-0.1.1/mfglib/env/examples/beach_bar.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/building_evacuation.py` & `mfglib-0.1.1/mfglib/env/examples/building_evacuation.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/conservative_treasure_hunting.py` & `mfglib-0.1.1/mfglib/env/examples/conservative_treasure_hunting.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/crowd_motion.py` & `mfglib-0.1.1/mfglib/env/examples/crowd_motion.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/equilibrium_price.py` & `mfglib-0.1.1/mfglib/env/examples/equilibrium_price.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/left_right.py` & `mfglib-0.1.1/mfglib/env/examples/left_right.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/linear_quadratic.py` & `mfglib-0.1.1/mfglib/env/examples/linear_quadratic.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/random_linear.py` & `mfglib-0.1.1/mfglib/env/examples/random_linear.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/rock_paper_scissors.py` & `mfglib-0.1.1/mfglib/env/examples/rock_paper_scissors.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/env/examples/susceptible_infected.py` & `mfglib-0.1.1/mfglib/env/examples/susceptible_infected.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/mean_field.py` & `mfglib-0.1.1/mfglib/mean_field.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/metrics.py` & `mfglib-0.1.1/mfglib/metrics.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/mfglib/policy.py` & `mfglib-0.1.1/mfglib/policy.py`

 * *Files identical despite different names*

### Comparing `mfglib-0.1.0/pyproject.toml` & `mfglib-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "mfglib"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Library for Mean-Field Games"
 authors = [
     "Xin Guo <xinguo@berkeley.edu>",
     "Anran Hu <anranhu0107@gmail.com>",
     "Matteo Santamaria <matteosantamaria@berkely.edu>",
     "Mahan Tajrobehkar <mahan_tajrobehkar@berkeley.edu>",  
     "Junzi Zhang <saslascroyale@gmail.com>",
 ]
 readme = "README.md"
+license = "MIT"
+documentation = "https://mfglib.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "^2.0.0"
 optuna = "^3.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `mfglib-0.1.0/PKG-INFO` & `mfglib-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: mfglib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Library for Mean-Field Games
+License: MIT
 Author: Xin Guo
 Author-email: xinguo@berkeley.edu
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: optuna (>=3.1.0,<4.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
+Project-URL: Documentation, https://mfglib.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 <h1 align="center">MFGLib: A Library for Mean-Field Games</h1>
 
 <p align="center">
+    <a href='https://mfglib.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/mfglib/badge/?version=latest' alt='Documentation Status' />
+    </a>
     <a href="http://mypy-lang.org/"><img alt="Checked with mypy" src="http://www.mypy-lang.org/static/mypy_badge.svg"></a>
+    <a href="https://github.com/charliermarsh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&label=linting" alt="Ruff" style="max-width:100%;"></a>
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     <a href="https://pycqa.github.io/isort/"><img alt="Imports: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
     <a href="https://opensource.org/licenses/MIT"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
 </p>
 
 ## Overview
 MFGLib is an open-source Python library dedicated to solving Nash equilibria (NEs) for generic mean-field games (MFGs) with a user-friendly and customizable interface, aiming at promoting both applications and research of MFGs. On one hand, it facilitates the creation and analysis of arbitrary user-defined MFG environments with minimal prior knowledge on MFGs. On the other hand, it serves as a modular and extensible code base
 for the community to easily prototype and implement new algorithms and environments of MFGs as well as their variants and generalizations.
 
 The official documentation for MFGLib is available at https://mfglib.readthedocs.io/en/latest/.
 
+## Installation
+
+MFGLib supports all major platforms and can be installed with `pip`:
+
+```
+$ pip install mfglib
+```
+
 ## Citing
 If you wish to cite `MFGLib`, please use the following:
 ```
 @misc{mfglib_code,
     author       = {Guo, X. and Hu, A. and Santamaria, M. and Tajrobehkar, M. and Zhang, J.},
     title        = {{MFGLib}: A Library for Mean Field Games, version 0.1.0},
     howpublished = {\url{https://github.com/radar-research-lab/MFGLib}},
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1 Name: mfglib Version: 0.1.0 Summary: A Library for Mean-
-Field Games Author: Xin Guo Author-email: xinguo@berkeley.edu Requires-Python:
->=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: optuna (>=3.1.0,<4.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: mfglib Version: 0.1.1 Summary: A Library for Mean-
+Field Games License: MIT Author: Xin Guo Author-email: xinguo@berkeley.edu
+Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: optuna (>=3.1.0,<4.0.0) Requires-
+Dist: torch (>=2.0.0,<3.0.0) Project-URL: Documentation, https://
+mfglib.readthedocs.io/en/latest/ Description-Content-Type: text/markdown
              ****** MFGLib: A Library for Mean-Field Games ******
-    [Checked_with_mypy] [Code_style:_black] [Imports:_isort] [License:_MIT]
+[Documentation_Status] [Checked_with_mypy] [Ruff] [Code_style:_black] [Imports:
+                             isort] [License:_MIT]
 ## Overview MFGLib is an open-source Python library dedicated to solving Nash
 equilibria (NEs) for generic mean-field games (MFGs) with a user-friendly and
 customizable interface, aiming at promoting both applications and research of
 MFGs. On one hand, it facilitates the creation and analysis of arbitrary user-
 defined MFG environments with minimal prior knowledge on MFGs. On the other
 hand, it serves as a modular and extensible code base for the community to
 easily prototype and implement new algorithms and environments of MFGs as well
 as their variants and generalizations. The official documentation for MFGLib is
-available at https://mfglib.readthedocs.io/en/latest/. ## Citing If you wish to
-cite `MFGLib`, please use the following: ``` @misc{mfglib_code, author = {Guo,
-X. and Hu, A. and Santamaria, M. and Tajrobehkar, M. and Zhang, J.}, title = {
-{MFGLib}: A Library for Mean Field Games, version 0.1.0}, howpublished = {\url
-{https://github.com/radar-research-lab/MFGLib}}, year = {2023} } ```
+available at https://mfglib.readthedocs.io/en/latest/. ## Installation MFGLib
+supports all major platforms and can be installed with `pip`: ``` $ pip install
+mfglib ``` ## Citing If you wish to cite `MFGLib`, please use the following:
+``` @misc{mfglib_code, author = {Guo, X. and Hu, A. and Santamaria, M. and
+Tajrobehkar, M. and Zhang, J.}, title = {{MFGLib}: A Library for Mean Field
+Games, version 0.1.0}, howpublished = {\url{https://github.com/radar-research-
+lab/MFGLib}}, year = {2023} } ```
```

