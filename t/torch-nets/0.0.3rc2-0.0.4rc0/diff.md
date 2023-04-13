# Comparing `tmp/torch-nets-0.0.3rc2.tar.gz` & `tmp/torch-nets-0.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-nets-0.0.3rc2.tar", last modified: Wed Apr 12 17:21:15 2023, max compression
+gzip compressed data, was "torch-nets-0.0.4rc0.tar", last modified: Thu Apr 13 19:09:08 2023, max compression
```

## Comparing `torch-nets-0.0.3rc2.tar` & `torch-nets-0.0.4rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.801274 torch-nets-0.0.3rc2/torch_nets/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/_augmented_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/_torch_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/torch_nets/core/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/_layer_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/_power_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/torch_nets/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/config/_activation_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/config/_layer_wise_attributes_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/core/config/_network_structure_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/torch_nets/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/plotting/_plot_weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.805274 torch-nets-0.0.3rc2/torch_nets/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 17:21:06.000000 torch-nets-0.0.3rc2/torch_nets/tools/_infer_network_architecture_from_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:21:15.801274 torch-nets-0.0.3rc2/torch_nets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 17:21:15.000000 torch-nets-0.0.3rc2/torch_nets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 17:21:15.000000 torch-nets-0.0.3rc2/torch_nets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:21:15.000000 torch-nets-0.0.3rc2/torch_nets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 17:21:15.000000 torch-nets-0.0.3rc2/torch_nets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 17:21:15.000000 torch-nets-0.0.3rc2/torch_nets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.392610 torch-nets-0.0.4rc0/torch_nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_augmented_torch_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_torch_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/_layer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/_power_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_activation_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_layer_wise_attributes_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_network_structure_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/plotting/_plot_weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/tools/_infer_network_architecture_from_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.392610 torch-nets-0.0.4rc0/torch_nets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/top_level.txt
```

### Comparing `torch-nets-0.0.3rc2/LICENSE` & `torch-nets-0.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/PKG-INFO` & `torch-nets-0.0.4rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.3rc2
+Version: 0.0.4rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -22,15 +22,15 @@
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.3rc2`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.3rc2 Summary: API to
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
 compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
 Harvard University - Broad Institute of MIT and Harvard - Massachussetts
 General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
 Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
 >3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
 Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc2`]
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
 (https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
```

### Comparing `torch-nets-0.0.3rc2/README.md` & `torch-nets-0.0.4rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.3rc2`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # Torch-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc2`]
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
 (https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
```

### Comparing `torch-nets-0.0.3rc2/setup.py` & `torch-nets-0.0.4rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="torch-nets",
-    version="0.0.3rc2",
+    version="0.0.4rc0",
     python_requires=">3.7.0",
     author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="API to compose PyTorch neural networks on the fly.",
```

### Comparing `torch-nets-0.0.3rc2/torch_nets/__init__.py` & `torch-nets-0.0.4rc0/torch_nets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """Main API __init__.py module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu",])
-__version__ = "0.0.3rc2"
+__version__ = "0.0.4rc0"
 
 
 # -- import network modules: -------------------------------------------------------------
 from ._torch_net import TorchNet
 from ._encoder import Encoder
 from ._decoder import Decoder
 from ._augmented_torch_net import AugmentedTorchNet
```

### Comparing `torch-nets-0.0.3rc2/torch_nets/_augmented_torch_net.py` & `torch-nets-0.0.4rc0/torch_nets/_augmented_torch_net.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,38 +88,34 @@
         -> updates self.in_features
         -> updates self.out_features
         
         """
         
         super(AugmentedTorchNet, self).__init__()
 
+        self.__parse__(locals())
+        
         self._in_features_orig = in_features
         self._out_features_orig = out_features
+        
         in_features += n_augment
         out_features += n_augment
 
         self.net = TorchNet(
             **ABCParse.function_kwargs(TorchNet, kwargs=locals())
-        )
-
-        self.__parse__(locals(), ignore=["net"])
+        )        
 
         if n_augment > 0:
             self._configure_augmented_output()
 
     def _configure_augmented_output(self):
-        self.net.names.append("augmented_output")
-        self.net.extend([torch.nn.Linear(self.out_features, self._out_features_orig)])
-        self.net._rename_nn_sequential_inplace(self.net, self.net.names)
+        self.net.add_module(
+            "augmented_output",
+            torch.nn.Linear(self.net.out_features, self._out_features_orig),
+        )
 
     def augment_input(self, input):
         x_aug = torch.zeros(input.shape[0], self.n_augment, device=input.device)
         return torch.cat([input, x_aug], 1)
 
     def forward(self, input):
         return self.net(self.augment_input(input))
-
-    def __repr__(self):
-        return (
-            f"{self.__class__.__name__}(in_features={self._in_features_orig}, "
-            f"out_features={self._out_features_orig}, net={repr(self.net)})"
-        )
```

### Comparing `torch-nets-0.0.3rc2/torch_nets/_decoder.py` & `torch-nets-0.0.4rc0/torch_nets/_decoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/_encoder.py` & `torch-nets-0.0.4rc0/torch_nets/_encoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/_torch_net.py` & `torch-nets-0.0.4rc0/torch_nets/_torch_net.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/_layer_builder.py` & `torch-nets-0.0.4rc0/torch_nets/core/_layer_builder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/_power_space.py` & `torch-nets-0.0.4rc0/torch_nets/core/_power_space.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/config/_activation_function_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_activation_function_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/config/_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/config/_layer_wise_attributes_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_layer_wise_attributes_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/core/config/_network_structure_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_network_structure_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/plotting/_plot_weights_and_biases.py` & `torch-nets-0.0.4rc0/torch_nets/plotting/_plot_weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets/tools/_infer_network_architecture_from_state.py` & `torch-nets-0.0.4rc0/torch_nets/tools/_infer_network_architecture_from_state.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.3rc2/torch_nets.egg-info/PKG-INFO` & `torch-nets-0.0.4rc0/torch_nets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.3rc2
+Version: 0.0.4rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -22,15 +22,15 @@
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.3rc2`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.3rc2 Summary: API to
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
 compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
 Harvard University - Broad Institute of MIT and Harvard - Massachussetts
 General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
 Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
 >3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
 Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc2`]
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
 (https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
```

### Comparing `torch-nets-0.0.3rc2/torch_nets.egg-info/SOURCES.txt` & `torch-nets-0.0.4rc0/torch_nets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

