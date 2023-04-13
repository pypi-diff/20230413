# Comparing `tmp/qp_flexzboost-0.1.tar.gz` & `tmp/qp_flexzboost-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp_flexzboost-0.1.tar", last modified: Fri Mar 24 05:06:50 2023, max compression
+gzip compressed data, was "qp_flexzboost-0.1.1.tar", last modified: Thu Apr 13 20:57:59 2023, max compression
```

## Comparing `qp_flexzboost-0.1.tar` & `qp_flexzboost-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.043071 qp_flexzboost-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.031071 qp_flexzboost-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.035071 qp_flexzboost-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/notebooks/intro_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/notebooks/cdf_demonstration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 05:06:50.043071 qp_flexzboost-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/src/qp_flexzboost/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/src/qp_flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-24 05:06:49.000000 qp_flexzboost-0.1/src/qp_flexzboost/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25703 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/src/qp_flexzboost/flexzboost_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-24 05:06:50.000000 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-24 05:06:50.000000 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 05:06:50.000000 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-24 05:06:50.000000 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 05:06:50.000000 qp_flexzboost-0.1/src/qp_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:50.039071 qp_flexzboost-0.1/tests/qp_flexzboost_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/tests/qp_flexzboost_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-24 05:06:34.000000 qp_flexzboost-0.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.590656 qp_flexzboost-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/cdf_demonstration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/minimal_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/source/performance_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/qp_flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25703 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/flexzboost_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py
```

### Comparing `qp_flexzboost-0.1/.github/workflows/linting.yml` & `qp_flexzboost-0.1.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/.github/workflows/publish-to-pypi.yml` & `qp_flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/.github/workflows/smoke-test.yml` & `qp_flexzboost-0.1.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/.github/workflows/testing-and-coverage.yml` & `qp_flexzboost-0.1.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/.gitignore` & `qp_flexzboost-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/.pre-commit-config.yaml` & `qp_flexzboost-0.1.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 repos:
 
+    # Compare the local template version to the latest remote template version
+    # This hook should always pass. It will print a message if the local version 
+    # is out of date.
+  - repo: https://github.com/lincc-frameworks/pre-commit-hooks
+    rev: v0.1
+    hooks:
+      - id: check-lincc-frameworks-template-version
+        name: Check template version
+        description: Compare current template version against latest
+        verbose: true
+
     # Clear output from jupyter notebooks so that only the input cells are committed.
   - repo: local
     hooks:
       - id: jupyter-nb-clear-output
         name: jupyter-nb-clear-output
         description: Clear output from Jupyter notebooks.
         files: \.ipynb$
@@ -53,15 +64,15 @@
       - id: isort
         name: isort (python files in src/ and tests/)
         description: Sort and organize imports in .py files.
         types: [python]
         files: ^(src|tests)/
 
 
-      # Analyze the src code style and report code that doesn't adhere.
+    # Analyze the src code style and report code that doesn't adhere.
   - repo: local
     hooks:
       - id: pylint
         name: pylint (python files in src/)
         entry: pylint
         language: system
         types: [python]
```

### Comparing `qp_flexzboost-0.1/LICENSE` & `qp_flexzboost-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/docs/Makefile` & `qp_flexzboost-0.1.1/docs/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?= -T -E -d _build/doctrees -D language=en
-EXCLUDENB 	  ?= -D exclude_patterns="notebooks/*"
+EXCLUDENB     ?= -D exclude_patterns="notebooks/*"
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = ../_readthedocs/
 
-.PHONY: help no-nb no-notebooks clean Makefile
+.PHONY: help clean Makefile no-nb no-notebooks
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 # Build all Sphinx docs locally, except the notebooks
 no-nb no-notebooks:
```

### Comparing `qp_flexzboost-0.1/docs/conf.py` & `qp_flexzboost-0.1.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 
 master_doc = "index"  # This assumes that sphinx-build is called from the root directory
 html_show_sourcelink = False  # Remove 'view source code' from top of page (for html, not python)
 add_module_names = False # Remove namespaces from class/method signatures
 
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
+autoapi_ignore = ["*/__main__.py", "*/_version.py"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `qp_flexzboost-0.1/notebooks/cdf_demonstration.ipynb` & `qp_flexzboost-0.1.1/docs/notebooks/cdf_demonstration.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9563521241830065%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'It also shows that the CDF approaches 1 for "*

 * *            "bump_threshold and sharpen_alpha values of `None` and non-`None`. ')], delete: [1]}}, "*

 * *            "2: {'source': {insert: [(2, 'import numpy as np\\n'), (4, 'import matplotlib.pyplot "*

 * *            "as plt')], delete: [6, 5, 4, 3]}}, 7: {'source': {insert: [(0, '# Here we specify a "*

 * *            "particular PDF id, and define a fine and course x grid.\\n')]}}, 12: {'source': "*

 * *            "{delete: [0]}},  […]*

```diff
@@ -1,31 +1,37 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# CDF Exploration notebook for `qp_flexzboost`"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "This notebook demonstrates that as the x grid resolution is increased, the CDF approaches 1.\n",
-                "It also shows that the CDF approaches 1 for bump_threshold and sharpen_alpha values of None and non-None. "
+                "It also shows that the CDF approaches 1 for bump_threshold and sharpen_alpha values of `None` and non-`None`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import qp\n",
                 "import qp_flexzboost\n",
+                "import numpy as np\n",
                 "from flexcode.basis_functions import BasisCoefs\n",
-                "import matplotlib.pyplot as plt\n",
-                "\n",
-                "print(qp_flexzboost.__file__)\n",
-                "print(qp.__file__)"
+                "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -47,14 +53,22 @@
                 "                                z_min=0.0,\n",
                 "                                z_max=3.0,\n",
                 "                                bump_threshold=None,\n",
                 "                                sharpen_alpha=None)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Next we'll build a `qp.Ensemble` from the test data and `basis_coefficients` object defined above."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fzb = qp.Ensemble(qp_flexzboost.flexzboost_create_from_basis_coef_object,\n",
                 "                  data=dict(weights=coefs, basis_coefficients_object=basis_coefficients))"
@@ -62,14 +76,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Here we specify a particular PDF id, and define a fine and course x grid.\n",
                 "pdf_id = 6\n",
                 "x_course = np.linspace(0,3,100)\n",
                 "x_fine = np.linspace(0,3,30000)"
             ]
         },
         {
             "cell_type": "code",
@@ -78,14 +93,22 @@
             "outputs": [],
             "source": [
                 "# Example PDF with no bump removal or peak sharpening\n",
                 "qp.plotting.plot_native(fzb[pdf_id], xlim=[0,3])"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Next we'll plot the numerical CDF of the same distribution using the course and fine x grids. Note that finer grid approaches 1 while, the course grid just exceeds 0.91."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Demonstrate that CDFs approach 1 as grid resolution increases\n",
                 "cdf_course = fzb[pdf_id].cdf(x_course)\n",
@@ -95,52 +118,62 @@
                 "plt.legend()\n",
                 "\n",
                 "print('Max CDF value, course grid:', np.max(cdf_course))\n",
                 "print('Max CDF value, fine grid:', np.max(cdf_fine))"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In this cell, we show that we can dynamically change the bump threshold and sharpening without having to rerun the model."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Here we show that we can dynamically change the bump threshold and sharpening without rerunning the model.\n",
                 "fzb.dist.bump_threshold = 0.1\n",
                 "fzb.dist.sharpen_alpha = 1.2"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "pdf_id = 6\n",
-                "x_course = np.linspace(0,3,100)\n",
-                "x_fine = np.linspace(0,3,30000)"
+                "Compare this plot to the PDF plotted in cell 6. It is the same PDF< but with bump thresholds and peak sharpening applied."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Example PDF with bump removal and peak sharpening\n",
                 "qp.plotting.plot_native(fzb[pdf_id], xlim=[0,3])"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Again, even with bump thresholding and peak sharpening, the numerical CDF will approach 1 for fine x grids. Note though, that the difference between the course and fine grids is more pronounced when including non-`None` bump threshold and sharpen alpha values. Here the fine grid approaches 1, while the course grid approaches 0.8. Recall in the previous example without bump threshold or peak sharpening, the course grid just exceeds 0.91."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Demonstrate that CDFs approach 1 as grid resolution increases\n",
                 "cdf_course = fzb[pdf_id].cdf(x_course)\n",
                 "cdf_fine = fzb[pdf_id].cdf(x_fine)\n",
                 "plt.plot(x_course, np.squeeze(cdf_course), label='Course')\n",
                 "plt.plot(x_fine, np.squeeze(cdf_fine), label='Fine')\n",
                 "plt.legend()\n",
                 "\n",
                 "print('Max CDF value, course grid:', np.max(cdf_course))\n",
```

### Comparing `qp_flexzboost-0.1/notebooks/demo.ipynb` & `qp_flexzboost-0.1.1/docs/notebooks/demo.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9383090062111801%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'import numpy as np')], delete: [8, 7, 6, 5]}}, 4: "*

 * *            "{'source': {delete: [0]}}, 8: {'source': {insert: [(0, '# The more user friendly "*

 * *            'technique for instantiating a qp.Ensemble. It requires fewer input parameters for the '*

 * *            'user to provide. Under the hood, it will be converted to the second technique shown '*

 * *            "next.\\n'), (2, '\\n'), (3, '# The second technique, which requires multiple "*

 * *            "parameters to be […]*

```diff
@@ -1,33 +1,53 @@
 {
     "cells": [
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Demonstration notebook for `qp_flexzboost`"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "This notebook showcases the general functionality of provided by qp and qp_flexzboost."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "import qp\n",
                 "import qp_flexzboost\n",
                 "from flexcode.basis_functions import BasisCoefs\n",
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "\n",
-                "print(qp_flexzboost.__file__)\n",
-                "print(qp.__file__)"
+                "import numpy as np"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "First, we'll retrieve some real world example coefficients (i.e. weights) and define a `basis_coefficients` object."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Retrieve some real world example coefficients (i.e. weights) that are used for testing.\n",
                 "qp_flexzboost.FlexzboostGen.make_test_data()\n",
                 "coefs = qp_flexzboost.FlexzboostGen.test_data['weights']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -64,66 +84,104 @@
                 "\n",
                 "# xx_vals = np.tile(x, [10, 1])\n",
                 "# print(xx_vals.shape)\n",
                 "# yy_vals = basis_coefficients.evaluate(xx_vals)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "There are two ways to instantiate a `qp.Ensemble` that contains `qp_flexzboost` distributions. The first way is to use `qp_flexzboost.flexzboost_create_from_basis_coef_object`. It's more user friendly and is unpacked on users behalf, into the second way - using `qp_flexzboost.flexzboost`. Either approach will result in identical `qp.Ensemble` objects for identical inputs."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#Demonstrate building the ensemble using either the BasisCoefs object or the individual properties of the BasisCoef object\n",
+                "# The more user friendly technique for instantiating a qp.Ensemble. It requires fewer input parameters for the user to provide. Under the hood, it will be converted to the second technique shown next.\n",
                 "fzb = qp.Ensemble(qp_flexzboost.flexzboost_create_from_basis_coef_object, data=dict(weights=coefs, basis_coefficients_object=basis_coefficients))\n",
+                "\n",
+                "# The second technique, which requires multiple parameters to be listed explicitly is easier for `qp` machinery to work with.\n",
                 "fzb2 = qp.Ensemble(qp_flexzboost.flexzboost, \n",
-                "                   data=dict(weights=coefs, basis_system_enum_value=1, z_min=0.0, z_max=3.0, bump_threshold=0.1, sharpen_alpha=1.2))\n",
-                "print(fzb.dist)\n",
-                "print(fzb2.dist)"
+                "                   data=dict(weights=coefs, basis_system_enum_value=1, z_min=0.0, z_max=3.0, bump_threshold=0.1, sharpen_alpha=1.2))"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To drive the point home, we demonstrate that the output PDF values are the same regardless of whether the ensemble is constructed with a BasisCoef or with the individual properties of the BasisCoef. If the values in the two `Ensembles` are the same, we expect an output value of 0.0."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Demonstrate that the output PDF values are the same regardless of whether the ensemble\n",
-                "# is constructed with a BasisCoef or with the individual properties of the BasisCoef\n",
                 "pdf_id = 6\n",
                 "x = np.linspace(0,3,100)\n",
                 "\n",
                 "print(np.sum(fzb[pdf_id].pdf(x) - fzb2[pdf_id].pdf(x)))"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Simple demonstraition of the built in PDF plotting."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Demonstrate simple plotting of a single PDF in the ensemble\n",
                 "qp.plotting.plot_native(fzb[pdf_id], xlim=[0,3])"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Similarly a demonstration of plotting CDFs. The first selects a particular distribution from the `Ensemble` and retrieves the CDF. The second approach calculates the CDFs of all the distributions before selected one to plot. Here we've selected the same distribution to show that both methods produce the same results. "
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Demonstrate that CDFs work as expected\n",
                 "\n",
                 "# A single CDF from the ensemble\n",
-                "plt.plot(x, np.squeeze(fzb[pdf_id].cdf(x)), linewidth=5)\n",
+                "plt.plot(x, np.squeeze(fzb[pdf_id].cdf(x)), linewidth=5, label='Single CDF')\n",
                 "\n",
                 "# Calculate the CDF for all distributions in the ensemble, and then select one\n",
                 "cdfs = fzb.cdf(x)\n",
                 "cdfs[pdf_id]\n",
-                "plt.plot(x, cdfs[pdf_id], linestyle='--' )"
+                "plt.plot(x, cdfs[pdf_id], linestyle='--', label='Selected from all CDFs' )\n",
+                "plt.legend()\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The following demonstrates exactly what would be saved to disk for this `Ensemble`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -135,21 +193,27 @@
                 "print(tabs['meta'])\n",
                 "print()\n",
                 "print(\"Object Data\")\n",
                 "print(tabs['data'])"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The following demonstrates that the ensemble can be written to disk, and read back in with no loss of information."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Demonstrate that the ensemble can be written to disk, and read back in with no loss of information\n",
-                "\n",
                 "output_fits = \"test_output.fits\"\n",
                 "output_hdf5 = \"test_output.hdf5\"\n",
                 "\n",
                 "# delete the files if they already exist\n",
                 "try:\n",
                 "    os.unlink(output_hdf5)\n",
                 "    os.unlink(output_fits)\n",
@@ -168,16 +232,17 @@
                 "\n",
                 "# Show that the number of PDFs is the same after reading in the files\n",
                 "print(\"Initial number of pdfs:\", fzb.npdf)\n",
                 "print(\"Recovered number of pdfs, hdf5:\", fzb_reread_hdf5.npdf)\n",
                 "print(\"Recovered number of pdfs, fits:\", fzb_reread_fits.npdf)\n",
                 "\n",
                 "# Show that the plots for a given PDF are the same\n",
-                "_, ax = qp.plotting.plot_native(fzb_reread_hdf5[pdf_id], xlim=[0,3])\n",
-                "qp.plotting.plot_native(fzb_reread_fits[pdf_id], axes=ax)\n",
+                "_, ax = qp.plotting.plot_native(fzb_reread_hdf5[pdf_id], xlim=[0,3], linewidth=5, label='Original')\n",
+                "qp.plotting.plot_native(fzb_reread_fits[pdf_id], axes=ax, label='Read from disk')\n",
+                "plt.legend()\n",
                 "\n",
                 "# Show that nothing has been lost in the file type storage methods\n",
                 "pdf_hdf5 = fzb_reread_hdf5[pdf_id].pdf(x_vals)\n",
                 "pdf_fits = fzb_reread_fits[pdf_id].pdf(x_vals)\n",
                 "print(\"Total difference in file storage types:\", sum((pdf_fits-pdf_hdf5)**2))\n",
                 "\n",
                 "# show that all the parameters to define the BasisCoef object have been recovered\n",
@@ -190,37 +255,53 @@
                 "    os.unlink(output_hdf5)\n",
                 "    os.unlink(output_fits)\n",
                 "except FileNotFoundError:\n",
                 "    pass"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Here we show that the `qp_flexzboost` parameterization can be converted to other native `qp` representations. The conversion will be lossy, with the impact to the fidelity defined primarily by the x grid used in the conversion."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Demonstrate that the Flexzboost parameterization of the data can be converted\n",
                 "# to other representations. For instance here, an interpolated grid.\n",
                 "ens_interp = fzb.convert_to(qp.interp_gen, xvals=np.linspace(0,3,100))\n",
                 "\n",
                 "# Plot interpolated PDF (thick line)\n",
-                "qp.plotting.plot_native(ens_interp[pdf_id], xlim=[0,3], linewidth=5)\n",
+                "qp.plotting.plot_native(ens_interp[pdf_id], xlim=[0,3], linewidth=5, label='qp Interpolated')\n",
                 "\n",
                 "# Plot original, Flexzboost PDF (dashed line)\n",
-                "plt.plot(x, np.squeeze(fzb[pdf_id].pdf(x)), linestyle='--')"
+                "plt.plot(x, np.squeeze(fzb[pdf_id].pdf(x)), linestyle='--', label='FlexZBoost Original')\n",
+                "plt.legend()\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Here we demonstrate that the bump threshold and sharpening alpha parameters can be changed dynamically without rerunning the model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#Demonstrating that the bump threshold and sharpening alpha parameters can be changed without rerunning the model.\n",
                 "# Set the bump threshold and sharpening parameters to the original values\n",
                 "fzb.dist.bump_threshold = 0.1\n",
                 "fzb.dist.sharpen_alpha = 1.2\n",
                 "\n",
                 "# Plot original, Flexzboost PDF (dashed line)\n",
                 "plt.plot(x, np.squeeze(fzb[pdf_id].pdf(x)), linewidth=5, label='Non-None bump and sharpen parameters')\n",
                 "\n",
```

### Comparing `qp_flexzboost-0.1/pyproject.toml` & `qp_flexzboost-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,18 @@
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 dynamic = ["version"]
 dependencies = [
-    "deprecated",
     "flexcode",
     "ipykernel", # Support for Jupyter notebooks
     "numpy >= 1.24",
-    "qp-prob>=0.7.1", # The primary dependency
+    "qp-prob[full]>=0.8.1", # The primary dependency
     "scipy >= 1.9.0",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `qp_flexzboost-0.1/src/.pylintrc` & `qp_flexzboost-0.1.1/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/src/qp_flexzboost/flexzboost_pdf.py` & `qp_flexzboost-0.1.1/src/qp_flexzboost/flexzboost_pdf.py`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/src/qp_flexzboost.egg-info/SOURCES.txt` & `qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
 docs/requirements.txt
 docs/notebooks/README.md
-docs/notebooks/intro_notebook.ipynb
-notebooks/README.md
-notebooks/cdf_demonstration.ipynb
-notebooks/demo.ipynb
+docs/notebooks/cdf_demonstration.ipynb
+docs/notebooks/demo.ipynb
+docs/notebooks/minimal_notebook.ipynb
+docs/source/performance_comparison.rst
 src/.pylintrc
 src/qp_flexzboost/__init__.py
 src/qp_flexzboost/_version.py
 src/qp_flexzboost/flexzboost_pdf.py
 src/qp_flexzboost.egg-info/PKG-INFO
 src/qp_flexzboost.egg-info/SOURCES.txt
 src/qp_flexzboost.egg-info/dependency_links.txt
```

### Comparing `qp_flexzboost-0.1/tests/.pylintrc` & `qp_flexzboost-0.1.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py` & `qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         """Ensure that the survival function works as expected"""
         xpts = flexzboost_test_data['test_xvals']
         sfs = flexzboost_ensemble.sf(xpts)
         cdfs = flexzboost_ensemble.cdf(xpts)
         check_sf = sfs + cdfs
         assert_all_small(check_sf-1, atol=2e-2, test_name="sf")
 
-    def test_inverse_survival_function(self, flexzboost_ensemble, flexzboost_test_data):
+    def test_inverse_survival_function(self, flexzboost_ensemble):
         """Test that the ISF output has the right shape"""
         isf = flexzboost_ensemble.isf(QUANTS)
         assert flexzboost_ensemble.npdf == isf.shape[0]
         assert isf.shape[1] == QUANTS.shape[0]
 
     def test_random_variates_size(self, flexzboost_ensemble):
         """Demonstrate that random variates can be extracted from the distributions"""
```

### Comparing `qp_flexzboost-0.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py` & `qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py`

 * *Files identical despite different names*

