# Comparing `tmp/aidd-codebase-0.1.9.tar.gz` & `tmp/aidd-codebase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidd-codebase-0.1.9.tar", max compression
+gzip compressed data, was "aidd-codebase-0.2.0.tar", max compression
```

## Comparing `aidd-codebase-0.1.9.tar` & `aidd-codebase-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,26 @@
--rw-r--r--   0        0        0     1066 2022-06-15 13:18:24.144845 aidd-codebase-0.1.9/LICENSE
--rw-r--r--   0        0        0     2180 2022-06-15 14:22:55.624839 aidd-codebase-0.1.9/README.md
--rw-r--r--   0        0        0       22 2022-06-15 09:23:37.774000 aidd-codebase-0.1.9/aidd_codebase/__init__.py
--rw-r--r--   0        0        0        0 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/data_utils/__init__.py
--rw-r--r--   0        0        0     2554 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/data_utils/augmentation.py
--rw-r--r--   0        0        0     1182 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/data_utils/collate.py
--rw-r--r--   0        0        0     8642 2022-06-22 08:01:54.839769 aidd-codebase-0.1.9/aidd_codebase/data_utils/dataprocessors.py
--rw-r--r--   0        0        0     1788 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/data_utils/datasets.py
--rw-r--r--   0        0        0       83 2022-06-22 08:01:54.839769 aidd-codebase-0.1.9/aidd_codebase/datamodules/__init__.py
--rw-r--r--   0        0        0      109 2022-06-15 09:27:59.046000 aidd-codebase-0.1.9/aidd_codebase/datamodules/datachoice.py
--rw-r--r--   0        0        0    11584 2022-06-22 08:10:17.068790 aidd-codebase-0.1.9/aidd_codebase/datamodules/smiles.py
--rw-r--r--   0        0        0     2801 2022-06-22 08:01:54.839769 aidd-codebase-0.1.9/aidd_codebase/datamodules/tokenizer.py
--rw-r--r--   0        0        0       36 2022-06-21 12:11:20.335521 aidd-codebase-0.1.9/aidd_codebase/framework/__init__.py
--rw-r--r--   0        0        0     5839 2022-06-24 13:59:53.330144 aidd-codebase-0.1.9/aidd_codebase/framework/framework.py
--rw-r--r--   0        0        0     1479 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/framework/loggers.py
--rw-r--r--   0        0        0      407 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/framework/loopchoice.py
--rw-r--r--   0        0        0     4367 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/framework/loops.py
--rw-r--r--   0        0        0     1017 2022-06-21 12:11:20.335521 aidd-codebase-0.1.9/aidd_codebase/framework/loss.py
--rw-r--r--   0        0        0     1659 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/framework/metrics.py
--rw-r--r--   0        0        0      521 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/framework/opt_ensembling.py
--rw-r--r--   0        0        0      297 2022-06-15 09:29:30.667000 aidd-codebase-0.1.9/aidd_codebase/framework/optimizers.py
--rw-r--r--   0        0        0     1045 2022-06-22 08:10:17.068790 aidd-codebase-0.1.9/aidd_codebase/framework/scheduling.py
--rw-r--r--   0        0        0      592 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/framework/tracking.py
--rw-r--r--   0        0        0        0 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/math_utils/__init__.py
--rw-r--r--   0        0        0     2749 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/math_utils/cross_product.py
--rw-r--r--   0        0        0        7 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/math_utils/positional_encoding.py
--rw-r--r--   0        0        0      109 2022-06-20 11:10:26.922176 aidd-codebase-0.1.9/aidd_codebase/models/__init__.py
--rw-r--r--   0        0        0     2856 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/models/decoder.py
--rw-r--r--   0        0        0        0 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/models/embedding/__init__.py
--rw-r--r--   0        0        0      526 2022-06-15 09:29:30.691000 aidd-codebase-0.1.9/aidd_codebase/models/embedding/embedding.py
--rw-r--r--   0        0        0     1316 2022-06-15 09:29:30.631000 aidd-codebase-0.1.9/aidd_codebase/models/embedding/input_adapters.py
--rw-r--r--   0        0        0     3842 2022-06-15 09:29:30.643000 aidd-codebase-0.1.9/aidd_codebase/models/embedding/positional.py
--rw-r--r--   0        0        0     2849 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/models/encoder.py
--rw-r--r--   0        0        0      110 2022-06-15 09:29:30.635000 aidd-codebase-0.1.9/aidd_codebase/models/modelchoice.py
--rw-r--r--   0        0        0        0 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/models/modules/__init__.py
--rw-r--r--   0        0        0     1094 2022-06-15 09:29:30.723000 aidd-codebase-0.1.9/aidd_codebase/models/modules/activation.py
--rw-r--r--   0        0        0     5220 2022-06-15 09:29:30.739000 aidd-codebase-0.1.9/aidd_codebase/models/modules/attention.py
--rw-r--r--   0        0        0     1200 2022-06-15 09:29:30.611000 aidd-codebase-0.1.9/aidd_codebase/models/modules/feedforward.py
--rw-r--r--   0        0        0     4337 2022-06-15 09:29:30.655000 aidd-codebase-0.1.9/aidd_codebase/models/modules/highway_units.py
--rw-r--r--   0        0        0     1685 2022-06-15 09:29:30.731000 aidd-codebase-0.1.9/aidd_codebase/models/modules/highwaycnn.py
--rw-r--r--   0        0        0     1809 2022-06-15 09:29:30.623000 aidd-codebase-0.1.9/aidd_codebase/models/modules/modules.py
--rw-r--r--   0        0        0      302 2022-06-15 09:29:30.651000 aidd-codebase-0.1.9/aidd_codebase/models/modules/switches.py
--rw-r--r--   0        0        0     2248 2022-06-15 09:29:30.715000 aidd-codebase-0.1.9/aidd_codebase/models/modules/textcnn.py
--rw-r--r--   0        0        0     1541 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/models/modules/transformer_layers.py
--rw-r--r--   0        0        0     1364 2022-06-15 09:29:30.707000 aidd-codebase-0.1.9/aidd_codebase/models/modules/utils.py
--rw-r--r--   0        0        0     3015 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/models/seq2seq.py
--rw-r--r--   0        0        0        0 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/__init__.py
--rw-r--r--   0        0        0      622 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/callbacks.py
--rw-r--r--   0        0        0     4981 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/utils/config.py
--rw-r--r--   0        0        0     1626 2022-06-24 12:59:03.853785 aidd-codebase-0.1.9/aidd_codebase/utils/device.py
--rw-r--r--   0        0        0     1083 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/directories.py
--rw-r--r--   0        0        0      117 2022-06-24 13:00:10.357879 aidd-codebase-0.1.9/aidd_codebase/utils/environmentchoice.py
--rw-r--r--   0        0        0     1005 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/initiator.py
--rw-r--r--   0        0        0     1071 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/loading_saving.py
--rw-r--r--   0        0        0     5876 2022-06-24 12:10:16.888265 aidd-codebase-0.1.9/aidd_codebase/utils/metacoding.py
--rw-r--r--   0        0        0      497 2022-06-22 07:16:06.275326 aidd-codebase-0.1.9/aidd_codebase/utils/tools.py
--rw-r--r--   0        0        0       36 2022-06-15 09:13:16.236000 aidd-codebase-0.1.9/aidd_codebase/utils/typescripts.py
--rw-r--r--   0        0        0     1246 2022-06-24 14:15:30.470846 aidd-codebase-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3097 2022-06-24 14:16:27.212818 aidd-codebase-0.1.9/setup.py
--rw-r--r--   0        0        0     3177 2022-06-24 14:16:27.213411 aidd-codebase-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2351 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/datamodules/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/framework/__init__.py
+-rw-r--r--   0        0        0     1005 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/framework/initiator.py
+-rw-r--r--   0        0        0     1479 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/framework/loggers.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/models/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/models/modules/__init__.py
+-rw-r--r--   0        0        0     3114 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/models/net_classifier.py
+-rw-r--r--   0        0        0       43 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/new_project/__init__.py
+-rw-r--r--   0        0        0     1192 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/new_project/main.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/new_project/src/__init__.py
+-rw-r--r--   0        0        0      206 2022-11-03 15:12:31.133933 aidd-codebase-0.2.0/aidd_codebase/registries.py
+-rw-r--r--   0        0        0      504 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/start_project.py
+-rw-r--r--   0        0        0        0 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/__init__.py
+-rw-r--r--   0        0        0     1655 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/callbacks.py
+-rw-r--r--   0        0        0     1345 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/config_checker.py
+-rw-r--r--   0        0        0     1626 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/device.py
+-rw-r--r--   0        0        0      234 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/helper_functions.py
+-rw-r--r--   0        0        0      842 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/setup.py
+-rw-r--r--   0        0        0      632 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/tools.py
+-rw-r--r--   0        0        0       36 2022-11-03 15:12:31.137933 aidd-codebase-0.2.0/aidd_codebase/utils/typescripts.py
+-rw-r--r--   0        0        0     1246 2022-11-03 15:14:33.996387 aidd-codebase-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3241 2022-11-03 15:14:41.807179 aidd-codebase-0.2.0/setup.py
+-rw-r--r--   0        0        0     3348 2022-11-03 15:14:41.807593 aidd-codebase-0.2.0/PKG-INFO
```

### Comparing `aidd-codebase-0.1.9/LICENSE` & `aidd-codebase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aidd-codebase-0.1.9/README.md` & `aidd-codebase-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AIDD Codebase
 
 ![PyPI](https://img.shields.io/pypi/v/aidd-codebase)
 ![PyPI](https://img.shields.io/pypi/pyversions/aidd-codebase)
-![PyPI](https://img.shields.io/github/license/AIDD-ESR1/AIDD-codebase)
+![PyPI](https://img.shields.io/github/license/aidd-msca/aidd-codebase)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)
 
 A high-level codebase for deep learning development in drug discovery applications using PyTorch-Lightning.
 
 ## Dependencies
 
 The codebase requires the following additional dependencies
 - CUDA >= 11.4
@@ -16,16 +17,16 @@
 - Optionally supports: tensorboard and/or wandb
 
 
 ## Installation
 
 The codebase can be installed from PyPI using `pip`, or your package manager of choice, with
 
-```
-pip install aidd-codebase
+```bash
+$ pip install aidd-codebase
 ```
 
 ## Usage
 
 1. __*Configuration*__: The coding framework has a number of argument dataclasses in the file *arguments.py*. This file contains all standard arguments for each of the models. Because they are dataclasses, you can easily adapt them to your own needs. 
 <br> 
 Does your Seq2Seq adaptation need an extra argument? Import the Seq2SeqArguments from arguments.py, create your own dataclass which inherits it and add your extra argument. <br> <br>
@@ -62,8 +63,8 @@
 
 All fellows of the AIDD consortium have contributed to the packaged.
 
 ## Code of Conduct
 
 Everyone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
 
- 
+
```

### Comparing `aidd-codebase-0.1.9/aidd_codebase/framework/loggers.py` & `aidd-codebase-0.2.0/aidd_codebase/framework/loggers.py`

 * *Files identical despite different names*

### Comparing `aidd-codebase-0.1.9/aidd_codebase/utils/device.py` & `aidd-codebase-0.2.0/aidd_codebase/utils/device.py`

 * *Files identical despite different names*

### Comparing `aidd-codebase-0.1.9/aidd_codebase/utils/initiator.py` & `aidd-codebase-0.2.0/aidd_codebase/framework/initiator.py`

 * *Files identical despite different names*

### Comparing `aidd-codebase-0.1.9/pyproject.toml` & `aidd-codebase-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "aidd-codebase"
-version = "0.1.9"
+version = "0.2.0"
 description = "High-level codebase for deep learning development in drug discovery."
 authors = ["Peter Hartog <peter.hartog@hotmail.nl>", "Emma Svensson <svensson@ml.jku.at>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/AIDD-ESR1/AIDD-codebase"
-repository = "https://github.com/AIDD-ESR1/AIDD-codebase"
+homepage = "https://github.com/aidd-msca/aidd-codebase"
+repository = "https://github.com/aidd-msca/aidd-codebase"
 keywords = ["aidd", "drug discovery", "deep learning"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: GPU :: NVIDIA CUDA :: 11.4",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 include = [
```

### Comparing `aidd-codebase-0.1.9/setup.py` & `aidd-codebase-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['aidd_codebase',
- 'aidd_codebase.data_utils',
  'aidd_codebase.datamodules',
  'aidd_codebase.framework',
- 'aidd_codebase.math_utils',
  'aidd_codebase.models',
- 'aidd_codebase.models.embedding',
  'aidd_codebase.models.modules',
+ 'aidd_codebase.new_project',
+ 'aidd_codebase.new_project.src',
  'aidd_codebase.utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aidd-codebase',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'High-level codebase for deep learning development in drug discovery.',
-    'long_description': '# AIDD Codebase\n\n![PyPI](https://img.shields.io/pypi/v/aidd-codebase)\n![PyPI](https://img.shields.io/pypi/pyversions/aidd-codebase)\n![PyPI](https://img.shields.io/github/license/AIDD-ESR1/AIDD-codebase)\n\nA high-level codebase for deep learning development in drug discovery applications using PyTorch-Lightning.\n\n## Dependencies\n\nThe codebase requires the following additional dependencies\n- CUDA >= 11.4\n- PyTorch >= 1.9\n- Pytorch-Lightning >= 1.5 \n- RDKit \n- Optionally supports: tensorboard and/or wandb\n\n\n## Installation\n\nThe codebase can be installed from PyPI using `pip`, or your package manager of choice, with\n\n```\npip install aidd-codebase\n```\n\n## Usage\n\n1. __*Configuration*__: The coding framework has a number of argument dataclasses in the file *arguments.py*. This file contains all standard arguments for each of the models. Because they are dataclasses, you can easily adapt them to your own needs. \n<br> \nDoes your Seq2Seq adaptation need an extra argument? Import the Seq2SeqArguments from arguments.py, create your own dataclass which inherits it and add your extra argument. <br> <br>\n*It is important to note that the order of supplying arguments to a script goes as follows:* <br>\n- --flags override config.yaml <br>\n- config.yaml overrides default values in arguments.py <br>\n- default values from arguments.py are used when no other values are supplied<br>\nAt the end, it stores all arguments in config.yaml\n<br><br>\n\n2. __*Use*__: The coding framework has four main parts: <br>\n- utils\n- data_utils\n- models\n- interpretation\n\nThese parts should be used \n&nbsp; \n\n3. __*File Setup*__: The setup of the files in the system is best used as followed:<br>\ncoding_framework<br> \n|-- ..<br> \nESR X<br> \n|-- project 1<br> \n  |-- data<br> \n    |-- ..<br> \n  |-- Arguments.py<br> \n  |-- config.yaml<br> \n  |-- main.py<br>\n  |-- datamodule.py<br>\n  |-- pl_framework.py<br>\n\n## Contributors\n\nAll fellows of the AIDD consortium have contributed to the packaged.\n\n## Code of Conduct\n\nEveryone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).\n\n ',
+    'long_description': '# AIDD Codebase\n\n![PyPI](https://img.shields.io/pypi/v/aidd-codebase)\n![PyPI](https://img.shields.io/pypi/pyversions/aidd-codebase)\n![PyPI](https://img.shields.io/github/license/aidd-msca/aidd-codebase)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)\n\nA high-level codebase for deep learning development in drug discovery applications using PyTorch-Lightning.\n\n## Dependencies\n\nThe codebase requires the following additional dependencies\n- CUDA >= 11.4\n- PyTorch >= 1.9\n- Pytorch-Lightning >= 1.5 \n- RDKit \n- Optionally supports: tensorboard and/or wandb\n\n\n## Installation\n\nThe codebase can be installed from PyPI using `pip`, or your package manager of choice, with\n\n```bash\n$ pip install aidd-codebase\n```\n\n## Usage\n\n1. __*Configuration*__: The coding framework has a number of argument dataclasses in the file *arguments.py*. This file contains all standard arguments for each of the models. Because they are dataclasses, you can easily adapt them to your own needs. \n<br> \nDoes your Seq2Seq adaptation need an extra argument? Import the Seq2SeqArguments from arguments.py, create your own dataclass which inherits it and add your extra argument. <br> <br>\n*It is important to note that the order of supplying arguments to a script goes as follows:* <br>\n- --flags override config.yaml <br>\n- config.yaml overrides default values in arguments.py <br>\n- default values from arguments.py are used when no other values are supplied<br>\nAt the end, it stores all arguments in config.yaml\n<br><br>\n\n2. __*Use*__: The coding framework has four main parts: <br>\n- utils\n- data_utils\n- models\n- interpretation\n\nThese parts should be used \n&nbsp; \n\n3. __*File Setup*__: The setup of the files in the system is best used as followed:<br>\ncoding_framework<br> \n|-- ..<br> \nESR X<br> \n|-- project 1<br> \n  |-- data<br> \n    |-- ..<br> \n  |-- Arguments.py<br> \n  |-- config.yaml<br> \n  |-- main.py<br>\n  |-- datamodule.py<br>\n  |-- pl_framework.py<br>\n\n## Contributors\n\nAll fellows of the AIDD consortium have contributed to the packaged.\n\n## Code of Conduct\n\nEveryone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).\n\n \n',
     'author': 'Peter Hartog',
     'author_email': 'peter.hartog@hotmail.nl',
     'maintainer': None,
     'maintainer_email': None,
-    'url': 'https://github.com/AIDD-ESR1/AIDD-codebase',
+    'url': 'https://github.com/aidd-msca/aidd-codebase',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `aidd-codebase-0.1.9/PKG-INFO` & `aidd-codebase-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aidd-codebase
-Version: 0.1.9
+Version: 0.2.0
 Summary: High-level codebase for deep learning development in drug discovery.
-Home-page: https://github.com/AIDD-ESR1/AIDD-codebase
+Home-page: https://github.com/aidd-msca/aidd-codebase
 License: MIT
 Keywords: aidd,drug discovery,deep learning
 Author: Peter Hartog
 Author-email: peter.hartog@hotmail.nl
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.4
@@ -15,22 +15,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: tensorboard (>=2.6,<3.0)
 Requires-Dist: wandb (>=0.12.16,<0.13.0)
-Project-URL: Repository, https://github.com/AIDD-ESR1/AIDD-codebase
+Project-URL: Repository, https://github.com/aidd-msca/aidd-codebase
 Description-Content-Type: text/markdown
 
 # AIDD Codebase
 
 ![PyPI](https://img.shields.io/pypi/v/aidd-codebase)
 ![PyPI](https://img.shields.io/pypi/pyversions/aidd-codebase)
-![PyPI](https://img.shields.io/github/license/AIDD-ESR1/AIDD-codebase)
+![PyPI](https://img.shields.io/github/license/aidd-msca/aidd-codebase)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jlyEd1yxhvFCN82YqEFI82q2n0k_y06F?usp=sharing)
 
 A high-level codebase for deep learning development in drug discovery applications using PyTorch-Lightning.
 
 ## Dependencies
 
 The codebase requires the following additional dependencies
 - CUDA >= 11.4
@@ -40,16 +41,16 @@
 - Optionally supports: tensorboard and/or wandb
 
 
 ## Installation
 
 The codebase can be installed from PyPI using `pip`, or your package manager of choice, with
 
-```
-pip install aidd-codebase
+```bash
+$ pip install aidd-codebase
 ```
 
 ## Usage
 
 1. __*Configuration*__: The coding framework has a number of argument dataclasses in the file *arguments.py*. This file contains all standard arguments for each of the models. Because they are dataclasses, you can easily adapt them to your own needs. 
 <br> 
 Does your Seq2Seq adaptation need an extra argument? Import the Seq2SeqArguments from arguments.py, create your own dataclass which inherits it and add your extra argument. <br> <br>
@@ -87,7 +88,8 @@
 All fellows of the AIDD consortium have contributed to the packaged.
 
 ## Code of Conduct
 
 Everyone interacting in the codebase, issue trackers, chat rooms, and mailing lists is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
 
  
+
```

