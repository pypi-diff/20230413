# Comparing `tmp/carate-0.3.5.tar.gz` & `tmp/carate-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carate-0.3.5.tar", last modified: Wed Apr  5 20:44:00 2023, max compression
+gzip compressed data, was "carate-0.3.6.tar", last modified: Thu Apr 13 20:04:07 2023, max compression
```

## Comparing `carate-0.3.5.tar` & `carate-0.3.6.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.525436 carate-0.3.5/
--rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.5/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1001)     6667 2023-04-05 20:44:00.525436 carate-0.3.5/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     6096 2023-04-02 15:05:26.000000 carate-0.3.5/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.522103 carate-0.3.5/carate/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.5/carate/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-04 21:05:18.000000 carate-0.3.5/carate/automate.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-04 21:05:18.000000 carate-0.3.5/carate/config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1944 2023-04-04 21:05:18.000000 carate-0.3.5/carate/default_interface.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.522103 carate-0.3.5/carate/evaluation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.5/carate/evaluation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-04 21:05:18.000000 carate-0.3.5/carate/evaluation/base.py
--rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-04 21:05:18.000000 carate-0.3.5/carate/evaluation/classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)    11450 2023-04-05 18:06:56.000000 carate-0.3.5/carate/evaluation/regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-04 21:05:18.000000 carate-0.3.5/carate/load_data.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.525436 carate-0.3.5/carate/models/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.5/carate/models/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-04 21:05:18.000000 carate-0.3.5/carate/models/base_model.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-04 21:05:18.000000 carate-0.3.5/carate/models/cgc_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-04 21:05:18.000000 carate-0.3.5/carate/models/cgc_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-04 21:05:18.000000 carate-0.3.5/carate/optimizer.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.525436 carate-0.3.5/carate/plotting/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.5/carate/plotting/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    10672 2023-04-04 21:05:18.000000 carate-0.3.5/carate/plotting/base_plots.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-04 21:05:18.000000 carate-0.3.5/carate/run.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.525436 carate-0.3.5/carate/utils/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.5/carate/utils/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-04 21:05:18.000000 carate-0.3.5/carate/utils/convert_to_json.py
--rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-04 21:05:18.000000 carate-0.3.5/carate/utils/model_files.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-04 21:05:18.000000 carate-0.3.5/carate/utils/training_result_parser.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.522103 carate-0.3.5/carate.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     6667 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      991 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-05 20:44:00.000000 carate-0.3.5/carate.egg-info/top_level.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-05 18:07:08.000000 carate-0.3.5/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-05 20:44:00.525436 carate-0.3.5/setup.cfg
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-05 20:44:00.525436 carate-0.3.5/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.5/tests/test_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)      731 2023-04-03 21:47:29.000000 carate-0.3.5/tests/test_cli.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.5/tests/test_config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2650 2023-03-29 19:35:13.000000 carate-0.3.5/tests/test_data_loader.py
--rw-r--r--   0 developer  (1001) developer  (1001)      499 2023-03-31 14:49:20.000000 carate-0.3.5/tests/test_plotting.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2344 2023-03-30 15:56:56.000000 carate-0.3.5/tests/test_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.5/tests/test_runner.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.5/tests/test_utils_convert_py_to_json.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/
+-rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.6/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-13 20:04:07.588658 carate-0.3.6/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.6/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-04 21:05:18.000000 carate-0.3.6/carate/automate.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-04 21:05:18.000000 carate-0.3.6/carate/config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1944 2023-04-04 21:05:18.000000 carate-0.3.6/carate/default_interface.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/evaluation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/base.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-04 21:05:18.000000 carate-0.3.6/carate/evaluation/classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    11463 2023-04-13 19:57:17.000000 carate-0.3.6/carate/evaluation/regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-04 21:05:18.000000 carate-0.3.6/carate/load_data.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/models/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/base_model.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/cgc_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-04 21:05:18.000000 carate-0.3.6/carate/models/cgc_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-04 21:05:18.000000 carate-0.3.6/carate/optimizer.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate/plotting/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/plotting/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    12811 2023-04-13 19:49:45.000000 carate-0.3.6/carate/plotting/base_plots.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1313 2023-04-13 19:45:37.000000 carate-0.3.6/carate/plotting/plot_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-13 19:15:30.000000 carate-0.3.6/carate/plotting/plot_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-04 21:05:18.000000 carate-0.3.6/carate/run.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/carate/utils/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/convert_to_json.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/model_files.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-04 21:05:18.000000 carate-0.3.6/carate/utils/training_result_parser.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.585324 carate-0.3.6/carate.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     1065 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-13 20:04:07.000000 carate-0.3.6/carate.egg-info/top_level.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-13 20:03:40.000000 carate-0.3.6/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-13 20:04:07.588658 carate-0.3.6/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-13 20:04:07.588658 carate-0.3.6/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.6/tests/test_cli.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.6/tests/test_data_loader.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      902 2023-04-13 19:42:15.000000 carate-0.3.6/tests/test_plotting.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2344 2023-03-30 15:56:56.000000 carate-0.3.6/tests/test_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.6/tests/test_runner.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.6/tests/test_utils_convert_py_to_json.py
```

### Comparing `carate-0.3.5/LICENSE` & `carate-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/PKG-INFO` & `carate-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,126 +1,141 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.5
+Version: 0.3.6
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CARATE
+
 [![Downloads](https://static.pepy.tech/personalized-badge/carate?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/carate)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue) 
-![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667) 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
+![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 
 ![Bert goes into the karate club](bert_goes_into_the_karate_club.png)
 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Scope](#3-scope)
+- [4. Installation on CPU](#4-installation-on-cpu)
+  - [4.1. Build manually](#41-build-manually)
+  - [4.2. Installation from repo](#42-installation-from-repo)
+- [5. Usage](#5-usage)
+  - [5.1. Start a run](#51-start-a-run)
+  - [5.2. Training results](#52-training-results)
+- [6. Build on the project](#6-build-on-the-project)
+- [7. Support the development](#7-support-the-development)
+- [8. Cite](#8-cite)
+<!-- /TOC -->
 
-# Why 
+## 1. Why
 
 Molecular representation is wrecked. Seriously! We chemists talked for decades with an ancient language about something we can't comprehend with that language. We have to stop it, now!
 
-# What 
+## 2. What
 
-The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule. 
+The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule.
 
 For a chemist it is quite intuitive but seldomly modelled as such: A molecule exhibits properties through its combined *electronic and structural features*
 
-* Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git). 
+- Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git).
 
-* Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes). 
+- Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes).
 
-* The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
+- The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
 
-* Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
-# Scope
+- Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
 
-The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks. 
+## 3. Scope
 
+The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks.
 
+## 4. Installation on CPU
 
-# Installation on CPU 
+Prepare system
 
-Prepare system 
 ```bash
 sudo apt-get install python3-dev libffi-dev
 ```
 
-## Build manually
+### 4.1. Build manually
 
-```bash 
+```bash
 pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cpu 
 pip install torch-scatter torch-sparse torch-geometric rdkit-pypi networkx[default] matplotlib
 pip install torch-cluster 
 pip install torch-spline-conv 
-``` 
+```
 
-# Faster way 
+### 4.2. Installation from repo
 
 Inside the directory of your git-clone:
 
 ```bash
 pip install -e .
 ```
 
-# Usage 
+## 5. Usage
+
+The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you.
 
-The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you. 
+Finally, with the new `pyproject.toml` it is possible to
 
-Finally, with the new `pyproject.toml` it is possible to 
-```bash 
+```bash
 pip install carate
 ```
+
 The installation will install torch with CUDA, so the decision of the library what hardware to use goes JIT (just-in-time). At the moment only CPU/GPU is implemented and FPGA/TPU and others are ignored. Further development of the package will then focus on avoiding special library APIs but make the pattern adaptable to an arbitrary algorithmic/numerical backend.
 
 ```bash
 carate -c path_to_config_file.py
 ```
 
-## Start a run
+### 5.1. Start a run
 
 To start a run you need to define the configuration. You can do so by defining a `.json` or a `config.py` file
 
 Examples for `config.py` files are given in `config_files`
 
-Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file 
+Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file
 
-## Training results 
+### 5.2. Training results
 
-Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure. 
+Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure.
 
 Previous experiments suggest to harden the machine for training to avoid unwanted side-effects as shutdowns, data loss, or data diffusion. You may still send intermediate results through the network, but store the large chunks on the hardened device.
 
 Therefore, any ETL or data processing might not be affected by any interruption on the training machine.
 
-# Build on the project
+## 6. Build on the project
 
-Building on the code is not recommended as the project will be continued in another library (building with that would make most sense). 
+Building on the code is not recommended as the project will be continued in another library (building with that would make most sense).
 
 However, you may still use the models as they are by the means of the library production ready.
 
-In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations 
+In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations
 
-* [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
+- [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
 
-We have to admit it though: There was a security incident on 31st of March 2023, so the results from 
-Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such 
-that any picky reviewer can check where there happened weird stuff, I made a mistake, or there 
+We have to admit it though: There was a security incident on 31st of March 2023, so the results from
+Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such
+that any picky reviewer can check where there happened weird stuff, I made a mistake, or there
 was an incident and requests more reproductions. That should solve the issue for now!
 
-# Support the development
+## 7. Support the development
 
 If you are happy about substantial progress in chemistry and life sciences that is not commercial first but citizen first, well then just
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
-
-
-# Cite 
+## 8. Cite
 
 There is a preprint available on bioRxiv. Read the [preprint](https://www.biorxiv.org/content/10.1101/2022.02.12.470636v1)
```

### Comparing `carate-0.3.5/README.md` & `carate-0.3.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,127 @@
 # CARATE
+
 [![Downloads](https://static.pepy.tech/personalized-badge/carate?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/carate)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue) 
-![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667) 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
+![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 
 ![Bert goes into the karate club](bert_goes_into_the_karate_club.png)
 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Scope](#3-scope)
+- [4. Installation on CPU](#4-installation-on-cpu)
+  - [4.1. Build manually](#41-build-manually)
+  - [4.2. Installation from repo](#42-installation-from-repo)
+- [5. Usage](#5-usage)
+  - [5.1. Start a run](#51-start-a-run)
+  - [5.2. Training results](#52-training-results)
+- [6. Build on the project](#6-build-on-the-project)
+- [7. Support the development](#7-support-the-development)
+- [8. Cite](#8-cite)
+<!-- /TOC -->
 
-# Why 
+## 1. Why
 
 Molecular representation is wrecked. Seriously! We chemists talked for decades with an ancient language about something we can't comprehend with that language. We have to stop it, now!
 
-# What 
+## 2. What
 
-The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule. 
+The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule.
 
 For a chemist it is quite intuitive but seldomly modelled as such: A molecule exhibits properties through its combined *electronic and structural features*
 
-* Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git). 
+- Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git).
 
-* Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes). 
+- Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes).
 
-* The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
+- The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
 
-* Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
-# Scope
+- Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
 
-The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks. 
+## 3. Scope
 
+The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks.
 
+## 4. Installation on CPU
 
-# Installation on CPU 
+Prepare system
 
-Prepare system 
 ```bash
 sudo apt-get install python3-dev libffi-dev
 ```
 
-## Build manually
+### 4.1. Build manually
 
-```bash 
+```bash
 pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cpu 
 pip install torch-scatter torch-sparse torch-geometric rdkit-pypi networkx[default] matplotlib
 pip install torch-cluster 
 pip install torch-spline-conv 
-``` 
+```
 
-# Faster way 
+### 4.2. Installation from repo
 
 Inside the directory of your git-clone:
 
 ```bash
 pip install -e .
 ```
 
-# Usage 
+## 5. Usage
+
+The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you.
 
-The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you. 
+Finally, with the new `pyproject.toml` it is possible to
 
-Finally, with the new `pyproject.toml` it is possible to 
-```bash 
+```bash
 pip install carate
 ```
+
 The installation will install torch with CUDA, so the decision of the library what hardware to use goes JIT (just-in-time). At the moment only CPU/GPU is implemented and FPGA/TPU and others are ignored. Further development of the package will then focus on avoiding special library APIs but make the pattern adaptable to an arbitrary algorithmic/numerical backend.
 
 ```bash
 carate -c path_to_config_file.py
 ```
 
-## Start a run
+### 5.1. Start a run
 
 To start a run you need to define the configuration. You can do so by defining a `.json` or a `config.py` file
 
 Examples for `config.py` files are given in `config_files`
 
-Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file 
+Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file
 
-## Training results 
+### 5.2. Training results
 
-Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure. 
+Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure.
 
 Previous experiments suggest to harden the machine for training to avoid unwanted side-effects as shutdowns, data loss, or data diffusion. You may still send intermediate results through the network, but store the large chunks on the hardened device.
 
 Therefore, any ETL or data processing might not be affected by any interruption on the training machine.
 
-# Build on the project
+## 6. Build on the project
 
-Building on the code is not recommended as the project will be continued in another library (building with that would make most sense). 
+Building on the code is not recommended as the project will be continued in another library (building with that would make most sense).
 
 However, you may still use the models as they are by the means of the library production ready.
 
-In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations 
+In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations
 
-* [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
+- [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
 
-We have to admit it though: There was a security incident on 31st of March 2023, so the results from 
-Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such 
-that any picky reviewer can check where there happened weird stuff, I made a mistake, or there 
+We have to admit it though: There was a security incident on 31st of March 2023, so the results from
+Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such
+that any picky reviewer can check where there happened weird stuff, I made a mistake, or there
 was an incident and requests more reproductions. That should solve the issue for now!
 
-# Support the development
+## 7. Support the development
 
 If you are happy about substantial progress in chemistry and life sciences that is not commercial first but citizen first, well then just
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
+## 8. Cite
 
-
-# Cite 
-
-There is a preprint available on bioRxiv. Read the [preprint](https://www.biorxiv.org/content/10.1101/2022.02.12.470636v1)
+There is a preprint available on bioRxiv. Read the [preprint](https://www.biorxiv.org/content/10.1101/2022.02.12.470636v1)
```

### Comparing `carate-0.3.5/carate/automate.py` & `carate-0.3.6/carate/automate.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/config.py` & `carate-0.3.6/carate/config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/default_interface.py` & `carate-0.3.6/carate/default_interface.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/evaluation/base.py` & `carate-0.3.6/carate/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/evaluation/regression.py` & `carate-0.3.6/carate/evaluation/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,18 +151,19 @@
         ) = self._get_defaults(locals())
 
         # data container
         result = {}
         test_mse = []
         train_mae = []
         train_mse = []
-        tmp = {}
+        
 
         save_model_parameters(model_net=model_net, save_dir=result_save_dir)
         for i in range(num_cv):
+            tmp = {}
             loaded_dataset: torch.utils.data.Dataset
             (
                 test_dataset,
                 train_dataset,
                 test_loader,
                 train_loader,
                 loaded_dataset,
```

### Comparing `carate-0.3.5/carate/load_data.py` & `carate-0.3.6/carate/load_data.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/models/cgc_classification.py` & `carate-0.3.6/carate/models/cgc_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/models/cgc_regression.py` & `carate-0.3.6/carate/models/cgc_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/optimizer.py` & `carate-0.3.6/carate/optimizer.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/plotting/base_plots.py` & `carate-0.3.6/carate/plotting/base_plots.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 """
 Plotting module for PyTorch prototyping
 
 :author: Julian M. Kleber
 """
-"""
-Plotting module for PyTorch prototyping
-
-:author: Julian M. Kleber
-"""
-
-
 from typing import Type, Optional, Dict, Any, List, Tuple
-import pandas as pd
+import logging
 import numpy as np
 import matplotlib.pyplot as plt
-from amarium.utils import load_json_from_file, prepare_file_name_saving, attach_slash
-from collections import ChainMap
-import logging
+from amarium.utils import load_json_from_file, prepare_file_name_saving, append_slash
+
 
 logging.basicConfig(
     filename="train.log",
     encoding="utf-8",
     level=logging.DEBUG,
     format="%(asctime)s %(message)s",
 )
@@ -28,121 +20,149 @@
 
 def plot_range_band_multi(
     result: List[Dict[str, float]],
     key_vals: List[str],
     file_name: str,
     alpha: float = 0.5,
     save_dir: Optional[str] = None,
+    title_text: Optional[str] = None,
 ) -> None:
-    fig, ax = plt.subplots()
-    ax.set_xlabel("Training step")
+    """
+    The plot_range_band_multi function is used to plot multiple range bands on the same graph.
+    The function takes in a list of dictionaries, each dictionary containing the results from one
+    cross-validation run.It also takes in a list of keys that correspond to values within each
+    dictionary that should be plotted as range bands. The function then plots all these values as
+    separate lines with their corresponding ranges filled in between them.
+
+    :param result:List[Dict[str: Used to Pass in the list of dictionaries
+    :param float]]: Used to Set the alpha value of the fill.
+    :param key_vals:List[str]: Used to Specify which metrics to plot.
+    :param file_name:str: Used to name the file that will be saved.
+    :param alpha:float=0.5: Used to Set the transparency of the fill between.
+    :param save_dir:Optional[str]=None: Used to Save the plot in a specific directory.
+    :param : Used to Set the transparency of the fill between min and max values.
+    :return: A plot of the average, maximum and minimum values.
+
+    :doc-author: Julian M. Kleber
+    """
+
+    fig, axis = plt.subplots()
+    axis.set_xlabel("Training step")
 
     for i in range(len(key_vals)):
         max_val: List[float]
         min_val: List[float]
         avg_val: List[float]
 
         max_val, min_val, avg_val = unpack_cross_validation(
             result=result, key_val=key_vals[i]
         )
         logging.info(f"Max values are: {max_val}")
         logging.info(f"Min values are: {min_val}")
         logging.info(f"Avg values are: {avg_val}")
 
-        ax.plot(avg_val, label=key_vals[i])
-        plot_range_fill(max_val, min_val, avg_val, alpha, ax)
-
-    ax.set_ylabel("Value")
-    ax.legend()
+        axis.plot(avg_val, label=key_vals[i])
+        plot_range_fill(max_val, min_val, alpha, axis)
 
+    axis.set_ylabel("Value")
+    axis.legend()
+    axis.set_title(title_text)
     save_publication_graphic(fig_object=fig, file_name=file_name, prefix=save_dir)
 
 
 def plot_range_band_single(
-    result: List[Dict[str, float]],
+    result: List[Dict[str, List[float]]],
     key_val: str,
     file_name: str,
     alpha: float = 0.5,
     save_dir: Optional[str] = None,
+    legend_text: Optional[str] = None,
 ) -> None:
     """
     The plot_range_band function takes in a list of dictionaries, each dictionary containing the
     results from one run.
     It then plots the average value for each key_val (e.g., 'accuracy') and also plots a
     range band between the minimum and maximum values for that key_val across all runs.
 
-    :param result:List[Dict[str: Used to Plot the results of each run.
-    :param float]]: Used to Specify the type of data that is being passed into the function.
-    :param key_val:str: Used to Specify which key in the dictionary to plot.
-    :param file_name:str: Used to Save the plot as a png file.
+    :param result:List[Dict[str: Used to plot the results of each run.
+    :param float]]: Used to specify the type of data that is being passed into the function.
+    :param key_val:str: Used to specify which key in the dictionary to plot.
+    :param file_name:str: Used to save the plot as a png file.
     :return: A plot with the average value of a list, and the minimum and maximum values.
 
-    :doc-author: Julian M. kleber
+    :doc-author: Julian M. Kleber
     """
     max_val: List[float]
     min_val: List[float]
     avg_val: List[float]
 
     max_val, min_val, avg_val = unpack_cross_validation(result=result, key_val=key_val)
 
-    fig, ax = plt.subplots()
-    ax.plot(avg_val, "-")
-    plot_range_fill(max_val, min_val, avg_val, alpha, ax)
-
-    ax.set_ylim(0.0, 1.01)
-    ax.set_ylabel(key_val)
-    ax.set_xlabel("Training step")
+    fig, axis = plt.subplots()
+    if legend_text is not None:
+        axis.plot(avg_val, "-", label=legend_text)
+    else:
+        axis.plot(avg_val, "-", label=legend_text)
+    plot_range_fill(max_val, min_val, alpha, axis)
+
+    axis.set_ylim(0.0, 1.01)
+    axis.set_ylabel(key_val)
+    if legend_text is not None:
+        axis.legend()
+
+    axis.set_xlabel("Training step")
 
     save_publication_graphic(fig_object=fig, file_name=file_name, prefix=save_dir)
 
 
 def plot_range_fill(
-    max_val: List[float], min_val: List[float], avg_val: List[float], alpha: float, ax
+    max_val: List[float], min_val: List[float], alpha: float, axis
 ) -> None:
     """
     The plot_range_lines function takes in three lists of floats, max_val, min_val and avg_val.
     It then plots the average value as a line graph with the training steps on the x-axis and
     the average values on the y-axis. It also fills in between each point with a color to show
     the range of values for that particular step.
 
     :param max_val:List[float]: Used to Plot the maximum value of each training step.
     :param min_val:List[float]: Used to Plot the minimum value of each metric.
     :param avg_val:List[float]: Used to Plot the average value of a given metric.
     :return: A plot with the average value, max value and min values for each training step.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     training_steps = np.arange(0, len(max_val), 1)
-    ax.fill_between(training_steps, min_val, max_val, alpha=alpha)
+    axis.fill_between(training_steps, min_val, max_val, alpha=alpha)
 
 
 def unpack_cross_validation(
-    result: List[Dict[str, float]], key_val: str
+    result: List[Dict[str, List[float]]], key_val: str
 ) -> Tuple[List[float]]:
     """
     The unpack_cross_validation function takes in a list of dictionaries, and a key value.
     It then unpacks the values associated with that key into three lists: max_val, min_val, avg_val.
     These lists are returned as a tuple.
 
     :param result:List[Dict[str: Used to Store the result of each iteration.
     :param float]]: Used to Store the results of the cross validation.
     :param key_val:str: Used to Specify which key in the dictionary to use for the unpacking.
     :return: The max, min and average value of the key_val parameter.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     max_val = []
     min_val = []
     avg_val = []
 
     arr_res = np.zeros((len(result), len(result[0][key_val])))
 
     for i, res in enumerate(result):
+        assert len(res[key_val]) == arr_res.shape[1], str(len(res[key_val])) +str(arr_res.shape[1])
         arr_res[i, :] = res[key_val]
 
     for i in range(arr_res.shape[1]):
         max_val.append(get_max(arr_res[:, i].tolist()))
         min_val.append(get_min(arr_res[:, i].tolist()))
         avg_val.append(get_avg(arr_res[:, i].tolist()))
 
@@ -170,37 +190,51 @@
         file_name=file_name, prefix=prefix, suffix=".png"
     )
     plt.tight_layout()
     plt.savefig(file_name, dpi=300)
 
 
 def get_stacked_list(
-    path_to_directory: str, column_name: str, num_cv: int, json_name: str
+    path_to_directory: str, num_cv: int, json_name: str
 ) -> List[Dict[str, float]]:
+    """
+    The get_stacked_list function takes in a path to a directory, the name of the column
+    that we want to stack, and the number of cross-validation folds. It then returns a list
+    of dictionaries that contain all of our stacked results.
+
+    :param path_to_directory:str: Used to Specify the directory where the json files are stored.
+    :param column_name:str: Used to Specify the column name of the dataframe in which we
+    want to get.
+    :param num_cv:int: Used to Specify the number of cross validation runs.
+    :param json_name:str: Used to Specify the name of the json file that will be parsed.
+    :return: A list of dictionaries, where each dictionary is the accuracy for a single cv.
+
+    :doc-author: Julian M. Kleber
+    """
+
     results = []
 
-    path_to_directory = attach_slash(path_to_directory)
+    path_to_directory = append_slash(path_to_directory)
 
     for i in range(num_cv):
         logging.info(f"Attempting cv {i}")
 
         result = parse_acc_list_json(
             path_to_json=path_to_directory + f"CV_{i}/" + json_name
         )
         results.append(result)
         logging.info(f"parsed results for CV {i}")
 
     return results
 
 
-def parse_old_file_format_for_plot(
-    stacked_list: List[float], path_to_json: str
-) -> List[List[float]]:
+def parse_old_file_format_for_plot(path_to_json: str) -> List[List[float]]:
     """
-    The parse_old_file_format_for_plot function takes in a path to a json file and returns the following:
+    The parse_old_file_format_for_plot function takes in a path to a json file and returns the
+    following:
 
     :param path_to_json:str: Used to Specify the path to the json file that we want to parse.
     :return: A list of dictionaries.
 
     :doc-author: Julian M. Kleber
     """
 
@@ -208,40 +242,44 @@
     train_frames_acc = parse_min_max_avg(result_acc["Train_acc"])
     test_frames_acc = parse_min_max_avg(result_acc["Test_acc"])
     return train_frames_acc, test_frames_acc
 
 
 def parse_acc_list_json(path_to_json: str) -> Dict[str, Any]:
     """
-    The parse_acc_list_json function takes in a path to a json file and returns the contents of that json file as a dictionary.
-    The function also parses the "Acc" key in the dictionary, which contains lists of tuples containing train and test accuracy values.
-    The function then separates these tuples into two separate lists, one for train accuracy values and one for test accuracy values.
-    These new lists are added to the original dictionary under keys "Acc_train" and "Acc_val", respectively.
+    The parse_acc_list_json function takes in a path to a json file and returns the contents of
+    that json file as a dictionary.The function also parses the "Acc" key in the dictionary,
+    which contains lists of tuples containing train and test accuracy values.
+    The function then separates these tuples into two separate lists, one for train accuracy values
+    and one for test accuracy values. These new lists are added to the original dictionary under
+    keys "Acc_train" and "Acc_val", respectively.
 
     :param path_to_json:str: Used to Specify the path to the json file.
     :return: A dictionary with the following keys:.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     result = load_json_from_file(path_to_json)
     return result
 
 
 def parse_acc_list_json_old_format(path_to_json: str) -> Dict[str, Any]:
     """
-    The parse_acc_list_json function takes in a path to a json file and returns the contents of that json file as a dictionary.
-    The function also parses the "Acc" key in the dictionary, which contains lists of tuples containing train and test accuracy values.
-    The function then separates these tuples into two separate lists, one for train accuracy values and one for test accuracy values.
-    These new lists are added to the original dictionary under keys "Acc_train" and "Acc_val", respectively.
+    The parse_acc_list_json function takes in a path to a json file and returns the contents of
+    that json file as a dictionary.The function also parses the "Acc" key in the dictionary, which
+    contains lists of tuples containing train and test accuracy values.
+    The function then separates these tuples into two separate lists, one for train accuracy values
+    and one for test accuracy values.These new lists are added to the original dictionary under
+    keys "Acc_train" and "Acc_val", respectively.
 
     :param path_to_json:str: Used to Specify the path to the json file.
     :return: A dictionary with the following keys:.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     result = load_json_from_file(path_to_json)
     acc_store = result["Acc"]
     train_acc = []
     test_acc = []
 
@@ -260,15 +298,15 @@
 def parse_min_max_avg(result_list: List[List[float]]) -> List[float]:
     """
     The parse_min function takes a list of lists and returns the minimum value for each sublist.
 
     :param result_list:List[List[float]]: Used to Store the results of the simulation.
     :return: A list of the minimum values for each step.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     minima = []
     maxima = []
     averages = []
     for i in range(len(result_list[0])):
         step_list = result_list[:, i]
@@ -282,15 +320,16 @@
 
 
 def get_avg(step_list: List[float]) -> float:
     """
     The get_avg function takes a list of floats and returns the average value.
 
 
-    :param step_list:List[float]: Used to Tell the function that it will be taking a list of floats as an argument.
+    :param step_list:List[float]: Used to Tell the function that it will be taking a list of
+    floats as an argument.
     :return: The mean of the step_list.
 
     :doc-author: Julian M. Kleber
     """
 
     return float(np.mean(step_list))
 
@@ -299,24 +338,25 @@
     """
     The get_max function takes a list of floats and returns the maximum value in that list.
 
 
     :param step_list:List[float]: Used to Tell the function that step_list is a list of floats.
     :return: The maximum value in the list.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     return float(np.max(step_list))
 
 
 def get_min(step_list: List[float]) -> float:
     """
     The get_min function takes a list of floats and returns the minimum value in that list.
 
-    :param step_list:List[float]: Used to Specify the type of parameter that is being passed into the function.
+    :param step_list:List[float]: Used to Specify the type of parameter that is being passed
+    into the function.
     :return: The minimum value in the step_list.
 
-    :doc-author: Trelent
+    :doc-author: Julian M. Kleber
     """
 
     return float(np.min(step_list))
```

### Comparing `carate-0.3.5/carate/run.py` & `carate-0.3.6/carate/run.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/utils/convert_to_json.py` & `carate-0.3.6/carate/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/utils/model_files.py` & `carate-0.3.6/carate/utils/model_files.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate/utils/training_result_parser.py` & `carate-0.3.6/carate/utils/training_result_parser.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/carate.egg-info/PKG-INFO` & `carate-0.3.6/carate.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,126 +1,141 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.5
+Version: 0.3.6
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CARATE
+
 [![Downloads](https://static.pepy.tech/personalized-badge/carate?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/carate)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue) 
-![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667) 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
+![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 
 ![Bert goes into the karate club](bert_goes_into_the_karate_club.png)
 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Scope](#3-scope)
+- [4. Installation on CPU](#4-installation-on-cpu)
+  - [4.1. Build manually](#41-build-manually)
+  - [4.2. Installation from repo](#42-installation-from-repo)
+- [5. Usage](#5-usage)
+  - [5.1. Start a run](#51-start-a-run)
+  - [5.2. Training results](#52-training-results)
+- [6. Build on the project](#6-build-on-the-project)
+- [7. Support the development](#7-support-the-development)
+- [8. Cite](#8-cite)
+<!-- /TOC -->
 
-# Why 
+## 1. Why
 
 Molecular representation is wrecked. Seriously! We chemists talked for decades with an ancient language about something we can't comprehend with that language. We have to stop it, now!
 
-# What 
+## 2. What
 
-The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule. 
+The success of transformer models is evident. Applied to molecules we need a graph-based transformer. Such models can then learn hidden representations of a molecule better suited to describe a molecule.
 
 For a chemist it is quite intuitive but seldomly modelled as such: A molecule exhibits properties through its combined *electronic and structural features*
 
-* Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git). 
+- Evidence of this perspective  was given in [chembee](https://codeberg.org/sail.black/chembee.git).
 
-* Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes). 
+- Mathematical equivalence of the variational principle and neural networks was given in the thesis [Markov-chain modelling of dynmaic interation patterns in supramolecular complexes](https://www.researchgate.net/publication/360107521_Markov-chain_modelling_of_dynamic_interaction_patterns_in_supramolecular_complexes).
 
-* The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
+- The failure of the BOA is described in the case of diatomic tranistion metal fluorides is described in the preprint: [Can Fluorine form triple bonds?](https://chemrxiv.org/engage/chemrxiv/article-details/620f745121686706d17ac316)
 
-* Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
-# Scope
+- Evidence of quantum-mechanical simulations via molecular dynamics is given in a seminal work [Direct Simulation of Bose-Einstein-Condensates using molecular dynmaics and the Lennard-Jones potential](https://www.researchgate.net/publication/360560870_Direct_simulation_of_Bose-Einstein_condesates_using_molecular_dynamics_and_the_Lennard-Jones_potential)
 
-The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks. 
+## 3. Scope
 
+The aim is to implement the algorithm in a reusable way, e.g. for the [chembee](https://codeberg.org/sail.black/chembee.git) pattern. Actually, the chembee pattern is mimicked in this project to provide a stand alone tool. The overall structure of the program is reusable for other deep-learning projects and will be transferred to an own project that should work similar to opinionated frameworks.
 
+## 4. Installation on CPU
 
-# Installation on CPU 
+Prepare system
 
-Prepare system 
 ```bash
 sudo apt-get install python3-dev libffi-dev
 ```
 
-## Build manually
+### 4.1. Build manually
 
-```bash 
+```bash
 pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cpu 
 pip install torch-scatter torch-sparse torch-geometric rdkit-pypi networkx[default] matplotlib
 pip install torch-cluster 
 pip install torch-spline-conv 
-``` 
+```
 
-# Faster way 
+### 4.2. Installation from repo
 
 Inside the directory of your git-clone:
 
 ```bash
 pip install -e .
 ```
 
-# Usage 
+## 5. Usage
+
+The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you.
 
-The program is meant to be run as a simple CLI. You can specify the configuration either via a `JSON` and use the program as a microservice, or you may run it locally from the command line. It is up to you. 
+Finally, with the new `pyproject.toml` it is possible to
 
-Finally, with the new `pyproject.toml` it is possible to 
-```bash 
+```bash
 pip install carate
 ```
+
 The installation will install torch with CUDA, so the decision of the library what hardware to use goes JIT (just-in-time). At the moment only CPU/GPU is implemented and FPGA/TPU and others are ignored. Further development of the package will then focus on avoiding special library APIs but make the pattern adaptable to an arbitrary algorithmic/numerical backend.
 
 ```bash
 carate -c path_to_config_file.py
 ```
 
-## Start a run
+### 5.1. Start a run
 
 To start a run you need to define the configuration. You can do so by defining a `.json` or a `config.py` file
 
 Examples for `config.py` files are given in `config_files`
 
-Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file 
+Or you can check the the `tutorial.ipynb` in `notebooks` how to use the package with a `.json` file
 
-## Training results 
+### 5.2. Training results
 
-Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure. 
+Most of the training results are saved in a accumulative json on the disk. The reason is to have enough redundancy in case of data failure.
 
 Previous experiments suggest to harden the machine for training to avoid unwanted side-effects as shutdowns, data loss, or data diffusion. You may still send intermediate results through the network, but store the large chunks on the hardened device.
 
 Therefore, any ETL or data processing might not be affected by any interruption on the training machine.
 
-# Build on the project
+## 6. Build on the project
 
-Building on the code is not recommended as the project will be continued in another library (building with that would make most sense). 
+Building on the code is not recommended as the project will be continued in another library (building with that would make most sense).
 
 However, you may still use the models as they are by the means of the library production ready.
 
-In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations 
+In case you can't wait for the picky scientist in me, you can still build on my intermediate results. You can find them in the following locations
 
-* [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
+- [Google Drive](https://drive.google.com/drive/folders/1ikY_EW-Uadkybb--TvxXFgoZtCQtniyH?usp=sharing)
 
-We have to admit it though: There was a security incident on 31st of March 2023, so the results from 
-Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such 
-that any picky reviewer can check where there happened weird stuff, I made a mistake, or there 
+We have to admit it though: There was a security incident on 31st of March 2023, so the results from
+Alchemy and ZINC are still waiting. I logged all experiments  I did and uploaded the log, such
+that any picky reviewer can check where there happened weird stuff, I made a mistake, or there
 was an incident and requests more reproductions. That should solve the issue for now!
 
-# Support the development
+## 7. Support the development
 
 If you are happy about substantial progress in chemistry and life sciences that is not commercial first but citizen first, well then just
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
-
-
-# Cite 
+## 8. Cite
 
 There is a preprint available on bioRxiv. Read the [preprint](https://www.biorxiv.org/content/10.1101/2022.02.12.470636v1)
```

### Comparing `carate-0.3.5/carate.egg-info/SOURCES.txt` & `carate-0.3.6/carate.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 carate/evaluation/regression.py
 carate/models/__init__.py
 carate/models/base_model.py
 carate/models/cgc_classification.py
 carate/models/cgc_regression.py
 carate/plotting/__init__.py
 carate/plotting/base_plots.py
+carate/plotting/plot_classification.py
+carate/plotting/plot_regression.py
 carate/utils/__init__.py
 carate/utils/convert_to_json.py
 carate/utils/model_files.py
 carate/utils/training_result_parser.py
 tests/test_classification.py
 tests/test_cli.py
 tests/test_config.py
```

### Comparing `carate-0.3.5/pyproject.toml` & `carate-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carate"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Providing reproducible modeling"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `carate-0.3.5/tests/test_classification.py` & `carate-0.3.6/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/tests/test_cli.py` & `carate-0.3.6/tests/test_cli.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 import subprocess
 
 from amarium.utils import search_subdirs
 
 from tests.utils import check_result_files
 
+
 def test_cli_func():
     if os.path.isdir("tests/data"):
         shutil.rmtree("tests/data")
 
-
     subprocess.run(["bash", "install.sh"])
     config_filepath = "tests/config/regression_test_config_override.py"
     result = subprocess.run(
         ["carate", "-c", config_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     errs = result.stderr.decode()
     run_title = "ZINC_test"
     data_set_name = "ZINC_test"
     result_dir = f"tests/results/{run_title}"
     check_result_files(
         result_dir=result_dir, run_title=run_title, data_set_name=data_set_name
-    )
+    )
```

### Comparing `carate-0.3.5/tests/test_config.py` & `carate-0.3.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/tests/test_data_loader.py` & `carate-0.3.6/tests/test_data_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,35 +62,35 @@
         dataset_name=dataset_name,
         test_ratio=test_ratio,
         batch_size=batch_size,
         custom_size=custom_size,
     )
 
     test_dataset, train_dataset, test_loader, train_loader, dataset = loader.load_data(
-        dataset_name, test_ratio, dataset_save_path, custom_size = custom_size
+        dataset_name, test_ratio, dataset_save_path, custom_size=custom_size
     )
 
     assert str(loader) == "StandardMoleculeNet"
     assert len(test_dataset) == 10
     assert len(train_dataset) == 90
-    
+
     dataset_save_path = "tests/data/"
     dataset_name = "ZINC_test"
     test_ratio = 10
     batch_size = 64
     shuffle = True
-    custom_size = 100 
+    custom_size = 100
 
     loader = StandardDatasetTUDataset(
         dataset_save_path=dataset_save_path,
         dataset_name=dataset_name,
         test_ratio=test_ratio,
         batch_size=batch_size,
     )
 
     test_dataset, train_dataset, test_loader, train_loader, dataset = loader.load_data(
-        dataset_name, test_ratio, dataset_save_path, custom_size = custom_size
+        dataset_name, test_ratio, dataset_save_path, custom_size=custom_size
     )
 
     assert str(loader) == "StandardTUDataset"
     assert len(test_dataset) == 10
-    assert len(train_dataset) == 90
+    assert len(train_dataset) == 90
```

### Comparing `carate-0.3.5/tests/test_regression.py` & `carate-0.3.6/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/tests/test_runner.py` & `carate-0.3.6/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.5/tests/test_utils_convert_py_to_json.py` & `carate-0.3.6/tests/test_utils_convert_py_to_json.py`

 * *Files identical despite different names*

