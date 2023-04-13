# Comparing `tmp/torch-nets-0.0.4.tar.gz` & `tmp/torch-nets-0.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-nets-0.0.4.tar", last modified: Thu Apr 13 19:19:17 2023, max compression
+gzip compressed data, was "torch-nets-0.0.4rc0.tar", last modified: Thu Apr 13 19:09:08 2023, max compression
```

## Comparing `torch-nets-0.0.4.tar` & `torch-nets-0.0.4rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.759992 torch-nets-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 19:19:08.000000 torch-nets-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-13 19:19:17.759992 torch-nets-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-13 19:19:08.000000 torch-nets-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:19:17.759992 torch-nets-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-13 19:19:08.000000 torch-nets-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.755992 torch-nets-0.0.4/torch_nets/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/_augmented_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/_torch_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.755992 torch-nets-0.0.4/torch_nets/core/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/_layer_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/_power_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.759992 torch-nets-0.0.4/torch_nets/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/config/_activation_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/config/_layer_wise_attributes_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/core/config/_network_structure_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.759992 torch-nets-0.0.4/torch_nets/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/plotting/_plot_weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.759992 torch-nets-0.0.4/torch_nets/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 19:19:08.000000 torch-nets-0.0.4/torch_nets/tools/_infer_network_architecture_from_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:19:17.755992 torch-nets-0.0.4/torch_nets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-13 19:19:17.000000 torch-nets-0.0.4/torch_nets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 19:19:17.000000 torch-nets-0.0.4/torch_nets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:19:17.000000 torch-nets-0.0.4/torch_nets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:19:17.000000 torch-nets-0.0.4/torch_nets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:19:17.000000 torch-nets-0.0.4/torch_nets.egg-info/top_level.txt
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

### Comparing `torch-nets-0.0.4/LICENSE` & `torch-nets-0.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/PKG-INFO` & `torch-nets-0.0.4rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.4
+Version: 0.0.4rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ![logo](./docs/imgs/torch-nets.logo.png)
-<!-- # Torch-Nets -->
+# Torch-Nets
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
+<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4`](https://pypi.org/project/torch-nets))
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
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4 Summary: API to compose
-PyTorch neural networks on the fly. Author: Michael E. Vinyard - Harvard
-University - Broad Institute of MIT and Harvard - Massachussetts General
-Hospital Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Bio-Informatics Requires-Python: >3.7.0 Description-
-Content-Type: text/markdown License-File: LICENSE # ![logo](./docs/imgs/torch-
-nets.logo.png)  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
-torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version]
-(https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black)  Compose PyTorch neural networks
-with ease. ### Installation From PYPI (current version: [`v0.0.4`](https://
-pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
+compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
+Harvard University - Broad Institute of MIT and Harvard - Massachussetts
+General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
+Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
+>3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
+Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
+nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
+badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
```

### Comparing `torch-nets-0.0.4/README.md` & `torch-nets-0.0.4rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# ![logo](./docs/imgs/torch-nets.logo.png)
-<!-- # Torch-Nets -->
+# Torch-Nets
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
+<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4`](https://pypi.org/project/torch-nets))
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
@@ -1,23 +1,22 @@
-# ![logo](./docs/imgs/torch-nets.logo.png)  [![PyPI pyversions](https://
-img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/
-torch-nets/) [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https:/
-/badge.fury.io/py/torch-nets) [![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black)  Compose
-PyTorch neural networks with ease. ### Installation From PYPI (current version:
-[`v0.0.4`](https://pypi.org/project/torch-nets)) ```python pip install torch-
-nets ``` Alternatively, install the development version from GitHub: ```shell
-git clone https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip
-install -e . ``` ### Example API use-cases ```python from torch_nets import
-TorchNet ``` #### Create a feed-forward neural network The only required
-arguments are `in_features` and `out_features`. The network can be made as
-simple or complex as you want through optional parameters. ```python net =
-TorchNet( in_features=50, out_features=50, hidden=[400, 400],
-activation="LeakyReLU", dropout=0.2, bias=True, output_bias=True, ) ```  See
-output
+# Torch-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
+nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
+badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
+( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
 ``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
 out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
 (activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
 (linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
 Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
 (output): Sequential( (linear): Linear(in_features=400, out_features=50,
 bias=True) ) ) ```  ### Documentation For more information, including examples
```

### Comparing `torch-nets-0.0.4/setup.py` & `torch-nets-0.0.4rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="torch-nets",
-    version="0.0.4",
+    version="0.0.4rc0",
     python_requires=">3.7.0",
     author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="API to compose PyTorch neural networks on the fly.",
```

### Comparing `torch-nets-0.0.4/torch_nets/__init__.py` & `torch-nets-0.0.4rc0/torch_nets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """Main API __init__.py module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu",])
-__version__ = "0.0.4"
+__version__ = "0.0.4rc0"
 
 
 # -- import network modules: -------------------------------------------------------------
 from ._torch_net import TorchNet
 from ._encoder import Encoder
 from ._decoder import Decoder
 from ._augmented_torch_net import AugmentedTorchNet
```

### Comparing `torch-nets-0.0.4/torch_nets/_augmented_torch_net.py` & `torch-nets-0.0.4rc0/torch_nets/_augmented_torch_net.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/_decoder.py` & `torch-nets-0.0.4rc0/torch_nets/_decoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/_encoder.py` & `torch-nets-0.0.4rc0/torch_nets/_encoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/_torch_net.py` & `torch-nets-0.0.4rc0/torch_nets/_torch_net.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/_layer_builder.py` & `torch-nets-0.0.4rc0/torch_nets/core/_layer_builder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/_power_space.py` & `torch-nets-0.0.4rc0/torch_nets/core/_power_space.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/config/_activation_function_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_activation_function_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/config/_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/config/_layer_wise_attributes_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_layer_wise_attributes_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/core/config/_network_structure_config.py` & `torch-nets-0.0.4rc0/torch_nets/core/config/_network_structure_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/plotting/_plot_weights_and_biases.py` & `torch-nets-0.0.4rc0/torch_nets/plotting/_plot_weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets/tools/_infer_network_architecture_from_state.py` & `torch-nets-0.0.4rc0/torch_nets/tools/_infer_network_architecture_from_state.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4/torch_nets.egg-info/PKG-INFO` & `torch-nets-0.0.4rc0/torch_nets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.4
+Version: 0.0.4rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ![logo](./docs/imgs/torch-nets.logo.png)
-<!-- # Torch-Nets -->
+# Torch-Nets
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
+<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4`](https://pypi.org/project/torch-nets))
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
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4 Summary: API to compose
-PyTorch neural networks on the fly. Author: Michael E. Vinyard - Harvard
-University - Broad Institute of MIT and Harvard - Massachussetts General
-Hospital Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Bio-Informatics Requires-Python: >3.7.0 Description-
-Content-Type: text/markdown License-File: LICENSE # ![logo](./docs/imgs/torch-
-nets.logo.png)  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
-torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version]
-(https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black)  Compose PyTorch neural networks
-with ease. ### Installation From PYPI (current version: [`v0.0.4`](https://
-pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
+compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
+Harvard University - Broad Institute of MIT and Harvard - Massachussetts
+General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
+Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
+>3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
+Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
+nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
+badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
+networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
```

### Comparing `torch-nets-0.0.4/torch_nets.egg-info/SOURCES.txt` & `torch-nets-0.0.4rc0/torch_nets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

