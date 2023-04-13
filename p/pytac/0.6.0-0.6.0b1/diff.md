# Comparing `tmp/pytac-0.6.0.tar.gz` & `tmp/pytac-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytac-0.6.0.tar", last modified: Thu Apr 13 10:22:14 2023, max compression
+gzip compressed data, was "pytac-0.6.0b1.tar", last modified: Wed Apr 12 14:55:22 2023, max compression
```

## Comparing `pytac-0.6.0.tar` & `pytac-0.6.0b1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.674622 pytac-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-13 10:22:05.000000 pytac-0.6.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.650622 pytac-0.6.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 10:22:05.000000 pytac-0.6.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 10:22:05.000000 pytac-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 10:22:05.000000 pytac-0.6.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 10:22:05.000000 pytac-0.6.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 10:22:05.000000 pytac-0.6.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 10:22:05.000000 pytac-0.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 10:22:05.000000 pytac-0.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 10:22:05.000000 pytac-0.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-13 10:22:05.000000 pytac-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-04-13 10:22:14.674622 pytac-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-13 10:22:05.000000 pytac-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/images/control-structure.png
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/explanations/docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/explanations/what-is-pytac.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.658622 pytac-0.6.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/tutorials/basic-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-13 10:22:05.000000 pytac-0.6.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-13 10:22:05.000000 pytac-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:22:14.674622 pytac-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.662622 pytac-0.6.0/src/pytac/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/cothread_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/cs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/src/pytac/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.662622 pytac-0.6.0/src/pytac/data/DIAD/
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIAD/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.662622 pytac-0.6.0/src/pytac/data/DIADSP/
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADSP/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.662622 pytac-0.6.0/src/pytac/data/DIADTHz/
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/DIADTHz/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.666622 pytac-0.6.0/src/pytac/data/I04/
--rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.666622 pytac-0.6.0/src/pytac/data/I04SP/
--rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04SP/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.666622 pytac-0.6.0/src/pytac/data/I04THz/
--rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/I04THz/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.666622 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/SRI0913_MOGA/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.670622 pytac-0.6.0/src/pytac/data/VMX/
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMX/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.670622 pytac-0.6.0/src/pytac/data/VMXSP/
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXSP/unitconv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.670622 pytac-0.6.0/src/pytac/data/VMXTHz/
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/simple_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/uc_pchip_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/uc_poly_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data/VMXTHz/unitconv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/load_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 10:22:05.000000 pytac-0.6.0/src/pytac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.662622 pytac-0.6.0/src/pytac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 10:22:14.000000 pytac-0.6.0/src/pytac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.674622 pytac-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.654622 pytac-0.6.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.674622 pytac-0.6.0/tests/data/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/data/dummy/elements.csv
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/data/dummy/epics_devices.csv
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/data/dummy/families.csv
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_cothread_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_epics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_invalid_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 10:22:05.000000 pytac-0.6.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:22:14.674622 pytac-0.6.0/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-04-13 10:22:05.000000 pytac-0.6.0/utils/load_mml.m
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-13 10:22:05.000000 pytac-0.6.0/utils/load_unitconv.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.789343 pytac-0.6.0b1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 14:55:14.000000 pytac-0.6.0b1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-12 14:55:14.000000 pytac-0.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-04-12 14:55:22.813344 pytac-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-12 14:55:14.000000 pytac-0.6.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/control-structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/explanations/docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/explanations/what-is-pytac.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/tutorials/basic-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-12 14:55:14.000000 pytac-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:55:22.813344 pytac-0.6.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/cothread_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/cs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/src/pytac/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac/data/DIAD/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/DIADSP/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/DIADTHz/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/I04/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/I04SP/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/I04THz/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/VMX/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/src/pytac/data/VMXSP/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/src/pytac/data/VMXTHz/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/unitconv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/load_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/tests/data/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_cothread_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_invalid_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-04-12 14:55:14.000000 pytac-0.6.0b1/utils/load_mml.m
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-12 14:55:14.000000 pytac-0.6.0b1/utils/load_unitconv.m
```

### Comparing `pytac-0.6.0/.devcontainer/devcontainer.json` & `pytac-0.6.0b1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/CONTRIBUTING.rst` & `pytac-0.6.0b1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/actions/install_requirements/action.yml` & `pytac-0.6.0b1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/dependabot.yml` & `pytac-0.6.0b1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/pages/make_switcher.py` & `pytac-0.6.0b1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/workflows/code.yml` & `pytac-0.6.0b1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/workflows/docs.yml` & `pytac-0.6.0b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/workflows/docs_clean.yml` & `pytac-0.6.0b1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.github/workflows/linkcheck.yml` & `pytac-0.6.0b1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.gitignore` & `pytac-0.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/.vscode/launch.json` & `pytac-0.6.0b1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/Dockerfile` & `pytac-0.6.0b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/LICENSE` & `pytac-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/PKG-INFO` & `pytac-0.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytac
-Version: 0.6.0
+Version: 0.6.0b1
 Summary: Python Toolkit for Accelerator Controls
 Author-email: Will Rogers <diamhighlvlapps@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytac-0.6.0/README.rst` & `pytac-0.6.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/conf.py` & `pytac-0.6.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `pytac-0.6.0b1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/explanations/decisions.rst` & `pytac-0.6.0b1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/build-docs.rst` & `pytac-0.6.0b1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/lint.rst` & `pytac-0.6.0b1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/make-release.rst` & `pytac-0.6.0b1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/pin-requirements.rst` & `pytac-0.6.0b1/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/test-container.rst` & `pytac-0.6.0b1/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/how-to/update-tools.rst` & `pytac-0.6.0b1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/index.rst` & `pytac-0.6.0b1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/reference/standards.rst` & `pytac-0.6.0b1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/developer/tutorials/dev-install.rst` & `pytac-0.6.0b1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/images/control-structure.png` & `pytac-0.6.0b1/docs/images/control-structure.png`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/images/dls-favicon.ico` & `pytac-0.6.0b1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/images/dls-logo.svg` & `pytac-0.6.0b1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/index.rst` & `pytac-0.6.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/explanations/docs-structure.rst` & `pytac-0.6.0b1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/explanations/what-is-pytac.rst` & `pytac-0.6.0b1/docs/user/explanations/what-is-pytac.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/index.rst` & `pytac-0.6.0b1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/reference/api.rst` & `pytac-0.6.0b1/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/tutorials/basic-tutorial.rst` & `pytac-0.6.0b1/docs/user/tutorials/basic-tutorial.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/docs/user/tutorials/installation.rst` & `pytac-0.6.0b1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/pyproject.toml` & `pytac-0.6.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/__init__.py` & `pytac-0.6.0b1/src/pytac/__init__.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/cothread_cs.py` & `pytac-0.6.0b1/src/pytac/cothread_cs.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/cs.py` & `pytac-0.6.0b1/src/pytac/cs.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIAD/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADSP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/DIADTHz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04SP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/I04THz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/elements.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/families.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/SRI0913_MOGA/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMX/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXSP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data/VMXTHz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/data_source.py` & `pytac-0.6.0b1/src/pytac/data_source.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/device.py` & `pytac-0.6.0b1/src/pytac/device.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/element.py` & `pytac-0.6.0b1/src/pytac/element.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/exceptions.py` & `pytac-0.6.0b1/src/pytac/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/lattice.py` & `pytac-0.6.0b1/src/pytac/lattice.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/load_csv.py` & `pytac-0.6.0b1/src/pytac/load_csv.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/units.py` & `pytac-0.6.0b1/src/pytac/units.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac/utils.py` & `pytac-0.6.0b1/src/pytac/utils.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/src/pytac.egg-info/PKG-INFO` & `pytac-0.6.0b1/src/pytac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytac
-Version: 0.6.0
+Version: 0.6.0b1
 Summary: Python Toolkit for Accelerator Controls
 Author-email: Will Rogers <diamhighlvlapps@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytac-0.6.0/src/pytac.egg-info/SOURCES.txt` & `pytac-0.6.0b1/src/pytac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/conftest.py` & `pytac-0.6.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_cothread_cs.py` & `pytac-0.6.0b1/tests/test_cothread_cs.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_data_source.py` & `pytac-0.6.0b1/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_device.py` & `pytac-0.6.0b1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_element.py` & `pytac-0.6.0b1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_epics.py` & `pytac-0.6.0b1/tests/test_epics.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_invalid_classes.py` & `pytac-0.6.0b1/tests/test_invalid_classes.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_lattice.py` & `pytac-0.6.0b1/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_load.py` & `pytac-0.6.0b1/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_machine.py` & `pytac-0.6.0b1/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_units.py` & `pytac-0.6.0b1/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/tests/test_utils.py` & `pytac-0.6.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/utils/load_mml.m` & `pytac-0.6.0b1/utils/load_mml.m`

 * *Files identical despite different names*

### Comparing `pytac-0.6.0/utils/load_unitconv.m` & `pytac-0.6.0b1/utils/load_unitconv.m`

 * *Files identical despite different names*

