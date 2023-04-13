# Comparing `tmp/qp_flexzboost-0.1.1.tar.gz` & `tmp/qp_flexzboost-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp_flexzboost-0.1.1.tar", last modified: Thu Apr 13 20:57:59 2023, max compression
+gzip compressed data, was "qp_flexzboost-0.1.2.tar", last modified: Thu Apr 13 21:00:59 2023, max compression
```

## Comparing `qp_flexzboost-0.1.1.tar` & `qp_flexzboost-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.590656 qp_flexzboost-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/cdf_demonstration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks/minimal_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/docs/source/performance_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/qp_flexzboost/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25703 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/src/qp_flexzboost/flexzboost_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 20:57:59.000000 qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.594656 qp_flexzboost-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:59.598656 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-13 20:57:40.000000 qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/notebooks/cdf_demonstration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/notebooks/minimal_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/docs/source/performance_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.251590 qp_flexzboost-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/src/qp_flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/src/qp_flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25703 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/src/qp_flexzboost/flexzboost_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 21:00:59.000000 qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:59.255590 qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-13 21:00:49.000000 qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/test_flexzboost_pdf.py
```

### Comparing `qp_flexzboost-0.1.1/.github/workflows/linting.yml` & `qp_flexzboost-0.1.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml` & `qp_flexzboost-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/.github/workflows/smoke-test.yml` & `qp_flexzboost-0.1.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/.github/workflows/testing-and-coverage.yml` & `qp_flexzboost-0.1.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/.gitignore` & `qp_flexzboost-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/.pre-commit-config.yaml` & `qp_flexzboost-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/LICENSE` & `qp_flexzboost-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/PKG-INFO` & `qp_flexzboost-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp_flexzboost
-Version: 0.1.1
+Version: 0.1.2
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>, Drew Oldag <awoldag@uw.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `qp_flexzboost-0.1.1/README.md` & `qp_flexzboost-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/Makefile` & `qp_flexzboost-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/conf.py` & `qp_flexzboost-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/index.rst` & `qp_flexzboost-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/notebooks/cdf_demonstration.ipynb` & `qp_flexzboost-0.1.2/docs/notebooks/cdf_demonstration.ipynb`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/notebooks/demo.ipynb` & `qp_flexzboost-0.1.2/docs/notebooks/demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/notebooks/minimal_notebook.ipynb` & `qp_flexzboost-0.1.2/docs/notebooks/minimal_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/docs/source/performance_comparison.rst` & `qp_flexzboost-0.1.2/docs/source/performance_comparison.rst`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/pyproject.toml` & `qp_flexzboost-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 dynamic = ["version"]
 dependencies = [
     "flexcode",
-    "ipykernel", # Support for Jupyter notebooks
     "numpy >= 1.24",
-    "qp-prob[full]>=0.8.1", # The primary dependency
+    "qp-prob>=0.8.1", # The primary dependency
     "scipy >= 1.9.0",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
-    "pytest",
+    "ipykernel", # Support for Jupyter notebooks
+    "pytest", # Used for unit testing
     "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
+    "qp-prob[full]>=0.8.1", # The primary dependency
     "sphinx==6.1.3", # Used to automatically generate documentation
     "sphinx_rtd_theme==1.2.0", # Used to render documentation
     "sphinx-autoapi==2.0.1", # Used to automatically generate api documentation
     "pylint", # Used for static linting of files
     "nbconvert", # Needed for pre-commit check to clear output from Python notebooks
     "nbsphinx", # Used to itegrate Python notebooks into Sphinx documentation
     "ipython", # Also used in building notebooks into Sphinx
```

### Comparing `qp_flexzboost-0.1.1/src/.pylintrc` & `qp_flexzboost-0.1.2/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/src/qp_flexzboost/flexzboost_pdf.py` & `qp_flexzboost-0.1.2/src/qp_flexzboost/flexzboost_pdf.py`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/PKG-INFO` & `qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-flexzboost
-Version: 0.1.1
+Version: 0.1.2
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>, Drew Oldag <awoldag@uw.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `qp_flexzboost-0.1.1/src/qp_flexzboost.egg-info/SOURCES.txt` & `qp_flexzboost-0.1.2/src/qp_flexzboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/tests/.pylintrc` & `qp_flexzboost-0.1.2/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py` & `qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/test_flexzboost_ensemble.py`

 * *Files identical despite different names*

### Comparing `qp_flexzboost-0.1.1/tests/qp_flexzboost_tests/test_flexzboost_pdf.py` & `qp_flexzboost-0.1.2/tests/qp_flexzboost_tests/test_flexzboost_pdf.py`

 * *Files identical despite different names*

