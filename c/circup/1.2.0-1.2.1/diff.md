# Comparing `tmp/circup-1.2.0.tar.gz` & `tmp/circup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circup-1.2.0.tar", last modified: Mon Apr 10 19:30:05 2023, max compression
+gzip compressed data, was "circup-1.2.1.tar", last modified: Thu Apr 13 00:48:10 2023, max compression
```

## Comparing `circup-1.2.0.tar` & `circup-1.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-10 19:29:52.000000 circup-1.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-10 19:29:52.000000 circup-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-10 19:29:52.000000 circup-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:29:52.000000 circup-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 19:29:52.000000 circup-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 19:29:52.000000 circup-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-10 19:29:52.000000 circup-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-10 19:29:52.000000 circup-1.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/CODE_OF_CONDUCT.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-10 19:29:52.000000 circup-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/CONTRIBUTING.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:29:52.000000 circup-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-10 19:30:05.158273 circup-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-04-10 19:29:52.000000 circup-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.150273 circup-1.2.0/circup/
--rw-r--r--   0 runner    (1001) docker     (123)    61068 2023-04-10 19:29:52.000000 circup-1.2.0/circup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/circup/config/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-10 19:29:52.000000 circup-1.2.0/circup/config/bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:29:52.000000 circup-1.2.0/circup/config/bundle_config.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/circup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 19:30:05.000000 circup-1.2.0/circup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.154273 circup-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:29:52.000000 circup-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:29:52.000000 circup-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-10 19:29:52.000000 circup-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-10 19:29:52.000000 circup-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-04-10 19:29:52.000000 circup-1.2.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/docs/logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 19:29:52.000000 circup-1.2.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 19:29:52.000000 circup-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 19:29:52.000000 circup-1.2.0/requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:30:05.158273 circup-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-10 19:29:52.000000 circup-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/bad_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bad_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bundle.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/bundle.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 19:29:52.000000 circup-1.2.0/tests/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/device.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:30:05.158273 circup-1.2.0/tests/dir_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:29:52.000000 circup-1.2.0/tests/dir_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 19:29:52.000000 circup-1.2.0/tests/dir_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-10 19:29:52.000000 circup-1.2.0/tests/import_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module_cp7.mpy
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/local_module_cp7.mpy.license
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_exists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_exists.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_missing.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/mount_missing.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-10 19:29:52.000000 circup-1.2.0/tests/remote_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config_local.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_bundle_config_local.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    40224 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_circup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_module.mpy
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:29:52.000000 circup-1.2.0/tests/test_module.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.956197 circup-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.944197 circup-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-13 00:47:59.000000 circup-1.2.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 00:47:59.000000 circup-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.944197 circup-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-13 00:47:59.000000 circup-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-13 00:47:59.000000 circup-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 00:47:59.000000 circup-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 00:47:59.000000 circup-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-13 00:47:59.000000 circup-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-13 00:47:59.000000 circup-1.2.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/CODE_OF_CONDUCT.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-13 00:47:59.000000 circup-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/CONTRIBUTING.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-13 00:47:59.000000 circup-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.944197 circup-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-13 00:47:59.000000 circup-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 00:47:59.000000 circup-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 00:47:59.000000 circup-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-13 00:48:10.956197 circup-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-04-13 00:47:59.000000 circup-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.944197 circup-1.2.1/circup/
+-rw-r--r--   0 runner    (1001) docker     (123)    61088 2023-04-13 00:47:59.000000 circup-1.2.1/circup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.948197 circup-1.2.1/circup/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 00:47:59.000000 circup-1.2.1/circup/config/bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 00:47:59.000000 circup-1.2.1/circup/config/bundle_config.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.948197 circup-1.2.1/circup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 00:48:10.000000 circup-1.2.1/circup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.948197 circup-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.948197 circup-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-13 00:47:59.000000 circup-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 00:47:59.000000 circup-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-13 00:47:59.000000 circup-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 00:47:59.000000 circup-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-04-13 00:47:59.000000 circup-1.2.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/docs/logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-13 00:47:59.000000 circup-1.2.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 00:47:59.000000 circup-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 00:47:59.000000 circup-1.2.1/requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 00:48:10.956197 circup-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-13 00:47:59.000000 circup-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.956197 circup-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:59.000000 circup-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.956197 circup-1.2.1/tests/bad_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:59.000000 circup-1.2.1/tests/bad_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 00:47:59.000000 circup-1.2.1/tests/bad_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 00:47:59.000000 circup-1.2.1/tests/bad_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 00:47:59.000000 circup-1.2.1/tests/bundle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/bundle.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 00:47:59.000000 circup-1.2.1/tests/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/device.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:48:10.956197 circup-1.2.1/tests/dir_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:47:59.000000 circup-1.2.1/tests/dir_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 00:47:59.000000 circup-1.2.1/tests/dir_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 00:47:59.000000 circup-1.2.1/tests/import_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 00:47:59.000000 circup-1.2.1/tests/local_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 00:47:59.000000 circup-1.2.1/tests/local_module_cp7.mpy
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/local_module_cp7.mpy.license
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 00:47:59.000000 circup-1.2.1/tests/mount_exists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/mount_exists.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-13 00:47:59.000000 circup-1.2.1/tests/mount_missing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/mount_missing.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 00:47:59.000000 circup-1.2.1/tests/remote_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_bundle_config_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_bundle_config_local.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    40224 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_circup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_module.mpy
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:47:59.000000 circup-1.2.1/tests/test_module.mpy.license
```

### Comparing `circup-1.2.0/.github/ISSUE_TEMPLATE.md` & `circup-1.2.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `circup-1.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.github/workflows/build.yml` & `circup-1.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.github/workflows/release.yml` & `circup-1.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.gitignore` & `circup-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.pre-commit-config.yaml` & `circup-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/.pylintrc` & `circup-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/CODE_OF_CONDUCT.rst` & `circup-1.2.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/CONTRIBUTING.rst` & `circup-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/LICENSE` & `circup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/LICENSES/CC-BY-4.0.txt` & `circup-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/LICENSES/MIT.txt` & `circup-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/LICENSES/Unlicense.txt` & `circup-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/PKG-INFO` & `circup-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `circup-1.2.0/README.rst` & `circup-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/circup/__init__.py` & `circup-1.2.1/circup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1307,15 +1307,17 @@
 @click.option(
     "-r",
     "--requirement",
     type=click.Path(exists=True, dir_okay=False),
     help="specify a text file to install all modules listed in the text file."
     " Typically requirements.txt.",
 )
-@click.option("--auto", "-a", help="Install the modules imported in code.py.")
+@click.option(
+    "--auto", "-a", is_flag=True, help="Install the modules imported in code.py."
+)
 @click.option(
     "--auto-file",
     default=None,
     help="Specify the name of a file on the board to read for auto install."
     " Also accepts an absolute path or a local ./ path.",
 )
 @click.pass_context
```

### Comparing `circup-1.2.0/circup.egg-info/PKG-INFO` & `circup-1.2.1/circup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `circup-1.2.0/circup.egg-info/SOURCES.txt` & `circup-1.2.1/circup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/docs/_static/favicon.ico` & `circup-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/docs/conf.py` & `circup-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/docs/logo.png` & `circup-1.2.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/requirements.txt` & `circup-1.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/setup.py` & `circup-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/tests/bundle.json` & `circup-1.2.1/tests/bundle.json`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/tests/mount_exists.txt` & `circup-1.2.1/tests/mount_exists.txt`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/tests/test_circup.py` & `circup-1.2.1/tests/test_circup.py`

 * *Files identical despite different names*

### Comparing `circup-1.2.0/tests/test_module.mpy` & `circup-1.2.1/tests/test_module.mpy`

 * *Files identical despite different names*

