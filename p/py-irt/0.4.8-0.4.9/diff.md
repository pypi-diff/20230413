# Comparing `tmp/py-irt-0.4.8.tar.gz` & `tmp/py_irt-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-irt-0.4.8.tar", max compression
+gzip compressed data, was "py_irt-0.4.9.tar", max compression
```

## Comparing `py-irt-0.4.8.tar` & `py_irt-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1121 2022-07-07 17:42:01.524707 py-irt-0.4.8/LICENSE
--rw-r--r--   0        0        0     4902 2022-06-30 12:50:38.723550 py-irt-0.4.8/README.md
--rw-r--r--   0        0        0       16 2022-04-08 14:09:26.669213 py-irt-0.4.8/py_irt/__init__.py
--rw-r--r--   0        0        0    10230 2023-01-18 16:35:13.839100 py-irt-0.4.8/py_irt/cli.py
--rw-r--r--   0        0        0     1758 2023-01-18 16:35:13.839100 py-irt-0.4.8/py_irt/config.py
--rw-r--r--   0        0        0     5469 2023-01-18 16:35:13.839100 py-irt-0.4.8/py_irt/dataset.py
--rw-r--r--   0        0        0     3581 2022-07-07 17:43:10.053036 py-irt-0.4.8/py_irt/initializers.py
--rw-r--r--   0        0        0     3102 2022-07-07 17:43:15.325061 py-irt-0.4.8/py_irt/io.py
--rw-r--r--   0        0        0        0 2022-04-08 14:09:26.669213 py-irt-0.4.8/py_irt/models/__init__.py
--rw-r--r--   0        0        0     2770 2022-07-07 17:43:59.421272 py-irt-0.4.8/py_irt/models/abstract_model.py
--rw-r--r--   0        0        0    11158 2022-07-07 17:44:10.217323 py-irt-0.4.8/py_irt/models/amortized_1pl.py
--rw-r--r--   0        0        0     9746 2022-07-07 17:43:42.229190 py-irt-0.4.8/py_irt/models/four_param_logistic.py
--rw-r--r--   0        0        0     9457 2022-07-07 17:43:48.497220 py-irt-0.4.8/py_irt/models/multidim_2pl.py
--rw-r--r--   0        0        0    10941 2022-07-07 17:43:53.905245 py-irt-0.4.8/py_irt/models/one_param_logistic.py
--rw-r--r--   0        0        0    10149 2022-09-26 13:00:53.001108 py-irt-0.4.8/py_irt/models/three_param_logistic.py
--rw-r--r--   0        0        0    12418 2022-07-07 17:44:16.209352 py-irt-0.4.8/py_irt/models/two_param_logistic.py
--rw-r--r--   0        0        0     2713 2022-07-07 17:43:36.137161 py-irt-0.4.8/py_irt/scoring.py
--rw-r--r--   0        0        0     8246 2023-01-18 16:35:13.843100 py-irt-0.4.8/py_irt/training.py
--rw-r--r--   0        0        0      896 2023-01-18 16:36:31.627539 py-irt-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6018 2023-01-18 16:38:07.886368 py-irt-0.4.8/setup.py
--rw-r--r--   0        0        0     5756 2023-01-18 16:38:07.886710 py-irt-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1121 2022-07-07 17:42:01.524707 py_irt-0.4.9/LICENSE
+-rw-r--r--   0        0        0     4902 2022-06-30 12:50:38.723550 py_irt-0.4.9/README.md
+-rw-r--r--   0        0        0       16 2022-04-08 14:09:26.669213 py_irt-0.4.9/py_irt/__init__.py
+-rw-r--r--   0        0        0    10230 2023-01-18 16:35:13.839100 py_irt-0.4.9/py_irt/cli.py
+-rw-r--r--   0        0        0     1758 2023-01-18 16:35:13.839100 py_irt-0.4.9/py_irt/config.py
+-rw-r--r--   0        0        0     5469 2023-01-18 16:35:13.839100 py_irt-0.4.9/py_irt/dataset.py
+-rw-r--r--   0        0        0     3581 2022-07-07 17:43:10.053036 py_irt-0.4.9/py_irt/initializers.py
+-rw-r--r--   0        0        0     3102 2022-07-07 17:43:15.325061 py_irt-0.4.9/py_irt/io.py
+-rw-r--r--   0        0        0        0 2022-04-08 14:09:26.669213 py_irt-0.4.9/py_irt/models/__init__.py
+-rw-r--r--   0        0        0     2770 2022-07-07 17:43:59.421272 py_irt-0.4.9/py_irt/models/abstract_model.py
+-rw-r--r--   0        0        0    11158 2022-07-07 17:44:10.217323 py_irt-0.4.9/py_irt/models/amortized_1pl.py
+-rw-r--r--   0        0        0     9746 2022-07-07 17:43:42.229190 py_irt-0.4.9/py_irt/models/four_param_logistic.py
+-rw-r--r--   0        0        0     9457 2022-07-07 17:43:48.497220 py_irt-0.4.9/py_irt/models/multidim_2pl.py
+-rw-r--r--   0        0        0    10941 2022-07-07 17:43:53.905245 py_irt-0.4.9/py_irt/models/one_param_logistic.py
+-rw-r--r--   0        0        0    10149 2022-09-26 13:00:53.001108 py_irt-0.4.9/py_irt/models/three_param_logistic.py
+-rw-r--r--   0        0        0    12418 2022-07-07 17:44:16.209352 py_irt-0.4.9/py_irt/models/two_param_logistic.py
+-rw-r--r--   0        0        0     2713 2022-07-07 17:43:36.137161 py_irt-0.4.9/py_irt/scoring.py
+-rw-r--r--   0        0        0     8284 2023-03-30 14:37:32.775040 py_irt-0.4.9/py_irt/training.py
+-rw-r--r--   0        0        0      912 2023-03-30 14:41:55.168541 py_irt-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5786 1970-01-01 00:00:00.000000 py_irt-0.4.9/PKG-INFO
```

### Comparing `py-irt-0.4.8/LICENSE` & `py_irt-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/README.md` & `py_irt-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/cli.py` & `py_irt-0.4.9/py_irt/cli.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/config.py` & `py_irt-0.4.9/py_irt/config.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/dataset.py` & `py_irt-0.4.9/py_irt/dataset.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/initializers.py` & `py_irt-0.4.9/py_irt/initializers.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/io.py` & `py_irt-0.4.9/py_irt/io.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/abstract_model.py` & `py_irt-0.4.9/py_irt/models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/amortized_1pl.py` & `py_irt-0.4.9/py_irt/models/amortized_1pl.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/four_param_logistic.py` & `py_irt-0.4.9/py_irt/models/four_param_logistic.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/multidim_2pl.py` & `py_irt-0.4.9/py_irt/models/multidim_2pl.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/one_param_logistic.py` & `py_irt-0.4.9/py_irt/models/one_param_logistic.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/three_param_logistic.py` & `py_irt-0.4.9/py_irt/models/three_param_logistic.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/models/two_param_logistic.py` & `py_irt-0.4.9/py_irt/models/two_param_logistic.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/scoring.py` & `py_irt-0.4.9/py_irt/scoring.py`

 * *Files identical despite different names*

### Comparing `py-irt-0.4.8/py_irt/training.py` & `py_irt-0.4.9/py_irt/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pathlib import Path
 
 import typer
 import torch
 
 from pyro.infer import SVI, Trace_ELBO
 import pyro
+#from pyro.optim import ExponentialLR
 
 from rich.console import Console
 from rich.live import Live
 from rich.table import Table
 
 from sklearn.feature_extraction.text import CountVectorizer
```

### Comparing `py-irt-0.4.8/pyproject.toml` & `py_irt-0.4.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-irt"
-version = "0.4.8"
+version = "0.4.9"
 readme = "README.md"
 homepage = "https://github.com/nd-ball/py-irt/"
 description = "Bayesian IRT models in Python"
 authors = ["John P. Lalor <john.lalor@nd.edu>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
@@ -15,23 +15,23 @@
 rich = "^9.3.0"
 scipy = "^1.6.3"
 typer = "^0.3.2"
 pydantic = "^1.8.2"
 scikit-learn = "1.2"
 toml = "^0.10.2"
 ordered-set = "^4.1.0"
-
+torch = "<2.0.0"
 [tool.poetry.dev-dependencies]
 codecov = "^2.1.11"
 pytest = "^6.2.4"
 pytest-cov = "^2.12.1"
 pylint = "^2.8.3"
 black = "^21.5b2"
 isort = "^5.8.0"
-ipython = "^7.31.1"
+ipython = "^8.10.0"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 known_first_party = "py_irt"
 profile = "black"
```

### Comparing `py-irt-0.4.8/setup.py` & `py_irt-0.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,167 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-irt
+Version: 0.4.9
+Summary: Bayesian IRT models in Python
+Home-page: https://github.com/nd-ball/py-irt/
+License: MIT
+Author: John P. Lalor
+Author-email: john.lalor@nd.edu
+Requires-Python: >=3.8,<3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: numpy (>=1.22.0)
+Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
+Requires-Dist: pandas (>=1.1,<2.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: pyro-ppl (>=1.6.0,<2.0.0)
+Requires-Dist: rich (>=9.3.0,<10.0.0)
+Requires-Dist: scikit-learn (==1.2)
+Requires-Dist: scipy (>=1.6.3,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: torch (<2.0.0)
+Requires-Dist: typer (>=0.3.2,<0.4.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['py_irt', 'py_irt.models']
+[![Build Status](https://travis-ci.com/nd-ball/py-irt.svg?branch=master)](https://travis-ci.com/nd-ball/py-irt)
+[![codecov.io](https://codecov.io/gh/nd-ball/py-irt/coverage.svg?branch=master)](https://codecov.io/gh/nd-ball/py-irt)
 
-package_data = \
-{'': ['*']}
+# py-irt
 
-install_requires = \
-['numpy>=1.22.0',
- 'ordered-set>=4.1.0,<5.0.0',
- 'pandas>=1.1,<2.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'pyro-ppl>=1.6.0,<2.0.0',
- 'rich>=9.3.0,<10.0.0',
- 'scikit-learn==1.2',
- 'scipy>=1.6.3,<2.0.0',
- 'toml>=0.10.2,<0.11.0',
- 'typer>=0.3.2,<0.4.0']
-
-entry_points = \
-{'console_scripts': ['py-irt = py_irt.cli:app']}
-
-setup_kwargs = {
-    'name': 'py-irt',
-    'version': '0.4.8',
-    'description': 'Bayesian IRT models in Python',
-    'long_description': '[![Build Status](https://travis-ci.com/nd-ball/py-irt.svg?branch=master)](https://travis-ci.com/nd-ball/py-irt)\n[![codecov.io](https://codecov.io/gh/nd-ball/py-irt/coverage.svg?branch=master)](https://codecov.io/gh/nd-ball/py-irt)\n\n# py-irt\n\nBayesian IRT models in Python\n\n## Overview\n\nThis repository includes code for fitting Item Response Theory (IRT) models using variational inference.\n\nAt present, the one parameter logistic (1PL) model, aka Rasch model, two parameter logistic model (2PL) and four parameter logistic model (4PL) have been implemented.\nThe user can specify whether vague or hierarchical priors are used.\nThe three-parameter logistic model is in the pipeline and will be added when available.\n\n## License\n\npy-irt is licensed under the [MIT license](https://opensource.org/licenses/MIT).\n\n## Installation\n\npy-irt is now available on PyPi!\n\n### Pre-reqs\n\n1. Install [PyTorch](https://pytorch.org/get-started/locally/).\n2. Install [Pyro](https://pyro.ai/)\n3. Install py-irt:\n\n```shell\npip install py-irt\n```\n\nOR\n\nInstall [Poetry](https://python-poetry.org/docs/#installation)\n\n```shell\ngit clone https://github.com/nd-ball/py-irt.git\ncd py-irt\npoetry install\n```\n\n## Usage\n\nOnce you install from PyPI, you can use the following command to fit an IRT\nmodel on the scored predictions of a dataset. For example, if you were to run py-irt with the 4PL model on the scored predictions of different transformer models on the SQuAD dataset, you\'d do this:\n`py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`\n\n## FAQ\n\n1. What kind of output should I expect on running the command to train an IRT model?\n\nYou should see something like this when you run the command given above:\n![image](https://user-images.githubusercontent.com/40918514/123986740-3eccd100-d9cf-11eb-8e58-ba5ad6c977ce.png)\n\n2. I tried installing py-irt using pip from PyPI. But when I try to run the command `py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`, I get an error that says `bash: py-irt: command not found`. How do I fix this?\n\nThe CLI interface was implemented in PyPi version 0.2.1. If you are getting this error try updating py-irt:\n\n`pip install --upgrade py-irt`\n\nAlternatively, you can install the latest version from github:\n\n```shell\ngit clone https://github.com/nd-ball/py-irt.git\ncd py-irt\nmv ~/py-irt/py_irt/cli.py ~/py-irt/\npython cli.py train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/\n```\n\n3. How do I evaluate a trained IRT model?\n\nIf you have already trained an IRT model you can use the following command:\n\n`py-irt evaluate 4pl ~/path/to/data/best_parameters.json ~/path/to/data/test_pairs.jsonlines /path/to/output/eg/test-4pl/`\n\nWhere `test_pairs.jsonlines` is a jsonlines file with the following format:\n\n```\n{"subject_id": "ken", "item_id": "q1"}\n{"subject_id": "ken", "item_id": "q2"}\n{"subject_id": "burt", "item_id": "q1"}\n{"subject_id": "burt", "item_id": "q3"}\n```\n\nIf you would like to both train and evaluate a model you can use the following command:\n\n`py-irt train-and-evaluate 4pl ~/path/to/data/squad.jsonlines /path/to/output/eg/test-4pl/`\n\nBy default this will train a model with 90% of the provided data and evaluate with the remaining 10%.\nTo change this behavior you can add `--evaluation all` to the command above. \nThe model will train and evaluate against all of the data.\n\n## Citations\n\nIf you use this code, please consider citing the following papers:\n\n```shell\n@inproceedings{lalor2019emnlp,\n  author    = {Lalor, John P and Wu, Hao and Yu, Hong},\n  title     = {Learning Latent Parameters without Human Response Patterns: Item Response Theory with Artificial Crowds},\n  year      = {2019},\n  booktitle = {Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing},\n}\n```\n\n```shell\n@inproceedings{rodriguez2021evaluation,\n  title={Evaluation Examples Are Not Equally Informative: How Should That Change NLP Leaderboards?},\n  author={Rodriguez, Pedro and Barrow, Joe and Hoyle, Alexander Miserlis and Lalor, John P and Jia, Robin and Boyd-Graber, Jordan},\n  booktitle={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},\n  pages={4486--4503},\n  year={2021}\n}\n```\n\nImplementation is based on the following paper:\n\n```shell\n@article{natesan2016bayesian,\n  title={Bayesian prior choice in IRT estimation using MCMC and variational Bayes},\n  author={Natesan, Prathiba and Nandakumar, Ratna and Minka, Tom and Rubright, Jonathan D},\n  journal={Frontiers in psychology},\n  volume={7},\n  pages={1422},\n  year={2016},\n  publisher={Frontiers}\n}\n```\n\n## Contributing\n\nThis is research code. Pull requests and issues are welcome!\n\n## Questions?\n\nLet me know if you have any requests, bugs, etc.\n\nEmail: john.lalor@nd.edu\n',
-    'author': 'John P. Lalor',
-    'author_email': 'john.lalor@nd.edu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/nd-ball/py-irt/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.10',
+Bayesian IRT models in Python
+
+## Overview
+
+This repository includes code for fitting Item Response Theory (IRT) models using variational inference.
+
+At present, the one parameter logistic (1PL) model, aka Rasch model, two parameter logistic model (2PL) and four parameter logistic model (4PL) have been implemented.
+The user can specify whether vague or hierarchical priors are used.
+The three-parameter logistic model is in the pipeline and will be added when available.
+
+## License
+
+py-irt is licensed under the [MIT license](https://opensource.org/licenses/MIT).
+
+## Installation
+
+py-irt is now available on PyPi!
+
+### Pre-reqs
+
+1. Install [PyTorch](https://pytorch.org/get-started/locally/).
+2. Install [Pyro](https://pyro.ai/)
+3. Install py-irt:
+
+```shell
+pip install py-irt
+```
+
+OR
+
+Install [Poetry](https://python-poetry.org/docs/#installation)
+
+```shell
+git clone https://github.com/nd-ball/py-irt.git
+cd py-irt
+poetry install
+```
+
+## Usage
+
+Once you install from PyPI, you can use the following command to fit an IRT
+model on the scored predictions of a dataset. For example, if you were to run py-irt with the 4PL model on the scored predictions of different transformer models on the SQuAD dataset, you'd do this:
+`py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`
+
+## FAQ
+
+1. What kind of output should I expect on running the command to train an IRT model?
+
+You should see something like this when you run the command given above:
+![image](https://user-images.githubusercontent.com/40918514/123986740-3eccd100-d9cf-11eb-8e58-ba5ad6c977ce.png)
+
+2. I tried installing py-irt using pip from PyPI. But when I try to run the command `py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`, I get an error that says `bash: py-irt: command not found`. How do I fix this?
+
+The CLI interface was implemented in PyPi version 0.2.1. If you are getting this error try updating py-irt:
+
+`pip install --upgrade py-irt`
+
+Alternatively, you can install the latest version from github:
+
+```shell
+git clone https://github.com/nd-ball/py-irt.git
+cd py-irt
+mv ~/py-irt/py_irt/cli.py ~/py-irt/
+python cli.py train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/
+```
+
+3. How do I evaluate a trained IRT model?
+
+If you have already trained an IRT model you can use the following command:
+
+`py-irt evaluate 4pl ~/path/to/data/best_parameters.json ~/path/to/data/test_pairs.jsonlines /path/to/output/eg/test-4pl/`
+
+Where `test_pairs.jsonlines` is a jsonlines file with the following format:
+
+```
+{"subject_id": "ken", "item_id": "q1"}
+{"subject_id": "ken", "item_id": "q2"}
+{"subject_id": "burt", "item_id": "q1"}
+{"subject_id": "burt", "item_id": "q3"}
+```
+
+If you would like to both train and evaluate a model you can use the following command:
+
+`py-irt train-and-evaluate 4pl ~/path/to/data/squad.jsonlines /path/to/output/eg/test-4pl/`
+
+By default this will train a model with 90% of the provided data and evaluate with the remaining 10%.
+To change this behavior you can add `--evaluation all` to the command above. 
+The model will train and evaluate against all of the data.
+
+## Citations
+
+If you use this code, please consider citing the following papers:
+
+```shell
+@inproceedings{lalor2019emnlp,
+  author    = {Lalor, John P and Wu, Hao and Yu, Hong},
+  title     = {Learning Latent Parameters without Human Response Patterns: Item Response Theory with Artificial Crowds},
+  year      = {2019},
+  booktitle = {Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing},
+}
+```
+
+```shell
+@inproceedings{rodriguez2021evaluation,
+  title={Evaluation Examples Are Not Equally Informative: How Should That Change NLP Leaderboards?},
+  author={Rodriguez, Pedro and Barrow, Joe and Hoyle, Alexander Miserlis and Lalor, John P and Jia, Robin and Boyd-Graber, Jordan},
+  booktitle={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},
+  pages={4486--4503},
+  year={2021}
+}
+```
+
+Implementation is based on the following paper:
+
+```shell
+@article{natesan2016bayesian,
+  title={Bayesian prior choice in IRT estimation using MCMC and variational Bayes},
+  author={Natesan, Prathiba and Nandakumar, Ratna and Minka, Tom and Rubright, Jonathan D},
+  journal={Frontiers in psychology},
+  volume={7},
+  pages={1422},
+  year={2016},
+  publisher={Frontiers}
 }
+```
+
+## Contributing
+
+This is research code. Pull requests and issues are welcome!
+
+## Questions?
+
+Let me know if you have any requests, bugs, etc.
 
+Email: john.lalor@nd.edu
 
-setup(**setup_kwargs)
```

