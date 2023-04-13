# Comparing `tmp/iqm-cortex-cli-3.4.tar.gz` & `tmp/iqm-cortex-cli-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-3.4.tar", last modified: Wed Mar 22 10:09:45 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-3.5.tar", last modified: Thu Apr 13 08:39:21 2023, max compression
```

## Comparing `iqm-cortex-cli-3.4.tar` & `iqm-cortex-cli-3.5.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.748293 iqm-cortex-cli-3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.752293 iqm-cortex-cli-3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.752293 iqm-cortex-cli-3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.748293 iqm-cortex-cli-3.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.752293 iqm-cortex-cli-3.4/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.752293 iqm-cortex-cli-3.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.748293 iqm-cortex-cli-3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/src/cortex_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 10:09:45.000000 iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20488 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/circuit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34837 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:09:45.756293 iqm-cortex-cli-3.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/qasm_qubit_placement.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/valid_circuit.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/valid_circuit.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/valid_circuit_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/resources/valid_circuit_qasm_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-22 10:09:13.000000 iqm-cortex-cli-3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40133 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20504 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/circuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/qasm_qubit_placement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit_qasm_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tox.ini
```

### Comparing `iqm-cortex-cli-3.4/.github/workflows/ci.yml` & `iqm-cortex-cli-3.5/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -13,36 +13,36 @@
       matrix:
         platform: [ ubuntu-latest, macos-latest, windows-latest ]
         python-version: [ '3.9', '3.10.6' ]
         # Replace 3.10.6 with 3.10 when mypy bug is fixed
         # https://github.com/python/mypy/issues/13627
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e ".[dev]"
           python -m pip install tox-gh-actions==2.12.0
       - name: Run tests
         run: tox
   test_docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e ".[dev, docs]"
       - name: Test if docs can be built
```

### Comparing `iqm-cortex-cli-3.4/.github/workflows/publish.yml` & `iqm-cortex-cli-3.5/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         required: true
 
 jobs:
   push_to_pypi:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Fetch all history for all tags and branches
         run: git fetch --prune --unshallow
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e ".[dev,cicd]"
       - name: Build and publish
@@ -36,19 +36,19 @@
           TWINE_USERNAME: ${{ secrets.PYPI_USER }}
           TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
   publish_docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e ".[dev]"
           sudo apt-get install graphviz
```

### Comparing `iqm-cortex-cli-3.4/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-3.5/.github/workflows/tag_and_release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,27 @@
       - 'CHANGELOG.rst'
 
 jobs:
   check_version:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Check version in changelog
         run: bash ./tag-from-pipeline.sh verify_changelog_version
 
   create_tag_and_release:
     needs: check_version
     runs-on: ubuntu-latest
     if: ${{ github.ref == 'refs/heads/main' }}
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Create new tag and release
         run: bash ./tag-from-pipeline.sh create_new_tag
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `iqm-cortex-cli-3.4/CHANGELOG.rst` & `iqm-cortex-cli-3.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 3.5
+===========
+
+* Allow user to update a temporary password in ``auth login`` command. `#41 <https://github.com/iqm-finland/cortex-cli/pull/41>`_
+
 Version 3.4
 ===========
 
 * "Pin down" supported Python versions to 3.9 and 3.10. `#38 <https://github.com/iqm-finland/cortex-cli/pull/38>`_
 * Configure Tox to skip missing versions of Python interpreters when running tests. `#38 <https://github.com/iqm-finland/cortex-cli/pull/38>`_
 * Move project metadata and configuration to ``pyproject.toml``. `#38 <https://github.com/iqm-finland/cortex-cli/pull/38>`_
```

### Comparing `iqm-cortex-cli-3.4/DEVELOPMENT.rst` & `iqm-cortex-cli-3.5/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/LICENSE.rst` & `iqm-cortex-cli-3.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/PKG-INFO` & `iqm-cortex-cli-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 3.4
+Version: 3.5
 Summary: CLI for executing quantum circuits
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-3.4/README.rst` & `iqm-cortex-cli-3.5/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/Makefile` & `iqm-cortex-cli-3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_static/images/favicon.ico` & `iqm-cortex-cli-3.5/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_static/images/logo.png` & `iqm-cortex-cli-3.5/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-3.5/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-3.5/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_templates/page.html` & `iqm-cortex-cli-3.5/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/_templates/versioning.html` & `iqm-cortex-cli-3.5/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/docs/conf.py` & `iqm-cortex-cli-3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/pyproject.toml` & `iqm-cortex-cli-3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.9, <3.11"
 dependencies = [
     "click >= 7.1.2",
     "jsonschema >= 4.6.0",
+    "mechanize >= 0.4.8",
     "psutil >= 5.9.2",
     "pydantic >= 1.10.2, < 2.0",
     "python-daemon >= 2.3.0",
     "requests >= 2.26.0"
 ]
 
 [project.urls]
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/__init__.py` & `iqm-cortex-cli-3.5/src/cortex_cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """IQM's command-line interface (CLI) for executing quantum circuits.
 """
-from importlib.metadata import PackageNotFoundError, version
+from importlib.metadata import PackageNotFoundError, version  # type: ignore
 
 try:
     DIST_NAME = 'iqm-cortex-cli'
     __version__ = version(DIST_NAME)
 except PackageNotFoundError:
     __version__ = 'unknown'
 finally:
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/auth.py` & `iqm-cortex-cli-3.5/src/cortex_cli/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,25 +17,30 @@
 
 from base64 import b64decode
 from enum import Enum
 import json
 import time
 from typing import Optional
 
+import mechanize  # type: ignore
 from pydantic import BaseModel, Field
 import requests
 
 REFRESH_MARGIN_SECONDS = 15
 AUTH_REQUESTS_TIMEOUT = 20
 
 
 class ClientAuthenticationError(RuntimeError):
     """Something went wrong with user authentication."""
 
 
+class ClientAccountSetupError(RuntimeError):
+    """User's account has not been fully set up yet."""
+
+
 class GrantType(str, Enum):
     """
     Type of token request.
     """
 
     PASSWORD = 'password'
     REFRESH = 'refresh_token'
@@ -74,21 +79,52 @@
 
     data = AuthRequest(client_id=client_id, grant_type=GrantType.PASSWORD, username=username, password=password)
 
     request_url = f'{url}/realms/{realm}/protocol/openid-connect/token'
     result = requests.post(request_url, data=data.dict(exclude_none=True), timeout=AUTH_REQUESTS_TIMEOUT)
     if result.status_code == 404:
         raise ClientAuthenticationError(f'token endpoint is not available at {url}')
+    if result.status_code == 400 and result.json().get('error_description', '') == 'Account is not fully set up':
+        raise ClientAccountSetupError('Account is not fully set up')
     if result.status_code != 200:
         raise ClientAuthenticationError('invalid username and/or password')
     tokens = result.json()
     tokens = {key: tokens.get(key, '') for key in ['access_token', 'refresh_token']}
     return tokens
 
 
+def update_password(url: str, realm: str, username: str, password: str, new_password: str):
+    """Update temporary password using authentication server's account view.
+
+    This works only when account has a temporary password,
+    not to be used for changing permanent passwords.
+    """
+    browser = mechanize.Browser()
+    browser.set_handle_robots(False)
+    browser.open(f'{url}/realms/{realm}/account')
+
+    # Enter old credentials into login form
+    browser.select_form(nr=0)
+    browser['username'] = username
+    browser['password'] = password
+    browser.submit()
+
+    # Enter new credentials into password update form
+    browser.select_form(nr=0)
+    browser['password-new'] = new_password
+    browser['password-confirm'] = new_password
+    browser.submit()
+
+    # Check that password update was successful
+    if not browser.geturl().startswith(f'{url}/realms/{realm}/account'):
+        raise RuntimeError('submitting new password failed')
+
+    browser.close()
+
+
 def refresh_request(url: str, realm: str, client_id: str, refresh_token: str) -> Optional[dict[str, str]]:
     """Sends refresh request to the authentication server.
 
     Raises:
         Timeout: no response from auth server within the timeout period
         ConnectionError: connecting the auth server failed on all retries
         ClientAuthenticationError: updating the tokens failed
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/circuit.py` & `iqm-cortex-cli-3.5/src/cortex_cli/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-3.5/src/cortex_cli/cortex_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,19 +31,21 @@
 from pydantic import ValidationError
 import requests
 from requests.exceptions import ConnectionError, Timeout  # pylint: disable=redefined-builtin
 
 from cortex_cli import DIST_NAME, __version__
 from cortex_cli.auth import (
     AUTH_REQUESTS_TIMEOUT,
+    ClientAccountSetupError,
     ClientAuthenticationError,
     login_request,
     logout_request,
     refresh_request,
     time_left_seconds,
+    update_password,
 )
 from cortex_cli.circuit import CIRCUIT_MISSING_DEPS_MSG, parse_qasm_circuit, validate_circuit
 from cortex_cli.models import ConfigFile, TokensFile
 from cortex_cli.token_manager import check_token_manager, daemonize_token_manager, start_token_manager
 from cortex_cli.utils import missing_packages, read_file, read_json
 
 # pylint: disable=too-many-lines
@@ -518,15 +520,15 @@
     '--refresh-period', default=REFRESH_PERIOD, show_default=True, help='How often to refresh tokens (in seconds).'
 )
 @click.option('--no-daemon', is_flag=True, default=False, help='Start token manager in foreground, not as daemon.')
 @click.option(
     '--no-refresh', is_flag=True, default=False, help='Login, but do not start token manager to refresh tokens.'
 )
 @click.option('-v', '--verbose', is_flag=True, help='Print extra information.')
-def login(  # pylint: disable=too-many-arguments, too-many-locals, too-many-branches
+def login(  # pylint: disable=too-many-arguments, too-many-locals, too-many-branches, too-many-statements
     config_file: str,
     username: str,
     password: str,
     refresh_period: int,
     no_daemon: bool,
     no_refresh: bool,
     verbose: bool,
@@ -549,23 +551,43 @@
             return
 
     # Login with username and password
     username = username or config.username or click.prompt('Username')
     if config.username:
         click.echo(f'Username: {username}')
     password = password or click.prompt('Password', hide_input=True)
+    tokens = None
 
-    try:
-        tokens = login_request(auth_server_url, realm, client_id, username, password)
-    except ConnectionError as exc:
-        raise click.ClickException(f'Authentication server at {auth_server_url} is not accessible') from exc
-    except Timeout as exc:
-        raise click.ClickException(f'Authentication server at {auth_server_url} is not responding') from exc
-    except ClientAuthenticationError as error:
-        raise click.ClickException(f'Failed to authenticate, {error}') from error
+    while tokens is None:
+        try:
+            tokens = login_request(auth_server_url, realm, client_id, username, password)
+        except ConnectionError as exc:
+            raise click.ClickException(f'Authentication server at {auth_server_url} is not accessible') from exc
+        except Timeout as exc:
+            raise click.ClickException(f'Authentication server at {auth_server_url} is not responding') from exc
+        except ClientAuthenticationError as error:
+            raise click.ClickException(f'Failed to authenticate, {error}') from error
+        except ClientAccountSetupError:
+            click.echo('Your account is not fully set up yet. You have to update your password.')
+            while True:
+                new_password = click.prompt('New password', hide_input=True)
+                cfm_password = click.prompt('Confirm new password', hide_input=True)
+                if new_password == cfm_password and new_password != password:
+                    break
+                if new_password == password:
+                    click.echo('New password must be different from old password')
+                else:
+                    click.echo('Confirmation must match the new password')
+            try:
+                update_password(auth_server_url, realm, username, password, new_password)
+                logger.info('Updated temporary password of %s', username)
+            except Exception as error:
+                raise click.ClickException(f'Failed to update password, {error}')
+            password = new_password
+            tokens = None
 
     logger.info('Logged in successfully as %s', username)
     save_tokens_file(tokens_file, tokens, auth_server_url)
     click.echo(
         f"""
 To use the tokens file with IQM Client or IQM Client-based software, set the environment variable:
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/models.py` & `iqm-cortex-cli-3.5/src/cortex_cli/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-3.5/src/cortex_cli/token_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `iqm-cortex-cli-3.4/src/cortex_cli/utils.py` & `iqm-cortex-cli-3.5/src/cortex_cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Utility functions for Cortex CLI.
 """
-import importlib.util
+import importlib.util  # type: ignore
 import json
 
 import click
 
 
 def read_file(filename: str) -> str:
     """Opens and reads the given file.
```

### Comparing `iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 3.4
+Version: 3.5
 Summary: CLI for executing quantum circuits
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-3.4/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 src/iqm_cortex_cli.egg-info/requires.txt
 src/iqm_cortex_cli.egg-info/top_level.txt
 tests/.pylintrc
 tests/__init__.py
 tests/auth_test.py
 tests/circuit_test.py
 tests/conftest.py
+tests/cortex_cli_auth_login_test.py
+tests/cortex_cli_auth_logout_test.py
+tests/cortex_cli_auth_status_test.py
+tests/cortex_cli_init_test.py
 tests/cortex_cli_test.py
 tests/token_manager_test.py
 tests/resources/config.json
 tests/resources/qasm_qubit_placement.json
 tests/resources/tokens.json
 tests/resources/valid_circuit.json
 tests/resources/valid_circuit.qasm
```

### Comparing `iqm-cortex-cli-3.4/tag-from-pipeline.sh` & `iqm-cortex-cli-3.5/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/tests/auth_test.py` & `iqm-cortex-cli-3.5/tests/auth_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `iqm-cortex-cli-3.4/tests/circuit_test.py` & `iqm-cortex-cli-3.5/tests/circuit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Tests for Cortex CLI's circuit commands
 """
-from importlib.metadata import version
+from importlib.metadata import version  # type: ignore
 from io import BytesIO, TextIOWrapper
 import json
 import os
 from uuid import uuid4
 
 from click.testing import CliRunner
 from iqm_client import Instruction
```

### Comparing `iqm-cortex-cli-3.4/tests/conftest.py` & `iqm-cortex-cli-3.5/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -112,23 +112,25 @@
 
 
 def prepare_tokens(
     access_token_lifetime: int,
     refresh_token_lifetime: int,
     previous_refresh_token: Optional[str] = None,
     status_code: int = 200,
+    response_data: Optional[dict] = None,
     **credentials,
 ) -> dict[str, str]:
     """Prepare tokens and set them to be returned for a token request.
 
     Args:
         access_token_lifetime: seconds from current time to access token expire time
         refresh_token_lifetime: seconds from current time to refresh token expire time
         previous_refresh_token: refresh token to be used in refresh request
         status_code: status code to return for token request
+        response_data: data to return for token request if other than the tokens
         credentials: dict containing auth_server_url, username and password
 
     Returns:
          Prepared tokens as a dict.
     """
     if previous_refresh_token is None:
         request_data = AuthRequest(
@@ -142,19 +144,22 @@
             client_id=CLIENT_ID, grant_type=GrantType.REFRESH, refresh_token=previous_refresh_token
         )
 
     tokens = {
         'access_token': make_token('Bearer', access_token_lifetime),
         'refresh_token': make_token('Refresh', refresh_token_lifetime),
     }
+    if response_data is None:
+        response_data = tokens
+
     when(requests).post(
         f'{credentials["auth_server_url"]}/realms/{REALM_NAME}/protocol/openid-connect/token',
         data=request_data.dict(exclude_none=True),
         timeout=AUTH_REQUESTS_TIMEOUT,
-    ).thenReturn(MockJsonResponse(status_code, tokens))
+    ).thenReturn(MockJsonResponse(status_code, response_data))
 
     return tokens
 
 
 def prepare_auth_server_urls(
     config_dict: dict[str, str], invalid_url: str = 'http://invalid.com', invalid_realm: str = 'invalid'
 ):
```

### Comparing `iqm-cortex-cli-3.4/tests/resources/tokens.json` & `iqm-cortex-cli-3.5/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/tests/resources/valid_circuit_2.json` & `iqm-cortex-cli-3.5/tests/resources/valid_circuit_2.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/tests/resources/valid_circuit_qasm_result.json` & `iqm-cortex-cli-3.5/tests/resources/valid_circuit_qasm_result.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.4/tests/token_manager_test.py` & `iqm-cortex-cli-3.5/tests/token_manager_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 IQM client developers
+# Copyright 2021-2023 IQM client developers
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `iqm-cortex-cli-3.4/tox.ini` & `iqm-cortex-cli-3.5/tox.ini`

 * *Files identical despite different names*

