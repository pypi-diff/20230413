# Comparing `tmp/xchembku-1.0.2.tar.gz` & `tmp/xchembku-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.0.2.tar", last modified: Sun Apr  9 12:23:27 2023, max compression
+gzip compressed data, was "xchembku-1.1.0.tar", last modified: Thu Apr 13 08:38:26 2023, max compression
```

## Comparing `xchembku-1.0.2.tar` & `xchembku-1.1.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.932704 xchembku-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.904703 xchembku-1.0.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.904703 xchembku-1.0.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-09 12:23:17.000000 xchembku-1.0.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-09 12:23:17.000000 xchembku-1.0.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-09 12:23:17.000000 xchembku-1.0.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.896704 xchembku-1.0.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-09 12:23:17.000000 xchembku-1.0.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-09 12:23:17.000000 xchembku-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-09 12:23:17.000000 xchembku-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 12:23:17.000000 xchembku-1.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.908704 xchembku-1.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 12:23:17.000000 xchembku-1.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 12:23:17.000000 xchembku-1.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 12:23:17.000000 xchembku-1.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 12:23:17.000000 xchembku-1.0.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 12:23:17.000000 xchembku-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-09 12:23:27.932704 xchembku-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-09 12:23:17.000000 xchembku-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-09 12:23:17.000000 xchembku-1.0.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.896704 xchembku-1.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.912704 xchembku-1.0.2/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.916704 xchembku-1.0.2/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.916704 xchembku-1.0.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 12:23:17.000000 xchembku-1.0.2/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-09 12:23:17.000000 xchembku-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:23:27.932704 xchembku-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.900704 xchembku-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.916704 xchembku-1.0.2/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.916704 xchembku-1.0.2/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.916704 xchembku-1.0.2/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.920704 xchembku-1.0.2/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.920704 xchembku-1.0.2/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.924703 xchembku-1.0.2/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.924703 xchembku-1.0.2/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.924703 xchembku-1.0.2/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 12:23:27.000000 xchembku-1.0.2/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.924703 xchembku-1.0.2/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.928704 xchembku-1.0.2/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.928704 xchembku-1.0.2/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-09 12:23:17.000000 xchembku-1.0.2/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.932704 xchembku-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:23:27.932704 xchembku-1.0.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-09 12:23:17.000000 xchembku-1.0.2/tests/test_crystal_well_droplocation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-13 08:38:18.000000 xchembku-1.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-13 08:38:18.000000 xchembku-1.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 08:38:18.000000 xchembku-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-13 08:38:18.000000 xchembku-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 08:38:18.000000 xchembku-1.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 08:38:18.000000 xchembku-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-13 08:38:26.715559 xchembku-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-13 08:38:18.000000 xchembku-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 08:38:18.000000 xchembku-1.1.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-13 08:38:18.000000 xchembku-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:38:26.715559 xchembku-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_well_droplocation.py
```

### Comparing `xchembku-1.0.2/.dae-devops/Makefile` & `xchembku-1.1.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/conventions.rst` & `xchembku-1.1.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/developing.rst` & `xchembku-1.1.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/devops.rst` & `xchembku-1.1.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/docs_structure.rst` & `xchembku-1.1.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/installing.rst` & `xchembku-1.1.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/docs/testing.rst` & `xchembku-1.1.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.dae-devops/project.yaml` & `xchembku-1.1.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.devcontainer/Dockerfile` & `xchembku-1.1.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.devcontainer/devcontainer.json` & `xchembku-1.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/CONTRIBUTING.rst` & `xchembku-1.1.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/actions/install_requirements/action.yml` & `xchembku-1.1.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/dependabot.yml` & `xchembku-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/pages/make_switcher.py` & `xchembku-1.1.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/workflows/code.yml` & `xchembku-1.1.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/workflows/docs.yml` & `xchembku-1.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/workflows/docs_clean.yml` & `xchembku-1.1.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.github/workflows/linkcheck.yml` & `xchembku-1.1.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.gitignore` & `xchembku-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.gitlab-ci.yml` & `xchembku-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/.vscode/launch.json` & `xchembku-1.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/LICENSE` & `xchembku-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/PKG-INFO` & `xchembku-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.0.2
+Version: 1.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.0.2/README.rst` & `xchembku-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/configurations/development.yaml` & `xchembku-1.1.0/configurations/development.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 # The external access bits.
 external_access_bits:
     database_filename: &DATABASE_FILENAME /scratch/${USER}/xchembku/databases/runtime/xchembku.sqlite
     dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
     dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
 
 # The xchembku_dataface client/server composite.
+xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
+    type: "xchembku_lib.xchembku_datafaces.direct"
+    database:
+        type: "xchembku_lib.xchembku_databases.normsql"
+        filename: *DATABASE_FILENAME
+        log_level: "WARNING"
+
+# The xchembku_dataface client/server composite.
 xchembku_dataface_specification:
     type: "xchembku_lib.xchembku_datafaces.aiohttp"
     type_specific_tbd:
         # The remote xchembku_dataface server access.
         aiohttp_specification:
             server: *XCHEMBKU_DATAFACE_SERVER
             client: *XCHEMBKU_DATAFACE_CLIENT
         # The local implementation of the xchembku_dataface.
-        actual_xchembku_dataface_specification:
-            type: "xchembku_lib.xchembku_datafaces.direct"
-            database:
-                type: "xchembku_lib.xchembku_databases.normsql"
-                filename: *DATABASE_FILENAME
-                log_level: "WARNING"
+        actual_xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     context:
         start_as: coro
```

### Comparing `xchembku-1.0.2/docs/conf.py` & `xchembku-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/docs/images/dls-favicon.ico` & `xchembku-1.1.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/docs/images/dls-logo.svg` & `xchembku-1.1.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/docs/index.rst` & `xchembku-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.1.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/docs/user/index.rst` & `xchembku-1.1.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/pyproject.toml` & `xchembku-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.1.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.0.2
+Version: 1.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.0.2/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.1.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_api/context_base.py` & `xchembku-1.1.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.1.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,23 +130,23 @@
 
         # Dicts are returned, so parse them into models.
         models = [CrystalWellModel(**record) for record in records]
 
         return models
 
     # ----------------------------------------------------------------------------------------
-    async def originate_crystal_wells(
+    async def upsert_crystal_wells(
         self,
         models: List[CrystalWellModel],
     ) -> None:
         """"""
 
         records: List[Dict] = [model.dict() for model in models]
         await self.__send_protocolj(
-            "originate_crystal_wells_serialized",
+            "upsert_crystal_wells_serialized",
             records,
         )
 
         return None
 
     # ----------------------------------------------------------------------------------------
     async def update_crystal_wells(
```

### Comparing `xchembku-1.0.2/src/xchembku_api/datafaces/context.py` & `xchembku-1.1.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.1.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_api/exceptions.py` & `xchembku-1.1.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.1.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import uuid
 from typing import Optional
 
 from pydantic import BaseModel
 
 
-class CrystalPlateModel(BaseModel):
+class CrystalWellModel(BaseModel):
     """
-    Model containing plate information.
+    Model containing well information.
 
-    Typically this structure is populated and transmitted by the rockminer package.
+    Typically this structure is populated and transmitted by the rockingest package.
     """
 
     uuid: str
-    # ID from the Plate table.
-    formulatrix__plate__id: int
-    barcode: str
-    visit: str
+
+    # This is the plate on which the well resides.
+    crystal_plate_uuid: str
+
+    # This is the well's position on the plate, such as A01_1, A01_2, etc.
+    # TODO: Enforce crystal_well.position unique among wells in plate.
+    position: str
+
+    # This is the filename containing the well's image.
+    filename: str
+
+    # This is the error reading and parsing the image file, if any.
+    error: Optional[str]
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.0.2/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.1.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
     Typically this structure is populated and transmitted by the chimpflow.
     """
 
     uuid: str
     crystal_well_uuid: Optional[str] = None
     drop_detected: Optional[bool] = None
-    auto_target_position_x: Optional[int] = None
-    auto_target_position_y: Optional[int] = None
+    auto_target_x: Optional[int] = None
+    auto_target_y: Optional[int] = None
     well_centroid_x: Optional[int] = None
     well_centroid_y: Optional[int] = None
     number_of_crystals: Optional[int] = None
     crystal_coordinates: Optional[List[Tuple[int, int]]] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
```

### Comparing `xchembku-1.0.2/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.1.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     Model containing crystal well droplocation information.
 
     Typically this structure is populated and transmitted by the chimpflow.
     """
 
     uuid: str
     crystal_well_uuid: Optional[str] = None
-    confirmed_target_position_x: Optional[int] = None
-    confirmed_target_position_y: Optional[int] = None
+    confirmed_target_x: Optional[int] = None
+    confirmed_target_y: Optional[int] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.0.2/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.1.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import uuid
 from typing import Optional
 
 from pydantic import BaseModel
 
 
-class CrystalWellModel(BaseModel):
+class CrystalPlateModel(BaseModel):
     """
-    Model containing well information.
+    Model containing plate information.
 
-    Typically this structure is populated and transmitted by the rockingest package.
+    Typically this structure is populated and transmitted by the rockminer package.
     """
 
     uuid: str
-    crystal_plate_uuid: str
-    filename: str
-    error: Optional[str]
+    # ID from the Plate table.
+    formulatrix__plate__id: int
+    # Directory stem where wells were mined from.
+    # Also used by echolocator to format the export csv filename.
+    rockminer_collected_stem: Optional[str] = None
+    # The 4-letter barcode.
+    barcode: str
+    # The visit gleaned from the Formulatrix database.
+    visit: str
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.0.2/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.1.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
     Typically this structure is returned by queries.
     """
 
     # Stuff from the original record.
     uuid: str
     visit: str
+    position: str
     filename: str
     error: Optional[str]
     created_on: str
 
     # Stuff from the autolocation.
-    auto_target_position_x: Optional[int] = None
-    auto_target_position_y: Optional[int] = None
+    auto_target_x: Optional[int] = None
+    auto_target_y: Optional[int] = None
     well_centroid_x: Optional[int] = None
     well_centroid_y: Optional[int] = None
     drop_detected: Optional[bool] = None
     number_of_crystals: Optional[int] = None
 
     # Stuff from the droplocation.
     crystal_well_droplocation_uuid: Optional[str] = None
-    confirmed_target_position_x: Optional[int] = None
-    confirmed_target_position_y: Optional[int] = None
+    confirmed_target_x: Optional[int] = None
+    confirmed_target_y: Optional[int] = None
```

### Comparing `xchembku-1.0.2/src/xchembku_cli/main.py` & `xchembku-1.1.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_cli/subcommands/base.py` & `xchembku-1.1.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_cli/subcommands/service.py` & `xchembku-1.1.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_cli/version.py` & `xchembku-1.1.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/__main__.py` & `xchembku-1.1.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/contexts/base.py` & `xchembku-1.1.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.1.0/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/databases/databases.py` & `xchembku-1.1.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/databases/normsql.py` & `xchembku-1.1.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.1.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,17 @@
                     sql_type = "REAL"
                 elif field_type == bool:
                     sql_type = "BOOLEAN"
 
                 self.fields[field_name] = {"type": sql_type}
 
         # Add indexes.
+        self.fields["position"]["index"] = True
+        self.fields["filename"]["index"] = True
+        self.fields["crystal_plate_uuid"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellAutolocationsTable(TableDefinition):
     # ----------------------------------------------------------------------------------------
     def __init__(self):
```

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/context.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     async def upsert_crystal_plates(
         self,
         models: List[CrystalPlateModel],
         why="upsert_crystal_plates",
     ) -> Dict:
         """
         Caller provides the crystal plate record with the fields to be updated.
+
+        We don't insert the same formulatrix__plate__id twice.
+
+        TODO: Find more efficient way to upsert_crystal_plates in batch.
         """
 
         inserted_count = 0
         updated_count = 0
 
         # Loop over all the models to be upserted.
         for model in models:
```

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import logging
 from typing import Dict, List
 
 from dls_normsql.constants import CommonFieldnames
 from dls_utilpack.describe import describe
 
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
@@ -14,93 +15,97 @@
 logger = logging.getLogger(__name__)
 
 
 class DirectCrystalWells(DirectBase):
     """ """
 
     # ----------------------------------------------------------------------------------------
-    async def originate_crystal_wells_serialized(self, records: List[Dict]) -> None:
+    async def upsert_crystal_wells_serialized(
+        self,
+        records: List[Dict],
+        why=None,
+    ) -> Dict:
         # We are being given json, so parse it into models.
         models = [CrystalWellModel(**record) for record in records]
         # Return the method doing the work.
-        return await self.originate_crystal_wells(models)
+        return await self.upsert_crystal_wells(models, why=why)
 
     # ----------------------------------------------------------------------------------------
-    async def originate_crystal_wells(self, models: List[CrystalWellModel]) -> None:
-        """
-        Caller provides the records containing fields to be created.
-        The filename field should be unique in all records.
+    async def upsert_crystal_wells(
+        self,
+        models: List[CrystalWellModel],
+        why="upsert_crystal_wells",
+    ) -> Dict:
         """
+        Caller provides the crystal well record with the fields to be updated.
 
-        # We're being given models, so serialize them into dicts to give to the sql.
-        records = [model.dict() for model in models]
-
-        return await self.insert(
-            "crystal_wells",
-            records,
-            why="originate_crystal_wells",
-        )
+        We don't insert the same filename twice.
 
-    # ----------------------------------------------------------------------------------------
-    async def update_crystal_wells_serialized(self, records: List[Dict]) -> Dict:
-        # We are being given json, so parse it into models.
-        models = [CrystalWellModel(**record) for record in records]
-        # Return the method doing the work.
-        return await self.update_crystal_wells(models)
+        TODO: Consider an alternate way besides filename to distinguish duplicate crystal wells in upsert.
 
-    # ----------------------------------------------------------------------------------------
-    async def update_crystal_wells(
-        self, models: List[CrystalWellModel], why=None
-    ) -> Dict:
-        """
-        Caller provides the crystal well record with the fields to be updated.
+        TODO: Find more efficient way to upsert_crystal_wells in batch.
         """
 
-        # We're being given models, so serialize them into dicts to give to the sql.
-        records = [model.dict() for model in models]
+        inserted_count = 0
+        updated_count = 0
 
-        count = 0
-        for record in records:
-            result = await self.update(
-                "crystal_wells",
-                record,
-                f"({CommonFieldnames.UUID} = ?)",
-                subs=[record[CommonFieldnames.UUID]],
+        # Loop over all the models to be upserted.
+        for model in models:
+            # Find any existing record for this model object.
+            records = await self.query(
+                "SELECT * FROM crystal_wells WHERE filename = ?",
+                subs=[model.filename],
                 why=why,
             )
-            count += result.get("count", 0)
-
-        return {"count": count}
-
-    # ----------------------------------------------------------------------------------------
-    async def fetch_crystal_wells_filenames_serialized(
-        self, limit: int = 1, why=None
-    ) -> List[Dict]:
-        """ """
-
-        # Get the models from the direct call.
-        models = await self.fetch_crystal_wells_filenames(limit=limit, why=why)
-
-        # Serialize models into dicts to give to the response.
-        records = [model.dict() for model in models]
 
-        return records
+            if len(records) > 0:
+                # Make a copy of the model record and remove some fields not to update.
+                model_copy = copy.deepcopy(model.dict())
+                model_copy.pop(CommonFieldnames.UUID)
+                model_copy.pop(CommonFieldnames.CREATED_ON)
+                model_copy.pop("filename")
+                model_copy.pop("crystal_plate_uuid")
+                result = await self.update(
+                    "crystal_wells",
+                    model_copy,
+                    "(filename = ?)",
+                    subs=[model.filename],
+                    why=why,
+                )
+                updated_count += result.get("count", 0)
+            else:
+                await self.insert(
+                    "crystal_wells",
+                    [model.dict()],
+                    why=why,
+                )
+                inserted_count += 1
+
+        return {
+            "updated_count": updated_count,
+            "inserted_count": inserted_count,
+        }
 
     # ----------------------------------------------------------------------------------------
     async def fetch_crystal_wells_filenames(
         self, limit: int = 1, why=None
     ) -> List[CrystalWellModel]:
         """
         Filenams for ALL wells ever.
         """
 
         if why is None:
             why = "API fetch_crystal_wells_filenames"
         records = await self.query(
-            "SELECT crystal_wells.filename, crystal_wells.crystal_plate_uuid"
+            "SELECT"
+            " crystal_wells.uuid,"
+            " crystal_wells.position,"
+            " crystal_wells.filename,"
+            " crystal_wells.crystal_plate_uuid,"
+            f" crystal_wells.{CommonFieldnames.CREATED_ON}"
             f" FROM crystal_wells"
             f" ORDER BY {CommonFieldnames.CREATED_ON}",
             why=why,
         )
 
         # Parse the records returned by sql into models.
         models = [CrystalWellModel(**record) for record in records]
@@ -183,18 +188,22 @@
         where = "WHERE"
 
         if why is None:
             why = "API fetch_crystal_wells_needing_droplocation"
 
         query = (
             "\nSELECT crystal_wells.*,"
-            "\n  crystal_well_autolocations.auto_target_position_x,"
-            "\n  crystal_well_autolocations.auto_target_position_y,"
-            "\n  crystal_well_droplocations.confirmed_target_position_x,"
-            "\n  crystal_well_droplocations.confirmed_target_position_y,"
+            "\n  crystal_well_autolocations.auto_target_x,"
+            "\n  crystal_well_autolocations.auto_target_y,"
+            "\n  crystal_well_autolocations.well_centroid_x,"
+            "\n  crystal_well_autolocations.well_centroid_y,"
+            "\n  crystal_well_autolocations.drop_detected,"
+            "\n  crystal_well_autolocations.number_of_crystals,"
+            "\n  crystal_well_droplocations.confirmed_target_x,"
+            "\n  crystal_well_droplocations.confirmed_target_y,"
             "\n  crystal_plates.visit"
             "\nFROM crystal_wells"
             "\nJOIN crystal_well_autolocations ON crystal_well_autolocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_well_droplocations ON crystal_well_droplocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_plates ON crystal_plates.uuid = crystal_wells.crystal_plate_uuid"
         )
 
@@ -203,14 +212,32 @@
             query += (
                 "\n/* Just certain filenames. */"
                 f"\n{where} crystal_wells.filename GLOB ?"
             )
             subs.append(filter.filename_pattern)
             where = "AND"
 
+        # Caller wants specific barcode?
+        if filter.barcode is not None:
+            query += (
+                "\n/* Just a wells on plates with a certain barcode. */"
+                f"\n{where} crystal_plates.barcode = ?"
+            )
+            subs.append(filter.barcode)
+            where = "AND"
+
+        # Caller wants specific visit?
+        if filter.visit is not None:
+            query += (
+                "\n/* Just a wells on plates with a certain visit. */"
+                f"\n{where} crystal_plates.visit = ?"
+            )
+            subs.append(filter.visit)
+            where = "AND"
+
         # Caller wants only those not yet confirmed?
         if filter.is_confirmed is False:
             query += (
                 "\n/* Exclude crystal wells which already have confirmed drop locations. */"
                 f"\n{where} crystal_wells.uuid NOT IN (SELECT crystal_well_uuid FROM crystal_well_droplocations)"
             )
             where = "AND"
@@ -221,15 +248,15 @@
             query += (
                 "\n/* Include only crystal wells which already have confirmed drop locations. */"
                 f"\n{where} crystal_wells.uuid IN (SELECT crystal_well_uuid FROM crystal_well_droplocations)"
             )
             where = "AND"
 
         # Caller wants only those which are confirmed but do not have usable coordinates?
-        usable_sql = "SELECT crystal_well_uuid FROM crystal_well_droplocations WHERE confirmed_target_position_x IS NOT NULL AND confirmed_target_position_y IS NOT NULL"
+        usable_sql = "SELECT crystal_well_uuid FROM crystal_well_droplocations WHERE confirmed_target_x IS NOT NULL AND confirmed_target_y IS NOT NULL"
         if filter.is_usable is False:
             query += (
                 "\n/* Include only crystal wells which DO NOT have drop locations with usable coordinates. */"
                 f"\n{where} crystal_wells.uuid NOT IN ({usable_sql})"
             )
             where = "AND"
```

### Comparing `xchembku-1.0.2/src/xchembku_lib/version.py` & `xchembku-1.1.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/tests/base.py` & `xchembku-1.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/tests/configurations/service.yaml` & `xchembku-1.1.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/tests/conftest.py` & `xchembku-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/tests/test_crystal_plate.py` & `xchembku-1.1.0/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.0.2/tests/test_crystal_well_autolocation.py` & `xchembku-1.1.0/tests/test_crystal_well_autolocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,25 @@
             barcode="xyzw",
             visit="cm00001-1",
         )
 
         # Write two well records.
         filename1 = "abc.jpg"
         crystal_well_model1 = CrystalWellModel(
-            crystal_plate_uuid=crystal_plate_model.uuid, filename=filename1
+            position="01A_1",
+            crystal_plate_uuid=crystal_plate_model.uuid,
+            filename=filename1,
         )
         filename2 = "xyz.jpg"
         crystal_well_model2 = CrystalWellModel(
-            crystal_plate_uuid=crystal_plate_model.uuid, filename=filename2
-        )
-        await dataface.originate_crystal_wells(
-            [crystal_well_model1, crystal_well_model2]
+            position="01A_2",
+            crystal_plate_uuid=crystal_plate_model.uuid,
+            filename=filename2,
         )
+        await dataface.upsert_crystal_wells([crystal_well_model1, crystal_well_model2])
 
         # Fetch all the wells which need autolocation.
         crystal_well_models = await dataface.fetch_crystal_wells_needing_autolocation(
             limit=100
         )
 
         assert len(crystal_well_models) == 2
```

### Comparing `xchembku-1.0.2/tests/test_crystal_well_droplocation.py` & `xchembku-1.1.0/tests/test_crystal_well_droplocation.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,17 +106,18 @@
         """ """
 
         # Reference the dataface object which the context has set up as the default.
         dataface = xchembku_datafaces_get_default()
 
         # Make a plate for the wells we will create.
         self.__visit = "cm00001-1"
+        self.__barcode = "xyzw"
         self.__crystal_plate_model = CrystalPlateModel(
             formulatrix__plate__id=1,
-            barcode="xyzw",
+            barcode=self.__barcode,
             visit=self.__visit,
         )
 
         # Write plate record.
         await dataface.upsert_crystal_plates(
             [self.__crystal_plate_model],
         )
@@ -147,14 +148,26 @@
 
         await self.__check(dataface, CrystalWellFilterModel(limit=1), 1, "limit 1")
         await self.__check(dataface, CrystalWellFilterModel(limit=2), 2, "limit 2")
         await self.__check(
             dataface, CrystalWellFilterModel(is_confirmed=True), 3, "confirmed only"
         )
         await self.__check(
+            dataface,
+            CrystalWellFilterModel(barcode=self.__barcode, is_confirmed=True),
+            3,
+            "confirmed only, barcode",
+        )
+        await self.__check(
+            dataface,
+            CrystalWellFilterModel(barcode="abcd", is_confirmed=True),
+            0,
+            "confirmed only, other barcode",
+        )
+        await self.__check(
             dataface, CrystalWellFilterModel(is_confirmed=False), 2, "unconfirmed only"
         )
 
         # Check the anchor query forward.
         await self.__check(
             dataface,
             CrystalWellFilterModel(anchor=models[3].uuid, direction=1, limit=1),
@@ -225,30 +238,50 @@
         await self.__check(
             dataface,
             CrystalWellFilterModel(is_confirmed=True, is_usable=False),
             0,
             "confirmed but unusable only",
         )
         crystal_well_models = await self.__check(
-            dataface, CrystalWellFilterModel(is_usable=True), 3, "usable only"
+            dataface,
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                is_usable=True,
+            ),
+            3,
+            "usable only, visit",
+        )
+
+        crystal_well_models = await self.__check(
+            dataface,
+            CrystalWellFilterModel(
+                barcode=self.__barcode,
+                is_usable=True,
+            ),
+            3,
+            "usable only, barcode",
         )
 
         # Change one of the usable to unusable.
         t = CrystalWellDroplocationModel(
             crystal_well_uuid=crystal_well_models[0].uuid,
-            confirmed_target_position_x=None,
-            confirmed_target_position_y=None,
+            confirmed_target_x=None,
+            confirmed_target_y=None,
         )
 
         await dataface.upsert_crystal_well_droplocations([t])
 
         # Check the usable queries again.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(is_confirmed=True, is_usable=False),
+            CrystalWellFilterModel(
+                visit=self.__visit,
+                is_confirmed=True,
+                is_usable=False,
+            ),
             1,
             "confirmed but unusable only",
         )
         crystal_well_models = await self.__check(
             dataface,
             CrystalWellFilterModel(is_usable=True),
             2,
@@ -265,36 +298,37 @@
             letter = "b"
 
         filename = "%03d%s.jpg" % (self.__injected_count, letter)
         self.__injected_count += 1
 
         # Create the well object.
         m = CrystalWellModel(
+            position="01A_1",
             crystal_plate_uuid=self.__crystal_plate_model.uuid,
             filename=filename,
         )
 
         # Write well record.
-        await dataface.originate_crystal_wells([m])
+        await dataface.upsert_crystal_wells([m])
 
         if autolocation:
             # Add a crystal well autolocation.
             ta = CrystalWellAutolocationModel(
                 crystal_well_uuid=m.uuid,
                 number_of_crystals=10,
             )
 
             await dataface.originate_crystal_well_autolocations([ta])
 
         if droplocation:
             # Add a crystal well droplocation.
             td = CrystalWellDroplocationModel(
                 crystal_well_uuid=m.uuid,
-                confirmed_target_position_x=10,
-                confirmed_target_position_y=11,
+                confirmed_target_x=10,
+                confirmed_target_y=11,
             )
 
             await dataface.upsert_crystal_well_droplocations([td])
 
         return m
 
     # ----------------------------------------------------------------------------------------
```

