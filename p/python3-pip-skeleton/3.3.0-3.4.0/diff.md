# Comparing `tmp/python3-pip-skeleton-3.3.0.tar.gz` & `tmp/python3-pip-skeleton-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-pip-skeleton-3.3.0.tar", last modified: Wed Nov 16 12:19:24 2022, max compression
+gzip compressed data, was "python3-pip-skeleton-3.4.0.tar", last modified: Thu Apr 13 08:15:16 2023, max compression
```

## Comparing `python3-pip-skeleton-3.3.0.tar` & `python3-pip-skeleton-3.4.0.tar`

### file list

```diff
@@ -1,92 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.855632 python3-pip-skeleton-3.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.855632 python3-pip-skeleton-3.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     3023 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6551 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5557 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    99678 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12006 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (121)    21331 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.859632 python3-pip-skeleton-3.3.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/explanations/docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/explanations/skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/explanations/why-pre-commit.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/explanations/why-src.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/explanations/why-use-skeleton.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/how-to/excalidraw.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/how-to/existing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/how-to/pypi.rst
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/how-to/update.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/docs/user/tutorials/new.rst
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.855632 python3-pip-skeleton-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8627 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-16 12:19:24.000000 python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:19:24.863632 python3-pip-skeleton-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/tests/test_adopt.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-16 12:19:14.000000 python3-pip-skeleton-3.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.538402 python3-pip-skeleton-3.4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/explanations/skeleton.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0003-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0004-why-src.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0005-pyproject-toml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0006-setuptools-scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0007-dev-dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0008-use-tox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0009-sphinx-theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0010-vscode-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0011-requirements-txt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0012-containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/why-use-skeleton.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/excalidraw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/existing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/maintain-your-own-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/tutorials/new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.538402 python3-pip-skeleton-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/tests/test_adopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/tests/test_cli.py
```

### Comparing `python3-pip-skeleton-3.3.0/.devcontainer/Dockerfile` & `python3-pip-skeleton-3.4.0/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
 FROM python:3.11 as build
 
-ARG PIP_OPTIONS
+ARG PIP_OPTIONS=.
 
 # Add any system dependencies for the developer/build environment here e.g.
 # RUN apt-get update && apt-get upgrade -y && \
 #     apt-get install -y --no-install-recommends \
 #     desired-packages \
 #     && rm -rf /var/lib/apt/lists/*
```

### Comparing `python3-pip-skeleton-3.3.0/.devcontainer/devcontainer.json` & `python3-pip-skeleton-3.4.0/.devcontainer/devcontainer.json`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,52 @@
-// For format details, see https://aka.ms/devcontainer.json
+// For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
-        "dockerfile": "Dockerfile",
+        "dockerfile": "../Dockerfile",
         "target": "build",
         // Only upgrade pip, we will install the project below
         "args": {
             "PIP_OPTIONS": "--upgrade pip"
         }
     },
     "remoteEnv": {
         "DISPLAY": "${localEnv:DISPLAY}"
     },
+    // Add the URLs of features you want added when the container is built.
+    "features": {
+        "ghcr.io/devcontainers/features/common-utils:1": {
+            "username": "none",
+            "upgradePackages": false
+        }
+    },
     // Set *default* container specific settings.json values on container create.
     "settings": {
         "python.defaultInterpreterPath": "/venv/bin/python"
     },
-    // Add the IDs of extensions you want installed when the container is created.
-    "extensions": [
-        "ms-python.python",
-        "ms-python.vscode-pylance"
-    ],
+    "customizations": {
+        "vscode": {
+            // Add the IDs of extensions you want installed when the container is created.
+            "extensions": [
+                "ms-python.python",
+                "tamasfe.even-better-toml",
+                "redhat.vscode-yaml",
+                "ryanluker.vscode-coverage-gutters"
+            ]
+        }
+    },
     // Make sure the files we are mapping into the container exist on the host
     "initializeCommand": "bash -c 'for i in $HOME/.inputrc; do [ -f $i ] || touch $i; done'",
     "runArgs": [
         "--net=host",
-        "--security-opt=label=type:container_runtime_t",
-        "-v=${localEnv:HOME}/.ssh:/root/.ssh",
-        "-v=${localEnv:HOME}/.inputrc:/root/.inputrc"
+        "--security-opt=label=type:container_runtime_t"
     ],
     "mounts": [
+        "source=${localEnv:HOME}/.ssh,target=/root/.ssh,type=bind",
+        "source=${localEnv:HOME}/.inputrc,target=/root/.inputrc,type=bind",
         // map in home directory - not strictly necessary but useful
         "source=${localEnv:HOME},target=${localEnv:HOME},type=bind,consistency=cached"
     ],
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
```

### Comparing `python3-pip-skeleton-3.3.0/.github/CONTRIBUTING.rst` & `python3-pip-skeleton-3.4.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.github/actions/install_requirements/action.yml` & `python3-pip-skeleton-3.4.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.github/dependabot.yml` & `python3-pip-skeleton-3.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.github/pages/make_switcher.py` & `python3-pip-skeleton-3.4.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.github/workflows/code.yml` & `python3-pip-skeleton-3.4.0/.github/workflows/code.yml`

 * *Files 8% similar despite different names*

```diff
@@ -98,15 +98,15 @@
       - name: Upload sdist and wheel as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist
 
       - name: Check for packaging errors
-        run: pipx run twine check dist/*
+        run: pipx run twine check --strict dist/*
 
       - name: Install python packages
         uses: ./.github/actions/install_requirements
         with:
           python_version: ${{env.CONTAINER_PYTHON}}
           requirements_file: requirements.txt
           install_options: dist/*.whl
@@ -130,15 +130,15 @@
       # image names must be all lower case
       - name: Generate image repo name
         run: echo IMAGE_REPOSITORY=ghcr.io/$(tr '[:upper:]' '[:lower:]' <<< "${{ github.repository }}") >> $GITHUB_ENV
 
       - name: Download wheel and lockfiles
         uses: actions/download-artifact@v3
         with:
-          path: .devcontainer
+          path: artifacts/
 
       - name: Log in to GitHub Docker Registry
         if: github.event_name != 'pull_request'
         uses: docker/login-action@v2
         with:
           registry: ghcr.io
           username: ${{ github.actor }}
@@ -161,46 +161,51 @@
         uses: docker/build-push-action@v3
         with:
           build-args: |
             PIP_OPTIONS=-r lockfiles/requirements.txt dist/*.whl
           push: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
           load: ${{ ! (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) }}
           tags: ${{ steps.meta.outputs.tags }}
-          context: .devcontainer
+          labels: ${{ steps.meta.outputs.labels }}
+          context: artifacts/
+          file: ./Dockerfile
           # If you have a long docker build, uncomment the following to turn on caching
           # For short build times this makes it a little slower
           #cache-from: type=gha
           #cache-to: type=gha,mode=max
 
       - name: Test cli works in runtime image
         run: docker run ${{ env.IMAGE_REPOSITORY }} --version
 
   release:
     # upload to PyPI and make a release on every tag
     needs: [lint, dist, test]
     if: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
     runs-on: ubuntu-latest
+    env:
+      HAS_PYPI_TOKEN: ${{ secrets.PYPI_TOKEN != '' }}
 
     steps:
       - uses: actions/download-artifact@v3
 
       - name: Fixup blank lockfiles
         # Github release artifacts can't be blank
         run: for f in lockfiles/*; do [ -s $f ] || echo '# No requirements' >> $f; done
 
       - name: Github Release
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@1e07f4398721186383de40550babbdf2b84acfc5 # v0.1.14
+        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844 # v0.1.15
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           files: |
             dist/*
             lockfiles/*
           generate_release_notes: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Publish to PyPI
+        if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `python3-pip-skeleton-3.3.0/.github/workflows/docs.yml` & `python3-pip-skeleton-3.4.0/.github/workflows/docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -42,12 +42,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.event_name == 'push' && github.actor != 'dependabot[bot]'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@de7ea6f8efb354206b205ef54722213d99067935 # v3.9.0
+        uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `python3-pip-skeleton-3.3.0/.github/workflows/docs_clean.yml` & `python3-pip-skeleton-3.4.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.github/workflows/linkcheck.yml` & `python3-pip-skeleton-3.4.0/.github/workflows/linkcheck.yml`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,14 @@
   workflow_dispatch:
   schedule:
     # Run weekly to check URL links still resolve
     - cron: "0 8 * * WED"
 
 jobs:
   docs:
-    strategy:
-      fail-fast: false
-      matrix:
-        python: ["3.10"]
-
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Install python packages
```

### Comparing `python3-pip-skeleton-3.3.0/.gitignore` & `python3-pip-skeleton-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/.vscode/launch.json` & `python3-pip-skeleton-3.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/LICENSE` & `python3-pip-skeleton-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/PKG-INFO` & `python3-pip-skeleton-3.4.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,54 @@
-Metadata-Version: 2.1
-Name: python3-pip-skeleton
-Version: 3.3.0
-Summary: The CLI for adopting the python3-pip-skeleton framework
-Home-page: https://github.com/DiamondLightSource/python3-pip-skeleton-cli
-Author: Tom Cobb
-Author-email: tom.cobb@diamond.ac.uk
-License: Apache License 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 python3-pip-skeleton-cli
 ===========================
 
 |code_ci| |docs_ci| |coverage| |pypi_version| |license|
 
-This skeleton module (inspired by `jaraco/skeleton
-<https://blog.jaraco.com/skeleton/>`_) is a generic Python project structure
-which provides a means to keep tools and techniques in sync between multiple
-Python projects.
+``python3-pip-skeleton-cli`` provides the documentation
+and a command line tool to enable the adoption of python3-pip-skeleton_
+into a new or existing Python project.
 
 ============== ==============================================================
 PyPI           ``pip install python3-pip-skeleton``
 Source code    https://github.com/DiamondLightSource/python3-pip-skeleton-cli
 Documentation  https://DiamondLightSource.github.io/python3-pip-skeleton-cli
 Releases       https://github.com/DiamondLightSource/python3-pip-skeleton-cli/releases
 ============== ==============================================================
 
-It integrates the following tools:
+The related python3-pip-skeleton_ repository contains the source
+code that can be merged into new or existing projects, and pulled from to
+keep them up to date. It can also serve as a working example for those who
+would prefer to cherry-pick.
+
+python3-pip-skeleton_ is inspired by `jaraco/skeleton
+<https://blog.jaraco.com/skeleton/>`_.
+It provides a generic Python project structure
+and allows developers to keep tools and techniques in sync between multiple
+Python projects. It integrates the following tools:
 
 - pip and setuptools_scm for version management
 - Pre-commit with black, flake8 and isort for static analysis
 - Pytest for code and coverage
 - Sphinx for tutorials, how-to guides, explanations and reference documentation
 - GitHub Actions for code and docs CI and deployment to PyPI and GitHub Pages
 - tox -p: runs pre-commit, pytest, mypy and make docs
   - which verifies all the things that CI does
 - If you use VSCode, it will run black, flake8, isort and mypy on save
 
-The the related skeleton_ repo for this module contains the source
-code that can be merged into new or existing projects, and pulled from to
-keep them up to date. It can also serve as a working example for those who
-would prefer to cherry-pick.
 
-.. _skeleton: https://github.com/DiamondLightSource/python3-pip-skeleton
+.. _python3-pip-skeleton: https://github.com/DiamondLightSource/python3-pip-skeleton
+
+Quick start
+-----------
 
-This ``python3-pip-skeleton-cli`` repo contains the
-docs and a command line tool to ease the adoption of this skeleton into a
-new project like this::
+To create a new project based on skeleton::
 
     python3-pip-skeleton new /path/to/be/created --org my_github_user_or_org
 
-and existing projects::
+or to adopt skeleton into existing projects::
 
     python3-pip-skeleton existing /path/to/existing/repo --org my_github_user_or_org
 
 .. |code_ci| image:: https://github.com/DiamondLightSource/python3-pip-skeleton-cli/actions/workflows/code.yml/badge.svg?branch=main
     :target: https://github.com/DiamondLightSource/python3-pip-skeleton-cli/actions/workflows/code.yml
     :alt: Code CI
```

### Comparing `python3-pip-skeleton-3.3.0/docs/conf.py` & `python3-pip-skeleton-3.4.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
+import sys
 from pathlib import Path
 from subprocess import check_output
 
+import requests
+
 import python3_pip_skeleton
 
 # -- General configuration ------------------------------------------------
 
 # General information about the project.
 project = "python3-pip-skeleton-cli"
 
@@ -122,33 +125,52 @@
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
 github_repo = project
 github_user = "DiamondLightSource"
+switcher_json = f"https://{github_user}.github.io/{github_repo}/switcher.json"
+switcher_exists = requests.get(switcher_json).ok
+if not switcher_exists:
+    print(
+        "*** Can't read version switcher, is GitHub pages enabled? \n"
+        "    Once Docs CI job has successfully run once, set the "
+        "Github pages source branch to be 'gh-pages' at:\n"
+        f"    https://github.com/{github_user}/{github_repo}/settings/pages",
+        file=sys.stderr,
+    )
 
 # Theme options for pydata_sphinx_theme
+# We don't check switcher because there are 3 possible states for a repo:
+# 1. New project, docs are not published so there is no switcher
+# 2. Existing project with latest skeleton, switcher exists and works
+# 3. Existing project with old skeleton that makes broken switcher,
+#    switcher exists but is broken
+# Point 3 makes checking switcher difficult, because the updated skeleton
+# will fix the switcher at the end of the docs workflow, but never gets a chance
+# to complete as the docs build warns and fails.
 html_theme_options = dict(
     logo=dict(
         text=project,
     ),
     use_edit_page_button=True,
     github_url=f"https://github.com/{github_user}/{github_repo}",
     icon_links=[
         dict(
             name="PyPI",
             url="https://pypi.org/project/python3-pip-skeleton",
             icon="fas fa-cube",
         )
     ],
     switcher=dict(
-        json_url=f"https://{github_user}.github.io/{github_repo}/switcher.json",
+        json_url=switcher_json,
         version_match=version,
     ),
+    check_switcher=True,
     navbar_end=["theme-switcher", "icon-links", "version-switcher"],
     external_links=[
         dict(
             name="Release Notes",
             url=f"https://github.com/{github_user}/{github_repo}/releases",
         )
     ],
```

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/explanations/decisions.rst` & `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/how-to/build-docs.rst` & `python3-pip-skeleton-3.4.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/how-to/lint.rst` & `python3-pip-skeleton-3.4.0/docs/developer/how-to/lint.rst`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     $ tox -e pre-commit
 
 Or you can install a pre-commit hook that will run each time you do a ``git
 commit`` on just the files that have changed::
 
     $ pre-commit install
 
+It is also possible to `automatically enable pre-commit on cloned repositories <https://pre-commit.com/#automatically-enabling-pre-commit-on-repositories>`_.
+This will result in pre-commits being enabled on every repo your user clones from now on.
+
 Fixing issues
 -------------
 
 If black reports an issue you can tell it to reformat all the files in the
 repository::
 
     $ black .
```

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/how-to/make-release.rst` & `python3-pip-skeleton-3.4.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/how-to/update-tools.rst` & `python3-pip-skeleton-3.4.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/index.rst` & `python3-pip-skeleton-3.4.0/docs/developer/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,26 +28,28 @@
             how-to/contribute
             how-to/build-docs
             how-to/run-tests
             how-to/static-analysis
             how-to/lint
             how-to/update-tools
             how-to/make-release
+            how-to/pin-requirements
+            how-to/test-container
 
         +++
 
         Practical step-by-step guides for day-to-day dev tasks.
 
     .. grid-item-card:: :material-regular:`apartment;3em`
 
         .. toctree::
             :caption: Explanations
             :maxdepth: 1
 
-            explanations/decisions
+            explanations/skeleton
 
         +++
 
         Explanations of how and why the architecture is why it is.
 
     .. grid-item-card:: :material-regular:`description;3em`
```

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/reference/standards.rst` & `python3-pip-skeleton-3.4.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/developer/tutorials/dev-install.rst` & `python3-pip-skeleton-3.4.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/images/dls-favicon.ico` & `python3-pip-skeleton-3.4.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/images/dls-logo.svg` & `python3-pip-skeleton-3.4.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/images/excalidraw-example.svg` & `python3-pip-skeleton-3.4.0/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/images/git_merge.png` & `python3-pip-skeleton-3.4.0/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/index.rst` & `python3-pip-skeleton-3.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/user/explanations/skeleton.rst` & `python3-pip-skeleton-3.4.0/docs/developer/explanations/skeleton.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/user/explanations/why-src.rst` & `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0004-why-src.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,29 @@
-Why use a source directory
-==========================
+.. _src:
 
-This skeleton repo has made the decision to use a source directory. The reasons
-for this are set out in `Hynek's article`_ and summarized below.
+4. Use a source directory
+=========================
+
+Date: 2023-01-18
+
+Status
+------
+
+Accepted
+
+Context
+-------
+
+We need to decide how to structure the source code in skeleton based projects.
+
+
+Decision
+--------
+
+As per `Hynek's article`_ and summarized below.
 
 .. _Hynek's article: https://hynek.me/articles/testing-packaging/
 
 The main advantage is that the source directory cannot shadow installed packages
 as it would if it was in the root of the repository. This means that if you
 install the package, then run the tests, they will run against the installed
 package and not the source directory, testing for packaging bugs.
@@ -22,7 +39,12 @@
 - ``test`` job with ``lock: true`` does an `editable install`_ of the
   package. This is the mode that is used at development time, as modifications
   to sources can be tested without reinstalling.
 - ``test`` job with ``lock: false`` does a regular install, which
   checks that all files needed for the tests are packaged with the distribution.
 
 .. _editable install: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
+
+Consequences
+------------
+
+See the article linked above.
```

### Comparing `python3-pip-skeleton-3.3.0/docs/user/explanations/why-use-skeleton.rst` & `python3-pip-skeleton-3.4.0/docs/user/explanations/why-use-skeleton.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Why use a skeleton structure?
+Why Use a Skeleton Structure?
 =============================
 
 Many projects start from some kind of template. These define some basic
 structure, customized with project specific variables, that developers can add
 their code into. One example of this is cookiecutter_.
 
 .. _cookiecutter: https://cookiecutter.readthedocs.io
```

### Comparing `python3-pip-skeleton-3.3.0/docs/user/how-to/excalidraw.rst` & `python3-pip-skeleton-3.4.0/docs/user/how-to/excalidraw.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/user/how-to/existing.rst` & `python3-pip-skeleton-3.4.0/docs/user/how-to/existing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 How to adopt the skeleton in an existing repo
 =============================================
 
 If you have an existing repo and would like to adopt the skeleton structure
 then you can use the commandline tool to merge the skeleton into your repo::
 
-    python3-pip-skeleton existing /path/to/existing/repo --org my_github_user_or_org
+    python3-pip-skeleton existing /path/to/existing/repo --org my_github_user_or_org --skeleton-org some_institution
 
 This will:
 
 - Take the repo name from the last element of the path
 - Take the package name from the repo name unless overridden by ``--package``
 - Clone the existing repo in /tmp
 - Create a new orphan merge branch from the skeleton repo
+- Use the version of the skeleton in ``some_institution``'s organization (default ``DiamondLightSource``)
 - Create a single commit that modifies the skeleton with the repo and package name
 - Push that merge branch back to the existing repo
 - Merge with the currently checked out branch, leaving you to fix the conflicts
 
 .. note::
 
     To enable publishing to PyPI see `../how-to/pypi` 
 
+.. note::
+
+    To install the pre-commit see `../../developer/how-to/lint`
+
 Example merge
 -------------
 
 As an example, `scanspec #46
 <https://github.com/dls-controls/scanspec/pull/46>`_ shows the what this
 adoption looks like. The commandline tool was run on the existing repo::
```

### Comparing `python3-pip-skeleton-3.3.0/docs/user/how-to/pypi.rst` & `python3-pip-skeleton-3.4.0/docs/user/how-to/pypi.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/user/how-to/update.rst` & `python3-pip-skeleton-3.4.0/docs/user/how-to/update.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.3.0/docs/user/index.rst` & `python3-pip-skeleton-3.4.0/docs/user/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -22,35 +22,34 @@
 
     .. grid-item-card:: :material-regular:`directions;3em`
 
         .. toctree::
             :caption: How-to Guides
             :maxdepth: 1
 
+            how-to/maintain-your-own-skeleton
             how-to/run-container
             how-to/existing
             how-to/update
             how-to/excalidraw
-            how-to/pypi            
+            how-to/pypi
 
         +++
 
         Practical step-by-step guides for the more experienced user.
 
     .. grid-item-card:: :material-regular:`info;3em`
 
         .. toctree::
             :caption: Explanations
             :maxdepth: 1
 
-            explanations/docs-structure
+            explanations/structure
             explanations/why-use-skeleton
-            explanations/why-src
-            explanations/why-pre-commit
-            explanations/skeleton            
+            explanations/decisions
 
         +++
 
         Explanations of how the library works and why it works that way.
 
     .. grid-item-card:: :material-regular:`menu_book;3em`
```

### Comparing `python3-pip-skeleton-3.3.0/docs/user/tutorials/installation.rst` & `python3-pip-skeleton-3.4.0/docs/user/tutorials/installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 
 It is recommended that you install into a “virtual environment” so this
 installation will not interfere with any existing Python software::
 
     $ python3 -m venv /path/to/venv
     $ source /path/to/venv/bin/activate
 
+.. note::
+
+    You may wish to deactivate any existing virual environments before sourcing the new
+    environment. Deactivation can be performed by executing:
+    
+    - :code:`conda deactivate` for conda
+    - :code:`deactivate` for venv or virtualenv
+    - :code:`exit` for pipenv
+
 
 Installing the library
 ----------------------
 
 You can now use ``pip`` to install the library and its dependencies::
 
     $ python3 -m pip install python3-pip-skeleton
```

### Comparing `python3-pip-skeleton-3.3.0/docs/user/tutorials/new.rst` & `python3-pip-skeleton-3.4.0/docs/user/tutorials/new.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Creating a new repo from the skeleton
 =====================================
 
-Once you have followed the `installation` tutorial, you can use the
+Once you have followed the ``installation`` tutorial, you can use the
 commandline tool to make a new repo that inherits the skeleton::
 
-    python3-pip-skeleton new /path/to/be/created --org my_github_user_or_org
+    python3-pip-skeleton new /path/to/be/created --org my_github_user_or_org --skeleton-org some_institution
 
 This will:
 
 - Take the repo name from the last element of the path
 - Take the package name from the repo name unless overridden by ``--package``
 - Create a new repo at the requested path, forked from the skeleton repo
 - Create a single commit that modifies the skeleton with the repo and package name
+- Use the version of the skeleton in ``some_institution``'s organization (default ``DiamondLightSource``)
 
 
 Getting started with your new repo
 ----------------------------------
 
 Your new repo has a workflow based on pip. The first thing to do is to use
 pip to install packages in a virtual environment::
 
-    virtual .venv
+    python -m venv .venv
     source .venv/bin/activate
     pip install -e .[dev]
 
+.. note::
+
+    You may wish to deactivate any existing virual environments before sourcing the new
+    environment. Deactivation can be performed by executing:
+
+    - :code:`conda deactivate` for conda
+    - :code:`deactivate` for venv or virtualenv
+    - :code:`exit` for pipenv
+
 You can then run any entry points declared in setup.cfg e.g.::
 
     python3-pip-skeleton --version
 
 will run the python interpreter with access to all the packages you need to
 develop your repo.
 
@@ -36,14 +46,19 @@
 
 The Github Actions Continuous Integration will publish your package to PyPI.
 To do so you need a PyPI account and and a PyPI Token configured in your 
 project or github Organization. 
 
 see `../how-to/pypi`
 
+Setting up pre-commit
+---------------------
+
+To install the pre-commit see `../../developer/how-to/lint`.
+
 Running the tests
 -----------------
 
 There are also some extra convenience scripts provided via tox::
 
     tox -p
```

### Comparing `python3-pip-skeleton-3.3.0/src/python3_pip_skeleton.egg-info/SOURCES.txt` & `python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.rst
+Dockerfile
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-.devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
 .github/workflows/code.yml
@@ -20,37 +19,48 @@
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/genindex.rst
 docs/index.rst
 docs/developer/index.rst
-docs/developer/explanations/decisions.rst
-docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+docs/developer/explanations/skeleton.rst
 docs/developer/how-to/build-docs.rst
 docs/developer/how-to/contribute.rst
 docs/developer/how-to/lint.rst
 docs/developer/how-to/make-release.rst
+docs/developer/how-to/pin-requirements.rst
 docs/developer/how-to/run-tests.rst
 docs/developer/how-to/static-analysis.rst
+docs/developer/how-to/test-container.rst
 docs/developer/how-to/update-tools.rst
 docs/developer/reference/standards.rst
 docs/developer/tutorials/dev-install.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
 docs/images/excalidraw-example.svg
 docs/images/git_merge.png
 docs/user/index.rst
-docs/user/explanations/docs-structure.rst
-docs/user/explanations/skeleton.rst
-docs/user/explanations/why-pre-commit.rst
-docs/user/explanations/why-src.rst
+docs/user/explanations/decisions.rst
+docs/user/explanations/structure.rst
 docs/user/explanations/why-use-skeleton.rst
+docs/user/explanations/decisions/0001-record-architecture-decisions.rst
+docs/user/explanations/decisions/0003-docs-structure.rst
+docs/user/explanations/decisions/0004-why-src.rst
+docs/user/explanations/decisions/0005-pyproject-toml.rst
+docs/user/explanations/decisions/0006-setuptools-scm.rst
+docs/user/explanations/decisions/0007-dev-dependencies.rst
+docs/user/explanations/decisions/0008-use-tox.rst
+docs/user/explanations/decisions/0009-sphinx-theme.rst
+docs/user/explanations/decisions/0010-vscode-settings.rst
+docs/user/explanations/decisions/0011-requirements-txt.rst
+docs/user/explanations/decisions/0012-containers.rst
 docs/user/how-to/excalidraw.rst
 docs/user/how-to/existing.rst
+docs/user/how-to/maintain-your-own-skeleton.rst
 docs/user/how-to/pypi.rst
 docs/user/how-to/run-container.rst
 docs/user/how-to/update.rst
 docs/user/reference/api.rst
 docs/user/tutorials/installation.rst
 docs/user/tutorials/new.rst
 src/python3_pip_skeleton/__init__.py
```

