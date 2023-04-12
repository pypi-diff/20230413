# Comparing `tmp/summerepi2-1.2.1.tar.gz` & `tmp/summerepi2-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summerepi2-1.2.1.tar", max compression
+gzip compressed data, was "summerepi2-1.2.2.tar", max compression
```

## Comparing `summerepi2-1.2.1.tar` & `summerepi2-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1930 2023-04-05 00:33:04.703810 summerepi2-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4008 2023-04-05 00:35:47.450662 summerepi2-1.2.1/README.md
--rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.1/summer2/__init__.py
--rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.1/summer2/adjust.py
--rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.1/summer2/compartment.py
--rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.1/summer2/compute_bak/__init__.py
--rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.1/summer2/compute_bak/compute_jax.py
--rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.1/summer2/derived_outputs.py
--rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.1/summer2/experimental/model_builder.py
--rw-r--r--   0        0        0      553 2023-04-05 00:33:04.726311 summerepi2-1.2.1/summer2/extras/test_models.py
--rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.1/summer2/flows.py
--rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.1/summer2/functions/__init__.py
--rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.1/summer2/functions/interpolate.py
--rw-r--r--   0        0        0     3453 2023-02-09 22:50:26.022665 summerepi2-1.2.1/summer2/functions/time.py
--rw-r--r--   0        0        0     1858 2023-01-17 01:00:51.208278 summerepi2-1.2.1/summer2/functions/util.py
--rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.1/summer2/inspect.py
--rw-r--r--   0        0        0    51975 2023-04-05 00:33:04.735811 summerepi2-1.2.1/summer2/model.py
--rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.1/summer2/parameters/__init__.py
--rw-r--r--   0        0        0    10693 2022-10-11 00:26:23.922637 summerepi2-1.2.1/summer2/parameters/param_impl.py
--rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.1/summer2/parameters/params.py
--rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.1/summer2/population.py
--rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.1/summer2/runner/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.1/summer2/runner/jax/__init__.py
--rw-r--r--   0        0        0     5107 2022-11-30 22:02:39.158382 summerepi2-1.2.1/summer2/runner/jax/derived_outputs.py
--rw-r--r--   0        0        0    24110 2023-04-04 20:13:36.901466 summerepi2-1.2.1/summer2/runner/jax/model_impl.py
--rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.1/summer2/runner/jax/ode.py
--rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.1/summer2/runner/jax/ode2.py
--rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.1/summer2/runner/jax/solvers.py
--rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.1/summer2/runner/jax/stratify.py
--rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.1/summer2/runner/model_runner.py
--rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.1/summer2/solver.py
--rw-r--r--   0        0        0    17065 2022-09-01 05:47:20.176421 summerepi2-1.2.1/summer2/stratification.py
--rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.1/summer2/tracker.py
--rw-r--r--   0        0        0     1799 2022-09-01 05:32:08.050495 summerepi2-1.2.1/summer2/utils.py
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 summerepi2-1.2.1/setup.py
--rw-r--r--   0        0        0     5470 1970-01-01 00:00:00.000000 summerepi2-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1930 2023-04-12 23:08:21.398477 summerepi2-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4101 2023-04-12 23:09:18.690955 summerepi2-1.2.2/README.md
+-rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.2/summer2/__init__.py
+-rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.2/summer2/adjust.py
+-rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.2/summer2/compartment.py
+-rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.2/summer2/compute_bak/__init__.py
+-rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.2/summer2/compute_bak/compute_jax.py
+-rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.2/summer2/derived_outputs.py
+-rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.2/summer2/experimental/model_builder.py
+-rw-r--r--   0        0        0      553 2023-04-05 00:33:04.726311 summerepi2-1.2.2/summer2/extras/test_models.py
+-rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.2/summer2/flows.py
+-rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.2/summer2/functions/__init__.py
+-rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.2/summer2/functions/interpolate.py
+-rw-r--r--   0        0        0     3453 2023-02-09 22:50:26.022665 summerepi2-1.2.2/summer2/functions/time.py
+-rw-r--r--   0        0        0     3670 2023-04-12 21:11:57.753156 summerepi2-1.2.2/summer2/functions/util.py
+-rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.2/summer2/inspect.py
+-rw-r--r--   0        0        0    51975 2023-04-05 00:33:04.735811 summerepi2-1.2.2/summer2/model.py
+-rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.2/summer2/parameters/__init__.py
+-rw-r--r--   0        0        0    10693 2022-10-11 00:26:23.922637 summerepi2-1.2.2/summer2/parameters/param_impl.py
+-rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.2/summer2/parameters/params.py
+-rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.2/summer2/population.py
+-rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.2/summer2/runner/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.2/summer2/runner/jax/__init__.py
+-rw-r--r--   0        0        0     5107 2022-11-30 22:02:39.158382 summerepi2-1.2.2/summer2/runner/jax/derived_outputs.py
+-rw-r--r--   0        0        0    24105 2023-04-11 21:29:43.015787 summerepi2-1.2.2/summer2/runner/jax/model_impl.py
+-rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.2/summer2/runner/jax/ode.py
+-rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.2/summer2/runner/jax/ode2.py
+-rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.2/summer2/runner/jax/solvers.py
+-rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.2/summer2/runner/jax/stratify.py
+-rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.2/summer2/runner/model_runner.py
+-rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.2/summer2/solver.py
+-rw-r--r--   0        0        0    17065 2022-09-01 05:47:20.176421 summerepi2-1.2.2/summer2/stratification.py
+-rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.2/summer2/tracker.py
+-rw-r--r--   0        0        0     1799 2022-09-01 05:32:08.050495 summerepi2-1.2.2/summer2/utils.py
+-rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 summerepi2-1.2.2/PKG-INFO
```

### Comparing `summerepi2-1.2.1/LICENSE.txt` & `summerepi2-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/pyproject.toml` & `summerepi2-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "summerepi2"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "http://summerepi.com/"
 documentation = "http://summerepi.com/"
 repository = "https://github.com/monash-emu/summer2"
 keywords = [
     "epidemiology",
```

### Comparing `summerepi2-1.2.1/README.md` & `summerepi2-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,17 @@
 
 Releases are numbered using [Semantic Versioning](https://semver.org/)
 
 - 1.0.0/1:
   - Initial release
 - 1.2.1
   - Dropped support for Python 3.7.  Variety of bugfixes and expanded features, see documentation
+- 1.2.2
+  - Added capture utils
+  - Removed inner jit in model building to improve debugging
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
 - Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)
```

### Comparing `summerepi2-1.2.1/summer2/adjust.py` & `summerepi2-1.2.2/summer2/adjust.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/compartment.py` & `summerepi2-1.2.2/summer2/compartment.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/compute_bak/compute_jax.py` & `summerepi2-1.2.2/summer2/compute_bak/compute_jax.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/derived_outputs.py` & `summerepi2-1.2.2/summer2/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/experimental/model_builder.py` & `summerepi2-1.2.2/summer2/experimental/model_builder.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/extras/test_models.py` & `summerepi2-1.2.2/summer2/extras/test_models.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/flows.py` & `summerepi2-1.2.2/summer2/flows.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/functions/interpolate.py` & `summerepi2-1.2.2/summer2/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/functions/time.py` & `summerepi2-1.2.2/summer2/functions/time.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/inspect.py` & `summerepi2-1.2.2/summer2/inspect.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/model.py` & `summerepi2-1.2.2/summer2/model.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/parameters/param_impl.py` & `summerepi2-1.2.2/summer2/parameters/param_impl.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/parameters/params.py` & `summerepi2-1.2.2/summer2/parameters/params.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/population.py` & `summerepi2-1.2.2/summer2/population.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/jax/derived_outputs.py` & `summerepi2-1.2.2/summer2/runner/jax/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/jax/model_impl.py` & `summerepi2-1.2.2/summer2/runner/jax/model_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
     param_frozen_cg, _ = runner.model.graph.freeze(dyn_params, source_inputs)
 
     # static_cg = param_frozen_cg.filter(exclude=ts_vars)
     # static_graph_func = static_cg.get_callable()(parameters=base_params)
 
     timestep_cg, static_cg = param_frozen_cg.freeze(ts_vars)
 
-    timestep_graph_func = jit(timestep_cg.get_callable())
+    timestep_graph_func = timestep_cg.get_callable()
     # timestep_graph_func = timestep_cg.get_callable()
     static_graph_func = static_cg.get_callable()
 
     rates_funcs = build_get_rates(runner, timestep_graph_func)
     get_rates = rates_funcs["get_rates"]
     get_flow_rates = rates_funcs["get_flow_rates"]
     get_rates_debug = rates_funcs["get_rates_debug"]
```

### Comparing `summerepi2-1.2.1/summer2/runner/jax/ode.py` & `summerepi2-1.2.2/summer2/runner/jax/ode.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/jax/ode2.py` & `summerepi2-1.2.2/summer2/runner/jax/ode2.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/jax/solvers.py` & `summerepi2-1.2.2/summer2/runner/jax/solvers.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/jax/stratify.py` & `summerepi2-1.2.2/summer2/runner/jax/stratify.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/runner/model_runner.py` & `summerepi2-1.2.2/summer2/runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/solver.py` & `summerepi2-1.2.2/summer2/solver.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/stratification.py` & `summerepi2-1.2.2/summer2/stratification.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/summer2/utils.py` & `summerepi2-1.2.2/summer2/utils.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.1/PKG-INFO` & `summerepi2-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: summerepi2
-Version: 1.2.1
+Version: 1.2.2
 Summary: Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.
 Home-page: http://summerepi.com/
 License: BSD-2-Clause
 Keywords: epidemiology,disease,compartmental,infectious
 Author: James Trauer
 Author-email: james.trauer@monash.edu
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: computegraph (==0.4.2)
-Requires-Dist: ipykernel (>=6.15.1,<7.0.0); extra == "docs"
-Requires-Dist: jax[cpu] (>=0.4); sys_platform == "darwin"
-Requires-Dist: jax[cpu] (>=0.4); sys_platform == "linux"
-Requires-Dist: matplotlib (>=3.4.3); extra == "docs"
-Requires-Dist: nbsphinx (>=0.8.2,<0.9.0); extra == "docs"
+Requires-Dist: ipykernel (>=6.15.1,<7.0.0) ; extra == "docs"
+Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "darwin"
+Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "linux"
+Requires-Dist: matplotlib (>=3.4.3) ; extra == "docs"
+Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs"
 Requires-Dist: networkx (>=2.6.2)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: pandas (>=1.3.2)
 Requires-Dist: plotly (>=5.5.0)
-Requires-Dist: recommonmark (>=0.7.1,<0.8.0); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0); extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8); extra == "docs"
+Requires-Dist: recommonmark (>=0.7.1,<0.8.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; extra == "docs"
 Project-URL: Documentation, http://summerepi.com/
 Project-URL: Repository, https://github.com/monash-emu/summer2
 Description-Content-Type: text/markdown
 
 # summer2: compartmental disease modelling in Python
 
 [![Automated Tests](https://github.com/monash-emu/summer2/actions/workflows/tests.yml/badge.svg)](https://github.com/monash-emu/summer2/actions/workflows/tests.yml)
@@ -122,14 +123,17 @@
 
 Releases are numbered using [Semantic Versioning](https://semver.org/)
 
 - 1.0.0/1:
   - Initial release
 - 1.2.1
   - Dropped support for Python 3.7.  Variety of bugfixes and expanded features, see documentation
+- 1.2.2
+  - Added capture utils
+  - Removed inner jit in model building to improve debugging
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
 - Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)
```

