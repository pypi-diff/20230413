# Comparing `tmp/neural-diffeqs-0.2.0rc0.tar.gz` & `tmp/neural-diffeqs-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-diffeqs-0.2.0rc0.tar", last modified: Tue Nov 22 06:01:22 2022, max compression
+gzip compressed data, was "neural-diffeqs-0.2.1rc0.tar", last modified: Thu Apr 13 21:23:37 2023, max compression
```

## Comparing `neural-diffeqs-0.2.0rc0.tar` & `neural-diffeqs-0.2.1rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/neural_diffeqs/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/_configure_forward.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/_neural_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs/_neural_sde.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-11-22 06:01:22.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-22 06:01:22.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 06:01:22.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-22 06:01:22.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-22 06:01:22.000000 neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-22 06:01:22.955762 neural-diffeqs-0.2.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-11-22 06:01:10.000000 neural-diffeqs-0.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.751340 neural-diffeqs-0.2.1rc0/neural_diffeqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_configure_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_neural_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_sde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.751340 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/setup.py
```

### Comparing `neural-diffeqs-0.2.0rc0/LICENSE` & `neural-diffeqs-0.2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.0rc0/PKG-INFO` & `neural-diffeqs-0.2.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-diffeqs
-Version: 0.2.0rc0
+Version: 0.2.1rc0
 Summary: neural differential equations
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural-diffeqs-0.2.0rc0/README.md` & `neural-diffeqs-0.2.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/_configure_forward.py` & `neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_configure_forward.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.0rc0/neural_diffeqs/_base/_neural_diffeq.py` & `neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_neural_diffeq.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.0rc0/neural_diffeqs/_neural_ode.py` & `neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_ode.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.0rc0/neural_diffeqs/_neural_sde.py` & `neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_sde.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,17 @@
         sigma_bias=True,
         mu_output_bias=True,
         sigma_output_bias=True,
         mu_potential=False,
         sigma_potential=False,
         noise_type: str = "general",
         sde_type: str = "ito",
-        brownian_size=1,
+        brownian_size: int =1,
+        mu_scalar: float = 1,
+        sigma_scalar: float = 1,
     ):
         """
         Instantiate a NeuralSDE.
 
         Parameters:
         -----------
         state_size
@@ -240,15 +242,15 @@
         (1) t required syntactically though not functionally.
 
         Examples:
         ---------
         >>> func = NeuralSDE(state_size)
         >>> x_hat_f = func.f(None, x)
         """
-        return self.mu_forward(self.mu, y0)
+        return self.mu_forward(self.mu, y0) * self.mu_scalar
 
     def g(self, t, y0):
         """
         Diffusion method (term) of the NeuralSDE.
 
         Parameters:
         -----------
@@ -272,8 +274,8 @@
         (1) t required syntactically though not functionally.
         
         Examples:
         ---------
         >>> func = NeuralSDE(state_size)
         >>> x_hat_g = func.g(None, x)
         """
-        return self._view_g_state(self.sigma_forward(self.sigma, y0))
+        return self._view_g_state(self.sigma_forward(self.sigma, y0)) * self.sigma_scalar
```

### Comparing `neural-diffeqs-0.2.0rc0/neural_diffeqs.egg-info/PKG-INFO` & `neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-diffeqs
-Version: 0.2.0rc0
+Version: 0.2.1rc0
 Summary: neural differential equations
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural-diffeqs-0.2.0rc0/setup.py` & `neural-diffeqs-0.2.1rc0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="neural-diffeqs",
-    version="0.2.0rc",
+    version="0.2.1rc",
     python_requires=">3.6.0",
     author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="neural differential equations",
     packages=setuptools.find_packages(),
     install_requires=[
-        "torch>=1.12",
+        "numpy==1.22.4",
+        "torch==1.13",
         "torch-nets>=0.0.1",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.6",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
```

