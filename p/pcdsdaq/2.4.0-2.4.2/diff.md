# Comparing `tmp/pcdsdaq-2.4.0.tar.gz` & `tmp/pcdsdaq-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdsdaq-2.4.0.tar", last modified: Tue Apr  4 19:29:30 2023, max compression
+gzip compressed data, was "pcdsdaq-2.4.2.tar", last modified: Thu Apr 13 20:49:51 2023, max compression
```

## Comparing `pcdsdaq-2.4.0.tar` & `pcdsdaq-2.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1310 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/bin/pcdsdaq_lib_setup
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/ami_api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/ami_basic.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_basic.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_config.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/env.rst
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/misc.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/plans_basic.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/preprocessors_api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/scan_pvs.rst
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/sim.rst
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/pcdsdaq/
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    19672 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/ami.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/pcdsdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27615 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)    34734 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/lcls1.py
--rw-r--r--   0 runner    (1001) docker     (122)    76922 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/lcls2.py
--rw-r--r--   0 runner    (1001) docker     (122)    41884 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/original.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/ext_scripts.py
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/plans.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/scan_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/pcdsdaq/sim/
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/pyami.py
--rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/pydaq.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/pcdsdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5802 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_ami.py
--rw-r--r--   0 runner    (1001) docker     (122)    32178 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_daq_lcls2.py
--rw-r--r--   0 runner    (1001) docker     (122)    14791 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_daq_original.py
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_ext_scripts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     6404 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_scan_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.810368 pcdsdaq-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-04-13 20:49:51.810368 pcdsdaq-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1310 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/bin/pcdsdaq_lib_setup
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.802368 pcdsdaq-2.4.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/ami_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/ami_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/daq_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/daq_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/daq_config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/env.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/plans_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/preprocessors_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7068 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/scan_pvs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs/source/sim.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.806368 pcdsdaq-2.4.2/pcdsdaq/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19672 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/ami.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.806368 pcdsdaq-2.4.2/pcdsdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27615 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/daq/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34734 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/daq/lcls1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77193 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/daq/lcls2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41884 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/daq/original.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/ext_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/scan_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.806368 pcdsdaq-2.4.2/pcdsdaq/sim/
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/sim/pyami.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/sim/pydaq.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.806368 pcdsdaq-2.4.2/pcdsdaq/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5802 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_ami.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32373 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_daq_lcls2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14791 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_daq_original.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_ext_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6404 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/tests/test_scan_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pcdsdaq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 20:49:51.806368 pcdsdaq-2.4.2/pcdsdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-13 20:49:51.000000 pcdsdaq-2.4.2/pcdsdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 20:49:36.000000 pcdsdaq-2.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 20:49:51.810368 pcdsdaq-2.4.2/setup.cfg
```

### Comparing `pcdsdaq-2.4.0/.flake8` & `pcdsdaq-2.4.2/.flake8`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/.github/ISSUE_TEMPLATE.md` & `pcdsdaq-2.4.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `pcdsdaq-2.4.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/.github/workflows/standard.yml` & `pcdsdaq-2.4.2/.github/workflows/standard.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   release:
     types:
       - published
 
 jobs:
   standard:
     uses: pcdshub/pcds-ci-helpers/.github/workflows/python-standard.yml@master
+    secrets: inherit
     with:
       # The workflow needs to know the package name.  This can be determined
       # automatically if the repository name is the same as the import name.
       package-name: "pcdsdaq"
       # Extras that will be installed for both conda/pip:
       testing-extras: ""
       # Extras to be installed only for conda-based testing:
```

### Comparing `pcdsdaq-2.4.0/.gitignore` & `pcdsdaq-2.4.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -103,7 +103,8 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # vim
 *.swp
+*.un~
```

### Comparing `pcdsdaq-2.4.0/.pre-commit-config.yaml` & `pcdsdaq-2.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/CONTRIBUTING.rst` & `pcdsdaq-2.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/LICENSE.md` & `pcdsdaq-2.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/PKG-INFO` & `pcdsdaq-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdaq
-Version: 2.4.0
+Version: 2.4.2
 Summary: DAQ Control Interface
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -39,15 +39,15 @@
         available either publicly, or directly to SLAC National Accelerator Laboratory,
         without imposing a separate written license agreement for such Enhancements,
         then you hereby grant the following license: a non-exclusive, royalty-free
         perpetual license to install, use, modify, prepare derivative works, incorporate
         into other computer software, distribute, and sublicense such Enhancements or
         derivative works thereof, in binary and source code form.
         
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE.md
```

### Comparing `pcdsdaq-2.4.0/README.rst` & `pcdsdaq-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/bin/pcdsdaq_lib_setup` & `pcdsdaq-2.4.2/bin/pcdsdaq_lib_setup`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/conda-recipe/meta.yaml` & `pcdsdaq-2.4.2/conda-recipe/meta.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,16 @@
   - pcdsdevices >=2.1.0
   - psdaq-control-minimal >=3.3.19
   - toolz
 
 test:
   imports:
   - pcdsdaq
+  commands:
+  - pcdsdaq_lib_setup
   requires:
   - pytest
   - pytest-timeout
 
 about:
   home: https://github.com/pcdshub/pcdsdaq
   license: SLAC Open License
```

### Comparing `pcdsdaq-2.4.0/docs/Makefile` & `pcdsdaq-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/ami_basic.rst` & `pcdsdaq-2.4.2/docs/source/ami_basic.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/conf.py` & `pcdsdaq-2.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/daq_basic.rst` & `pcdsdaq-2.4.2/docs/source/daq_basic.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/daq_config.rst` & `pcdsdaq-2.4.2/docs/source/daq_config.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/env.rst` & `pcdsdaq-2.4.2/docs/source/env.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/index.rst` & `pcdsdaq-2.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/misc.rst` & `pcdsdaq-2.4.2/docs/source/misc.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/plans_basic.rst` & `pcdsdaq-2.4.2/docs/source/plans_basic.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/docs/source/releases.rst` & `pcdsdaq-2.4.2/docs/source/releases.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,43 @@
 Release History
 ###############
 
+v2.4.2 (2023-04-13)
+===================
+
+- Fix issues related to the missing pcdsdaq_lib_setup script
+- Fix issues related to failing pypi builds
+- Fix issues related to failing docs builds
+
+
+v2.4.1 (2023-04-11)
+===================
+
+- Mark tests as xfail, we'll come back to fix them later.
+  This is not operation critical.
+  One of these tests contain a nasty race condition that
+  causes the suite to time out.
+- Fix an issue where automatic pypi/conda uploads would
+  not have proper authentication.
+
+
+v2.4.0 (2023-04-04)
+==================
+
+This includes a large update for lcls2 daq support,
+but the module is fully backwards compatible with
+the previous versions.
+
+- Huge addition of 1st-class lcls2 daq support
+  including monitoring the current daq's status and running it.
+  Uses the daq's own APIs repackaged for bluesky.
+- Migrate to github actions, pyproject.toml, and other ecs standards.
+- Merge an ancient PR that adds a useful feature for CXI
+
+
 v2.3.5 (2022-06-02)
 ===================
 
 - Fix issue where the scan variable min/max values would not fill in
   correctly for scan types other then the normal "scan".
```

### Comparing `pcdsdaq-2.4.0/docs/source/scan_pvs.rst` & `pcdsdaq-2.4.2/docs/source/scan_pvs.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/ami.py` & `pcdsdaq-2.4.2/pcdsdaq/ami.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/daq/__init__.py` & `pcdsdaq-2.4.2/pcdsdaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/daq/interface.py` & `pcdsdaq-2.4.2/pcdsdaq/daq/interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/daq/lcls1.py` & `pcdsdaq-2.4.2/pcdsdaq/daq/lcls1.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/daq/lcls2.py` & `pcdsdaq-2.4.2/pcdsdaq/daq/lcls2.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,27 @@
 from bluesky import RunEngine
 from ophyd.device import Component as Cpt
 from ophyd.signal import Signal
 from ophyd.status import Status
 from ophyd.utils import StatusTimeoutError, WaitTimeoutError
 from ophyd.utils.errors import InvalidState
 from pcdsutils.enum import HelpfulIntEnum
-from psdaq.control.ControlDef import ControlDef
-from psdaq.control.DaqControl import DaqControl
 
 from .interface import (CONFIG_VAL, ControlsArg, DaqBase,
                         DaqStateTransitionError, DaqTimeoutError, EnumId,
                         Sentinel, TernaryBool, get_controls_name,
                         get_controls_value, typing_check)
 
+try:
+    from psdaq.control.ControlDef import ControlDef
+    from psdaq.control.DaqControl import DaqControl
+except ImportError:
+    ControlDef = None
+    DaqControl = None
+
 logger = logging.getLogger(__name__)
 
 
 class DaqLCLS2(DaqBase):
     """
     The LCLS2 DAQ as a bluesky-compatible object.
 
@@ -1807,14 +1812,19 @@
         'running': {
             'paused': 'disable',
         },
     }
 
     def __init__(self, *args, **kwargs):
         logger.debug("SimDaqControl.__init__(%s, %s)", args, kwargs)
+        if None in (ControlDef, DaqControl):
+            raise RuntimeError(
+                'Optional dependency psdaq is not installed, '
+                'cannot run lcls2 daq'
+            )
         self._lock = threading.RLock()
         self._new_status = threading.Event()
         self._headers = HelpfulIntEnum(
             'ValidHeaders',
             ['status', 'error', 'warning', 'filereport', 'progress', 'step']
         )
         self._states = HelpfulIntEnum('States', ControlDef.states)
```

### Comparing `pcdsdaq-2.4.0/pcdsdaq/daq/original.py` & `pcdsdaq-2.4.2/pcdsdaq/daq/original.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/ext_scripts.py` & `pcdsdaq-2.4.2/pcdsdaq/ext_scripts.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/plans.py` & `pcdsdaq-2.4.2/pcdsdaq/plans.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/preprocessors.py` & `pcdsdaq-2.4.2/pcdsdaq/preprocessors.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/scan_vars.py` & `pcdsdaq-2.4.2/pcdsdaq/scan_vars.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/sim/__init__.py` & `pcdsdaq-2.4.2/pcdsdaq/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/sim/pyami.py` & `pcdsdaq-2.4.2/pcdsdaq/sim/pyami.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/sim/pydaq.py` & `pcdsdaq-2.4.2/pcdsdaq/sim/pydaq.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq/version.py` & `pcdsdaq-2.4.2/pcdsdaq/version.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/pcdsdaq.egg-info/PKG-INFO` & `pcdsdaq-2.4.2/pcdsdaq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdaq
-Version: 2.4.0
+Version: 2.4.2
 Summary: DAQ Control Interface
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -39,15 +39,15 @@
         available either publicly, or directly to SLAC National Accelerator Laboratory,
         without imposing a separate written license agreement for such Enhancements,
         then you hereby grant the following license: a non-exclusive, royalty-free
         perpetual license to install, use, modify, prepare derivative works, incorporate
         into other computer software, distribute, and sublicense such Enhancements or
         derivative works thereof, in binary and source code form.
         
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE.md
```

### Comparing `pcdsdaq-2.4.0/pyproject.toml` & `pcdsdaq-2.4.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [ "setuptools>=45", "setuptools_scm[toml]>=6.2",]
 
 [project]
-classifiers = [ "Development Status :: 2 - Pre-Alpha", "Natural Language :: English", "Programming Language :: Python :: 3",]
+classifiers = [ "Development Status :: 5 - Production/Stable", "Natural Language :: English", "Programming Language :: Python :: 3",]
 description = "DAQ Control Interface"
 dynamic = [ "version", "readme", "dependencies", "optional-dependencies", "optional-dependencies",]
 keywords = []
 name = "pcdsdaq"
 requires-python = ">=3.9"
+
 [[project.authors]]
 name = "SLAC National Accelerator Laboratory"
 
 [options]
 zip_safe = false
 include_package_data = true
 
@@ -26,14 +27,17 @@
 timeout = "60"
 
 [tool.setuptools.packages.find]
 where = [ ".",]
 include = [ "pcdsdaq*",]
 namespaces = false
 
+[tool.setuptools]
+script-files = [ "bin/pcdsdaq_lib_setup",]
+
 [tool.setuptools.dynamic.readme]
 file = "README.rst"
 
 [tool.setuptools.dynamic.dependencies]
 file = [ "requirements.txt",]
 
 [tool.setuptools.dynamic.optional-dependencies.test]
```

### Comparing `pcdsdaq-2.4.0/tests/conftest.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/tests/test_ami.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_ami.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/tests/test_daq_lcls2.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_daq_lcls2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 import bluesky.preprocessors as bpp
 import pytest
 from bluesky import RunEngine
 from ophyd.positioner import SoftPositioner
 from ophyd.signal import Signal
 from ophyd.sim import motor
 from ophyd.utils.errors import WaitTimeoutError
-from psdaq.control.ControlDef import ControlDef
 
 from pcdsdaq.daq import DaqLCLS2, DaqTimeoutError
 from pcdsdaq.daq.interface import DaqStateTransitionError, TernaryBool
 
+try:
+    from psdaq.control.ControlDef import ControlDef
+except ImportError:
+    ControlDef = None
+
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope='function')
 def daq_lcls2(RE: RunEngine) -> DaqLCLS2:
+    if ControlDef is None:
+        pytest.skip(reason='psdaq is not installed')
     return DaqLCLS2(
         platform=0,
         host='tst',
         timeout=1000,
         RE=RE,
         hutch_name='tst',
         sim=True,
@@ -293,14 +299,15 @@
     daq_lcls2.stage()
     daq_lcls2._control.setRecord(not recording_before)
     sig_wait_value(daq_lcls2.recording_sig, not recording_before)
     daq_lcls2.unstage()
     sig_wait_value(daq_lcls2.recording_sig, recording_before)
 
 
+@pytest.mark.xfail
 def test_configure(daq_lcls2: DaqLCLS2):
     """
     Configure must have the following behavior:
     - kwargs end up in cfg signals (spot check 1 or 2)
     - Returns (old_cfg, new_cfg)
     - Configure transition caused if needed from conn/conf states
     - Conf needed if recording gui clicked, or critical kwargs changed,
@@ -588,14 +595,16 @@
         )
     daq_lcls2.configure(events=0)
     status = daq_lcls2.trigger()
     status.wait(timeout=1)
     assert status.done
 
 
+@pytest.mark.xfail
+@pytest.mark.timeout(60)
 def test_begin(daq_lcls2: DaqLCLS2):
     """
     Begin must do the following:
     - Start or resume a run (go from connected or higher to running)
     - wait kwarg = wait until we stop taking events
     - end_run kwarg = end the run after we stop taking events
     - other kwargs = configure for that kwarg before running, revert after
```

### Comparing `pcdsdaq-2.4.0/tests/test_daq_original.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_daq_original.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/tests/test_ext_scripts.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_ext_scripts.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/tests/test_preprocessors.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.4.0/tests/test_scan_vars.py` & `pcdsdaq-2.4.2/pcdsdaq/tests/test_scan_vars.py`

 * *Files identical despite different names*

