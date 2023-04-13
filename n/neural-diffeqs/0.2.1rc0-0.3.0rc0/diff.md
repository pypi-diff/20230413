# Comparing `tmp/neural-diffeqs-0.2.1rc0.tar.gz` & `tmp/neural-diffeqs-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-diffeqs-0.2.1rc0.tar", last modified: Thu Apr 13 21:23:37 2023, max compression
+gzip compressed data, was "neural-diffeqs-0.3.0rc0.tar", last modified: Thu Apr 13 21:24:41 2023, max compression
```

## Comparing `neural-diffeqs-0.2.1rc0.tar` & `neural-diffeqs-0.3.0rc0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.751340 neural-diffeqs-0.2.1rc0/neural_diffeqs/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_configure_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_base/_neural_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_sde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:23:37.751340 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:23:37.000000 neural-diffeqs-0.2.1rc0/neural_diffeqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:23:37.755340 neural-diffeqs-0.2.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-13 21:23:24.000000 neural-diffeqs-0.2.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_diffeq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/setup.py
```

### Comparing `neural-diffeqs-0.2.1rc0/LICENSE` & `neural-diffeqs-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.2.1rc0/neural_diffeqs/_neural_ode.py` & `neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,58 @@
 
-__module_name__ = "_neural_ode.py"
-__doc__ = """Neural ODE module. Contains API-facing NeuralODE class."""
-__author__ = ", ".join(["Michael E. Vinyard"])
-__email__ = ", ".join(["vinyard@g.harvard.edu"])
-__version__ = "0.0.2"
+# -- import packages: ----------------------------------------------------------
+import torch
+import ABCParse
 
 
-# -- import packages: --------------------------------------------------------------------
-from torch_nets import TorchNet
-from typing import Union
+# -- import local dependencies: ------------------------------------------------
+from . import core
 
 
-# -- import local dependencies: ----------------------------------------------------------
-from ._base._neural_diffeq import NeuralDiffEq
+# -- import standard libraries and define types: -------------------------------
+from typing import Union, List, Any
+NoneType = type(None)
 
 
-# -- API-facing class: -------------------------------------------------------------------
-class NeuralODE(NeuralDiffEq):
-    """note: forward is a required method for torchdiffeq.odeint"""
+# -- Main operational class: ---------------------------------------------------
+class PotentialSDE(core.BaseSDE):
+    DIFFEQ_TYPE = "SDE"
     def __init__(
         self,
-        state_size: int,
-        hidden: list = [],
-        activation: str = "LeakyReLU",
-        dropout: Union[float, list] = 0,
-        bias: bool = True,
-        output_bias: bool = True,
-        potential_net: bool = False,
+        state_size,
+        mu_hidden: Union[List[int], int] = [2000, 2000],
+        sigma_hidden: Union[List[int], int] = [400, 400],
+        mu_activation: Union[str, List[str]] = "LeakyReLU",
+        sigma_activation: Union[str, List[str]] = "LeakyReLU",
+        mu_dropout: Union[float, List[float]] = 0.2,
+        sigma_dropout: Union[float, List[float]] = 0.2,
+        mu_bias: bool = True,
+        sigma_bias: List[bool] = True,
+        mu_output_bias: bool = True,
+        sigma_output_bias: bool = True,
+        mu_n_augment: int = 0,
+        sigma_n_augment: int = 0,
+        sde_type="ito",
+        noise_type="general",
+        brownian_dim=1,
+        coef_drift: float = 1.,
+        coef_diffusion: float = 1.,
     ):
-        """
-        Instantiate a NeuralODE.
+        super().__init__()
 
-        Parameters:
-        -----------
-        state_size
-            type: int
-
-        hidden
-            type: dict
-            default: {1: [200, 200]}
-
-        activation_function:
-            type: 'torch.nn.modules.activation.<func>'
-            default: torch.nn.Tanh,
-
-        potential_net
-            If True, overrides out_dim and output_bias, setting them to 1 and False, respectively.
-            type: bool
-            default: False
-
-        dropout
-            type: float
-            default: 0
-
-        input_bias
-            type: bool
-            default: True
-
-        output_bias
-            type: bool
-            default: True
-
-        Returns:
-        --------
-        None
+        mu_potential = True
+        self.__config__(locals())
         
-        Notes:
-        ------
-        """
-        
-        super(NeuralODE, self).__init__()
-        
-        if potential_net:
-            out_features, output_bias = 1, False
-        else:
-            out_features = state_size
-        
-        self.mu = TorchNet(
-            in_features=state_size,
-            out_features=out_features,
-            hidden=hidden,
-            activation=activation,
-            dropout=dropout,
-            bias=bias,
-            output_bias=output_bias,
-        )
-        self.__setup__(kwargs=locals())
-
-    def forward(self, t, y0):
-        """
-        Forward (drift, deterministic) method, core to NeuralODE.
-
-        Parameters:
-        -----------
-        t
-            time tensor of shape: (t,)
-            type: torch.Tensor
-            default: None
-
-        y0
-            state vector
-            type: torch.Tensor
-
-        Returns:
-        --------
-        forward(y0)
-            drift: Tensor of same shape as y0.
-            type: torch.Tensor
-
-        Notes:
-        ------
-        (1) t required syntactically though not functionally.
-
-        Examples:
-        ---------
-        >>> func = NeuralODE(state_size)
-        >>> x_hat_f = func.forward(None, x)
-        """
-        return self.mu_forward(self.mu, y0)
+    def _potential(self, y):
+        return self.mu(y)
+
+    def _gradient(self, ψ, y):
+        """use-case: output is directly psi (from a potential network)"""
+        return torch.autograd.grad(ψ, y, torch.ones_like(ψ), create_graph=True)[0]
+
+    def drift(self, y) -> torch.Tensor:
+        y = y.requires_grad_()
+        ψ = self._potential(y)
+        return self._gradient(ψ, y) * self.coef_drift
+
+    def diffusion(self, y) -> torch.Tensor:
+        return self.sigma(y).view(y.shape[0], y.shape[1], self.brownian_dim) * self.coef_diffusion
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neural-diffeqs-0.2.1rc0/setup.py` & `neural-diffeqs-0.3.0rc0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="neural-diffeqs",
-    version="0.2.1rc",
-    python_requires=">3.6.0",
-    author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
+    version="0.3.0rc0",
+    python_requires=">3.7.0",
+    author="Michael E. Vinyard",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    description="neural differential equations",
+    description="Neural differential equations made easy.",
     packages=setuptools.find_packages(),
     install_requires=[
         "numpy==1.22.4",
-        "torch==1.13",
-        "torch-nets>=0.0.1",
+        "torch>=2.0.0",
+        "torch-nets>=0.0.4",
+        "torchsde>=0.2.5",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

