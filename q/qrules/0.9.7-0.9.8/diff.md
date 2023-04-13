# Comparing `tmp/qrules-0.9.7.tar.gz` & `tmp/qrules-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrules-0.9.7.tar", last modified: Mon Feb 21 10:57:18 2022, max compression
+gzip compressed data, was "qrules-0.9.8.tar", last modified: Thu Apr 13 16:38:14 2023, max compression
```

## Comparing `qrules-0.9.7.tar` & `qrules-0.9.8.tar`

### file list

```diff
@@ -1,164 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.284595 qrules-0.9.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.272594 qrules-0.9.7/.constraints/
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-02-21 10:57:07.000000 qrules-0.9.7/.constraints/py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-02-21 10:57:07.000000 qrules-0.9.7/.constraints/py3.6.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-02-21 10:57:07.000000 qrules-0.9.7/.constraints/py3.7.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-02-21 10:57:07.000000 qrules-0.9.7/.constraints/py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-02-21 10:57:07.000000 qrules-0.9.7/.constraints/py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-02-21 10:57:07.000000 qrules-0.9.7/.cspell.json
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-02-21 10:57:07.000000 qrules-0.9.7/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-02-21 10:57:07.000000 qrules-0.9.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.272594 qrules-0.9.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.272594 qrules-0.9.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/ci-style.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/ci-tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/milestone.yml
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/pr-linting.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/requirements-cron.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-02-21 10:57:07.000000 qrules-0.9.7/.github/workflows/requirements-pr.yml
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-21 10:57:07.000000 qrules-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-02-21 10:57:07.000000 qrules-0.9.7/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-21 10:57:07.000000 qrules-0.9.7/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-02-21 10:57:07.000000 qrules-0.9.7/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     4465 2022-02-21 10:57:07.000000 qrules-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-21 10:57:07.000000 qrules-0.9.7/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-21 10:57:07.000000 qrules-0.9.7/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-02-21 10:57:07.000000 qrules-0.9.7/.pydocstyle
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-21 10:57:07.000000 qrules-0.9.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-21 10:57:07.000000 qrules-0.9.7/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-02-21 10:57:07.000000 qrules-0.9.7/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-02-21 10:57:07.000000 qrules-0.9.7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-02-21 10:57:07.000000 qrules-0.9.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-02-21 10:57:07.000000 qrules-0.9.7/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-02-21 10:57:07.000000 qrules-0.9.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-21 10:57:07.000000 qrules-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-02-21 10:57:18.284595 qrules-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-02-21 10:57:07.000000 qrules-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-02-21 10:57:07.000000 qrules-0.9.7/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-02-21 10:57:07.000000 qrules-0.9.7/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/.pydocstyle
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_relink_references.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_static/linebreaks-api.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_templates/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_templates/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_templates/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/_templates/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/docs/adr/
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/adr/template.md
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (121)    12308 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/references.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.276594 qrules-0.9.7/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/additional_particles.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11680 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/conservation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     7042 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/custom-topology.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9917 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/ls-coupling.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    13311 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/particle.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    18368 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/reaction.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11947 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage/visualize.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6308 2022-02-21 10:57:07.000000 qrules-0.9.7/docs/usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-21 10:57:07.000000 qrules-0.9.7/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-02-21 10:57:07.000000 qrules-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-02-21 10:57:07.000000 qrules-0.9.7/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-02-21 10:57:07.000000 qrules-0.9.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-02-21 10:57:18.284595 qrules-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-02-21 10:57:07.000000 qrules-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.268594 qrules-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/src/qrules/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    15459 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/_implementers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13033 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/_system_control.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/additional_definitions.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/argument_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)    19834 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/combinatorics.py
--rw-r--r--   0 runner    (1001) docker     (121)    31794 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/conservation_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/src/qrules/io/
--rw-r--r--   0 runner    (1001) docker     (121)     8841 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/io/_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    19727 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/io/_dot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/particle-validation.json
--rw-r--r--   0 runner    (1001) docker     (121)    25615 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/particle.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     7059 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/quantum_numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10962 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    43176 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/solving.py
--rw-r--r--   0 runner    (1001) docker     (121)    27386 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/topology.py
--rw-r--r--   0 runner    (1001) docker     (121)    37336 2022-02-21 10:57:07.000000 qrules-0.9.7/src/qrules/transition.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-21 10:57:17.000000 qrules-0.9.7/src/qrules/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/src/qrules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-02-21 10:57:18.000000 qrules-0.9.7/src/qrules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-02-21 10:57:18.000000 qrules-0.9.7/src/qrules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-21 10:57:18.000000 qrules-0.9.7/src/qrules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2022-02-21 10:57:18.000000 qrules-0.9.7/src/qrules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-21 10:57:18.000000 qrules-0.9.7/src/qrules.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/.pydocstyle
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/tests/channels/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/channels/test_d0_to_ks_kp_km.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/channels/test_jpsi_to_gamma_pi0_pi0.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/channels/test_nbody_reactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/channels/test_y_to_d0_d0bar_pi0_pi0.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/tests/output/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.280595 qrules-0.9.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.284595 qrules-0.9.7/tests/unit/conservation_rules/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_additive_qn.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_c_parity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5562 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_clebsch_gordan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_duck_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_g_parity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_gellmann_nishijima.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_helicity_conservation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_identical_particle_symmetrization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_parity_conservation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/conservation_rules/test_spin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.284595 qrules-0.9.7/tests/unit/io/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/io/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     9852 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/io/test_dot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/io/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_combinatorics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_parity_prefactor.py
--rw-r--r--   0 runner    (1001) docker     (121)    15671 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_particle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_pdg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_qrules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_quantum_numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    16384 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_system_control.py
--rw-r--r--   0 runner    (1001) docker     (121)    11392 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (121)     7302 2022-02-21 10:57:07.000000 qrules-0.9.7/tests/unit/test_transition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-02-21 10:57:07.000000 qrules-0.9.7/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:18.284595 qrules-0.9.7/typings/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-21 10:57:07.000000 qrules-0.9.7/typings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-02-21 10:57:07.000000 qrules-0.9.7/typings/.pydocstyle
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-02-21 10:57:07.000000 qrules-0.9.7/typings/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-21 10:57:07.000000 qrules-0.9.7/typings/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.932493 qrules-0.9.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.912493 qrules-0.9.8/.constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-13 16:38:03.000000 qrules-0.9.8/.constraints/py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-13 16:38:03.000000 qrules-0.9.8/.cspell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 16:38:03.000000 qrules-0.9.8/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-13 16:38:03.000000 qrules-0.9.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.912493 qrules-0.9.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.912493 qrules-0.9.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.912493 qrules-0.9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/clean-caches.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/pr-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-13 16:38:03.000000 qrules-0.9.8/.github/workflows/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 16:38:03.000000 qrules-0.9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-13 16:38:03.000000 qrules-0.9.8/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 16:38:03.000000 qrules-0.9.8/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 16:38:03.000000 qrules-0.9.8/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-13 16:38:03.000000 qrules-0.9.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 16:38:03.000000 qrules-0.9.8/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 16:38:03.000000 qrules-0.9.8/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 16:38:03.000000 qrules-0.9.8/.pydocstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-13 16:38:03.000000 qrules-0.9.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-13 16:38:03.000000 qrules-0.9.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 16:38:03.000000 qrules-0.9.8/.taplo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.916493 qrules-0.9.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-13 16:38:03.000000 qrules-0.9.8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-13 16:38:03.000000 qrules-0.9.8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 16:38:03.000000 qrules-0.9.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-13 16:38:03.000000 qrules-0.9.8/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 16:38:03.000000 qrules-0.9.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:38:03.000000 qrules-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-13 16:38:14.932493 qrules-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-13 16:38:03.000000 qrules-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-13 16:38:03.000000 qrules-0.9.8/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 16:38:03.000000 qrules-0.9.8/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.916493 qrules-0.9.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/.pydocstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_relink_references.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.916493 qrules-0.9.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_static/linebreaks-api.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.916493 qrules-0.9.8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_templates/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_templates/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_templates/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/_templates/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.916493 qrules-0.9.8/docs/adr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/adr/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.920493 qrules-0.9.8/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/additional_particles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/conservation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/custom-topology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/ls-coupling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/particle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/reaction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage/visualize.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-13 16:38:03.000000 qrules-0.9.8/docs/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 16:38:03.000000 qrules-0.9.8/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 16:38:03.000000 qrules-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-13 16:38:03.000000 qrules-0.9.8/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-13 16:38:03.000000 qrules-0.9.8/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-13 16:38:14.932493 qrules-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 16:38:03.000000 qrules-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.908493 qrules-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.920493 qrules-0.9.8/src/qrules/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/_implementers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/_system_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/additional_definitions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/argument_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/combinatorics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31339 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/conservation_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.924493 qrules-0.9.8/src/qrules/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/io/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/io/_dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/particle-validation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25539 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/quantum_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42366 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/solving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37686 2023-04-13 16:38:03.000000 qrules-0.9.8/src/qrules/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.924493 qrules-0.9.8/src/qrules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 16:38:14.000000 qrules-0.9.8/src/qrules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.924493 qrules-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/.pydocstyle
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.924493 qrules-0.9.8/tests/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_d0_to_ks_kp_km.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_jpsi_to_gamma_pi0_pi0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_lc_to_p_km_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_nbody_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_psi2s_to_eta_k_kstar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/channels/test_y_to_d0_d0bar_pi0_pi0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.924493 qrules-0.9.8/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.928493 qrules-0.9.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.932493 qrules-0.9.8/tests/unit/conservation_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_additive_qn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_c_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_clebsch_gordan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_duck_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_g_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_gellmann_nishijima.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_helicity_conservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_identical_particle_symmetrization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_parity_conservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/conservation_rules/test_spin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.932493 qrules-0.9.8/tests/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/io/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/io/test_dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/io/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_combinatorics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_final_state_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_parity_prefactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16096 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_pdg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_qrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_quantum_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_system_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-13 16:38:03.000000 qrules-0.9.8/tests/unit/test_transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-13 16:38:03.000000 qrules-0.9.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:14.932493 qrules-0.9.8/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 16:38:03.000000 qrules-0.9.8/typings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 16:38:03.000000 qrules-0.9.8/typings/.pydocstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 16:38:03.000000 qrules-0.9.8/typings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:38:03.000000 qrules-0.9.8/typings/__init__.pyi
```

### Comparing `qrules-0.9.7/.constraints/py3.10.txt` & `qrules-0.9.8/.constraints/py3.7.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,203 +1,198 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.7
+# by the following command:
 #
-#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.10.txt --strip-extras setup.py
+#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.7.txt --strip-extras setup.py
 #
-alabaster==0.7.12
-anyio==3.5.0
+accessible-pygments==0.0.4
+aiofiles==22.1.0
+aiosqlite==0.18.0
+alabaster==0.7.13
+anyio==3.6.2
 aquirdturtle-collapsible-headings==3.1.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
-astroid==2.9.3
-asttokens==2.0.5
-attrs==21.4.0
-babel==2.9.1
+arrow==1.2.3
+astroid==2.15.2
+attrs==22.2.0
+babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.10.0
-black==22.1.0
-bleach==4.1.0
-certifi==2021.10.8
-cffi==1.15.0
+beautifulsoup4==4.12.2
+black==23.3.0
+bleach==6.0.0
+cached-property==1.5.2
+certifi==2022.12.7
+cffi==1.15.1
 cfgv==3.3.1
-charset-normalizer==2.0.12
-click==8.0.4
-colorama==0.4.4
-coverage==6.3.2
-debugpy==1.5.1
+charset-normalizer==3.1.0
+click==8.1.3
+colorama==0.4.6
+coverage==7.2.3
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 deprecated==1.2.13
-distlib==0.3.4
-docutils==0.16
+dill==0.3.6
+distlib==0.3.6
+docutils==0.19
 entrypoints==0.4
+exceptiongroup==1.1.1
 execnet==1.9.0
-executing==0.8.2
-filelock==3.6.0
-flake8==4.0.1
-flake8-blind-except==0.2.0
-flake8-bugbear==22.1.11
-flake8-builtins==1.5.3
-flake8-comprehensions==3.8.0
-flake8-plugin-utils==1.3.2
-flake8-polyfill==1.0.2
-flake8-pytest-style==1.6.0
-flake8-rst-docstrings==0.2.5
-flake8-type-ignore==0.1.0.post2 ; python_version >= "3.8.0"
-flake8-use-fstring==1.3
-gitdb==4.0.9
-gitpython==3.1.27
-gprof2dot==2021.2.21
-graphviz==0.19.1
-greenlet==1.1.2
-hepunits==2.2.0
-identify==2.4.10
-idna==3.3
-imagesize==1.3.0
-importlib-metadata==4.11.1
-iniconfig==1.1.1
-ipykernel==6.9.1
-ipython==8.0.1
+fastjsonschema==2.16.3
+filelock==3.11.0
+fqdn==1.5.1
+gprof2dot==2022.7.29
+graphviz==0.20.1
+greenlet==2.0.2
+hepunits==2.3.2
+identify==2.5.22
+idna==3.4
+imagesize==1.4.1
+importlib-metadata==4.13.0 ; python_version < "3.8.0"
+importlib-resources==5.12.0
+iniconfig==2.0.0
+ipykernel==6.16.2
+ipython==7.34.0
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
-isort==5.10.1
-jedi==0.18.1
-jinja2==3.0.3
-json5==0.9.6
-jsonschema==4.4.0
-jupyter==1.0.0
-jupyter-cache==0.4.3
-jupyter-client==7.1.2
-jupyter-console==6.4.0
-jupyter-core==4.9.2
-jupyter-server==1.13.5
-jupyter-server-mathjax==0.2.4
-jupyter-sphinx==0.3.2
-jupyterlab==3.2.9
-jupyterlab-code-formatter==1.4.10
-jupyterlab-markup==1.0.1
-jupyterlab-myst==0.1.6 ; python_version >= "3.7.0"
-jupyterlab-pygments==0.1.2
-jupyterlab-server==2.10.3
-jupyterlab-widgets==1.0.2
+ipywidgets==8.0.6
+isoduration==20.11.0
+isort==5.11.5
+jedi==0.18.2
+jinja2==3.1.2
+json5==0.9.11
+jsonpointer==2.3
+jsonschema==4.17.3
+jupyter-cache==0.5.0
+jupyter-client==7.4.9
+jupyter-core==4.12.0
+jupyter-events==0.6.3
+jupyter-server==1.23.6
+jupyter-server-fileid==0.9.0
+jupyter-server-ydoc==0.8.0
+jupyter-ydoc==0.2.4
+jupyterlab==3.6.3
+jupyterlab-code-formatter==1.6.0
+jupyterlab-myst==1.1.3 ; python_version >= "3.7.0"
+jupyterlab-pygments==0.2.2
+jupyterlab-server==2.22.0
+jupyterlab-widgets==3.0.7
 latexcodec==2.0.1
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
 livereload==2.6.3
-markdown-it-py==1.1.0
-markupsafe==2.1.0
-matplotlib-inline==0.1.3
-mccabe==0.6.1
-mdit-py-plugins==0.2.8
-mistune==0.8.4
-mypy==0.931
-mypy-extensions==0.4.3
-myst-nb==0.13.2
-myst-parser==0.15.2
-nbclassic==0.3.5
-nbclient==0.5.11
-nbconvert==6.4.2
-nbdime==3.1.1
-nbformat==5.1.3
-nbmake==1.2
-nest-asyncio==1.5.4
-nodeenv==1.6.0
-notebook==6.4.8
-packaging==21.3
+markdown-it-py==2.2.0
+markupsafe==2.1.2
+matplotlib-inline==0.1.6
+mccabe==0.7.0
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==2.0.5
+mypy==1.2.0
+mypy-extensions==1.0.0
+myst-nb==0.17.1
+myst-parser==0.18.1
+nbclassic==0.5.5
+nbclient==0.5.13
+nbconvert==7.3.1
+nbformat==5.8.0
+nbmake==1.2.1
+nest-asyncio==1.5.6
+nodeenv==1.7.0
+notebook==6.5.4
+notebook-shim==0.2.2
+packaging==23.1
 pandocfilters==1.5.0
 parso==0.8.3
-particle==0.20.0
-pathspec==0.9.0
-pep517==0.12.0
-pep8-naming==0.12.1
+particle==0.22.0
+pathspec==0.11.1
 pexpect==4.8.0
 pickleshare==0.7.5
-pip-tools==6.5.1
-platformdirs==2.5.1
+pkgutil-resolve-name==1.3.10
+platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==2.17.0
-prometheus-client==0.13.1
-prompt-toolkit==3.0.28
+pre-commit==2.21.0
+prometheus-client==0.16.0
+prompt-toolkit==3.0.38
+psutil==5.9.4
 ptyprocess==0.7.0
-pure-eval==0.2.2
 py==1.11.0
 pybtex==0.24.0
-pybtex-docutils==1.0.1
-pycodestyle==2.8.0
+pybtex-docutils==1.0.2
 pycparser==2.21
-pydantic==1.9.0
-pydata-sphinx-theme==0.7.2
-pydocstyle==6.1.1
+pydantic==1.10.7
+pydata-sphinx-theme==0.13.3
+pydocstyle==6.3.0
 pydot==1.4.2
-pyflakes==2.4.0
-pygments==2.11.2
-pylint==2.12.2
-pyparsing==3.0.7
-pyrsistent==0.18.1
-pytest==6.2.5
-pytest-cov==3.0.0
-pytest-forked==1.4.0
+pygments==2.15.0
+pylint==2.17.2
+pyparsing==3.0.9
+pyrsistent==0.19.3
+pytest==7.3.0
+pytest-cov==4.0.0
 pytest-profiling==1.7.0
-pytest-xdist==2.5.0
+pytest-xdist==3.2.1
 python-constraint==1.4.0
 python-dateutil==2.8.2
-pytz==2021.3
+python-json-logger==2.0.7
+pytz==2023.3
 pyyaml==6.0
-pyzmq==22.3.0
-qtconsole==5.2.2
-qtpy==2.0.1
-requests==2.27.1
-restructuredtext-lint==1.3.2
+pyzmq==25.0.2
+requests==2.28.2
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
 send2trash==1.8.0
 six==1.16.0
-smmap==5.0.0
-sniffio==1.2.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
-sphinx==4.4.0
+soupsieve==2.4
+sphinx==5.3.0
 sphinx-autobuild==2021.3.14
-sphinx-book-theme==0.2.0
-sphinx-codeautolink==0.10.0
+sphinx-book-theme==1.0.1
+sphinx-codeautolink==0.14.1
 sphinx-comments==0.0.3
-sphinx-copybutton==0.5.0
-sphinx-panels==0.6.0
-sphinx-thebe==0.1.1
-sphinx-togglebutton==0.3.0
+sphinx-copybutton==0.5.1
+sphinx-design==0.4.1
+sphinx-thebe==0.2.1
+sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.2
-sphinxcontrib-bibtex==2.4.1
+sphinxcontrib-bibtex==2.5.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-hep-pdgref==0.1.4
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sphobjinv==2.2.1
-sqlalchemy==1.4.31
-stack-data==0.2.0
-terminado==0.13.1
-testpath==0.5.0
-toml==0.10.2
+sphobjinv==2.3.1
+sqlalchemy==1.4.47
+tabulate==0.9.0
+terminado==0.17.1
+tinycss2==1.2.1
 tomli==2.0.1
-tornado==6.1
-tox==3.24.5
-tqdm==4.62.3
-traitlets==5.1.1
-types-docutils==0.17.6
+tomlkit==0.11.7
+tornado==6.2
+tox==3.28.0 ; python_version < "3.8.0"
+tqdm==4.65.0
+traitlets==5.9.0
+typed-ast==1.5.4
+types-docutils==0.19.1.7
 types-pkg-resources==0.1.3
-types-pyyaml==6.0.4
-types-requests==2.27.10
-types-setuptools==57.4.9
-types-urllib3==1.26.9
-typing-extensions==4.1.1
-urllib3==1.26.8
-virtualenv==20.13.1
-wcwidth==0.2.5
+types-pyyaml==6.0.12.9
+types-requests==2.28.11.17
+types-setuptools==67.6.0.7
+types-urllib3==1.26.25.10
+typing-extensions==4.5.0 ; python_version < "3.10.0"
+uri-template==1.2.0
+urllib3==1.26.15
+virtualenv==20.21.0
+wcwidth==0.2.6
+webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.2.3
-wheel==0.37.1
-widgetsnbextension==3.5.2
-wrapt==1.13.3
-zipp==3.7.0
+websocket-client==1.5.1
+wheel==0.40.0
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+y-py==0.5.9
+ypy-websocket==0.8.2 ; python_version >= "3.7.0"
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `qrules-0.9.7/.constraints/py3.6.txt` & `qrules-0.9.8/.constraints/py3.6.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,200 +1,178 @@
 #
 # This file is autogenerated by pip-compile with python 3.6
 # To update, run:
 #
 #    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.6.txt --strip-extras setup.py
 #
-alabaster==0.7.12
-anyio==3.5.0
+alabaster==0.7.13
+anyio==3.6.2
 aquirdturtle-collapsible-headings==3.1.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
-astroid==2.9.3
+astroid==2.11.7
 async-generator==1.10
 attrs==21.4.0
-babel==2.9.1
+babel==2.11.0
 backcall==0.2.0
-beautifulsoup4==4.10.0
-black==22.1.0
+beautifulsoup4==4.12.2
+black==22.8.0
 bleach==4.1.0
-certifi==2021.10.8
-cffi==1.15.0
+certifi==2022.12.7
+cffi==1.15.1
 cfgv==3.3.1
 charset-normalizer==2.0.12
 click==8.0.4
-colorama==0.4.4
+colorama==0.4.5
 contextvars==2.4
 coverage==6.2
 dataclasses==0.8
 decorator==5.1.1
 defusedxml==0.7.1
-deprecated==1.2.13
-distlib==0.3.4
+dill==0.3.4
+distlib==0.3.6
 docutils==0.16
 entrypoints==0.4
 execnet==1.9.0
 filelock==3.4.1
-flake8==4.0.1
-flake8-blind-except==0.2.0
-flake8-bugbear==22.1.11
-flake8-builtins==1.5.3
-flake8-comprehensions==3.7.0
-flake8-plugin-utils==1.3.2
-flake8-polyfill==1.0.2
-flake8-pytest-style==1.6.0
-flake8-rst-docstrings==0.2.5
-flake8-use-fstring==1.3
 gitdb==4.0.9
 gitpython==3.1.18
-gprof2dot==2021.2.21
+gprof2dot==2022.7.29
 graphviz==0.19.1
-greenlet==1.1.2
-hepunits==2.2.0
+greenlet==2.0.2
+hepunits==2.2.1
 identify==2.4.4
-idna==3.3
-imagesize==1.3.0
-immutables==0.16
-importlib-metadata==4.2.0
+idna==3.4
+imagesize==1.4.1
+immutables==0.19
+importlib-metadata==4.8.3 ; python_version < "3.8.0"
 importlib-resources==3.0.0
 iniconfig==1.1.1
 ipykernel==5.5.6
 ipython==7.16.3
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
+ipywidgets==7.7.5
 isort==5.10.1
 jedi==0.17.2
 jinja2==3.0.3
-json5==0.9.6
+json5==0.9.11
 jsonschema==3.2.0
-jupyter==1.0.0
 jupyter-cache==0.4.3
 jupyter-client==7.1.2
-jupyter-console==6.4.0
 jupyter-core==4.9.2
 jupyter-server==1.13.1
 jupyter-server-mathjax==0.2.3
 jupyter-sphinx==0.3.2
 jupyterlab==3.2.9
-jupyterlab-code-formatter==1.4.10
+jupyterlab-code-formatter==1.6.0
 jupyterlab-pygments==0.1.2
 jupyterlab-server==2.10.3
-jupyterlab-widgets==1.0.2
+jupyterlab-widgets==1.1.4
 latexcodec==2.0.1
 lazy-object-proxy==1.7.1
 livereload==2.6.3
 markdown-it-py==1.1.0
 markupsafe==2.0.1
-mccabe==0.6.1
+mccabe==0.7.0
 mdit-py-plugins==0.2.8
 mistune==0.8.4
-mypy==0.931
-mypy-extensions==0.4.3
+mypy==0.971
+mypy-extensions==1.0.0
 myst-nb==0.13.2
 myst-parser==0.15.2
 nbclassic==0.3.5
 nbclient==0.5.9
 nbconvert==6.0.7
 nbdime==3.1.1
 nbformat==5.1.3
-nbmake==1.2
-nest-asyncio==1.5.4
+nbmake==1.2.1
+nest-asyncio==1.5.6
 nodeenv==1.6.0
-notebook==6.4.8
+notebook==6.4.10
 packaging==21.3
 pandocfilters==1.5.0
 parso==0.7.1
-particle==0.20.0
+particle==0.20.1
 pathspec==0.9.0
-pep517==0.12.0
-pep8-naming==0.12.1
 pexpect==4.8.0
 pickleshare==0.7.5
-pip-tools==6.4.0
 platformdirs==2.4.0
 pluggy==1.0.0
 pre-commit==2.17.0
-prometheus-client==0.13.1
-prompt-toolkit==3.0.28
+prometheus-client==0.16.0
+prompt-toolkit==3.0.36
 ptyprocess==0.7.0
 py==1.11.0
 pybtex==0.24.0
-pybtex-docutils==1.0.1
-pycodestyle==2.8.0
+pybtex-docutils==1.0.2
 pycparser==2.21
-pydantic==1.9.0
+pydantic==1.9.2
 pydata-sphinx-theme==0.7.2
-pydocstyle==6.1.1
+pydocstyle==6.3.0
 pydot==1.4.2
-pyflakes==2.4.0
-pygments==2.11.2
-pylint==2.12.2
-pyparsing==3.0.7
+pygments==2.14.0
+pylint==2.13.9
+pyparsing==3.0.9
 pyrsistent==0.18.0
-pytest==6.2.5
-pytest-cov==3.0.0
-pytest-forked==1.4.0
+pytest==7.0.1
+pytest-cov==4.0.0
 pytest-profiling==1.7.0
-pytest-xdist==2.5.0
+pytest-xdist==3.0.2
 python-constraint==1.4.0
 python-dateutil==2.8.2
-pytz==2021.3
+pytz==2023.3
 pyyaml==6.0
-pyzmq==22.3.0
-qtconsole==5.2.2
-qtpy==2.0.1
+pyzmq==25.0.2
 requests==2.27.1
-restructuredtext-lint==1.3.2
 send2trash==1.8.0
 six==1.16.0
 smmap==5.0.0
 sniffio==1.2.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
-sphinx==4.3.2 ; python_version < "3.8.0"
+soupsieve==2.3.2.post1
+sphinx==4.5.0
 sphinx-autobuild==2021.3.14
 sphinx-book-theme==0.2.0
-sphinx-codeautolink==0.10.0
+sphinx-codeautolink==0.12.1
 sphinx-comments==0.0.3
 sphinx-copybutton==0.5.0
-sphinx-panels==0.6.0
-sphinx-thebe==0.1.1
-sphinx-togglebutton==0.3.0
+sphinx-design==0.0.13
+sphinx-thebe==0.2.1
+sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.2
-sphinxcontrib-bibtex==2.4.1
+sphinxcontrib-bibtex==2.5.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-hep-pdgref==0.1.4
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sphobjinv==2.2.1
-sqlalchemy==1.4.31
+sphobjinv==2.3.1
+sqlalchemy==1.4.47
 terminado==0.12.1
-testpath==0.5.0
+testpath==0.6.0
 toml==0.10.2
 tomli==1.2.3
 tornado==6.1
-tox==3.24.5
-tqdm==4.62.3
+tox==3.28.0 ; python_version < "3.8.0"
+tqdm==4.64.1
 traitlets==4.3.3
-typed-ast==1.5.2
-types-docutils==0.17.6
+typed-ast==1.5.4
+types-docutils==0.19.1.7
 types-pkg-resources==0.1.3
-types-pyyaml==6.0.4
-types-requests==2.27.10
-types-setuptools==57.4.9
-types-urllib3==1.26.9
-typing-extensions==4.1.1 ; python_version < "3.8.0"
-urllib3==1.26.8
-virtualenv==20.13.1
-wcwidth==0.2.5
+types-pyyaml==6.0.12.9
+types-requests==2.28.11.17
+types-setuptools==67.6.0.7
+types-urllib3==1.26.25.10
+typing-extensions==4.1.1 ; python_version < "3.10.0"
+urllib3==1.26.15
+virtualenv==20.15.1 ; python_version < "3.7.0"
+wcwidth==0.2.6
 webencodings==0.5.1
-websocket-client==1.2.3
+websocket-client==1.3.1
 wheel==0.37.1
-widgetsnbextension==3.5.2
-wrapt==1.13.3
+widgetsnbextension==3.6.4
+wrapt==1.15.0
 zipp==3.6.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `qrules-0.9.7/.constraints/py3.7.txt` & `qrules-0.9.8/.constraints/py3.11.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,213 @@
 #
-# This file is autogenerated by pip-compile with python 3.7
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.7.txt --strip-extras setup.py
+#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.11.txt --strip-extras setup.py
 #
-alabaster==0.7.12
-anyio==3.5.0
+accessible-pygments==0.0.4
+aiofiles==22.1.0
+aiosqlite==0.18.0
+alabaster==0.7.13
+anyio==3.6.2
 aquirdturtle-collapsible-headings==3.1.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
-astroid==2.9.3
-attrs==21.4.0
-babel==2.9.1
+arrow==1.2.3
+astroid==2.15.2
+asttokens==2.2.1
+attrs==22.2.0
+babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.10.0
-black==22.1.0
-bleach==4.1.0
-certifi==2021.10.8
-cffi==1.15.0
+beautifulsoup4==4.12.2
+black==23.3.0
+bleach==6.0.0
+cachetools==5.3.0
+certifi==2022.12.7
+cffi==1.15.1
 cfgv==3.3.1
-charset-normalizer==2.0.12
-click==8.0.4
-colorama==0.4.4
-coverage==6.3.2
-debugpy==1.5.1
+chardet==5.1.0
+charset-normalizer==3.1.0
+click==8.1.3
+colorama==0.4.6
+comm==0.1.3
+coverage==7.2.3
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 deprecated==1.2.13
-distlib==0.3.4
-docutils==0.16
-entrypoints==0.4
+dill==0.3.6
+distlib==0.3.6
+docutils==0.19
 execnet==1.9.0
-filelock==3.6.0
-flake8==4.0.1
-flake8-blind-except==0.2.0
-flake8-bugbear==22.1.11
-flake8-builtins==1.5.3
-flake8-comprehensions==3.8.0
+executing==1.2.0
+fastjsonschema==2.16.3
+filelock==3.11.0
+flake8==6.0.0 ; python_version >= "3.8.0"
+flake8-blind-except==0.2.1 ; python_version >= "3.8.0"
+flake8-bugbear==23.3.23 ; python_version >= "3.8.0"
+flake8-builtins==2.1.0 ; python_version >= "3.8.0"
+flake8-comprehensions==3.12.0 ; python_version >= "3.8.0"
+flake8-future-import==0.4.7 ; python_version >= "3.8.0"
 flake8-plugin-utils==1.3.2
-flake8-polyfill==1.0.2
-flake8-pytest-style==1.6.0
-flake8-rst-docstrings==0.2.5
-flake8-use-fstring==1.3
-gitdb==4.0.9
-gitpython==3.1.27
-gprof2dot==2021.2.21
-graphviz==0.19.1
-greenlet==1.1.2
-hepunits==2.2.0
-identify==2.4.10
-idna==3.3
-imagesize==1.3.0
-importlib-metadata==4.2.0
-importlib-resources==5.4.0
-iniconfig==1.1.1
-ipykernel==6.9.1
-ipython==7.31.1
+flake8-pytest-style==1.7.2 ; python_version >= "3.8.0"
+flake8-rst-docstrings==0.3.0 ; python_version >= "3.8.0"
+flake8-type-ignore==0.1.0.post2 ; python_version >= "3.8.0"
+flake8-use-fstring==1.4 ; python_version >= "3.8.0"
+fqdn==1.5.1
+gprof2dot==2022.7.29
+graphviz==0.20.1
+greenlet==2.0.2
+hepunits==2.3.2
+identify==2.5.22
+idna==3.4
+imagesize==1.4.1
+importlib-metadata==6.3.0
+iniconfig==2.0.0
+ipykernel==6.22.0
+ipython==8.12.0
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
-isort==5.10.1
-jedi==0.18.1
-jinja2==3.0.3
-json5==0.9.6
-jsonschema==4.4.0
-jupyter==1.0.0
-jupyter-cache==0.4.3
-jupyter-client==7.1.2
-jupyter-console==6.4.0
-jupyter-core==4.9.2
-jupyter-server==1.13.5
-jupyter-server-mathjax==0.2.4
-jupyter-sphinx==0.3.2
-jupyterlab==3.2.9
-jupyterlab-code-formatter==1.4.10
-jupyterlab-markup==1.0.1
-jupyterlab-myst==0.1.6 ; python_version >= "3.7.0"
-jupyterlab-pygments==0.1.2
-jupyterlab-server==2.10.3
-jupyterlab-widgets==1.0.2
+ipywidgets==8.0.6
+isoduration==20.11.0
+isort==5.12.0
+jedi==0.18.2
+jinja2==3.1.2
+json5==0.9.11
+jsonpointer==2.3
+jsonschema==4.17.3
+jupyter-cache==0.5.0
+jupyter-client==8.1.0
+jupyter-core==5.3.0
+jupyter-events==0.6.3
+jupyter-server==2.5.0
+jupyter-server-fileid==0.9.0
+jupyter-server-terminals==0.4.4
+jupyter-server-ydoc==0.8.0
+jupyter-ydoc==0.2.4
+jupyterlab==3.6.3
+jupyterlab-code-formatter==1.6.0
+jupyterlab-myst==1.1.3 ; python_version >= "3.7.0"
+jupyterlab-pygments==0.2.2
+jupyterlab-server==2.22.0
+jupyterlab-widgets==3.0.7
 latexcodec==2.0.1
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
 livereload==2.6.3
-markdown-it-py==1.1.0
-markupsafe==2.1.0
-matplotlib-inline==0.1.3
-mccabe==0.6.1
-mdit-py-plugins==0.2.8
-mistune==0.8.4
-mypy==0.931
-mypy-extensions==0.4.3
-myst-nb==0.13.2
-myst-parser==0.15.2
-nbclassic==0.3.5
-nbclient==0.5.11
-nbconvert==6.4.2
-nbdime==3.1.1
-nbformat==5.1.3
-nbmake==1.2
-nest-asyncio==1.5.4
-nodeenv==1.6.0
-notebook==6.4.8
-packaging==21.3
+markdown-it-py==2.2.0
+markupsafe==2.1.2
+matplotlib-inline==0.1.6
+mccabe==0.7.0
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==2.0.5
+mypy==1.2.0
+mypy-extensions==1.0.0
+myst-nb==0.17.1
+myst-parser==0.18.1
+nbclassic==0.5.5
+nbclient==0.5.13
+nbconvert==7.3.1
+nbformat==5.8.0
+nbmake==1.2.1
+nest-asyncio==1.5.6
+nodeenv==1.7.0
+notebook==6.5.4
+notebook-shim==0.2.2
+packaging==23.1
 pandocfilters==1.5.0
 parso==0.8.3
-particle==0.20.0
-pathspec==0.9.0
-pep517==0.12.0
-pep8-naming==0.12.1
+particle==0.22.0
+pathspec==0.11.1
+pep8-naming==0.13.3 ; python_version >= "3.8.0"
 pexpect==4.8.0
 pickleshare==0.7.5
-pip-tools==6.5.1
-platformdirs==2.5.1
+platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==2.17.0
-prometheus-client==0.13.1
-prompt-toolkit==3.0.28
+pre-commit==3.2.2
+prometheus-client==0.16.0
+prompt-toolkit==3.0.38
+psutil==5.9.4
 ptyprocess==0.7.0
-py==1.11.0
+pure-eval==0.2.2
 pybtex==0.24.0
-pybtex-docutils==1.0.1
-pycodestyle==2.8.0
+pybtex-docutils==1.0.2
+pycodestyle==2.10.0
 pycparser==2.21
-pydantic==1.9.0
-pydata-sphinx-theme==0.7.2
-pydocstyle==6.1.1
+pydantic==1.10.7
+pydata-sphinx-theme==0.13.3
+pydocstyle==6.3.0
 pydot==1.4.2
-pyflakes==2.4.0
-pygments==2.11.2
-pylint==2.12.2
-pyparsing==3.0.7
-pyrsistent==0.18.1
-pytest==6.2.5
-pytest-cov==3.0.0
-pytest-forked==1.4.0
+pyflakes==3.0.1
+pygments==2.15.0
+pylint==2.17.2
+pyparsing==3.0.9
+pyproject-api==1.5.1
+pyrsistent==0.19.3
+pytest==7.3.0
+pytest-cov==4.0.0
 pytest-profiling==1.7.0
-pytest-xdist==2.5.0
+pytest-xdist==3.2.1
 python-constraint==1.4.0
 python-dateutil==2.8.2
-pytz==2021.3
+python-json-logger==2.0.7
 pyyaml==6.0
-pyzmq==22.3.0
-qtconsole==5.2.2
-qtpy==2.0.1
-requests==2.27.1
-restructuredtext-lint==1.3.2
+pyzmq==25.0.2
+requests==2.28.2
+restructuredtext-lint==1.4.0
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
 send2trash==1.8.0
 six==1.16.0
-smmap==5.0.0
-sniffio==1.2.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
-sphinx==4.3.2 ; python_version < "3.8.0"
+soupsieve==2.4
+sphinx==5.3.0
 sphinx-autobuild==2021.3.14
-sphinx-book-theme==0.2.0
-sphinx-codeautolink==0.10.0
+sphinx-book-theme==1.0.1
+sphinx-codeautolink==0.14.1
 sphinx-comments==0.0.3
-sphinx-copybutton==0.5.0
-sphinx-panels==0.6.0
-sphinx-thebe==0.1.1
-sphinx-togglebutton==0.3.0
-sphinxcontrib-applehelp==1.0.2
-sphinxcontrib-bibtex==2.4.1
+sphinx-copybutton==0.5.1
+sphinx-design==0.4.1
+sphinx-thebe==0.2.1
+sphinx-togglebutton==0.3.2
+sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-bibtex==2.5.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-hep-pdgref==0.1.4
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sphobjinv==2.2.1
-sqlalchemy==1.4.31
-terminado==0.13.1
-testpath==0.5.0
-toml==0.10.2
-tomli==2.0.1
-tornado==6.1
-tox==3.24.5
-tqdm==4.62.3
-traitlets==5.1.1
-typed-ast==1.5.2
-types-docutils==0.17.6
+sphobjinv==2.3.1
+sqlalchemy==1.4.47
+stack-data==0.6.2
+tabulate==0.9.0
+terminado==0.17.1
+tinycss2==1.2.1
+tomlkit==0.11.7
+tornado==6.2
+tox==4.4.11
+tqdm==4.65.0
+traitlets==5.9.0
+types-docutils==0.19.1.7
 types-pkg-resources==0.1.3
-types-pyyaml==6.0.4
-types-requests==2.27.10
-types-setuptools==57.4.9
-types-urllib3==1.26.9
-typing-extensions==4.1.1 ; python_version < "3.8.0"
-urllib3==1.26.8
-virtualenv==20.13.1
-wcwidth==0.2.5
+types-pyyaml==6.0.12.9
+types-requests==2.28.11.17
+types-setuptools==67.6.0.7
+types-urllib3==1.26.25.10
+typing-extensions==4.5.0
+uri-template==1.2.0
+urllib3==1.26.15
+virtualenv==20.21.0
+wcwidth==0.2.6
+webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.2.3
-wheel==0.37.1
-widgetsnbextension==3.5.2
-wrapt==1.13.3
-zipp==3.7.0
+websocket-client==1.5.1
+wheel==0.40.0
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+y-py==0.5.9
+ypy-websocket==0.8.2 ; python_version >= "3.7.0"
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `qrules-0.9.7/.constraints/py3.8.txt` & `qrules-0.9.8/.constraints/py3.10.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,215 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.8.txt --strip-extras setup.py
+#    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.10.txt --strip-extras setup.py
 #
-alabaster==0.7.12
-anyio==3.5.0
+accessible-pygments==0.0.4
+aiofiles==22.1.0
+aiosqlite==0.18.0
+alabaster==0.7.13
+anyio==3.6.2
 aquirdturtle-collapsible-headings==3.1.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
-astroid==2.9.3
-asttokens==2.0.5
-attrs==21.4.0
-babel==2.9.1
+arrow==1.2.3
+astroid==2.15.2
+asttokens==2.2.1
+attrs==22.2.0
+babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.10.0
-black==22.1.0
-bleach==4.1.0
-certifi==2021.10.8
-cffi==1.15.0
+beautifulsoup4==4.12.2
+black==23.3.0
+bleach==6.0.0
+cachetools==5.3.0
+certifi==2022.12.7
+cffi==1.15.1
 cfgv==3.3.1
-charset-normalizer==2.0.12
-click==8.0.4
-colorama==0.4.4
-coverage==6.3.2
-debugpy==1.5.1
+chardet==5.1.0
+charset-normalizer==3.1.0
+click==8.1.3
+colorama==0.4.6
+comm==0.1.3
+coverage==7.2.3
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 deprecated==1.2.13
-distlib==0.3.4
-docutils==0.16
-entrypoints==0.4
+dill==0.3.6
+distlib==0.3.6
+docutils==0.19
+exceptiongroup==1.1.1
 execnet==1.9.0
-executing==0.8.2
-filelock==3.6.0
-flake8==4.0.1
-flake8-blind-except==0.2.0
-flake8-bugbear==22.1.11
-flake8-builtins==1.5.3
-flake8-comprehensions==3.8.0
+executing==1.2.0
+fastjsonschema==2.16.3
+filelock==3.11.0
+flake8==6.0.0 ; python_version >= "3.8.0"
+flake8-blind-except==0.2.1 ; python_version >= "3.8.0"
+flake8-bugbear==23.3.23 ; python_version >= "3.8.0"
+flake8-builtins==2.1.0 ; python_version >= "3.8.0"
+flake8-comprehensions==3.12.0 ; python_version >= "3.8.0"
+flake8-future-import==0.4.7 ; python_version >= "3.8.0"
 flake8-plugin-utils==1.3.2
-flake8-polyfill==1.0.2
-flake8-pytest-style==1.6.0
-flake8-rst-docstrings==0.2.5
+flake8-pytest-style==1.7.2 ; python_version >= "3.8.0"
+flake8-rst-docstrings==0.3.0 ; python_version >= "3.8.0"
 flake8-type-ignore==0.1.0.post2 ; python_version >= "3.8.0"
-flake8-use-fstring==1.3
-gitdb==4.0.9
-gitpython==3.1.27
-gprof2dot==2021.2.21
-graphviz==0.19.1
-greenlet==1.1.2
-hepunits==2.2.0
-identify==2.4.10
-idna==3.3
-imagesize==1.3.0
-importlib-metadata==4.11.1
-importlib-resources==5.4.0
-iniconfig==1.1.1
-ipykernel==6.9.1
-ipython==8.0.1
+flake8-use-fstring==1.4 ; python_version >= "3.8.0"
+fqdn==1.5.1
+gprof2dot==2022.7.29
+graphviz==0.20.1
+greenlet==2.0.2
+hepunits==2.3.2
+identify==2.5.22
+idna==3.4
+imagesize==1.4.1
+importlib-metadata==6.3.0
+iniconfig==2.0.0
+ipykernel==6.22.0
+ipython==8.12.0
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
-isort==5.10.1
-jedi==0.18.1
-jinja2==3.0.3
-json5==0.9.6
-jsonschema==4.4.0
-jupyter==1.0.0
-jupyter-cache==0.4.3
-jupyter-client==7.1.2
-jupyter-console==6.4.0
-jupyter-core==4.9.2
-jupyter-server==1.13.5
-jupyter-server-mathjax==0.2.4
-jupyter-sphinx==0.3.2
-jupyterlab==3.2.9
-jupyterlab-code-formatter==1.4.10
-jupyterlab-markup==1.0.1
-jupyterlab-myst==0.1.6 ; python_version >= "3.7.0"
-jupyterlab-pygments==0.1.2
-jupyterlab-server==2.10.3
-jupyterlab-widgets==1.0.2
+ipywidgets==8.0.6
+isoduration==20.11.0
+isort==5.12.0
+jedi==0.18.2
+jinja2==3.1.2
+json5==0.9.11
+jsonpointer==2.3
+jsonschema==4.17.3
+jupyter-cache==0.5.0
+jupyter-client==8.1.0
+jupyter-core==5.3.0
+jupyter-events==0.6.3
+jupyter-server==2.5.0
+jupyter-server-fileid==0.9.0
+jupyter-server-terminals==0.4.4
+jupyter-server-ydoc==0.8.0
+jupyter-ydoc==0.2.4
+jupyterlab==3.6.3
+jupyterlab-code-formatter==1.6.0
+jupyterlab-myst==1.1.3 ; python_version >= "3.7.0"
+jupyterlab-pygments==0.2.2
+jupyterlab-server==2.22.0
+jupyterlab-widgets==3.0.7
 latexcodec==2.0.1
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
 livereload==2.6.3
-markdown-it-py==1.1.0
-markupsafe==2.1.0
-matplotlib-inline==0.1.3
-mccabe==0.6.1
-mdit-py-plugins==0.2.8
-mistune==0.8.4
-mypy==0.931
-mypy-extensions==0.4.3
-myst-nb==0.13.2
-myst-parser==0.15.2
-nbclassic==0.3.5
-nbclient==0.5.11
-nbconvert==6.4.2
-nbdime==3.1.1
-nbformat==5.1.3
-nbmake==1.2
-nest-asyncio==1.5.4
-nodeenv==1.6.0
-notebook==6.4.8
-packaging==21.3
+markdown-it-py==2.2.0
+markupsafe==2.1.2
+matplotlib-inline==0.1.6
+mccabe==0.7.0
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==2.0.5
+mypy==1.2.0
+mypy-extensions==1.0.0
+myst-nb==0.17.1
+myst-parser==0.18.1
+nbclassic==0.5.5
+nbclient==0.5.13
+nbconvert==7.3.1
+nbformat==5.8.0
+nbmake==1.2.1
+nest-asyncio==1.5.6
+nodeenv==1.7.0
+notebook==6.5.4
+notebook-shim==0.2.2
+packaging==23.1
 pandocfilters==1.5.0
 parso==0.8.3
-particle==0.20.0
-pathspec==0.9.0
-pep517==0.12.0
-pep8-naming==0.12.1
+particle==0.22.0
+pathspec==0.11.1
+pep8-naming==0.13.3 ; python_version >= "3.8.0"
 pexpect==4.8.0
 pickleshare==0.7.5
-pip-tools==6.5.1
-platformdirs==2.5.1
+platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==2.17.0
-prometheus-client==0.13.1
-prompt-toolkit==3.0.28
+pre-commit==3.2.2
+prometheus-client==0.16.0
+prompt-toolkit==3.0.38
+psutil==5.9.4
 ptyprocess==0.7.0
 pure-eval==0.2.2
-py==1.11.0
 pybtex==0.24.0
-pybtex-docutils==1.0.1
-pycodestyle==2.8.0
+pybtex-docutils==1.0.2
+pycodestyle==2.10.0
 pycparser==2.21
-pydantic==1.9.0
-pydata-sphinx-theme==0.7.2
-pydocstyle==6.1.1
+pydantic==1.10.7
+pydata-sphinx-theme==0.13.3
+pydocstyle==6.3.0
 pydot==1.4.2
-pyflakes==2.4.0
-pygments==2.11.2
-pylint==2.12.2
-pyparsing==3.0.7
-pyrsistent==0.18.1
-pytest==6.2.5
-pytest-cov==3.0.0
-pytest-forked==1.4.0
+pyflakes==3.0.1
+pygments==2.15.0
+pylint==2.17.2
+pyparsing==3.0.9
+pyproject-api==1.5.1
+pyrsistent==0.19.3
+pytest==7.3.0
+pytest-cov==4.0.0
 pytest-profiling==1.7.0
-pytest-xdist==2.5.0
+pytest-xdist==3.2.1
 python-constraint==1.4.0
 python-dateutil==2.8.2
-pytz==2021.3
+python-json-logger==2.0.7
 pyyaml==6.0
-pyzmq==22.3.0
-qtconsole==5.2.2
-qtpy==2.0.1
-requests==2.27.1
-restructuredtext-lint==1.3.2
+pyzmq==25.0.2
+requests==2.28.2
+restructuredtext-lint==1.4.0
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
 send2trash==1.8.0
 six==1.16.0
-smmap==5.0.0
-sniffio==1.2.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
-sphinx==4.4.0
+soupsieve==2.4
+sphinx==5.3.0
 sphinx-autobuild==2021.3.14
-sphinx-book-theme==0.2.0
-sphinx-codeautolink==0.10.0
+sphinx-book-theme==1.0.1
+sphinx-codeautolink==0.14.1
 sphinx-comments==0.0.3
-sphinx-copybutton==0.5.0
-sphinx-panels==0.6.0
-sphinx-thebe==0.1.1
-sphinx-togglebutton==0.3.0
-sphinxcontrib-applehelp==1.0.2
-sphinxcontrib-bibtex==2.4.1
+sphinx-copybutton==0.5.1
+sphinx-design==0.4.1
+sphinx-thebe==0.2.1
+sphinx-togglebutton==0.3.2
+sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-bibtex==2.5.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-hep-pdgref==0.1.4
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sphobjinv==2.2.1
-sqlalchemy==1.4.31
-stack-data==0.2.0
-terminado==0.13.1
-testpath==0.5.0
-toml==0.10.2
+sphobjinv==2.3.1
+sqlalchemy==1.4.47
+stack-data==0.6.2
+tabulate==0.9.0
+terminado==0.17.1
+tinycss2==1.2.1
 tomli==2.0.1
-tornado==6.1
-tox==3.24.5
-tqdm==4.62.3
-traitlets==5.1.1
-types-docutils==0.17.6
+tomlkit==0.11.7
+tornado==6.2
+tox==4.4.11
+tqdm==4.65.0
+traitlets==5.9.0
+types-docutils==0.19.1.7
 types-pkg-resources==0.1.3
-types-pyyaml==6.0.4
-types-requests==2.27.10
-types-setuptools==57.4.9
-types-urllib3==1.26.9
-typing-extensions==4.1.1
-urllib3==1.26.8
-virtualenv==20.13.1
-wcwidth==0.2.5
+types-pyyaml==6.0.12.9
+types-requests==2.28.11.17
+types-setuptools==67.6.0.7
+types-urllib3==1.26.25.10
+typing-extensions==4.5.0
+uri-template==1.2.0
+urllib3==1.26.15
+virtualenv==20.21.0
+wcwidth==0.2.6
+webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.2.3
-wheel==0.37.1
-widgetsnbextension==3.5.2
-wrapt==1.13.3
-zipp==3.7.0
+websocket-client==1.5.1
+wheel==0.40.0
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+y-py==0.5.9
+ypy-websocket==0.8.2 ; python_version >= "3.7.0"
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `qrules-0.9.7/.constraints/py3.9.txt` & `qrules-0.9.8/.constraints/py3.9.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,215 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile --extra=dev --no-annotate --output-file=.constraints/py3.9.txt --strip-extras setup.py
 #
-alabaster==0.7.12
-anyio==3.5.0
+accessible-pygments==0.0.4
+aiofiles==22.1.0
+aiosqlite==0.18.0
+alabaster==0.7.13
+anyio==3.6.2
 aquirdturtle-collapsible-headings==3.1.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
-astroid==2.9.3
-asttokens==2.0.5
-attrs==21.4.0
-babel==2.9.1
+arrow==1.2.3
+astroid==2.15.2
+asttokens==2.2.1
+attrs==22.2.0
+babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.10.0
-black==22.1.0
-bleach==4.1.0
-certifi==2021.10.8
-cffi==1.15.0
+beautifulsoup4==4.12.2
+black==23.3.0
+bleach==6.0.0
+cachetools==5.3.0
+certifi==2022.12.7
+cffi==1.15.1
 cfgv==3.3.1
-charset-normalizer==2.0.12
-click==8.0.4
-colorama==0.4.4
-coverage==6.3.2
-debugpy==1.5.1
+chardet==5.1.0
+charset-normalizer==3.1.0
+click==8.1.3
+colorama==0.4.6
+comm==0.1.3
+coverage==7.2.3
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 deprecated==1.2.13
-distlib==0.3.4
-docutils==0.16
-entrypoints==0.4
+dill==0.3.6
+distlib==0.3.6
+docutils==0.19
+exceptiongroup==1.1.1
 execnet==1.9.0
-executing==0.8.2
-filelock==3.6.0
-flake8==4.0.1
-flake8-blind-except==0.2.0
-flake8-bugbear==22.1.11
-flake8-builtins==1.5.3
-flake8-comprehensions==3.8.0
+executing==1.2.0
+fastjsonschema==2.16.3
+filelock==3.11.0
+flake8==6.0.0 ; python_version >= "3.8.0"
+flake8-blind-except==0.2.1 ; python_version >= "3.8.0"
+flake8-bugbear==23.3.23 ; python_version >= "3.8.0"
+flake8-builtins==2.1.0 ; python_version >= "3.8.0"
+flake8-comprehensions==3.12.0 ; python_version >= "3.8.0"
+flake8-future-import==0.4.7 ; python_version >= "3.8.0"
 flake8-plugin-utils==1.3.2
-flake8-polyfill==1.0.2
-flake8-pytest-style==1.6.0
-flake8-rst-docstrings==0.2.5
+flake8-pytest-style==1.7.2 ; python_version >= "3.8.0"
+flake8-rst-docstrings==0.3.0 ; python_version >= "3.8.0"
 flake8-type-ignore==0.1.0.post2 ; python_version >= "3.8.0"
-flake8-use-fstring==1.3
-gitdb==4.0.9
-gitpython==3.1.27
-gprof2dot==2021.2.21
-graphviz==0.19.1
-greenlet==1.1.2
-hepunits==2.2.0
-identify==2.4.10
-idna==3.3
-imagesize==1.3.0
-importlib-metadata==4.11.1
-iniconfig==1.1.1
-ipykernel==6.9.1
-ipython==8.0.1
+flake8-use-fstring==1.4 ; python_version >= "3.8.0"
+fqdn==1.5.1
+gprof2dot==2022.7.29
+graphviz==0.20.1
+greenlet==2.0.2
+hepunits==2.3.2
+identify==2.5.22
+idna==3.4
+imagesize==1.4.1
+importlib-metadata==6.3.0
+iniconfig==2.0.0
+ipykernel==6.22.0
+ipython==8.12.0
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
-isort==5.10.1
-jedi==0.18.1
-jinja2==3.0.3
-json5==0.9.6
-jsonschema==4.4.0
-jupyter==1.0.0
-jupyter-cache==0.4.3
-jupyter-client==7.1.2
-jupyter-console==6.4.0
-jupyter-core==4.9.2
-jupyter-server==1.13.5
-jupyter-server-mathjax==0.2.4
-jupyter-sphinx==0.3.2
-jupyterlab==3.2.9
-jupyterlab-code-formatter==1.4.10
-jupyterlab-markup==1.0.1
-jupyterlab-myst==0.1.6 ; python_version >= "3.7.0"
-jupyterlab-pygments==0.1.2
-jupyterlab-server==2.10.3
-jupyterlab-widgets==1.0.2
+ipywidgets==8.0.6
+isoduration==20.11.0
+isort==5.12.0
+jedi==0.18.2
+jinja2==3.1.2
+json5==0.9.11
+jsonpointer==2.3
+jsonschema==4.17.3
+jupyter-cache==0.5.0
+jupyter-client==8.1.0
+jupyter-core==5.3.0
+jupyter-events==0.6.3
+jupyter-server==2.5.0
+jupyter-server-fileid==0.9.0
+jupyter-server-terminals==0.4.4
+jupyter-server-ydoc==0.8.0
+jupyter-ydoc==0.2.4
+jupyterlab==3.6.3
+jupyterlab-code-formatter==1.6.0
+jupyterlab-myst==1.1.3 ; python_version >= "3.7.0"
+jupyterlab-pygments==0.2.2
+jupyterlab-server==2.22.0
+jupyterlab-widgets==3.0.7
 latexcodec==2.0.1
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
 livereload==2.6.3
-markdown-it-py==1.1.0
-markupsafe==2.1.0
-matplotlib-inline==0.1.3
-mccabe==0.6.1
-mdit-py-plugins==0.2.8
-mistune==0.8.4
-mypy==0.931
-mypy-extensions==0.4.3
-myst-nb==0.13.2
-myst-parser==0.15.2
-nbclassic==0.3.5
-nbclient==0.5.11
-nbconvert==6.4.2
-nbdime==3.1.1
-nbformat==5.1.3
-nbmake==1.2
-nest-asyncio==1.5.4
-nodeenv==1.6.0
-notebook==6.4.8
-packaging==21.3
+markdown-it-py==2.2.0
+markupsafe==2.1.2
+matplotlib-inline==0.1.6
+mccabe==0.7.0
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==2.0.5
+mypy==1.2.0
+mypy-extensions==1.0.0
+myst-nb==0.17.1
+myst-parser==0.18.1
+nbclassic==0.5.5
+nbclient==0.5.13
+nbconvert==7.3.1
+nbformat==5.8.0
+nbmake==1.2.1
+nest-asyncio==1.5.6
+nodeenv==1.7.0
+notebook==6.5.4
+notebook-shim==0.2.2
+packaging==23.1
 pandocfilters==1.5.0
 parso==0.8.3
-particle==0.20.0
-pathspec==0.9.0
-pep517==0.12.0
-pep8-naming==0.12.1
+particle==0.22.0
+pathspec==0.11.1
+pep8-naming==0.13.3 ; python_version >= "3.8.0"
 pexpect==4.8.0
 pickleshare==0.7.5
-pip-tools==6.5.1
-platformdirs==2.5.1
+platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==2.17.0
-prometheus-client==0.13.1
-prompt-toolkit==3.0.28
+pre-commit==3.2.2
+prometheus-client==0.16.0
+prompt-toolkit==3.0.38
+psutil==5.9.4
 ptyprocess==0.7.0
 pure-eval==0.2.2
-py==1.11.0
 pybtex==0.24.0
-pybtex-docutils==1.0.1
-pycodestyle==2.8.0
+pybtex-docutils==1.0.2
+pycodestyle==2.10.0
 pycparser==2.21
-pydantic==1.9.0
-pydata-sphinx-theme==0.7.2
-pydocstyle==6.1.1
+pydantic==1.10.7
+pydata-sphinx-theme==0.13.3
+pydocstyle==6.3.0
 pydot==1.4.2
-pyflakes==2.4.0
-pygments==2.11.2
-pylint==2.12.2
-pyparsing==3.0.7
-pyrsistent==0.18.1
-pytest==6.2.5
-pytest-cov==3.0.0
-pytest-forked==1.4.0
+pyflakes==3.0.1
+pygments==2.15.0
+pylint==2.17.2
+pyparsing==3.0.9
+pyproject-api==1.5.1
+pyrsistent==0.19.3
+pytest==7.3.0
+pytest-cov==4.0.0
 pytest-profiling==1.7.0
-pytest-xdist==2.5.0
+pytest-xdist==3.2.1
 python-constraint==1.4.0
 python-dateutil==2.8.2
-pytz==2021.3
+python-json-logger==2.0.7
 pyyaml==6.0
-pyzmq==22.3.0
-qtconsole==5.2.2
-qtpy==2.0.1
-requests==2.27.1
-restructuredtext-lint==1.3.2
+pyzmq==25.0.2
+requests==2.28.2
+restructuredtext-lint==1.4.0
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
 send2trash==1.8.0
 six==1.16.0
-smmap==5.0.0
-sniffio==1.2.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
-sphinx==4.4.0
+soupsieve==2.4
+sphinx==5.3.0
 sphinx-autobuild==2021.3.14
-sphinx-book-theme==0.2.0
-sphinx-codeautolink==0.10.0
+sphinx-book-theme==1.0.1
+sphinx-codeautolink==0.14.1
 sphinx-comments==0.0.3
-sphinx-copybutton==0.5.0
-sphinx-panels==0.6.0
-sphinx-thebe==0.1.1
-sphinx-togglebutton==0.3.0
-sphinxcontrib-applehelp==1.0.2
-sphinxcontrib-bibtex==2.4.1
+sphinx-copybutton==0.5.1
+sphinx-design==0.4.1
+sphinx-thebe==0.2.1
+sphinx-togglebutton==0.3.2
+sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-bibtex==2.5.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-hep-pdgref==0.1.4
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sphobjinv==2.2.1
-sqlalchemy==1.4.31
-stack-data==0.2.0
-terminado==0.13.1
-testpath==0.5.0
-toml==0.10.2
+sphobjinv==2.3.1
+sqlalchemy==1.4.47
+stack-data==0.6.2
+tabulate==0.9.0
+terminado==0.17.1
+tinycss2==1.2.1
 tomli==2.0.1
-tornado==6.1
-tox==3.24.5
-tqdm==4.62.3
-traitlets==5.1.1
-types-docutils==0.17.6
+tomlkit==0.11.7
+tornado==6.2
+tox==4.4.11
+tqdm==4.65.0
+traitlets==5.9.0
+types-docutils==0.19.1.7
 types-pkg-resources==0.1.3
-types-pyyaml==6.0.4
-types-requests==2.27.10
-types-setuptools==57.4.9
-types-urllib3==1.26.9
-typing-extensions==4.1.1
-urllib3==1.26.8
-virtualenv==20.13.1
-wcwidth==0.2.5
+types-pyyaml==6.0.12.9
+types-requests==2.28.11.17
+types-setuptools==67.6.0.7
+types-urllib3==1.26.25.10
+typing-extensions==4.5.0 ; python_version < "3.10.0"
+uri-template==1.2.0
+urllib3==1.26.15
+virtualenv==20.21.0
+wcwidth==0.2.6
+webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.2.3
-wheel==0.37.1
-widgetsnbextension==3.5.2
-wrapt==1.13.3
-zipp==3.7.0
+websocket-client==1.5.1
+wheel==0.40.0
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+y-py==0.5.9
+ypy-websocket==0.8.2 ; python_version >= "3.7.0"
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `qrules-0.9.7/.cspell.json` & `qrules-0.9.8/.cspell.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8447152445507708%*

 * *Differences: {"'allowCompoundWords'": 'True',*

 * * "'enableFiletypes'": "{insert: [(1, 'julia')]}",*

 * * "'ignorePaths'": "{insert: [(8, '.editorconfig'), (14, '.prettierignore'), (28, 'Manifest.toml'), "*

 * *                  "(29, 'Project.toml')]}",*

 * * "'ignoreWords'": "{insert: [(0, 'MAINT'), (21, 'docnb'), (71, 'pkpi')]}",*

 * * "'words'": "{insert: [(21, 'hashable')]}"}*

```diff
@@ -1,10 +1,12 @@
 {
+    "allowCompoundWords": true,
     "enableFiletypes": [
         "git-commit",
+        "julia",
         "jupyter"
     ],
     "flagWords": [
         "analyse",
         "colour",
         "comparision",
         "favour",
@@ -21,42 +23,47 @@
         "*.bib",
         "*.ico",
         "*.root",
         "*.rst_t",
         "*.svg",
         "*particle*.*ml",
         ".constraints/*.txt",
+        ".editorconfig",
         ".flake8*",
         ".gitignore",
         ".gitpod.*",
         ".mypy.ini",
         ".pre-commit-config.yaml",
+        ".prettierignore",
         ".pydocstyle*",
         ".pylintrc",
         ".readthedocs.yml",
         ".vscode/*",
         ".vscode/.gitignore",
         ".zenodo.json",
         "codecov.yml",
         "Dockerfile",
         "docs/_templates/*",
         "docs/adr/*/*",
         "docs/conf.py",
         "labels.toml",
         "Makefile",
+        "Manifest.toml",
+        "Project.toml",
         "pyproject.toml",
         "pyrightconfig.json",
         "pytest.ini",
         "requirements*.txt",
         "setup.cfg",
         "setup.py",
         "tox.ini",
         "typings"
     ],
     "ignoreWords": [
+        "MAINT",
         "adrs",
         "ampform",
         "arange",
         "asdict",
         "asdot",
         "astuple",
         "autoupdate",
@@ -69,14 +76,15 @@
         "codemirror",
         "colab",
         "commitlint",
         "compwa",
         "concat",
         "conds",
         "displaystyle",
+        "docnb",
         "doctest",
         "doctests",
         "dotprint",
         "dtype",
         "einsum",
         "epem",
         "eqnarray",
@@ -118,14 +126,15 @@
         "noreply",
         "nrows",
         "nsimplify",
         "pandoc",
         "permalinks",
         "phsp",
         "pids",
+        "pkpi",
         "precommit",
         "prefactor",
         "preorder",
         "prereleased",
         "pygments",
         "pylance",
         "pylintrc",
@@ -179,14 +188,15 @@
         "fermionic",
         "flatt\u00e9",
         "functors",
         "gell",
         "gordan",
         "graphviz",
         "hankel",
+        "hashable",
         "helicities",
         "helicity",
         "htmlcov",
         "imap",
         "ipynb",
         "ipython",
         "isort",
```

### Comparing `qrules-0.9.7/.flake8` & `qrules-0.9.8/.flake8`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 [flake8]
 application-import-names =
-    qrules
+  qrules
 filename =
-    ./docs/*.py
-    ./src/*.py
-    ./tests/*.py
+  ./docs/*.py
+  ./src/*.py
+  ./tests/*.py
 exclude =
-    **/__pycache__
-    **/_build
-    /typings/**
+  **/__pycache__
+  **/_build
+  /typings/**
 ignore =
-    # False positive with attribute docstrings
-    B018
-    # https://github.com/psf/black#slices
-    E203
-    # allowed by black
-    E231
-    # https://github.com/psf/black#line-length
-    E501
-    # should be possible to use {} in latex strings
-    FS003
-    # block quote ends without a blank line (black formatting)
-    RST201
-    # missing pygments
-    RST299
-    # unexpected indentation (related to google style docstring)
-    RST301
-    # enforce type ignore with mypy error codes (combined --extend-select=TI100)
-    TI1
-    # https://github.com/psf/black#line-breaks--binary-operators
-    W503
+  # False positive with attribute docstrings
+  B018
+  # https://github.com/psf/black#slices
+  E203
+  # allowed by black
+  E231
+  # already covered by black
+  E302
+  # https://github.com/psf/black#line-length
+  E501
+  # avoid any from __future__ import annotations, in combination with FI58
+  FI
+  # should be possible to use {} in latex strings
+  FS003
+  # block quote ends without a blank line (black formatting)
+  RST201
+  # missing pygments
+  RST299
+  # unexpected indentation (related to google style docstring)
+  RST301
+  # enforce type ignore with mypy error codes (combined --extend-select=TI100)
+  TI1
+  # https://github.com/psf/black#line-breaks--binary-operators
+  W503
 extend-select =
-    TI100
+  FI58
+  TI100
+per-file-ignores =
+  # casts with generics
+  src/qrules/topology.py:E731
 rst-roles =
-    attr
-    cite
-    class
-    doc
-    download
-    file
-    func
-    meth
-    mod
-    ref
+  attr
+  cite
+  class
+  doc
+  download
+  file
+  func
+  meth
+  mod
+  ref
 rst-directives =
-    deprecated
-    envvar
-    exception
-    seealso
+  autolink-preface
+  automethod
+  deprecated
+  envvar
+  exception
+  seealso
```

### Comparing `qrules-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md` & `qrules-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 
 ## System info
 
 Bug resulted on the following system:
 
 - OS: <!-- e.g. macOS, WSL Ubuntu, ...-->
 - Version <!-- e.g. 10.15, 20.04, ... -->
-- Python version: <!-- e.g. 3.6, 3.7, ... -->
+- Python version: <!-- e.g. 3.7, 3.8, ... -->
 - Virtual environment: <!-- e.g. venv, Conda, pip user install, ... -->
```

### Comparing `qrules-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md` & `qrules-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 name: Feature request
 about: Suggest an idea for this project
 title: ""
-labels: "💡 Enhancement"
+labels: "✨ Enhancement"
 assignees: ""
 ---
 
 ## Problem description
 
 <!-- Is your feature request related to a problem? Please provide a clear and
 concise description of what the problem is. [Example: "I'm always frustrated
```

### Comparing `qrules-0.9.7/.gitignore` & `qrules-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/.gitpod.yml` & `qrules-0.9.8/.gitpod.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,26 +9,30 @@
     pullRequestsFromForks: true
     addComment: false
     addBadge: false
     addLabel: false
 
 vscode:
   extensions:
-    - bungcip.better-toml
     - christian-kohler.path-intellisense
     - davidanson.vscode-markdownlint
     - eamodio.gitlens
     - editorconfig.editorconfig
     - esbenp.prettier-vscode
     - executablebookproject.myst-highlight
+    - github.vscode-github-actions
     - github.vscode-pull-request-github
     - joaompinto.vscode-graphviz
+    - ms-python.flake8
+    - ms-python.isort
+    - ms-python.pylint
     - ms-python.python
     - ms-python.vscode-pylance
+    - ms-vscode.live-server
     - ms-vsliveshare.vsliveshare
     - redhat.vscode-yaml
     - ryanluker.vscode-coverage-gutters
     - stkb.rewrap
     - streetsidesoftware.code-spell-checker
-    - travisillig.vscode-json-stable-stringify
+    - tamasfe.even-better-toml
     - tyriar.sort-lines
     - yzhang.markdown-all-in-one
```

### Comparing `qrules-0.9.7/.mypy.ini` & `qrules-0.9.8/.mypy.ini`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ignore_missing_imports = True
 [mypy-constraint.*]
 ignore_missing_imports = True
 [mypy-jsonschema.*]
 ignore_missing_imports = True
 [mypy-particle.*]
 ignore_missing_imports = True
+[mypy-py.*]
+ignore_missing_imports = True
 [mypy-pybtex.*]
 ignore_missing_imports = True
 [mypy-pydot.*]
 ignore_missing_imports = True
 [mypy-sphinx.*]
 ignore_missing_imports = True
 [mypy-sphobjinv.*]
```

### Comparing `qrules-0.9.7/.pre-commit-config.yaml` & `qrules-0.9.8/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,188 +1,185 @@
 ci:
-  autoupdate_commit_msg: "ci: autoupdate pre-commit hooks"
+  autoupdate_commit_msg: "MAINT: update pip constraints and pre-commit"
   autoupdate_schedule: quarterly # already done by requirements-cron.yml
   skip:
-    # local hooks
     - flake8
     - mypy
     - pylint
-    # hooks that don't work on pre-commit.ci
-    - editorconfig-checker
     - pyright
+    - taplo
 
 repos:
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: check-json
       - id: check-merge-conflict
       - id: check-toml
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
         exclude: >
           (?x)^(
             .*\.bib|
-            .*\.svg|
-            \.cspell\.json
+            .*\.svg
           )$
       - id: mixed-line-ending
       - id: name-tests-test
         name: Tests should start with test_
         args: ["--django"]
       - id: trailing-whitespace
 
   - repo: https://github.com/ComPWA/repo-maintenance
-    rev: 0.0.108
+    rev: 0.0.179
     hooks:
       - id: check-dev-files
         args:
-          - --pin-requirements
+          - --doc-apt-packages=graphviz
+          - --pin-requirements=monthly
+          - --repo-name=qrules
+          - --repo-title=QRules
       - id: fix-nbformat-version
       - id: format-setup-cfg
       - id: set-nb-cells
         args:
           - --add-install-cell
           - --additional-packages=IPython
           - --extras-require=doc,viz
 
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
+    hooks:
+      - id: nbqa-black
+        additional_dependencies:
+          - black>=22.1.0
+      - id: nbqa-flake8
+      - id: nbqa-isort
+      - id: nbqa-pyupgrade
+        args:
+          - --py36-plus
+
   - repo: https://github.com/psf/black
-    rev: 22.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v5.8.4
+    rev: v6.31.0
     hooks:
       - id: cspell
 
-  - repo: https://github.com/myint/docformatter
-    rev: v1.4
-    hooks:
-      - id: docformatter
-        args:
-          - --in-place
-          - --wrap-descriptions=79
-          - --wrap-summaries=79
-
   - repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: 2.4.0
+    rev: 2.7.1
     hooks:
       - id: editorconfig-checker
-        exclude: >
+        name: editorconfig
+        alias: ec
+        exclude: >-
           (?x)^(
             .*\.py
           )$
 
+  - repo: local
+    hooks:
+      - id: flake8
+        name: flake8
+        entry: flake8
+        language: system
+        types:
+          - python
+
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.31.1
+    rev: v0.33.0
     hooks:
       - id: markdownlint
 
-  - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.2.3
+  - repo: local
     hooks:
-      - id: nbqa-black
-        additional_dependencies:
-          - black>=22.1.0
-      - id: nbqa-flake8
-      - id: nbqa-isort
+      - id: mypy
+        name: mypy
+        entry: mypy
+        language: system
+        require_serial: true
+        types:
+          - python
 
-      - id: nbqa-pyupgrade
-        args:
-          - --py36-plus
   - repo: https://github.com/kynan/nbstripout
-    rev: 0.5.0
+    rev: 0.6.1
     hooks:
       - id: nbstripout
         args:
           - --extra-keys
           - |
             cell.metadata.code_folding
             cell.metadata.id
+            cell.metadata.user_expressions
             metadata.celltoolbar
             metadata.colab.name
             metadata.colab.provenance
             metadata.interpreter
-            metadata.language_info.codemirror_mode
-            metadata.language_info.file_extension
-            metadata.language_info.mimetype
-            metadata.language_info.nbconvert_exporter
-            metadata.language_info.pygments_lexer
             metadata.notify_time
             metadata.toc
             metadata.toc-autonumbering
             metadata.toc-showcode
             metadata.toc-showmarkdowntxt
             metadata.toc-showtags
             metadata.varInspector
+            metadata.vscode
+
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.5.1
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
 
   - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1
+    rev: 6.3.0
     hooks:
       - id: pydocstyle
 
-  - repo: https://github.com/ComPWA/mirrors-pyright
-    rev: v1.1.222
-    hooks:
-      - id: pyright
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
-    hooks:
-      - id: pyupgrade
-        args:
-          - --py36-plus
-
-  # The following tools have to be install locally, because they can also be
-  # used by code editors (e.g. linting and format-on-save).
-
   - repo: local
     hooks:
-      - id: flake8
-        name: flake8
-        entry: flake8
-        language: system
-        types:
-          - python
-
-      - id: mypy
-        name: mypy
-        entry: mypy
-        language: system
-        require_serial: true
-        types:
-          - python
-
       - id: pylint
         name: pylint
         entry: pylint
         args:
           - --rcfile=.pylintrc
           - --score=no
         language: system
         require_serial: true
         types:
           - python
+
+  - repo: https://github.com/ComPWA/mirrors-pyright
+    rev: v1.1.303
+    hooks:
+      - id: pyright
+
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        args:
+          - --py36-plus
+
+  - repo: https://github.com/ComPWA/mirrors-taplo
+    rev: v0.8.0
+    hooks:
+      - id: taplo
```

### Comparing `qrules-0.9.7/.pylintrc` & `qrules-0.9.8/.pylintrc`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # To see other available options:
 #   pylint --generate-rcfile > .pylintrc_new
 # and compare the output
 
 [BASIC]
 good-names-rgxs=
-    ^[p]$,
+  ^[p]$,
 
 [MASTER]
 ignore=
-    conf.py,
+  conf.py,
 ignore-patterns=
-    .*\.pyi
+  .*\.pyi
 
 [MESSAGES CONTROL]
 disable=
-    duplicate-code, # https://github.com/PyCQA/pylint/issues/214
-    invalid-unary-operand-type, # conflicts with attrs.field
-    logging-fstring-interpolation,
-    missing-class-docstring,    # pydocstyle
-    missing-function-docstring, # pydocstyle
-    missing-module-docstring,   # pydocstyle
-    no-member, # conflicts with attrs.field
-    not-an-iterable, # conflicts with attrs.field
-    not-callable, # conflicts with attrs.field
-    redefined-builtin, # flake8-built
-    too-few-public-methods, # data containers (attrs) and interface classes
-    unspecified-encoding, # http://pylint.pycqa.org/en/latest/whatsnew/2.10.html
-    unsubscriptable-object, # conflicts with attrs.field
-    unsupported-assignment-operation, # conflicts with attrs.field
-    unsupported-membership-test, # conflicts with attrs.field
-    unused-import, # https://www.flake8rules.com/rules/F401
+  abstract-class-instantiated,  # doesn't work well with Generic
+  duplicate-code, # https://github.com/PyCQA/pylint/issues/214
+  invalid-unary-operand-type, # conflicts with attrs.field
+  line-too-long,    # automatically fixed with black
+  logging-fstring-interpolation,
+  missing-class-docstring,    # pydocstyle
+  missing-function-docstring, # pydocstyle
+  missing-module-docstring,   # pydocstyle
+  no-member, # conflicts with attrs.field
+  no-name-in-module,  # already checked by mypy
+  not-a-mapping, # conflicts with attrs.field
+  not-an-iterable, # conflicts with attrs.field
+  not-callable, # conflicts with attrs.field
+  redefined-builtin, # flake8-built
+  too-few-public-methods, # data containers (attrs) and interface classes
+  unspecified-encoding, # http://pylint.pycqa.org/en/latest/whatsnew/2.10.html
+  unsubscriptable-object, # conflicts with attrs.field
+  unsupported-assignment-operation, # conflicts with attrs.field
+  unsupported-membership-test, # conflicts with attrs.field
+  unused-import, # https://www.flake8rules.com/rules/F401
 
 [SIMILARITIES]
 ignore-imports=yes # https://stackoverflow.com/a/30007053
 
 [VARIABLES]
 init-import=yes
```

### Comparing `qrules-0.9.7/.vscode/settings.json` & `qrules-0.9.8/.vscode/settings.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.678030303030303%*

 * *Differences: {"'[git-commit]'": "OrderedDict([('rewrap.wrappingColumn', 72)])",*

 * * "'editor.rulers'": '[88]',*

 * * "'flake8.importStrategy'": "'fromEnvironment'",*

 * * "'github-actions.workflows.pinned.workflows'": "['.github/workflows/ci.yml']",*

 * * "'isort.check'": 'True',*

 * * "'isort.importStrategy'": "'fromEnvironment'",*

 * * "'livePreview.defaultPreviewPath'": "'docs/_build/html'",*

 * * "'pylint.importStrategy'": "'fromEnvironment'",*

 * * "'python.analysis.inlayHints.pytestParameters'": 'True',*

 * * "'python.analysis.typeCheckingMode'": "'strict' […]*

```diff
@@ -1,13 +1,13 @@
 {
     "[bibtex]": {
         "editor.formatOnSave": false
     },
-    "[ipynb]": {
-        "editor.formatOnSave": false
+    "[git-commit]": {
+        "rewrap.wrappingColumn": 72
     },
     "[json]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[jsonc]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
@@ -28,61 +28,70 @@
         "coverage.xml"
     ],
     "coverage-gutters.coverageReportFileName": "**/htmlcov/index.html",
     "coverage-gutters.showGutterCoverage": false,
     "coverage-gutters.showLineCoverage": true,
     "editor.formatOnSave": true,
     "editor.rulers": [
-        80
+        88
     ],
     "files.watcherExclude": {
         "**/*_cache/**": true,
         "**/.eggs/**": true,
         "**/.git/**": true,
         "**/.tox/**": true
     },
+    "flake8.importStrategy": "fromEnvironment",
     "git.rebaseWhenSync": true,
+    "github-actions.workflows.pinned.workflows": [
+        ".github/workflows/ci.yml"
+    ],
+    "isort.check": true,
+    "isort.importStrategy": "fromEnvironment",
     "json.schemas": [
         {
             "fileMatch": [
                 "*particle*.json"
             ],
             "url": "./src/qrules/particle-validation.json"
         },
         {
             "fileMatch": [
                 ".zenodo.json"
             ],
             "url": "https://zenodo.org/schemas/deposits/records/legacyrecord.json"
         }
     ],
+    "livePreview.defaultPreviewPath": "docs/_build/html",
+    "pylint.importStrategy": "fromEnvironment",
     "python.analysis.autoImportCompletions": false,
     "python.analysis.diagnosticMode": "workspace",
+    "python.analysis.inlayHints.pytestParameters": true,
+    "python.analysis.typeCheckingMode": "strict",
     "python.formatting.provider": "black",
     "python.linting.banditEnabled": false,
     "python.linting.enabled": true,
-    "python.linting.flake8Enabled": true,
+    "python.linting.flake8Enabled": false,
     "python.linting.mypyEnabled": true,
     "python.linting.pydocstyleEnabled": true,
     "python.linting.pylamaEnabled": false,
-    "python.linting.pylintCategorySeverity.refactor": "Information",
-    "python.linting.pylintEnabled": true,
+    "python.linting.pylintEnabled": false,
     "python.testing.pytestArgs": [
         "--color=no",
         "--no-cov"
     ],
     "python.testing.pytestEnabled": true,
     "python.testing.unittestEnabled": false,
-    "rewrap.wrappingColumn": 79,
+    "rewrap.wrappingColumn": 88,
     "search.exclude": {
         "**/tests/**/__init__.py": true,
         "*/.pydocstyle": true,
         ".constraints/*.txt": true
     },
-    "telemetry.telemetryLevel": "off",
     "yaml.schemas": {
         "./src/qrules/particle-validation.json": [
             "*particle*.y*ml"
         ],
+        "https://json.schemastore.org/github-workflow.json": "./.github/workflows/requirements.yml",
         "https://raw.githubusercontent.com/readthedocs/readthedocs.org/master/readthedocs/rtd_tests/fixtures/spec/v2/schema.yml": ".readthedocs.yml"
     }
 }
```

### Comparing `qrules-0.9.7/.zenodo.json` & `qrules-0.9.8/.zenodo.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'creators'": "{0: {'name': 'Fritsch, Miriam'}, 1: {'name': 'Pflüger, Stefan'}, 2: {'name': 'de "*

 * *               "Boer, Remco'}, 4: {'affiliation': 'GSI Helmholtzzentrum für Schwerionenforschung', "*

 * *               "'name': 'Peters, Klaus'}, delete: [4]}"}*

```diff
@@ -1,33 +1,29 @@
 {
     "access_right": "open",
     "creators": [
         {
             "affiliation": "Ruhr University Bochum",
-            "name": "Pfl\u00fcger, Stefan"
+            "name": "Fritsch, Miriam"
         },
         {
             "affiliation": "Ruhr University Bochum",
-            "name": "de Boer. Remco"
+            "name": "Pfl\u00fcger, Stefan"
         },
         {
             "affiliation": "Ruhr University Bochum",
-            "name": "Fritsch, Miriam"
+            "name": "de Boer, Remco"
         },
         {
             "affiliation": "Johannes Gutenberg University Mainz",
             "name": "Gradl, Wolfgang"
         },
         {
-            "affiliation": "Ruhr University Bochum",
-            "name": "Wollenberg, Leonard"
-        },
-        {
-            "affiliation": "Ruhr University Bochum",
-            "name": "J\u00e4ger, Sebastian"
+            "affiliation": "GSI Helmholtzzentrum f\u00fcr Schwerionenforschung",
+            "name": "Peters, Klaus"
         }
     ],
     "description": "<p>QRules is a Python package for <strong>validating and generating particle reactions</strong>&nbsp;using quantum number conservation rules. The user only has to provide a certain set of boundary conditions (initial and final state, allowed interaction types, expected decay topologies, etc.). QRules will then span the space of allowed quantum numbers over all allowed decay topologies and particle instances that correspond with the sets of allowed quantum numbers it has found.</p>\n\n<p>The resulting state transition objects are particularly useful for <strong>amplitude analysis / Partial Wave Analysis</strong> as they contain all information (such as expected masses, widths, and spin projections) that is needed to formulate an amplitude model.</p>",
     "keywords": [
         "particle",
         "physics",
         "rule-based",
```

### Comparing `qrules-0.9.7/LICENSE` & `qrules-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/PKG-INFO` & `qrules-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrules
-Version: 0.9.7
+Version: 0.9.8
 Summary: Rule-based particle reaction problem solver on a quantum number level
 Home-page: UNKNOWN
 Author: Common Partial Wave Analysis
 Author-email: compwa-admin@ep1.rub.de
 Maintainer-email: compwa-admin@ep1.rub.de
 License: GPLv3 or later
 Project-URL: Tracker, https://github.com/ComPWA/qrules/issues
@@ -18,39 +18,38 @@
         
         [![PyPI package](https://badge.fury.io/py/qrules.svg)](https://pypi.org/project/qrules)
         [![Conda package](https://anaconda.org/conda-forge/qrules/badges/version.svg)](https://anaconda.org/conda-forge/qrules)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/qrules)](https://pypi.org/project/qrules)
         
         [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/qrules/stable?filepath=docs/usage)
         [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/qrules/blob/stable)
-        [![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/ComPWA/qrules)
-        [![GitPod](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
+        [![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/qrules)
+        [![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
         
         [![Documentation](https://readthedocs.org/projects/qrules/badge/?version=latest)](https://qrules.readthedocs.io)
         [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/qrules/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/qrules/main)
         [![pytest](https://github.com/ComPWA/qrules/workflows/pytest/badge.svg)](https://github.com/ComPWA/qrules/actions?query=branch%3Amain+workflow%3Apytest)
         [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
         [![Test coverage](https://codecov.io/gh/ComPWA/qrules/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/qrules)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/deeee5b9e2bb4b3daa655942c71e17da)](https://www.codacy.com/gh/ComPWA/qrules)
         [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
         [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort)
         
-        QRules is a Python package for **validating and generating particle reactions**
-        using quantum number conservation rules. The user only has to provide a certain
-        set of boundary conditions (initial and final state, allowed interaction types,
-        expected decay topologies, etc.). QRules will then span the space of allowed
-        quantum numbers over all allowed decay topologies and particle instances that
-        correspond with the sets of allowed quantum numbers it has found.
-        
-        The resulting state transition objects are particularly useful for **amplitude
-        analysis / Partial Wave Analysis** as they contain all information (such as
-        expected masses, widths, and spin projections) that is needed to formulate an
-        amplitude model.
+        QRules is a Python package for **validating and generating particle reactions** using
+        quantum number conservation rules. The user only has to provide a certain set of
+        boundary conditions (initial and final state, allowed interaction types, expected decay
+        topologies, etc.). QRules will then span the space of allowed quantum numbers over all
+        allowed decay topologies and particle instances that correspond with the sets of allowed
+        quantum numbers it has found.
+        
+        The resulting state transition objects are particularly useful for **amplitude analysis
+        / Partial Wave Analysis** as they contain all information (such as expected masses,
+        widths, and spin projections) that is needed to formulate an amplitude model.
         
         Visit [qrules.rtfd.io](https://qrules.readthedocs.io) for more information!
         
         For an overview of **upcoming releases and planned functionality**, see
         [here](https://github.com/ComPWA/qrules/milestones?direction=asc&sort=title&state=open).
         
         ## Available features
@@ -67,16 +66,15 @@
           - Large set of predefined rules
             - Spin/Angular momentum conservation
             - Quark and Lepton flavor conservation (incl. isospin)
             - Baryon number conservation
             - EM-charge conservation
             - Parity, C-Parity, G-Parity conservation
             - Mass conservation
-          - Predefined sets of conservation rules representing Strong, EM, Weak
-            interactions
+          - Predefined sets of conservation rules representing Strong, EM, Weak interactions
         
         ## Contribute
         
         See [`CONTRIBUTING.md`](./CONTRIBUTING.md)
         
 Keywords: HEP,PWA,amplitude analysis,partial wave analysis,particle physics,particles,physics
 Platform: UNKNOWN
@@ -89,22 +87,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: format
 Provides-Extra: flake8
 Provides-Extra: mypy
 Provides-Extra: lint
 Provides-Extra: sty
+Provides-Extra: jupyter
 Provides-Extra: dev
```

### Comparing `qrules-0.9.7/README.md` & `qrules-0.9.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,39 +5,38 @@
 
 [![PyPI package](https://badge.fury.io/py/qrules.svg)](https://pypi.org/project/qrules)
 [![Conda package](https://anaconda.org/conda-forge/qrules/badges/version.svg)](https://anaconda.org/conda-forge/qrules)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/qrules)](https://pypi.org/project/qrules)
 
 [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/qrules/stable?filepath=docs/usage)
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/qrules/blob/stable)
-[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/ComPWA/qrules)
-[![GitPod](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
+[![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/qrules)
+[![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
 
 [![Documentation](https://readthedocs.org/projects/qrules/badge/?version=latest)](https://qrules.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/qrules/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/qrules/main)
 [![pytest](https://github.com/ComPWA/qrules/workflows/pytest/badge.svg)](https://github.com/ComPWA/qrules/actions?query=branch%3Amain+workflow%3Apytest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
 [![Test coverage](https://codecov.io/gh/ComPWA/qrules/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/qrules)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/deeee5b9e2bb4b3daa655942c71e17da)](https://www.codacy.com/gh/ComPWA/qrules)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort)
 
-QRules is a Python package for **validating and generating particle reactions**
-using quantum number conservation rules. The user only has to provide a certain
-set of boundary conditions (initial and final state, allowed interaction types,
-expected decay topologies, etc.). QRules will then span the space of allowed
-quantum numbers over all allowed decay topologies and particle instances that
-correspond with the sets of allowed quantum numbers it has found.
-
-The resulting state transition objects are particularly useful for **amplitude
-analysis / Partial Wave Analysis** as they contain all information (such as
-expected masses, widths, and spin projections) that is needed to formulate an
-amplitude model.
+QRules is a Python package for **validating and generating particle reactions** using
+quantum number conservation rules. The user only has to provide a certain set of
+boundary conditions (initial and final state, allowed interaction types, expected decay
+topologies, etc.). QRules will then span the space of allowed quantum numbers over all
+allowed decay topologies and particle instances that correspond with the sets of allowed
+quantum numbers it has found.
+
+The resulting state transition objects are particularly useful for **amplitude analysis
+/ Partial Wave Analysis** as they contain all information (such as expected masses,
+widths, and spin projections) that is needed to formulate an amplitude model.
 
 Visit [qrules.rtfd.io](https://qrules.readthedocs.io) for more information!
 
 For an overview of **upcoming releases and planned functionality**, see
 [here](https://github.com/ComPWA/qrules/milestones?direction=asc&sort=title&state=open).
 
 ## Available features
@@ -54,13 +53,12 @@
   - Large set of predefined rules
     - Spin/Angular momentum conservation
     - Quark and Lepton flavor conservation (incl. isospin)
     - Baryon number conservation
     - EM-charge conservation
     - Parity, C-Parity, G-Parity conservation
     - Mass conservation
-  - Predefined sets of conservation rules representing Strong, EM, Weak
-    interactions
+  - Predefined sets of conservation rules representing Strong, EM, Weak interactions
 
 ## Contribute
 
 See [`CONTRIBUTING.md`](./CONTRIBUTING.md)
```

### Comparing `qrules-0.9.7/codecov.yml` & `qrules-0.9.8/codecov.yml`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/_relink_references.py` & `qrules-0.9.8/docs/_relink_references.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=import-error, import-outside-toplevel
 # pyright: reportMissingImports=false
 """Abbreviated the annotations generated by sphinx-autodoc.
 
-It's not necessary to generate the full path of type hints, because they are
-rendered as clickable links.
+It's not necessary to generate the full path of type hints, because they are rendered as
+clickable links.
 
 See also https://github.com/sphinx-doc/sphinx/issues/5868.
 """
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -24,15 +24,15 @@
 __REF_TYPE_SUBSTITUTIONS = {
     "None": "obj",
 }
 
 
 def _new_type_to_xref(
     target: str,
-    env: "BuildEnvironment" = None,
+    env: "BuildEnvironment" = None,  # type: ignore[assignment]
     suppress_prefix: bool = False,
 ) -> "pending_xref":
     if env:
         kwargs = {
             "py:module": env.ref_context.get("py:module"),
             "py:class": env.ref_context.get("py:class"),
         }
```

### Comparing `qrules-0.9.7/docs/_static/favicon.ico` & `qrules-0.9.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/_templates/genindex.html` & `qrules-0.9.8/docs/_templates/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,19 @@
   {%- if links[0][0] %}<strong
     >{% endif -%} {{ firstname|e }} {%- if links[0][0] %}</strong
   >{% endif -%}
 </a>
 
 {%- for ismain, link in links[1:] -%} ,
 <a href="{{ link }}"
-  >{% if ismain %}<strong
-    >{% endif -%} [{{ loop.index }}] {%- if ismain %}</strong
-  >{% endif -%}
+  >{% if ismain %}<strong>{% endif -%} [{{ loop.index }}] {%- if ismain %}</strong>{%
+  endif -%}
 </a>
-{%- endfor %} {%- else %} {{ firstname|e }} {%- endif %} {% endmacro %} {%-
-extends "layout.html" %} {% set title = _('Index') %} {% block body %}
+{%- endfor %} {%- else %} {{ firstname|e }} {%- endif %} {% endmacro %} {%- extends
+"layout.html" %} {% set title = _('Index') %} {% block body %}
 
 <h1 id="index">{{ _('Index') }}</h1>
 
 <div class="genindex-jumpbox">
   {% for key, dummy in genindexentries -%}
   <a href="#{{ key }}"><strong>{{ key }}</strong></a>
   {% if not loop.last %}| {% endif %} {%- endfor %}
```

### Comparing `qrules-0.9.7/docs/_templates/package.rst_t` & `qrules-0.9.8/docs/_templates/package.rst_t`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {%- macro automodule(modname, options) -%}
 .. automodule:: {{ modname }}
 {%- for option in options %}
-   :{{ option }}:
+  :{{ option }}:
 {%- endfor %}
 {%- endmacro %}
 
 {%- macro toctree(docnames) -%}
 .. toctree::
 {% for docname in docnames %}
-   {{ docname }}
+  {{ docname }}
 {%- endfor %}
 {%- endmacro %}
 
 {{ pkgname.split(".")[-1] | e | heading }}
 
 .. code-block:: python
 
-    import {{ pkgname }}
+  import {{ pkgname }}
 
 {%- if modulefirst and not is_namespace %}
 {{ automodule(pkgname, automodule_options) }}
 {% endif %}
 
 {%- if not modulefirst and not is_namespace %}
```

### Comparing `qrules-0.9.7/docs/adr/template.md` & `qrules-0.9.8/docs/adr/template.md`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/bibliography.bib` & `qrules-0.9.8/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/conf.py` & `qrules-0.9.8/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Configuration file for the Sphinx documentation builder.
 
-This file only contains a selection of the most common options. For a full
-list see the documentation:
-https://www.sphinx-doc.org/en/master/usage/configuration.html
+This file only contains a selection of the most common options. For a full list see the
+documentation: https://www.sphinx-doc.org/en/master/usage/configuration.html
 """
 
 import os
 import re
 import shutil
 import subprocess
 import sys
+from typing import Dict
 
 import requests
 
 # pyright: reportMissingImports=false
 import sphobjinv as soi
-from pkg_resources import get_distribution
 from pybtex.database import Entry
 from pybtex.plugin import register_plugin
 from pybtex.richtext import Tag, Text
 from pybtex.style.formatting.unsrt import Style as UnsrtStyle
 from pybtex.style.template import (
     FieldIsMissing,
     Node,
@@ -28,31 +27,46 @@
     href,
     join,
     node,
     sentence,
     words,
 )
 
+if sys.version_info < (3, 8):
+    from importlib_metadata import PackageNotFoundError
+    from importlib_metadata import version as get_package_version
+else:
+    from importlib.metadata import PackageNotFoundError
+    from importlib.metadata import version as get_package_version
+
 # -- Project information -----------------------------------------------------
 project = "QRules"
 PACKAGE = "qrules"
 REPO_NAME = "qrules"
 copyright = "2020, ComPWA"  # noqa: A001
 author = "Common Partial Wave Analysis"
 
+
 # https://docs.readthedocs.io/en/stable/builds.html
-BRANCH = os.environ.get("READTHEDOCS_VERSION", "stable")
-if BRANCH == "latest":
-    BRANCH = "main"
-if re.match(r"^\d+$", BRANCH):  # PR preview
-    BRANCH = "stable"
-
-if os.path.exists(f"../src/{PACKAGE}/version.py"):
-    __RELEASE = get_distribution(PACKAGE).version
-    version = ".".join(__RELEASE.split(".")[:3])
+def get_branch_name() -> str:
+    branch_name = os.environ.get("READTHEDOCS_VERSION", "stable")
+    if branch_name == "latest":
+        return "main"
+    if re.match(r"^\d+$", branch_name):  # PR preview
+        return "stable"
+    return branch_name
+
+
+BRANCH = get_branch_name()
+
+try:
+    __VERSION = get_package_version(PACKAGE)
+    version = ".".join(__VERSION.split(".")[:3])
+except PackageNotFoundError:
+    pass
 
 
 # -- Fetch logo --------------------------------------------------------------
 def fetch_logo(url: str, output_path: str) -> None:
     if os.path.exists(output_path):
         return
     online_content = requests.get(url, allow_redirects=True)
@@ -144,15 +158,15 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_codeautolink",
     "sphinx_comments",
     "sphinx_copybutton",
-    "sphinx_panels",
+    "sphinx_design",
     "sphinx_thebe",
     "sphinx_togglebutton",
     "sphinxcontrib.bibtex",
     "sphinxcontrib.hep.pdgref",
 ]
 exclude_patterns = [
     "**.ipynb_checkpoints",
@@ -180,21 +194,61 @@
 AUTODOC_INSERT_SIGNATURE_LINEBREAKS = True
 graphviz_output_format = "svg"
 html_copy_source = True  # needed for download notebook button
 html_css_files = []
 if AUTODOC_INSERT_SIGNATURE_LINEBREAKS:
     html_css_files.append("linebreaks-api.css")
 html_favicon = "_static/favicon.ico"
+html_last_updated_fmt = "%-d %B %Y"
 html_show_copyright = False
 html_show_sourcelink = False
 html_show_sphinx = False
 html_sourcelink_suffix = ""
 html_static_path = ["_static"]
 html_theme = "sphinx_book_theme"
 html_theme_options = {
+    "icon_links": [
+        {
+            "name": "Common Partial Wave Analysis",
+            "url": "https://compwa-org.rtfd.io",
+            "icon": "_static/favicon.ico",
+            "type": "local",
+        },
+        {
+            "name": "GitHub",
+            "url": f"https://github.com/ComPWA/{REPO_NAME}",
+            "icon": "fa-brands fa-github",
+        },
+        {
+            "name": "PyPI",
+            "url": f"https://pypi.org/project/{PACKAGE}",
+            "icon": "fa-brands fa-python",
+        },
+        {
+            "name": "Conda",
+            "url": f"https://anaconda.org/conda-forge/{PACKAGE}",
+            "icon": "https://avatars.githubusercontent.com/u/22454001?s=100",
+            "type": "url",
+        },
+        {
+            "name": "Launch on Binder",
+            "url": (
+                f"https://mybinder.org/v2/gh/ComPWA/{REPO_NAME}/{BRANCH}?filepath=docs"
+            ),
+            "icon": "https://mybinder.readthedocs.io/en/latest/_static/favicon.png",
+            "type": "url",
+        },
+        {
+            "name": "Launch on Colaboratory",
+            "url": f"https://colab.research.google.com/github/ComPWA/{REPO_NAME}/blob/{BRANCH}",
+            "icon": "https://avatars.githubusercontent.com/u/33467679?s=100",
+            "type": "url",
+        },
+    ],
+    "logo": {"text": "Quantum number conservation rules"},
     "repository_url": f"https://github.com/ComPWA/{REPO_NAME}",
     "repository_branch": BRANCH,
     "path_to_docs": "docs",
     "use_download_button": True,
     "use_edit_page_button": True,
     "use_issues_button": True,
     "use_repository_button": True,
@@ -204,18 +258,16 @@
         "deepnote_url": "https://deepnote.com",
         "notebook_interface": "jupyterlab",
         "thebe": True,
         "thebelab": True,
     },
     "show_navbar_depth": 2,
     "show_toc_level": 2,
-    "theme_dev_mode": True,
 }
-html_title = "Quantum number conservation rules"
-panels_add_bootstrap_css = False  # wider page width with sphinx-panels
+html_title = html_theme_options["logo"]["text"]  # type: ignore[index]
 pygments_style = "sphinx"
 todo_include_todos = False
 viewcode_follow_imported_members = True
 
 # Cross-referencing configuration
 default_role = "py:obj"
 primary_domain = "py"
@@ -229,21 +281,15 @@
     ("py:class", "typing_extensions.Protocol"),
     ("py:obj", "qrules.topology._K"),
     ("py:obj", "qrules.topology._V"),
 ]
 
 
 # Intersphinx settings
-version_remapping = {
-    "jsonschema": {
-        "4.3.2": "4.3.1",
-        "4.3.3": "4.3.1",
-        "4.4.0": "4.3.1",
-    },
-}
+version_remapping: Dict[str, Dict[str, str]] = {}
 
 
 def get_version(package_name: str) -> str:
     python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
     constraints_path = f"../.constraints/py{python_version}.txt"
     with open(constraints_path) as stream:
         constraints = stream.read()
@@ -267,24 +313,19 @@
         return installed_version
     return "stable"
 
 
 intersphinx_mapping = {
     "ampform": ("https://ampform.readthedocs.io/en/stable", None),
     "attrs": (f"https://www.attrs.org/en/{get_version('attrs')}", None),
-    "compwa-org": ("https://compwa-org.readthedocs.io/en/stable", None),
-    "constraint": (
-        "https://labix.org/doc/constraint/public",
-        "constraint.inv",
-    ),
+    "compwa-org": ("https://compwa-org.readthedocs.io", None),
+    "constraint": ("https://labix.org/doc/constraint/public", "constraint.inv"),
     "graphviz": ("https://graphviz.readthedocs.io/en/stable", None),
-    "jsonschema": (
-        f"https://python-jsonschema.readthedocs.io/en/v{get_version('jsonschema')}",
-        None,
-    ),
+    "IPython": (f"https://ipython.readthedocs.io/en/{get_version('IPython')}", None),
+    "jsonschema": ("https://python-jsonschema.readthedocs.io/en/stable", None),
     "mypy": ("https://mypy.readthedocs.io/en/stable", None),
     "pwa": ("https://pwa.readthedocs.io", None),
     "python": ("https://docs.python.org/3", None),
 }
 
 # Settings for autosectionlabel
 autosectionlabel_prefix_document = True
@@ -297,58 +338,55 @@
 
 # Settings for copybutton
 copybutton_prompt_is_regexp = True
 copybutton_prompt_text = r">>> |\.\.\. "  # doctest
 
 # Settings for linkcheck
 linkcheck_anchors = False
+linkcheck_ignore = [
+    "https://doi.org/10.1002/andp.19955070504",  # 403 for onlinelibrary.wiley.com
+]
 
 # Settings for myst_nb
-execution_timeout = -1
+nb_execution_show_tb = True
+nb_execution_timeout = -1
 nb_output_stderr = "remove"
-nb_render_priority = {
-    "html": (
-        "application/vnd.jupyter.widget-view+json",
-        "application/javascript",
-        "text/html",
-        "image/svg+xml",
-        "image/png",
-        "image/jpeg",
-        "text/markdown",
-        "text/latex",
-        "text/plain",
-    )
-}
-nb_render_priority["doctest"] = nb_render_priority["html"]
 
-jupyter_execute_notebooks = "off"
+nb_execution_mode = "off"
 if "EXECUTE_NB" in os.environ:
     print("\033[93;1mWill run Jupyter notebooks!\033[0m")
-    jupyter_execute_notebooks = "force"
+    nb_execution_mode = "cache"
 
 # Settings for myst-parser
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "dollarmath",
     "smartquotes",
     "substitution",
 ]
-BINDER_LINK = f"https://mybinder.org/v2/gh/ComPWA/{REPO_NAME}/{BRANCH}?filepath=docs/usage"
+BINDER_LINK = (
+    f"https://mybinder.org/v2/gh/ComPWA/{REPO_NAME}/{BRANCH}?filepath=docs/usage"
+)
 myst_substitutions = {
     "branch": BRANCH,
     "run_interactive": f"""
 ```{{margin}}
 Run this notebook [on Binder]({BINDER_LINK}) or
-{{ref}}`locally on Jupyter Lab <compwa-org:develop:Jupyter Notebooks>` to
-interactively modify the parameters.
+{{ref}}`locally on Jupyter Lab <compwa-org:develop:Jupyter Notebooks>` to interactively
+modify the parameters.
 ```
 """,
 }
 myst_update_mathjax = False
+suppress_warnings = [
+    # skipping unknown output mime type: application/json
+    # https://github.com/ComPWA/qrules/runs/8132605149?check_suite_focus=true#step:5:92
+    "mystnb.unknown_mime_type",
+]
 
 # Settings for sphinx_comments
 comments_config = {
     "hypothesis": True,
     "utterances": {
         "repo": f"ComPWA/{REPO_NAME}",
         "issue-term": "pathname",
@@ -393,22 +431,20 @@
     style = context["style"]
     formatted_names = [
         style.format_name(person, style.abbreviate_names) for person in persons
     ]
     return et_al(**kwargs)[formatted_names].format_data(context)
 
 
-class MyStyle(UnsrtStyle):
+class MyStyle(UnsrtStyle):  # pyright: ignore[reportUntypedBaseClass]
     def __init__(self) -> None:
         super().__init__(abbreviate_names=True)
 
     def format_names(self, role: Entry, as_sentence: bool = True) -> Node:
-        formatted_names = names(
-            role, sep=", ", sep2=" and ", last_sep=", and "
-        )
+        formatted_names = names(role, sep=", ", sep2=" and ", last_sep=", and ")
         if as_sentence:
             return sentence[formatted_names]
         else:
             return formatted_names
 
     def format_url(self, e: Entry) -> Node:
         return words[
```

### Comparing `qrules-0.9.7/docs/index.md` & `qrules-0.9.8/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,75 +11,72 @@
 {{ '[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/qrules/blob/{})'.format(branch) }}
 {{ '[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/qrules/{}?filepath=docs/usage)'.format(branch) }}
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 
 :::{margin}
 
-The original project was the
-[PWA Expert System](https://expertsystem.readthedocs.io). QRules originates
-from its
+The original project was the [PWA Expert System](https://expertsystem.readthedocs.io).
+QRules originates from its
 [`reaction`](https://expertsystem.readthedocs.io/en/stable/api/expertsystem.reaction.html)
 module.
 
 :::
 
-QRules is a Python package for **validating and generating particle reactions**
-using quantum number conservation rules. The user only has to provide a certain
-set of boundary conditions (initial and final state, allowed interaction types,
-expected decay topologies, etc.). QRules will then span the space of allowed
-quantum numbers over all allowed decay topologies and particle instances that
-correspond with the sets of allowed quantum numbers it has found.
-
-The resulting state transition objects are particularly useful for **amplitude
-analysis / Partial Wave Analysis** as they contain all information (such as
-expected masses, widths, and spin projections) that is needed to formulate an
-amplitude model.
-
-The {doc}`/usage` pages illustrate several features of {mod}`qrules`. You can
-run each of them as Jupyter notebooks with the {fa}`rocket` launch button in
-the top-right corner. Enjoy!
+QRules is a Python package for **validating and generating particle reactions** using
+quantum number conservation rules. The user only has to provide a certain set of
+boundary conditions (initial and final state, allowed interaction types, expected decay
+topologies, etc.). QRules will then span the space of allowed quantum numbers over all
+allowed decay topologies and particle instances that correspond with the sets of allowed
+quantum numbers it has found.
+
+The resulting state transition objects are particularly useful for **amplitude analysis
+/ Partial Wave Analysis** as they contain all information (such as expected masses,
+widths, and spin projections) that is needed to formulate an amplitude model.
+
+The {doc}`/usage` pages illustrate several features of {mod}`qrules`. You can run each
+of them as Jupyter notebooks with the {fa}`rocket` launch button in the top-right
+corner. Enjoy!
 
 ```{rubric} Internal design
 
 ```
 
 QRules consists of three major components:
 
 1. **State transition graphs**
 
    A {class}`.StateTransitionGraph` is a
-   [directed graph](https://en.wikipedia.org/wiki/Directed_graph) that consists
-   of **nodes** and **edges**. In a directed graph, each edge must be connected
-   to at least one node (in correspondence to
-   [Feynman graphs](https://en.wikipedia.org/wiki/Feynman_diagram)). This way,
-   a graph describes the transition from one state to another.
-
-   - **Edges** correspond to states (particles with spin). In other words,
-     edges are a collection of properties such as the quantum numbers that
-     characterize a state that the particle is in.
-
-   - **Nodes** represents interactions and contain all information for the
-     transition of this specific step. Most importantly, a node contains a
-     collection of conservation rules that have to be satisfied. An interaction
-     node has $M$ ingoing lines and $N$ outgoing lines, where
-     $M,N \in \mathbb{Z}$, $M > 0, N > 0$.
+   [directed graph](https://en.wikipedia.org/wiki/Directed_graph) that consists of
+   **nodes** and **edges**. In a directed graph, each edge must be connected to at least
+   one node (in correspondence to
+   [Feynman graphs](https://en.wikipedia.org/wiki/Feynman_diagram)). This way, a graph
+   describes the transition from one state to another.
+
+   - **Edges** correspond to states (particles with spin). In other words, edges are a
+     collection of properties such as the quantum numbers that characterize a state that
+     the particle is in.
+
+   - **Nodes** represents interactions and contain all information for the transition of
+     this specific step. Most importantly, a node contains a collection of conservation
+     rules that have to be satisfied. An interaction node has $M$ ingoing lines and $N$
+     outgoing lines, where $M,N \in \mathbb{Z}$, $M > 0, N > 0$.
 
 2. **Conservation rules**
 
-   The central component are the {mod}`.conservation_rules`. They belong to
-   individual nodes and receive properties about the node itself, as well as
-   properties of the ingoing and outgoing edges of that node. Based on those
-   properties the conservation rules determine whether edges pass or not.
+   The central component are the {mod}`.conservation_rules`. They belong to individual
+   nodes and receive properties about the node itself, as well as properties of the
+   ingoing and outgoing edges of that node. Based on those properties the conservation
+   rules determine whether edges pass or not.
 
 3. **Solvers**
 
-   The determination of the correct state properties in the graph is done by
-   solvers. New properties are set for intermediate edges and interaction nodes
-   and their validity is checked with the conservation rules.
+   The determination of the correct state properties in the graph is done by solvers.
+   New properties are set for intermediate edges and interaction nodes and their
+   validity is checked with the conservation rules.
 
 :::{margin}
 
 The main solver used by {mod}`qrules` is the
 [`constraint`](https://labix.org/doc/constraint) package for the
 [Constraint Satisfaction Problem](https://en.wikipedia.org/wiki/Constraint_satisfaction_problem)
 (CSP).
@@ -89,66 +86,59 @@
 ```{rubric} QRules workflow
 
 ```
 
 1. **Preparation**
 
    1.1. Build all possible topologies. A **topology** is represented by a
-   {class}`.StateTransitionGraph`, in which the edges and nodes are empty (no
-   particle information).
+   {class}`.StateTransitionGraph`, in which the edges and nodes are empty (no particle
+   information).
 
-   1.2. Fill the topology graphs with the user provided information. Typically
-   these are the graph's ingoing edges (initial state) and outgoing edges
-   (final state).
+   1.2. Fill the topology graphs with the user provided information. Typically these are
+   the graph's ingoing edges (initial state) and outgoing edges (final state).
 
 2. **Solving**
 
    2.1. _Propagate_ quantum number information through the complete graph while
-   respecting the specified conservation laws. Information like mass is not
-   used in this first solving step.
+   respecting the specified conservation laws. Information like mass is not used in this
+   first solving step.
 
-   2.2. _Clone_ graphs while inserting concrete matching particles for the
-   intermediate edges (mainly adds the mass variable).
+   2.2. _Clone_ graphs while inserting concrete matching particles for the intermediate
+   edges (mainly adds the mass variable).
 
-   2.3. _Validate_ the complete graphs, so run all conservation law check that
-   were postponed from the first step.
+   2.3. _Validate_ the complete graphs, so run all conservation law check that were
+   postponed from the first step.
 
 ```{rubric} Table of Contents
 
 ```
 
 ```{toctree}
 ---
 maxdepth: 2
 ---
 install
 usage
 references
+```
+
+```{toctree}
+---
+hidden:
+maxdepth: 2
+---
 API <api/qrules>
 Changelog <https://github.com/ComPWA/qrules/releases>
 Upcoming features <https://github.com/ComPWA/qrules/milestones?direction=asc&sort=title&state=open>
 Help developing <https://compwa-org.readthedocs.io/en/stable/develop.html>
 ```
 
-- {ref}`Python API <modindex>`
-- {ref}`General Index <genindex>`
-- {ref}`Search <search>`
-
 ```{toctree}
 ---
 caption: Related projects
 hidden:
 ---
 AmpForm <https://ampform.readthedocs.io>
 TensorWaves <https://tensorwaves.readthedocs.io>
 PWA Pages <https://pwa.readthedocs.io>
-```
-
-```{toctree}
----
-caption: ComPWA Organization
-hidden:
----
-Website <https://compwa-org.readthedocs.io>
-GitHub Repositories <https://github.com/ComPWA>
-About <https://compwa-org.readthedocs.io/en/stable/about.html>
+ComPWA project <https://compwa-org.readthedocs.io>
 ```
```

### Comparing `qrules-0.9.7/docs/install.md` & `qrules-0.9.8/docs/install.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,101 +4,106 @@
 [![Conda package](https://anaconda.org/conda-forge/qrules/badges/version.svg)](https://anaconda.org/conda-forge/qrules)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/qrules)](https://pypi.org/project/qrules)
 
 ## Quick installation
 
 The fastest way of installing this package is through PyPI or Conda:
 
-:::{tabbed} PyPI
+::::{tab-set}
+
+:::{tab-item} PyPI
 
 ```shell
 python3 -m pip install qrules
 ```
 
 :::
 
-:::{tabbed} Conda
+:::{tab-item} Conda
 
 ```shell
 conda install -c conda-forge qrules
 ```
 
 :::
 
-This installs the [latest release](https://github.com/ComPWA/qrules/releases)
-that you can find on the
-[`stable`](https://github.com/ComPWA/qrules/tree/stable) branch.
+::::
+
+This installs the [latest release](https://github.com/ComPWA/qrules/releases) that you
+can find on the [`stable`](https://github.com/ComPWA/qrules/tree/stable) branch.
 
 Optionally, you can install the dependencies required for
 {doc}`visualizing topologies </usage/visualize>` with the following
 {ref}`optional dependency syntax <compwa-org:develop:Optional dependencies>`:
 
 ```shell
 pip install qrules[viz]  # installs qrules with graphviz
 ```
 
-The latest version on the [`main`](https://github.com/ComPWA/qrules/tree/main)
-branch can be installed as follows:
+The latest version on the [`main`](https://github.com/ComPWA/qrules/tree/main) branch
+can be installed as follows:
 
 ```shell
 python3 -m pip install git+https://github.com/ComPWA/qrules@main
 ```
 
 ## Editable installation
 
 It is highly recommend to use the more dynamic
-{ref}`'editable installation' <compwa-org:develop:Editable installation>`. This
-allows you to:
+{ref}`'editable installation' <compwa-org:develop:Editable installation>`. This allows
+you to:
 
-- exactly
-  {ref}`pin all dependencies <compwa-org:develop:Pinning dependency versions>`
+- exactly {ref}`pin all dependencies <compwa-org:develop:Pinning dependency versions>`
   to a specific version, so that your work is **reproducible**.
 - edit the source code of the framework and
   {doc}`help improving it <compwa-org:develop>`.
 
-For this, you first need to get the source code with
-[Git](https://git-scm.com):
+For this, you first need to get the source code with [Git](https://git-scm.com):
 
 ```shell
 git clone https://github.com/ComPWA/qrules.git
 cd qrules
 ```
 
 Next, you install the project in editable mode with either
 [Conda](https://docs.conda.io) or [`pip`](https://pypi.org/project/pip). It's
 recommended to use Conda, because this also pins the version of Python.
 
-:::{tabbed} Conda
+::::{tab-set}
+
+:::{tab-item} Conda
 
 ```shell
 conda env create
 ```
 
 This installs the project in a Conda environment following the definitions in
 [`environment.yml`](https://github.com/ComPWA/qrules/blob/main/environment.yml).
 
 :::
 
-:::{tabbed} PyPI
+:::{tab-item} PyPI
 
 1. **[Recommended]** Create a virtual environment with
    [`venv`](https://docs.python.org/3/library/venv.html) (see
    {ref}`here <compwa-org:develop:Virtual environment>`).
 
 2. Install the project as an
-   {ref}`'editable installation' <compwa-org:develop:Editable installation>`
-   with {ref}`additional packages <compwa-org:develop:Optional dependencies>`
-   for the developer and all dependencies pinned through
+   {ref}`'editable installation' <compwa-org:develop:Editable installation>` with
+   {ref}`additional packages <compwa-org:develop:Optional dependencies>` for the
+   developer and all dependencies pinned through
    [constraints files](https://pip.pypa.io/en/stable/user_guide/#constraints-files):
 
    ```shell
    python3 -m pip install -c .constraints/py3.x.txt -e .[dev]
    ```
 
 :::
 
-See {ref}`compwa-org:develop:Updating` for how to update the dependencies when
-new commits come in.
+::::
+
+See {ref}`compwa-org:develop:Updating` for how to update the dependencies when new
+commits come in.
 
-That's all! Have a look at {doc}`/usage` to try out the package. You can also
-have a look at {doc}`compwa-org:develop` for tips on how to work with this
-'editable' developer setup!
+That's all! Have a look at {doc}`/usage` to try out the package. You can also have a
+look at {doc}`compwa-org:develop` for tips on how to work with this 'editable' developer
+setup!
```

### Comparing `qrules-0.9.7/docs/usage/additional_particles.yml` & `qrules-0.9.8/docs/usage/additional_particles.yml`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/usage/conservation.ipynb` & `qrules-0.9.8/docs/usage/conservation.ipynb`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/usage/custom-topology.ipynb` & `qrules-0.9.8/docs/usage/custom-topology.ipynb`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/usage/ls-coupling.ipynb` & `qrules-0.9.8/docs/usage/ls-coupling.ipynb`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/docs/usage/particle.ipynb` & `qrules-0.9.8/docs/usage/particle.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992399691358025%*

 * *Differences: {"'cells'": "{14: {'source': {insert: [(1, '    lambda p: p.strangeness == 1 and p.spin >= 1 and "*

 * *            "p.mass > 1.8 and p.mass < 1.9\\n')], delete: [4, 3, 2, 1]}}, 28: {'source': {insert: "*

 * *            '[(2, \'new_N1650_minus = create_antiparticle(new_N1650_plus, new_name="Modified '*

 * *            'N(1650)-")\\n\')], delete: [4, 3, 2]}}, 44: {\'source\': [\'As a side note, '*

 * *            '{mod}`qrules` provides [JSON schemas](https://json-schema.org) '*

 * *            '({download}`reaction/particle-valida […]*

```diff
@@ -151,18 +151,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "subset = particle_db.filter(\n",
-                "    lambda p: p.strangeness == 1\n",
-                "    and p.spin >= 1\n",
-                "    and p.mass > 1.8\n",
-                "    and p.mass < 1.9\n",
+                "    lambda p: p.strangeness == 1 and p.spin >= 1 and p.mass > 1.8 and p.mass < 1.9\n",
                 ")\n",
                 "subset.names"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -290,17 +287,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qrules.particle import create_antiparticle\n",
                 "\n",
-                "new_N1650_minus = create_antiparticle(\n",
-                "    new_N1650_plus, new_name=\"Modified N(1650)-\"\n",
-                ")\n",
+                "new_N1650_minus = create_antiparticle(new_N1650_plus, new_name=\"Modified N(1650)-\")\n",
                 "\n",
                 "particle_db.add(new_N1650_minus)\n",
                 "particle_db[\"Modified N(1650)-\"]"
             ]
         },
         {
             "cell_type": "markdown",
@@ -467,15 +462,15 @@
                 "output.names"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As a side note, {mod}`qrules` provides [JSON schemas](https://json-schema.org) ({download}`reaction/particle-validation.json <../../src/qrules/particle-validation.json>`) to validate your particle list files (see also {func}`jsonschema.validate`). If you have installed {mod}`qrules` as an {ref}`compwa-org:develop:Editable installation` and {ref}`use VSCode <develop:Visual Studio code>`, your YAML particle list are checked automatically in the GUI."
+                "As a side note, {mod}`qrules` provides [JSON schemas](https://json-schema.org) ({download}`reaction/particle-validation.json <../../src/qrules/particle-validation.json>`) to validate your particle list files (see also {func}`jsonschema.validators.validate`). If you have installed {mod}`qrules` as an {ref}`compwa-org:develop:Editable installation` and {ref}`use VSCode <develop:Visual Studio code>`, your YAML particle list are checked automatically in the GUI."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `qrules-0.9.7/docs/usage/reaction.ipynb` & `qrules-0.9.8/docs/usage/reaction.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9810891301597628%*

 * *Differences: {"'cells'": "{10: {'source': {insert: [(6, '    max_angular_momentum=2,\\n')]}}, 11: {'source': "*

 * *            "{insert: [(0, '```{admonition} State Transition Manager\\n'), (1, '---\\n'), (2, "*

 * *            "'class: dropdown\\n'), (3, '---\\n'), (4, 'The {class}`.StateTransitionManager` (STM) "*

 * *            'is the main user interface class of {mod}`qrules`. The boundary conditions of your '*

 * *            'physics problem, such as the initial state, final state, formalism type, etc., are '*

 * *            "defined  […]*

```diff
@@ -128,43 +128,39 @@
             "source": [
                 "from qrules import InteractionType, StateTransitionManager\n",
                 "\n",
                 "stm = StateTransitionManager(\n",
                 "    initial_state=[\"J/psi(1S)\"],\n",
                 "    final_state=[\"gamma\", \"pi0\", \"pi0\"],\n",
                 "    formalism=\"helicity\",\n",
+                "    max_angular_momentum=2,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "```{eval-rst}\n",
-                ".. admonition:: `.StateTransitionManager`\n",
-                "  :class: dropdown\n",
+                "```{admonition} State Transition Manager\n",
+                "---\n",
+                "class: dropdown\n",
+                "---\n",
+                "The {class}`.StateTransitionManager` (STM) is the main user interface class of {mod}`qrules`. The boundary conditions of your physics problem, such as the initial state, final state, formalism type, etc., are defined through this interface.\n",
                 "\n",
-                "  The `.StateTransitionManager` (STM) is the main user interface class of {mod}`qrules`. The boundary conditions of your physics problem, such as the initial state, final state, formalism type, etc., are defined through this interface.\n",
+                "* {meth}`.create_problem_sets` of the STM creates all problem sets \u2015 using the boundary conditions of the {obj}`.StateTransitionManager` instance. In total 3 steps are performed. The creation of reaction topologies. The creation of {obj}`.InitialFacts`, based on a topology and the initial and final state information. And finally the solving settings such as the conservation laws and quantum number domains to use at which point of the topology.\n",
                 "\n",
-                "  * `.create_problem_sets` of the STM creates all problem sets \u2015 using the boundary conditions of the `.StateTransitionManager` instance. In total 3 steps are performed. The creation of reaction topologies. The creation of `.InitialFacts`, based on a topology and the initial and final state information. And finally the solving settings such as the conservation laws and quantum number domains to use at which point of the topology.\n",
+                "* By default, all three interaction types ({attr}`~.InteractionType.EM`, {attr}`~.InteractionType.STRONG`, and {attr}`~.InteractionType.WEAK`) are used in the preparation stage. However, it is also possible to choose the allowed interaction types globally via {meth}`.set_allowed_interaction_types`.\n",
                 "\n",
-                "  * By default, all three interaction types (`~.InteractionType.EM`, `~.InteractionType.STRONG`, and `~.InteractionType.WEAK`) are used in the preparation stage. However, it is also possible to choose the allowed interaction types globally via `.set_allowed_interaction_types`.\n",
+                "  After the preparation step, you can modify the problem sets returned by {meth}`.create_problem_sets` to your liking. Since the output of this function contains quite a lot of information, {mod}`qrules` aids in the configuration (especially the STM).\n",
                 "\n",
-                "  After the preparation step, you can modify the problem sets returned by `.create_problem_sets` to your liking. Since the output of this function contains quite a lot of information, {mod}`qrules` aids in the configuration (especially the STM).\n",
+                "* A subset of particles that are allowed as intermediate states can also be specified: either through the {class}`STM's constructor <.StateTransitionManager>` or by setting the instance {code}`allowed_intermediate_particles`.\n",
+                "```\n",
                 "\n",
-                "  * A subset of particles that are allowed as intermediate states can also be specified: either through the `STM's constructor <.StateTransitionManager>` or by setting the instance :code:`allowed_intermediate_particles`.\n",
-                "```"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 ":::{tip}\n",
                 "\n",
                 "{doc}`custom-topology` shows how to provide custom {class}`.Topology` instances to the STM, so that you generate more than just isobar decays.\n",
                 "\n",
                 ":::"
             ]
         },
@@ -175,21 +171,16 @@
                 "## 2. Prepare Problem Sets"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Create all {class}`.ProblemSet`'s using the boundary conditions of the {class}`.StateTransitionManager` instance. By default it uses the **isobar model** (tree of two-body decays) to build {class}`.Topology`'s. Various {class}`.InitialFacts` are created for each topology based on the initial and final state. Lastly some reasonable default settings for the solving process are chosen. Remember that each interaction node defines its own set of conservation laws."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "Create all {class}`.ProblemSet`'s using the boundary conditions of the {class}`.StateTransitionManager` instance. By default it uses the **isobar model** (tree of two-body decays) to build {class}`.Topology`'s. Various {obj}`.InitialFacts` are created for each topology based on the initial and final state. Lastly some reasonable default settings for the solving process are chosen. Remember that each interaction node defines its own set of conservation laws.\n",
+                "\n",
                 "The {class}`.StateTransitionManager` (STM) defines three interaction types:"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -347,19 +338,15 @@
                 "reaction.get_intermediate_particles().names"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now note that, since a $\\gamma$ particle appears in one of the interaction nodes, {mod}`qrules` knows that this node **must involve EM interactions**! Because the node can be an effective interaction, the weak interaction cannot be excluded, as it contains only a subset of conservation laws.\n",
-                "\n",
-                "Since only the strong interaction was supposed to be used, this results in a warning and the STM automatically corrects the mistake.\n",
-                "\n",
-                "Once the EM interaction is included, this warning disappears. Be aware, however, that the EM interaction is now available globally. Hence, there now might be solutions in which both nodes are electromagnetic."
+                "Now note that, since a $\\gamma$ particle appears in one of the interaction nodes, {mod}`qrules` knows that this node **must involve EM interactions**! Because the node can be an effective interaction, the weak interaction cannot be excluded, as it contains only a subset of conservation laws. Since only the strong interaction was supposed to be used, this results in a warning and the STM automatically corrects the mistake. Once the EM interaction is included, this warning disappears."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -372,14 +359,54 @@
                 "reaction.get_intermediate_particles().names"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Be aware, however, that the {attr}`~.InteractionType.EM` interaction is now available globally, for each node in the decay topology. Hence, there now might be solutions in which both nodes are electromagnetic. This is fine for the decay $J/\\psi \\to \\gamma \\pi^0 \\pi^0$, but for decays that require the {attr}`~.InteractionType.WEAK` interaction type, you want to set the interaction type per **specific nodes**. Take for example the decay $\\Lambda_c^+ \\to p K^- \\pi^+$, which has a production node that is mediated by the weak force and a decay node that goes via the strong force. In this case, only limit the decay node to the {attr}`~.InteractionType.STRONG` force:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "lc2pkpi_stm = StateTransitionManager(\n",
+                "    initial_state=[\"Lambda(c)+\"],\n",
+                "    final_state=[\"p\", \"K-\", \"pi+\"],\n",
+                "    mass_conservation_factor=0.6,\n",
+                ")\n",
+                "lc2pkpi_stm.set_allowed_interaction_types([InteractionType.STRONG], node_id=1)\n",
+                "lc2pkpi_problem_sets = lc2pkpi_stm.create_problem_sets()\n",
+                "lc2pkpi_reaction = lc2pkpi_stm.find_solutions(lc2pkpi_problem_sets)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
+                "tags": [
+                    "hide-input"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "dot = io.asdot(lc2pkpi_reaction, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Great! Now we selected only the strongest contributions. Be aware, though, that there are more effects that can suppress certain decays, like small branching ratios. In this example, the initial state $J/\\Psi$ can decay into $\\pi^0 + \\rho^0$ or $\\pi^0 + \\omega$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -389,40 +416,57 @@
                 "| $\\rho^0\\to\\gamma+\\pi^0$ | 0.0006          |"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Unfortunately, the $\\rho^0$ mainly decays into $\\pi^0+\\pi^0$, not $\\gamma+\\pi^0$ and is therefore suppressed. This information is currently not known to {mod}`qrules`, but it is possible to hand {mod}`qrules` a list of allowed intermediate states."
+                "Unfortunately, the $\\rho^0$ mainly decays into $\\pi^0+\\pi^0$, not $\\gamma+\\pi^0$ and is therefore suppressed. This information is currently not known to {mod}`qrules`, but it is possible to hand {mod}`qrules` a list of allowed intermediate states,"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-output"
+                ]
             },
             "outputs": [],
             "source": [
-                "# particles are found by name comparison,\n",
-                "# i.e. f2 will find all f2's and f all f's independent of their spin\n",
                 "stm.set_allowed_intermediate_particles([\"f(0)\", \"f(2)\"])\n",
-                "\n",
                 "reaction = stm.find_solutions(problem_sets)\n",
-                "\n",
-                "print(\"found\", len(reaction.transitions), \"solutions!\")\n",
                 "reaction.get_intermediate_particles().names"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now we have selected all amplitudes that involve **f** states. The warnings appear only to notify the user that the list of solutions is not exhaustive: for certain edges in the graph, no suitable particle was found (since only f states were allowed)."
+                "or, using regular expressions,"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "stm.set_allowed_intermediate_particles(r\"f\\([02]\\)\", regex=True)\n",
+                "reaction = stm.find_solutions(problem_sets)\n",
+                "assert len(reaction.get_intermediate_particles().names) == 11"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now we have selected all amplitudes that involve **f** states:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -496,15 +540,17 @@
             "metadata": {},
             "source": [
                 "Handy if it takes a lot of computation time to re-generate the transitions!"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "```{tip}\n",
                 "The {mod}`ampform` package can formulate amplitude models based on the state transitions created by {mod}`qrules`. See {doc}`ampform:usage/amplitude`.\n",
                 "```"
             ]
         }
     ],
```

### Comparing `qrules-0.9.7/docs/usage/visualize.ipynb` & `qrules-0.9.8/docs/usage/visualize.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997674418604652%*

 * *Differences: {"'cells'": "{36: {'source': {insert: [(0, 'dot = qrules.io.asdot(reaction.transitions[:3], "*

 * *            "strip_spin=True, render_node=True)\\n')], delete: [2, 1, 0]}}}"}*

```diff
@@ -368,17 +368,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "dot = qrules.io.asdot(\n",
-                "    reaction.transitions[:3], strip_spin=True, render_node=True\n",
-                ")\n",
+                "dot = qrules.io.asdot(reaction.transitions[:3], strip_spin=True, render_node=True)\n",
                 "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `qrules-0.9.7/docs/usage.ipynb` & `qrules-0.9.8/docs/usage.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996%*

 * *Differences: {"'cells'": "{17: {'source': {insert: [(0, 'subset = pdg.filter(lambda p: p.spin in [2.5, 3.5, "*

 * *            '4.5] and p.name.startswith("N"))\\n\')], delete: [2, 1, 0]}}}'}*

```diff
@@ -196,17 +196,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "subset = pdg.filter(\n",
-                "    lambda p: p.spin in [2.5, 3.5, 4.5] and p.name.startswith(\"N\")\n",
-                ")\n",
+                "subset = pdg.filter(lambda p: p.spin in [2.5, 3.5, 4.5] and p.name.startswith(\"N\"))\n",
                 "subset.names"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `qrules-0.9.7/pyproject.toml` & `qrules-0.9.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,29 +19,32 @@
     | \.tox
     | \.venv
     | \.vscode
     | dist
 )/
 '''
 include = '\.pyi?$'
-line-length = 79
 preview = true
 target-version = [
+    "py310",
+    "py311",
     "py36",
     "py37",
     "py38",
     "py39",
 ]
 
 [tool.isort]
+known_third_party = "THIRDPARTY,particle"
 profile = "black"
 src_paths = [
     "src",
     "tests",
 ]
-line_length = 79
-known_third_party = "THIRDPARTY,particle"
 
 [tool.nbqa.addopts]
+black = [
+    "--line-length=85",
+]
 flake8 = [
     "--extend-ignore=E402,F821",
 ]
```

### Comparing `qrules-0.9.7/setup.cfg` & `qrules-0.9.8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
 	Typing :: Typed
 
 [options]
 python_requires = >=3.6
 setup_requires = 
@@ -45,63 +46,64 @@
 install_requires = 
 	attrs >=20.1.0  # on_setattr and https://www.attrs.org/en/stable/api.html#next-gen
 	jsonschema
 	particle
 	python-constraint
 	PyYAML
 	tqdm >=4.24.0  # autonotebook
-	typing-extensions; python_version <"3.8.0"
+	typing-extensions; python_version <"3.10.0"  # typing.TypeAlias
 packages = find:
 package_dir = 
 	=src
 
 [options.extras_require]
 viz = 
 	graphviz
 all = 
 	%(viz)s
 doc = 
 	%(viz)s
-	jupyter
-	myst-nb >=0.11  # myst_enable_extensions
-	nbclient >=0.5.5  # https://github.com/executablebooks/jupyter-book/issues/833
+	importlib-metadata; python_version <"3.8.0"
+	myst-nb  # nb_ configuration prefixes
 	Sphinx >=3
-	Sphinx <4.4; python_version <"3.8.0"  # https://github.com/ComPWA/qrules/runs/4833302679
 	sphinx-book-theme
 	sphinx-codeautolink[ipython]
 	sphinx-comments
 	sphinx-copybutton
-	sphinx-panels
+	sphinx-design
 	sphinx-thebe
 	sphinx-togglebutton
 	sphinxcontrib-bibtex >=2
 	sphinxcontrib-hep-pdgref
 	sphobjinv
 test = 
 	ipython
 	nbmake
+	nbmake !=1.3.*  # https://github.com/ComPWA/qrules/actions/runs/4116315964/jobs/7106216956#step:3:84
+	nbmake !=1.4.*  # https://github.com/ComPWA/qrules/actions/runs/4115785437/jobs/7104974879#step:3:82
 	pydot
 	pytest
 	pytest-cov
 	pytest-profiling
 	pytest-xdist
 format = 
 	black
 	isort
 flake8 = 
-	flake8 >=4  # extend-select
-	flake8-blind-except
-	flake8-bugbear
-	flake8-builtins
-	flake8-comprehensions
-	flake8-pytest-style
-	flake8-rst-docstrings
+	flake8 >=4; python_version >="3.8.0"
+	flake8-blind-except; python_version >="3.8.0"
+	flake8-bugbear; python_version >="3.8.0"
+	flake8-builtins; python_version >="3.8.0"
+	flake8-comprehensions; python_version >="3.8.0"
+	flake8-future-import; python_version >="3.8.0"
+	flake8-pytest-style; python_version >="3.8.0"
+	flake8-rst-docstrings; python_version >="3.8.0"
 	flake8-type-ignore; python_version >="3.8.0"
-	flake8-use-fstring
-	pep8-naming
+	flake8-use-fstring; python_version >="3.8.0"
+	pep8-naming; python_version >="3.8.0"
 mypy = 
 	mypy >=0.730  # attrs and error code support
 	types-docutils
 	types-pkg-resources
 	types-PyYAML
 	types-requests
 	types-setuptools
@@ -111,26 +113,31 @@
 	pydocstyle
 	pylint >=2.5  # good-names-rgxs
 sty = 
 	%(format)s
 	%(lint)s
 	%(test)s  # for pytest type hints
 	pre-commit >=1.4.0
+jupyter = 
+	aquirdturtle-collapsible-headings
+	jupyterlab
+	jupyterlab-code-formatter
+	jupyterlab-myst; python_version >="3.7.0"
+	ypy-websocket <0.8.3; python_version >="3.7.0"  # https://github.com/ComPWA/qrules/actions/runs/4350315417/jobs/7600906057#step:3:79
 dev = 
 	%(all)s
 	%(doc)s
+	%(jupyter)s
 	%(sty)s
 	%(test)s
-	aquirdturtle-collapsible-headings
-	jupyterlab
-	jupyterlab-code-formatter
-	jupyterlab-myst; python_version >="3.7.0"
-	pip-tools >=6.1.0  # for extras_require
 	sphinx-autobuild
 	tox >=1.9  # for skip_install, use_develop
+	tox !=4.*; python_version <"3.8.0"  # https://github.com/ComPWA/qrules/actions/runs/4116409504/jobs/7106431526#step:3:92
+	virtualenv !=20.16.*; python_version <"3.7.0"  # https://github.com/ComPWA/qrules/actions/runs/4116487921/jobs/7106603597#step:3:78
+	virtualenv !=20.17.*; python_version <"3.7.0"  # https://github.com/ComPWA/qrules/actions/runs/4116447949/jobs/7106515800#step:3:78
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 qrules = 
 	additional_definitions.yml
```

### Comparing `qrules-0.9.7/src/qrules/__init__.py` & `qrules-0.9.8/src/qrules/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 # pylint: disable=too-many-lines
 """A rule based system that facilitates particle reaction analysis.
 
-QRules generates allowed particle transitions from a set of conservation rules
-and boundary conditions as specified by the user. The user boundary conditions
-for a particle reaction problem are for example the initial state, final state,
-and allowed interactions.
+QRules generates allowed particle transitions from a set of conservation rules and
+boundary conditions as specified by the user. The user boundary conditions for a
+particle reaction problem are for example the initial state, final state, and allowed
+interactions.
 
 The core of `qrules` computes which transitions (represented by a
 `.StateTransitionGraph`) are allowed between a certain initial and final state.
-Internally, the system propagates the quantum numbers defined by the
-`particle` module through the `.StateTransitionGraph`, while
-satisfying the rules define by the :mod:`.conservation_rules` module. See
-:doc:`/usage/reaction` and :doc:`/usage/particle`.
+Internally, the system propagates the quantum numbers defined by the `particle` module
+through the `.StateTransitionGraph`, while satisfying the rules define by the
+:mod:`.conservation_rules` module. See :doc:`/usage/reaction` and
+:doc:`/usage/particle`.
 
-Finally, the `.io` module provides tools that can read and write the objects of
-this framework.
+Finally, the `.io` module provides tools that can read and write the objects of this
+framework.
 """
 
 from itertools import product
-from typing import (
-    Dict,
-    FrozenSet,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Set,
-    Union,
-)
+from typing import Dict, FrozenSet, Iterable, List, Optional, Sequence, Set, Union
 
 import attrs
 
 from . import io
 from .combinatorics import InitialFacts, StateDefinition, create_initial_facts
 from .conservation_rules import (
     BaryonNumberConservation,
@@ -58,28 +49,17 @@
 from .quantum_numbers import InteractionProperties
 from .settings import (
     ADDITIONAL_PARTICLES_DEFINITIONS_PATH,
     InteractionType,
     _halves_domain,
     _int_domain,
 )
-from .solving import (
-    GraphSettings,
-    NodeSettings,
-    QNResult,
-    Rule,
-    validate_full_solution,
-)
+from .solving import GraphSettings, NodeSettings, QNResult, Rule, validate_full_solution
 from .topology import create_n_body_topology
-from .transition import (
-    EdgeSettings,
-    ProblemSet,
-    ReactionInfo,
-    StateTransitionManager,
-)
+from .transition import EdgeSettings, ProblemSet, ReactionInfo, StateTransitionManager
 
 
 def check_reaction_violations(  # pylint: disable=too-many-arguments
     initial_state: Union[StateDefinition, Sequence[StateDefinition]],
     final_state: Sequence[StateDefinition],
     mass_conservation_factor: Optional[float] = 3.0,
     particle_db: Optional[ParticleCollection] = None,
@@ -95,28 +75,27 @@
 
     Args:
       initial_state: Shortform description of the initial state w/o spin
         projections.
       final_state: Shortform description of the final state w/o spin
         projections.
       mass_conservation_factor: Factor with which the width is multiplied when
-        checking for `.MassConservation`. Set to `None` in order to deactivate
-        mass conservation.
+        checking for `.MassConservation`. Set to `None` in order to deactivate mass
+        conservation.
       particle_db (Optional): Custom `.ParticleCollection` object.  Defaults to
         the `.ParticleCollection` returned by `.load_pdg`.
       max_angular_momentum: Maximum angular momentum over which to generate
         :math:`LS`-couplings.
       max_spin_magnitude: Maximum spin magnitude over which to generate
         :math:`LS`-couplings.
 
     Returns:
-      Set of least violating rules. The set can have multiple entries, as
-      several quantum numbers can be violated. Each entry in the frozenset
-      represents a group of rules that together violate all possible quantum
-      number configurations.
+      Set of least violating rules. The set can have multiple entries, as several
+      quantum numbers can be violated. Each entry in the frozenset represents a group of
+      rules that together violate all possible quantum number configurations.
 
     Example:
         >>> import qrules
         >>> qrules.check_reaction_violations(
         ...     initial_state="pi0",
         ...     final_state=["gamma", "gamma", "gamma"],
         ... )
@@ -159,71 +138,60 @@
         }
 
         edge_check_result = _check_violations(
             initial_facts[0],
             node_rules={},
             edge_rules={
                 edge_id: pure_edge_rules
-                for edge_id in topology.incoming_edge_ids
-                | topology.outgoing_edge_ids
+                for edge_id in topology.incoming_edge_ids | topology.outgoing_edge_ids
             },
         )
 
         if edge_check_result.violated_edge_rules:
             raise ValueError(
-                "Some edges violate"
-                f" {edge_check_result.violated_edge_rules.values()}"
+                f"Some edges violate {edge_check_result.violated_edge_rules.values()}"
             )
 
     def check_edge_qn_conservation() -> Set[FrozenSet[str]]:
         """Check if edge quantum numbers are conserved.
 
-        Those rules give the same results, independent on the node and spin
-        props. Note they are also independent of the topology and hence their
-        results are always correct.
+        Those rules give the same results, independent on the node and spin props. Note
+        they are also independent of the topology and hence their results are always
+        correct.
         """
         edge_qn_conservation_rules: Set[Rule] = {
-            BaryonNumberConservation(),
-            BottomnessConservation(),
-            ChargeConservation(),
-            CharmConservation(),
-            ElectronLNConservation(),
-            MuonLNConservation(),
-            StrangenessConservation(),
-            TauLNConservation(),
+            BaryonNumberConservation(),  # type: ignore[abstract]
+            BottomnessConservation(),  # type: ignore[abstract]
+            ChargeConservation(),  # type: ignore[abstract]
+            CharmConservation(),  # type: ignore[abstract]
+            ElectronLNConservation(),  # type: ignore[abstract]
+            MuonLNConservation(),  # type: ignore[abstract]
+            StrangenessConservation(),  # type: ignore[abstract]
+            TauLNConservation(),  # type: ignore[abstract]
             isospin_conservation,
         }
         if len(initial_state) == 1 and mass_conservation_factor is not None:
-            edge_qn_conservation_rules.add(
-                MassConservation(mass_conservation_factor)
-            )
+            edge_qn_conservation_rules.add(MassConservation(mass_conservation_factor))
 
         return {
             frozenset((x,))
             for x in _check_violations(
                 initial_facts[0],
-                node_rules={
-                    i: edge_qn_conservation_rules for i in topology.nodes
-                },
+                node_rules={i: edge_qn_conservation_rules for i in topology.nodes},
                 edge_rules={},
             ).violated_node_rules[node_id]
         }
 
     # Using a n-body topology is enough, to determine the violations reliably
     # since only certain spin rules require the isobar model. These spin rules
     # are not required here though.
     topology = create_n_body_topology(len(initial_state), len(final_state))
     node_id = next(iter(topology.nodes))
 
-    initial_facts = create_initial_facts(
-        topology=topology,
-        particle_db=particle_db,
-        initial_state=initial_state,
-        final_state=final_state,
-    )
+    initial_facts = create_initial_facts(initial_state, final_state, particle_db)
 
     check_pure_edge_rules()
     violations = check_edge_qn_conservation()
 
     # Create combinations of graphs for magnitudes of S and L, but only
     # if it is a two body reaction
     ls_combinations = [
@@ -297,45 +265,43 @@
     max_angular_momentum: int = 2,
     max_spin_magnitude: float = 2.0,
     topology_building: str = "isobar",
     number_of_threads: Optional[int] = None,
 ) -> ReactionInfo:
     """Generate allowed transitions between an initial and final state.
 
-    Serves as a facade to the `.StateTransitionManager` (see
-    :doc:`/usage/reaction`).
+    Serves as a facade to the `.StateTransitionManager` (see :doc:`/usage/reaction`).
 
     Arguments:
         initial_state (list): A list of particle names in the initial
-            state. You can specify spin projections for these particles with a
-            `tuple`, e.g. :code:`("J/psi(1S)", [-1, 0, +1])`. If spin
-            projections are not specified, all projections are taken, so the
-            example here would be equivalent to :code:`"J/psi(1S)"`.
+            state. You can specify spin projections for these particles with a `tuple`,
+            e.g. :code:`("J/psi(1S)", [-1, 0, +1])`. If spin projections are not
+            specified, all projections are taken, so the example here would be
+            equivalent to :code:`"J/psi(1S)"`.
 
         final_state (list): Same as :code:`initial_state`, but for final state
             particles.
 
         allowed_intermediate_particles (`list`, optional): A list of particle
-            states that you want to allow as intermediate states. This helps
-            (1) filter out resonances and (2) speed up computation time.
+            states that you want to allow as intermediate states. This helps (1) filter
+            out resonances and (2) speed up computation time.
 
         allowed_interaction_types: Interaction types you want to consider. For
             instance, :code:`["s", "em"]` results in `~.InteractionType.EM` and
             `~.InteractionType.STRONG` and :code:`["strong"]` results in
             `~.InteractionType.STRONG`.
 
         formalism (`str`, optional): Formalism that you intend to use in
             the eventual amplitude model.
 
         particle_db (`.ParticleCollection`, optional): The particles that you
-            want to be involved in the reaction. Uses `.load_pdg` by default.
-            It's better to use a subset for larger reactions, because of
-            the computation times. This argument is especially useful when you
-            want to use your own particle definitions (see
-            :doc:`/usage/particle`).
+            want to be involved in the reaction. Uses `.load_pdg` by default. It's
+            better to use a subset for larger reactions, because of the computation
+            times. This argument is especially useful when you want to use your own
+            particle definitions (see :doc:`/usage/particle`).
 
         mass_conservation_factor: Width factor that is taken into account for
             for the `.MassConservation` rule.
 
         max_angular_momentum: Maximum angular momentum over which to generate
             angular momenta.
 
@@ -349,16 +315,16 @@
             - :code:`"nbody"`: Use one central node and connect initial and final
               states to it
 
         number_of_threads: Number of cores with which to compute the allowed
             transitions. Defaults to the current value returned by
             :meth:`.settings.NumberOfThreads.get`.
 
-    An example (where, for illustrative purposes only, we specify all
-    arguments) would be:
+    An example (where, for illustrative purposes only, we specify all arguments) would
+    be:
 
     >>> import qrules
     >>> reaction = qrules.generate_transitions(
     ...     initial_state="D0",
     ...     final_state=["K~0", "K+", "K-"],
     ...     allowed_intermediate_particles=["a(0)(980)", "a(2)(1320)-"],
     ...     allowed_interaction_types=["e", "w"],
@@ -387,17 +353,15 @@
         max_angular_momentum=max_angular_momentum,
         max_spin_magnitude=max_spin_magnitude,
         topology_building=topology_building,
         number_of_threads=number_of_threads,
     )
     if allowed_interaction_types is not None:
         if isinstance(allowed_interaction_types, str):
-            interaction_types = [
-                InteractionType.from_str(allowed_interaction_types)
-            ]
+            interaction_types = [InteractionType.from_str(allowed_interaction_types)]
         else:
             interaction_types = [
                 InteractionType.from_str(description)
                 for description in allowed_interaction_types
             ]
         stm.set_allowed_interaction_types(list(interaction_types))
     problem_sets = stm.create_problem_sets()
```

### Comparing `qrules-0.9.7/src/qrules/_system_control.py` & `qrules-0.9.8/src/qrules/_system_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     NodeQuantumNumbers,
     Parity,
 )
 from .settings import InteractionType
 from .solving import GraphEdgePropertyMap, GraphNodePropertyMap, GraphSettings
 from .topology import StateTransitionGraph
 
+_LOGGER = logging.getLogger(__name__)
+
 Strength = float
 
-GraphSettingsGroups = Dict[
-    Strength, List[Tuple[StateTransitionGraph, GraphSettings]]
-]
+GraphSettingsGroups = Dict[Strength, List[Tuple[StateTransitionGraph, GraphSettings]]]
 
 
 def create_edge_properties(
     particle: Particle,
     spin_projection: Optional[float] = None,
 ) -> GraphEdgePropertyMap:
     edge_qn_mapping: Dict[str, Type[EdgeQuantumNumber]] = {
@@ -48,17 +48,15 @@
             elif "spin" in qn_name:
                 property_map[EdgeQuantumNumbers.spin_magnitude] = value
 
     if spin_projection is not None:
         property_map[EdgeQuantumNumbers.spin_projection] = spin_projection
     if isospin is not None:
         property_map[EdgeQuantumNumbers.isospin_magnitude] = isospin.magnitude
-        property_map[
-            EdgeQuantumNumbers.isospin_projection
-        ] = isospin.projection
+        property_map[EdgeQuantumNumbers.isospin_projection] = isospin.projection
     return property_map
 
 
 def create_node_properties(
     node_props: InteractionProperties,
 ) -> GraphNodePropertyMap:
     node_qn_mapping: Dict[str, Type[NodeQuantumNumber]] = {
@@ -77,71 +75,70 @@
                 "Missmatch between InteractionProperties and"
                 " NodeQuantumNumbers. NodeQuantumNumbers does not define"
                 f" {qn_name}"
             )
     return property_map
 
 
-def create_particle(
-    edge_props: GraphEdgePropertyMap, particle_db: ParticleCollection
+def find_particle(
+    state: GraphEdgePropertyMap, particle_db: ParticleCollection
 ) -> ParticleWithSpin:
     """Create a Particle with spin projection from a qn dictionary.
 
-    The implementation assumes the edge properties match the attributes of a
-    particle inside the `.ParticleCollection`.
+    The implementation assumes the edge properties match the attributes of a particle
+    inside the `.ParticleCollection`.
 
     Args:
         edge_props: The quantum number dictionary.
         particle_db: A `.ParticleCollection` which is used to retrieve a
           reference `.particle` to lower the memory footprint.
 
     Raises:
-        KeyError: If the edge properties do not contain the pid information or
-          no particle with the same pid is found in the `.ParticleCollection`.
+        KeyError: If the edge properties do not contain the pid information or no
+            particle with the same pid is found in the `.ParticleCollection`.
 
         ValueError: If the edge properties do not contain spin projection info.
     """
-    particle = particle_db.find(int(edge_props[EdgeQuantumNumbers.pid]))
-    if EdgeQuantumNumbers.spin_projection not in edge_props:
+    particle = particle_db.find(int(state[EdgeQuantumNumbers.pid]))
+    spin_projection = state.get(EdgeQuantumNumbers.spin_projection)
+    if spin_projection is None:
         raise ValueError(
-            f"{GraphEdgePropertyMap.__name__} does not contain a spin"
-            " projection"
+            f"{GraphEdgePropertyMap.__name__} does not contain a spin projection"
         )
-    spin_projection = edge_props[EdgeQuantumNumbers.spin_projection]
-
-    return (particle, spin_projection)
+    return particle, spin_projection
 
 
 def create_interaction_properties(
     qn_solution: GraphNodePropertyMap,
 ) -> InteractionProperties:
     converted_solution = {k.__name__: v for k, v in qn_solution.items()}
     kw_args = {
         x.name: converted_solution[x.name]
-        for x in attrs.fields(InteractionProperties)
+        for x in attrs.fields(InteractionProperties)  # type: ignore[arg-type]
         if x.name in converted_solution
     }
 
-    return attrs.evolve(InteractionProperties(), **kw_args)
+    return attrs.evolve(InteractionProperties(), **kw_args)  # type: ignore[arg-type]
 
 
 def filter_interaction_types(
     valid_determined_interaction_types: List[InteractionType],
     allowed_interaction_types: List[InteractionType],
 ) -> List[InteractionType]:
     int_type_intersection = list(
-        set(allowed_interaction_types)
-        & set(valid_determined_interaction_types)
+        set(allowed_interaction_types) & set(valid_determined_interaction_types)
     )
     if int_type_intersection:
         return int_type_intersection
-    logging.warning(
-        "The specified list of interaction types %s"
-        " does not intersect with the valid list of interaction types %s"
-        ".\nUsing valid list instead.",
+    _LOGGER.warning(
+        (
+            "The specified list of interaction types %s"
+            " does not intersect with the valid list of interaction types %s"
+            ".\nUsing valid list instead."
+        ),
         allowed_interaction_types,
         valid_determined_interaction_types,
     )
     return valid_determined_interaction_types
 
 
 class InteractionDeterminator(ABC):
@@ -201,17 +198,17 @@
     remove_qns_list: Optional[Set[Type[NodeQuantumNumber]]] = None,
     ignore_qns_list: Optional[Set[Type[NodeQuantumNumber]]] = None,
 ) -> List[StateTransitionGraph[ParticleWithSpin]]:
     if remove_qns_list is None:
         remove_qns_list = set()
     if ignore_qns_list is None:
         ignore_qns_list = set()
-    logging.info("removing duplicate solutions...")
-    logging.info(f"removing these qns from graphs: {remove_qns_list}")
-    logging.info(f"ignoring qns in graph comparison: {ignore_qns_list}")
+    _LOGGER.info("removing duplicate solutions...")
+    _LOGGER.info(f"removing these qns from graphs: {remove_qns_list}")
+    _LOGGER.info(f"ignoring qns in graph comparison: {ignore_qns_list}")
 
     filtered_solutions: List[StateTransitionGraph[ParticleWithSpin]] = []
     remove_counter = 0
     for sol_graph in solutions:
         sol_graph = _remove_qns_from_graph(sol_graph, remove_qns_list)
         found_graph = _check_equal_ignoring_qns(
             sol_graph, filtered_solutions, ignore_qns_list
@@ -219,15 +216,15 @@
         if found_graph is None:
             filtered_solutions.append(sol_graph)
         else:
             # check if found solution also has the prefactors
             # if not overwrite them
             remove_counter += 1
 
-    logging.info(f"removed {remove_counter} solutions")
+    _LOGGER.info(f"removed {remove_counter} solutions")
     return filtered_solutions
 
 
 def _remove_qns_from_graph(  # pylint: disable=too-many-branches
     graph: StateTransitionGraph[ParticleWithSpin],
     qn_list: Set[Type[NodeQuantumNumber]],
 ) -> StateTransitionGraph[ParticleWithSpin]:
@@ -244,17 +241,15 @@
 def _check_equal_ignoring_qns(
     ref_graph: StateTransitionGraph,
     solutions: List[StateTransitionGraph],
     ignored_qn_list: Set[Type[NodeQuantumNumber]],
 ) -> Optional[StateTransitionGraph]:
     """Define equal operator for graphs, ignoring certain quantum numbers."""
     if not isinstance(ref_graph, StateTransitionGraph):
-        raise TypeError(
-            "Reference graph has to be of type StateTransitionGraph"
-        )
+        raise TypeError("Reference graph has to be of type StateTransitionGraph")
     found_graph = None
     node_comparator = NodePropertyComparator(ignored_qn_list)
     for graph in solutions:
         if isinstance(graph, StateTransitionGraph):
             if graph.compare(
                 ref_graph,
                 edge_comparator=lambda e1, e2: e1 == e2,
@@ -298,16 +293,15 @@
     `.StateTransitionGraph` 's from a list. Only the graphs passing
     all supplied filters will be returned.
 
     Note:
         For the more advanced user, lambda functions can be used as filters.
 
     Example:
-        Selecting only the solutions, in which the :math:`\rho` decays via
-        p-wave:
+        Selecting only the solutions, in which the :math:`\rho` decays via p-wave:
 
         .. code-block:: python
 
             my_filter = require_interaction_property(
                 "rho",
                 InteractionQuantumNumberNames.L,
                 create_spin_domain([1], True),
@@ -327,31 +321,30 @@
     interaction_qn: Type[NodeQuantumNumber],
     allowed_values: List,
 ) -> Callable[[StateTransitionGraph[ParticleWithSpin]], bool]:
     """Filter function.
 
     Closure, which can be used as a filter function in :func:`.filter_graphs`.
 
-    It selects graphs based on a requirement on the property of specific
-    interaction nodes.
+    It selects graphs based on a requirement on the property of specific interaction
+    nodes.
 
     Args:
         ingoing_particle_name (str): name of particle, used to find nodes which
             have a particle with this name as "ingoing"
 
         interaction_qn ([Type[NodeQuantumNumber]]): interaction quantum number
 
         allowed_values (list): list of allowed values, that the interaction
             quantum number may take
 
     Return:
         Callable[Any, bool]:
-            - *True* if the graph has nodes with an ingoing particle of the
-              given name, and the graph fullfills the quantum number
-              requirement
+            - *True* if the graph has nodes with an ingoing particle of the given name,
+              and the graph fullfills the quantum number requirement
             - *False* otherwise
     """
 
     def check(graph: StateTransitionGraph[ParticleWithSpin]) -> bool:
         node_ids = _find_node_ids_with_ingoing_particle_name(
             graph, ingoing_particle_name
         )
```

### Comparing `qrules-0.9.7/src/qrules/argument_handling.py` & `qrules-0.9.8/src/qrules/argument_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Handles argument handling for rules.
 
-Responsibilities are the check of requirements for rules and the creation of
-the arguments from general graph property maps. The information is extracted
-from the type annotations of the rules.
+Responsibilities are the check of requirements for rules and the creation of the
+arguments from general graph property maps. The information is extracted from the type
+annotations of the rules.
 """
 
 import inspect
 from typing import (
     Any,
     Callable,
     Dict,
@@ -31,15 +31,15 @@
 from .quantum_numbers import EdgeQuantumNumber, NodeQuantumNumber, Parity
 
 Scalar = Union[int, float]
 
 # InteractionRule = Union[EdgeQNConservationRule, ConservationRule]
 Rule = Union[GraphElementRule, EdgeQNConservationRule, ConservationRule]
 
-_ElementType = TypeVar("_ElementType")
+_ElementType = TypeVar("_ElementType")  # pylint: disable=invalid-name
 
 GraphElementPropertyMap = Dict[Type[_ElementType], Scalar]
 GraphEdgePropertyMap = GraphElementPropertyMap[EdgeQuantumNumber]
 GraphNodePropertyMap = GraphElementPropertyMap[NodeQuantumNumber]
 
 
 def _is_optional(field_type: Optional[type]) -> bool:
@@ -49,41 +49,39 @@
     ):
         return True
     return False
 
 
 def _is_sequence_type(input_type: type) -> bool:
     origin = getattr(input_type, "__origin__", None)
+    # pylint: disable=unhashable-member
     return origin in {list, tuple, List, Tuple}
 
 
 def _is_edge_quantum_number(qn_type: Any) -> bool:
     return qn_type in EdgeQuantumNumber.__args__  # type: ignore[attr-defined]
 
 
 def _is_node_quantum_number(qn_type: Any) -> bool:
     return qn_type in NodeQuantumNumber.__args__  # type: ignore[attr-defined]
 
 
 class _CompositeArgumentCheck:
     def __init__(
         self,
-        class_field_types: Union[
-            List[EdgeQuantumNumber], List[NodeQuantumNumber]
-        ],
+        class_field_types: Union[List[EdgeQuantumNumber], List[NodeQuantumNumber]],
     ) -> None:
         self.__class_field_types = class_field_types
 
     def __call__(
         self,
         props: GraphElementPropertyMap,
     ) -> bool:
         return all(
-            class_field_type in props
-            for class_field_type in self.__class_field_types
+            class_field_type in props for class_field_type in self.__class_field_types
         )
 
 
 def _direct_qn_check(
     qn_type: Union[Type[EdgeQuantumNumber], Type[NodeQuantumNumber]]
 ) -> Callable[[GraphElementPropertyMap], bool]:
     def wrapper(props: GraphElementPropertyMap) -> bool:
@@ -127,17 +125,15 @@
         self, props: GraphElementPropertyMap[_ElementType]
     ) -> Optional[_ElementType]:
         if self.__obj_type in props:
             return self.__extract(props)
 
         return None
 
-    def __extract(
-        self, props: GraphElementPropertyMap[_ElementType]
-    ) -> _ElementType:
+    def __extract(self, props: GraphElementPropertyMap[_ElementType]) -> _ElementType:
         value = props[self.__obj_type]
         if value is None:
             return None
         if (
             "__supertype__" in self.__obj_type.__dict__
             and self.__obj_type.__supertype__ == Parity  # type: ignore[attr-defined]
         ):
@@ -145,19 +141,19 @@
         return self.__obj_type(value)  # type: ignore[call-arg]
 
 
 class _CompositeArgumentCreator:
     def __init__(self, class_type: type) -> None:
         self.__class_type = class_type
         self.__extractors = {
-            class_field.name: _ValueExtractor[EdgeQuantumNumber](
-                class_field.type
+            class_field.name: (
+                _ValueExtractor[EdgeQuantumNumber](class_field.type)
+                if _is_edge_quantum_number(class_field.type)
+                else _ValueExtractor[NodeQuantumNumber](class_field.type)
             )
-            if _is_edge_quantum_number(class_field.type)
-            else _ValueExtractor[NodeQuantumNumber](class_field.type)
             for class_field in attrs.fields(class_type)
         }
 
     def __call__(
         self,
         props: GraphElementPropertyMap,
     ) -> Any:
@@ -208,17 +204,15 @@
 
             if attrs.has(qn_type):
                 class_field_types = [
                     class_field.type
                     for class_field in attrs.fields(qn_type)
                     if not _is_optional(class_field.type)
                 ]
-                qn_check_function: Callable[
-                    ..., bool
-                ] = _CompositeArgumentCheck(
+                qn_check_function: Callable[..., bool] = _CompositeArgumentCheck(
                     class_field_types  # type: ignore[arg-type]
                 )
             else:
                 qn_check_function = _direct_qn_check(qn_type)
 
             if is_list:
                 qn_check_function = _sequence_input_check(qn_check_function)
@@ -236,17 +230,15 @@
             is_list = False
             qn_type = input_type
             if _is_sequence_type(input_type):
                 qn_type = input_type.__args__[0]  # type: ignore[attr-defined]
                 is_list = True
 
             if attrs.has(qn_type):
-                arg_builder: Callable[..., Any] = _CompositeArgumentCreator(
-                    qn_type
-                )
+                arg_builder: Callable[..., Any] = _CompositeArgumentCreator(qn_type)
             else:
                 if _is_edge_quantum_number(qn_type):
                     arg_builder = _ValueExtractor[EdgeQuantumNumber](qn_type)
                 elif _is_node_quantum_number(qn_type):
                     arg_builder = _ValueExtractor[NodeQuantumNumber](qn_type)
                 else:
                     raise TypeError(
@@ -265,42 +257,38 @@
         if (
             rule not in self.__rule_to_requirements_check
             or rule not in self.__rule_to_argument_builder
         ):
             rule_annotations = []
             rule_func_signature = inspect.signature(rule)
             if not rule_func_signature.return_annotation:
-                raise TypeError(
-                    f"missing return type annotation for rule {str(rule)}"
-                )
+                raise TypeError(f"missing return type annotation for rule {str(rule)}")
             for par in rule_func_signature.parameters.values():
                 if not par.annotation:
                     raise TypeError(
                         f"missing type annotations for argument {par.name}"
                         f" of rule {str(rule)}"
                     )
                 rule_annotations.append(par.annotation)
 
             # check type annotations are legal
             try:
                 self.__verify(rule_annotations)
             except TypeError as exception:
-                raise TypeError(
-                    f"rule {str(rule)}: {str(exception)}"
-                ) from exception
+                raise TypeError(f"rule {str(rule)}: {str(exception)}") from exception
 
             # then create requirements check function and add to dict
-            self.__rule_to_requirements_check[
-                rule
-            ] = self.__create_requirements_check(rule_annotations)
+            self.__rule_to_requirements_check[rule] = self.__create_requirements_check(
+                rule_annotations
+            )
 
             # then create arguments builder function and add to dict
-            self.__rule_to_argument_builder[
-                rule
-            ] = self.__create_argument_builder(rule_annotations)
+            self.__rule_to_argument_builder[rule] = self.__create_argument_builder(
+                rule_annotations
+            )
 
         return (
             self.__rule_to_requirements_check[rule],
             self.__rule_to_argument_builder[rule],
         )
```

### Comparing `qrules-0.9.7/src/qrules/combinatorics.py` & `qrules-0.9.8/src/qrules/combinatorics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Perform permutations on the edges of a `.StateTransitionGraph`.
 
-In a `.StateTransitionGraph`, the edges represent quantum states, while the
-nodes represent interactions. This module provides tools to permutate, modify
-or extract these edge and node properties.
+In a `.StateTransitionGraph`, the edges represent quantum states, while the nodes
+represent interactions. This module provides tools to permutate, modify or extract these
+edge and node properties.
 """
 
+import itertools
 from collections import OrderedDict
 from copy import deepcopy
-from itertools import permutations
 from typing import (
     Any,
     Callable,
     Dict,
-    Generator,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
-    Sized,
     Tuple,
     Union,
 )
 
 from attrs import field, frozen
 
 from qrules._implementers import implement_pretty_repr
-from qrules.particle import Particle, ParticleCollection
-
-from .particle import ParticleWithSpin
-from .quantum_numbers import InteractionProperties, arange
-from .topology import StateTransitionGraph, Topology, get_originating_node_list
+from qrules.particle import ParticleCollection, ParticleWithSpin
+from qrules.quantum_numbers import InteractionProperties, arange
+from qrules.topology import StateTransitionGraph, Topology, get_originating_node_list
 
 StateWithSpins = Tuple[str, Sequence[float]]
 StateDefinition = Union[str, StateWithSpins]
 
 
 @implement_pretty_repr
 @frozen
@@ -43,41 +39,40 @@
     edge_props: Dict[int, ParticleWithSpin] = field(factory=dict)
     node_props: Dict[int, InteractionProperties] = field(factory=dict)
 
 
 class _KinematicRepresentation:
     def __init__(
         self,
-        final_state: Optional[Union[Sequence[List[Any]], List[Any]]] = None,
-        initial_state: Optional[Union[Sequence[List[Any]], List[Any]]] = None,
+        final_state: Optional[Union[List[List[str]], List[str]]] = None,
+        initial_state: Optional[Union[List[List[str]], List[str]]] = None,
     ) -> None:
-        self.__initial_state: Optional[List[List[Any]]] = None
-        self.__final_state: Optional[List[List[Any]]] = None
+        self.__initial_state: Optional[List[List[str]]] = None
+        self.__final_state: Optional[List[List[str]]] = None
         if initial_state is not None:
-            self.__initial_state = self.__import(initial_state)
+            self.__initial_state = _sort_nested(ensure_nested_list(initial_state))
         if final_state is not None:
-            self.__final_state = self.__import(final_state)
+            self.__final_state = _sort_nested(ensure_nested_list(final_state))
 
     @property
-    def initial_state(self) -> Optional[List[List[Any]]]:
+    def initial_state(self) -> Optional[List[List[str]]]:
         return self.__initial_state
 
     @property
-    def final_state(self) -> Optional[List[List[Any]]]:
+    def final_state(self) -> Optional[List[List[str]]]:
         return self.__final_state
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, _KinematicRepresentation):
             return (
                 self.initial_state == other.initial_state
                 and self.final_state == other.final_state
             )
         raise ValueError(
-            f"Cannot compare {self.__class__.__name__} with"
-            f" {other.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with {other.__class__.__name__}"
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}("
             f"initial_state={self.initial_state}, "
             f"final_state={self.final_state})"
@@ -93,81 +88,60 @@
             [["gamma", "pi0"], ["gamma", "pi0", "pi0"]]
 
         This list will be compared **only** with the
         `~KinematicRepresentation.final_state`!
         """
 
         def is_sublist(
-            sub_representation: Optional[List[List[Any]]],
-            main_representation: Optional[List[List[Any]]],
+            sub_representation: Optional[List[List[str]]],
+            main_representation: Optional[List[List[str]]],
         ) -> bool:
             if main_representation is None:
                 if sub_representation is None:
                     return True
                 return False
             if sub_representation is None:
                 return True
             for group in sub_representation:
                 if group not in main_representation:
                     return False
             return True
 
         if isinstance(other, _KinematicRepresentation):
-            return is_sublist(
-                other.initial_state, self.initial_state
-            ) and is_sublist(other.final_state, self.final_state)
+            return is_sublist(other.initial_state, self.initial_state) and is_sublist(
+                other.final_state, self.final_state
+            )
         if isinstance(other, list):
             for item in other:
                 if not isinstance(item, list):
                     raise ValueError(
                         "Comparison representation needs to be a list of lists"
                     )
             return is_sublist(other, self.final_state)
         raise ValueError(
-            f"Cannot compare {self.__class__.__name__} with"
-            f" {other.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with {other.__class__.__name__}"
         )
 
-    def __import(
-        self, nested_list: Union[Sequence[Sequence[Any]], Sequence[Any]]
-    ) -> List[List[Any]]:
-        return self.__sort(self.__prepare(nested_list))
-
-    def __prepare(
-        self, nested_list: Union[Sequence[Sequence[Any]], Sequence[Any]]
-    ) -> List[List[Any]]:
-        if len(nested_list) == 0 or not isinstance(nested_list[0], list):
-            nested_list = [nested_list]
-        return [
-            [self.__extract_particle_name(item) for item in sub_list]
-            for sub_list in nested_list
-        ]
 
-    @staticmethod
-    def __sort(nested_list: List[List[Any]]) -> List[List[Any]]:
-        return sorted(sorted(sub_list) for sub_list in nested_list)
-
-    @staticmethod
-    def __extract_particle_name(item: object) -> str:
-        if isinstance(item, str):
-            return item
-        if isinstance(item, (tuple, list)) and isinstance(item[0], str):
-            return item[0]
-        if isinstance(item, Particle):
-            return item.name
-        if isinstance(item, dict) and "Name" in item:
-            return str(item["Name"])
-        raise ValueError(
-            f"Cannot extract particle name from {item.__class__.__name__}"
-        )
+def _sort_nested(nested_list: List[List[str]]) -> List[List[str]]:
+    return sorted(sorted(sub_list) for sub_list in nested_list)
+
+
+def ensure_nested_list(
+    nested_list: Union[List[str], List[List[str]]]
+) -> List[List[str]]:
+    if any(not isinstance(item, list) for item in nested_list):
+        nested_list = [nested_list]  # type: ignore[assignment]
+    if any(not isinstance(i, str) for lst in nested_list for i in lst):
+        raise ValueError("Not all grouping items are particle names")
+    return nested_list  # type: ignore[return-value]
 
 
 def _get_kinematic_representation(
-    topology: Topology,
-    initial_facts: Mapping[int, StateWithSpins],
+    topology: Topology, particle_names: Mapping[int, str]
 ) -> _KinematicRepresentation:
     r"""Group final or initial states by node, sorted by length of the group.
 
     The resulting sorted groups can be used to check whether two
     `.StateTransitionGraph` instances are kinematically identical. For
     instance, the following two graphs:
 
@@ -195,190 +169,90 @@
 
         kinematic_representation.final_state == \
             [["gamma", "gamma"], ["gamma", "gamma", "pi0"], \
              ["gamma", "gamma", "pi0", "pi0"]]
         kinematic_representation.initial_state == \
             [["J/psi"], ["J/psi"]]
 
-    and are therefore kinematically identical. The nested lists are sorted (by
-    `list` length and element content) for comparisons.
-
-    Note: more precisely, the states represented here by a `str` only also have
-    a list of allowed spin projections, for instance, :code:`("J/psi", [-1,
-    +1])`. Note that a `tuple` is also sortable.
+    and are therefore kinematically identical. The nested lists are sorted (by `list`
+    length and element content) for comparisons.
     """
 
-    def get_state_groupings(
-        edge_per_node_getter: Callable[[int], Iterable[int]]
-    ) -> List[Iterable[int]]:
-        return [edge_per_node_getter(i) for i in topology.nodes]
+    def get_state_groupings(get_edge: Callable[[int], Set[int]]) -> List[List[int]]:
+        return [sorted(get_edge(i)) for i in topology.nodes]
 
     def fill_groupings(
-        grouping_with_ids: Iterable[Iterable[int]],
-    ) -> List[List[StateWithSpins]]:
+        edge_id_groupings: Iterable[Iterable[int]],
+    ) -> List[List[str]]:
         return [
-            [initial_facts[edge_id] for edge_id in group]
-            for group in grouping_with_ids
+            [particle_names[edge_id] for edge_id in group]
+            for group in edge_id_groupings
         ]
 
     initial_state_edge_groups = fill_groupings(
         get_state_groupings(topology.get_originating_initial_state_edge_ids)
     )
     final_state_edge_groups = fill_groupings(
         get_state_groupings(topology.get_originating_final_state_edge_ids)
     )
     return _KinematicRepresentation(
         initial_state=initial_state_edge_groups,
         final_state=final_state_edge_groups,
     )
 
 
-def create_initial_facts(  # pylint: disable=too-many-locals
-    topology: Topology,
-    particle_db: ParticleCollection,
+def create_initial_facts(
     initial_state: Sequence[StateDefinition],
     final_state: Sequence[StateDefinition],
-    final_state_groupings: Optional[
-        Union[List[List[List[str]]], List[List[str]], List[str]]
-    ] = None,
+    particle_db: ParticleCollection,
 ) -> List[InitialFacts]:
-    def embed_in_list(some_list: List[Any]) -> List[List[Any]]:
-        if not isinstance(some_list[0], list):
-            return [some_list]
-        return some_list
-
-    allowed_kinematic_groupings = None
-    if final_state_groupings is not None:
-        final_state_groupings = embed_in_list(final_state_groupings)
-        final_state_groupings = embed_in_list(final_state_groupings)
-        allowed_kinematic_groupings = [
-            _KinematicRepresentation(final_state=grouping)
-            for grouping in final_state_groupings
-        ]
-
-    kinematic_permutation_graphs = _generate_kinematic_permutations(
-        topology=topology,
-        particle_db=particle_db,
-        initial_state=initial_state,
-        final_state=final_state,
-        allowed_kinematic_groupings=allowed_kinematic_groupings,
+    n_initial_states = len(initial_state)
+    n_final_states = len(final_state)
+    states = __create_states_with_spin_projections(
+        list(range(-n_initial_states, n_final_states)),
+        list(initial_state) + list(final_state),
+        particle_db,
     )
-    edge_initial_facts = []
-    for kinematic_permutation in kinematic_permutation_graphs:
-        spin_permutations = _generate_spin_permutations(
-            kinematic_permutation, particle_db
-        )
-        edge_initial_facts.extend(
-            [InitialFacts(edge_props=x) for x in spin_permutations]
-        )
-    return edge_initial_facts
+    spin_states = __generate_spin_combinations(states, particle_db)
+    return [InitialFacts(state) for state in spin_states]
 
 
-def _generate_kinematic_permutations(
-    topology: Topology,
+def __create_states_with_spin_projections(
+    edge_ids: Sequence[int],
+    state_definitions: Sequence[StateDefinition],
     particle_db: ParticleCollection,
-    initial_state: Sequence[StateDefinition],
-    final_state: Sequence[StateDefinition],
-    allowed_kinematic_groupings: Optional[
-        List[_KinematicRepresentation]
-    ] = None,
-) -> List[Dict[int, StateWithSpins]]:
-    def assert_number_of_states(
-        state_definitions: Sized, edge_ids: Sized
-    ) -> None:
-        if len(state_definitions) != len(edge_ids):
-            raise ValueError(
-                "Number of state definitions is not same as number of edge"
-                f" IDs:(len({state_definitions}) != len({edge_ids})"
-            )
-
-    assert_number_of_states(initial_state, topology.incoming_edge_ids)
-    assert_number_of_states(final_state, topology.outgoing_edge_ids)
-
-    def is_allowed_grouping(
-        kinematic_representation: _KinematicRepresentation,
-    ) -> bool:
-        if allowed_kinematic_groupings is None:
-            return True
-        for allowed_kinematic_grouping in allowed_kinematic_groupings:
-            if allowed_kinematic_grouping in kinematic_representation:
-                return True
-        return False
-
-    initial_state_with_projections = _safe_set_spin_projections(
-        initial_state, particle_db
-    )
-    final_state_with_projections = _safe_set_spin_projections(
-        final_state, particle_db
-    )
-
-    initial_facts_combinations: List[Dict[int, StateWithSpins]] = []
-    kinematic_representations: List[_KinematicRepresentation] = []
-    for permutation in _generate_outer_edge_permutations(
-        topology,
-        initial_state_with_projections,
-        final_state_with_projections,
-    ):
-        kinematic_representation = _get_kinematic_representation(
-            topology, permutation
+) -> Dict[int, StateWithSpins]:
+    if len(edge_ids) != len(state_definitions):
+        raise ValueError(
+            "Number of state definitions is not same as number of edge IDs"
         )
-        if kinematic_representation in kinematic_representations:
-            continue
-        if not is_allowed_grouping(kinematic_representation):
-            continue
-        kinematic_representations.append(kinematic_representation)
-        initial_facts_combinations.append(permutation)
-
-    return initial_facts_combinations
+    states = __safe_set_spin_projections(state_definitions, particle_db)
+    return dict(zip(edge_ids, states))
 
 
-def _safe_set_spin_projections(
-    list_of_states: Sequence[StateDefinition],
+def __safe_set_spin_projections(
+    state_definitions: Sequence[StateDefinition],
     particle_db: ParticleCollection,
 ) -> Sequence[StateWithSpins]:
-    def safe_set_spin_projections(
-        state: StateDefinition, particle_db: ParticleCollection
-    ) -> StateWithSpins:
+    def fill_spin_projections(state: StateDefinition) -> StateWithSpins:
         if isinstance(state, str):
             particle_name = state
-            particle = particle_db[state]
-            spin_projections = list(
-                arange(-particle.spin, particle.spin + 1, 1.0)
-            )
+            particle = particle_db[particle_name]
+            spin_projections = set(arange(-particle.spin, particle.spin + 1, 1.0))
             if particle.mass == 0.0:
                 if 0.0 in spin_projections:
-                    del spin_projections[spin_projections.index(0.0)]
-            state = (particle_name, spin_projections)
+                    spin_projections.remove(0.0)
+            return particle_name, sorted(spin_projections)
         return state
 
-    return [
-        safe_set_spin_projections(state, particle_db)
-        for state in list_of_states
-    ]
+    return [fill_spin_projections(state) for state in state_definitions]
 
 
-def _generate_outer_edge_permutations(
-    topology: Topology,
-    initial_state: Sequence[StateWithSpins],
-    final_state: Sequence[StateWithSpins],
-) -> Generator[Dict[int, StateWithSpins], None, None]:
-    initial_state_ids = list(topology.incoming_edge_ids)
-    final_state_ids = list(topology.outgoing_edge_ids)
-    for initial_state_permutation in permutations(initial_state):
-        for final_state_permutation in permutations(final_state):
-            yield dict(
-                zip(
-                    initial_state_ids + final_state_ids,
-                    initial_state_permutation + final_state_permutation,
-                )
-            )
-
-
-def _generate_spin_permutations(
-    initial_facts: Dict[int, StateWithSpins],
+def __generate_spin_combinations(
+    states_with_spin_projections: Dict[int, StateWithSpins],
     particle_db: ParticleCollection,
 ) -> List[Dict[int, ParticleWithSpin]]:
     def populate_edge_with_spin_projections(
         permutation: Dict[int, ParticleWithSpin],
         edge_id: int,
         state: StateWithSpins,
     ) -> List[Dict[int, ParticleWithSpin]]:
@@ -388,59 +262,127 @@
         for projection in spin_projections:
             temp_permutation = deepcopy(permutation)
             temp_permutation.update({edge_id: (particle, projection)})
             new_permutations.append(temp_permutation)
         return new_permutations
 
     initial_facts_permutations: List[Dict[int, ParticleWithSpin]] = [{}]
-    for edge_id, state in initial_facts.items():
+    for edge_id, state in states_with_spin_projections.items():
         temp_permutations = initial_facts_permutations
         initial_facts_permutations = []
         for temp_permutation in temp_permutations:
             initial_facts_permutations.extend(
-                populate_edge_with_spin_projections(
-                    temp_permutation, edge_id, state
-                )
+                populate_edge_with_spin_projections(temp_permutation, edge_id, state)
             )
 
     return initial_facts_permutations
 
 
-def __get_initial_state_edge_ids(
-    graph: StateTransitionGraph[ParticleWithSpin],
-) -> Iterable[int]:
-    return graph.topology.incoming_edge_ids
+def permutate_topology_kinematically(
+    topology: Topology,
+    initial_state: List[StateDefinition],
+    final_state: List[StateDefinition],
+    final_state_groupings: Optional[
+        Union[List[List[List[str]]], List[List[str]], List[str]]
+    ] = None,
+) -> List[Topology]:
+    def strip_spin(state: StateDefinition) -> str:
+        if isinstance(state, tuple):
+            return state[0]
+        return state
 
+    edge_ids = sorted(topology.incoming_edge_ids) + sorted(topology.outgoing_edge_ids)
+    states = initial_state + final_state
+    return _generate_kinematic_permutations(
+        topology,
+        particle_names={i: strip_spin(s) for i, s in zip(edge_ids, states)},
+        allowed_kinematic_groupings=__get_kinematic_groupings(final_state_groupings),
+    )
 
-def __get_final_state_edge_ids(
-    graph: StateTransitionGraph[ParticleWithSpin],
-) -> Iterable[int]:
-    return graph.topology.outgoing_edge_ids
+
+def _generate_kinematic_permutations(
+    topology: Topology,
+    particle_names: Dict[int, str],
+    allowed_kinematic_groupings: Optional[List[_KinematicRepresentation]] = None,
+) -> List[Topology]:
+    def is_allowed_grouping(kinematic_representation: _KinematicRepresentation) -> bool:
+        if allowed_kinematic_groupings is None:
+            return True
+        for allowed_kinematic_grouping in allowed_kinematic_groupings:
+            if allowed_kinematic_grouping in kinematic_representation:
+                return True
+        return False
+
+    permuted_topologies: List[Topology] = []
+    kinematic_representations: List[_KinematicRepresentation] = []
+    for permutation in _permutate_outer_edges(topology):
+        kinematic_representation = _get_kinematic_representation(
+            permutation, particle_names
+        )
+        if kinematic_representation in kinematic_representations:
+            continue
+        if not is_allowed_grouping(kinematic_representation):
+            continue
+        kinematic_representations.append(kinematic_representation)
+        permuted_topologies.append(permutation)
+    return permuted_topologies
+
+
+def _permutate_outer_edges(topology: Topology) -> List[Topology]:
+    initial_state_ids = sorted(topology.incoming_edge_ids)
+    final_state_ids = sorted(topology.outgoing_edge_ids)
+    topologies = set()
+    for initial_state_permutation in itertools.permutations(initial_state_ids):
+        for final_state_permutation in itertools.permutations(final_state_ids):
+            permutation = zip(
+                initial_state_ids + final_state_ids,
+                initial_state_permutation + final_state_permutation,
+            )
+            new_topology = topology.relabel_edges(dict(permutation))
+            topologies.add(new_topology)
+    return sorted(topologies)
+
+
+def __get_kinematic_groupings(
+    final_state_groupings: Union[
+        List[List[List[str]]],
+        List[List[str]],
+        List[str],
+        None,
+    ]
+) -> Optional[List[_KinematicRepresentation]]:
+    if final_state_groupings is None:
+        return None
+
+    def embed_in_list(some_list: List[Any]) -> List[List[Any]]:
+        if not isinstance(some_list[0], list):
+            return [some_list]
+        return some_list
+
+    final_state_groupings = embed_in_list(final_state_groupings)
+    final_state_groupings = embed_in_list(final_state_groupings)
+    return [_KinematicRepresentation(grouping) for grouping in final_state_groupings]
 
 
 def match_external_edges(
     graphs: List[StateTransitionGraph[ParticleWithSpin]],
 ) -> None:
     if not isinstance(graphs, list):
         raise TypeError("graphs argument is not of type list")
     if not graphs:
         return
     ref_graph_id = 0
     _match_external_edge_ids(graphs, ref_graph_id, __get_final_state_edge_ids)
-    _match_external_edge_ids(
-        graphs, ref_graph_id, __get_initial_state_edge_ids
-    )
+    _match_external_edge_ids(graphs, ref_graph_id, __get_initial_state_edge_ids)
 
 
 def _match_external_edge_ids(  # pylint: disable=too-many-locals
     graphs: List[StateTransitionGraph[ParticleWithSpin]],
     ref_graph_id: int,
-    external_edge_getter_function: Callable[
-        [StateTransitionGraph], Iterable[int]
-    ],
+    external_edge_getter_function: Callable[[StateTransitionGraph], Iterable[int]],
 ) -> None:
     ref_graph = graphs[ref_graph_id]
     # create external edge to particle mapping
     ref_edge_id_particle_mapping = _create_edge_id_particle_mapping(
         ref_graph, external_edge_getter_function(ref_graph)
     )
 
@@ -458,30 +400,40 @@
                 for key_2, value_2 in ref_mapping_copy.items():
                     if value == value_2:
                         edge_ids_mapping[key] = key_2
                         del ref_mapping_copy[key_2]
                         break
         if len(ref_mapping_copy) != 0:
             raise ValueError(
-                "Unable to match graphs, due to inherent graph"
-                " structure mismatch"
+                "Unable to match graphs, due to inherent graph structure mismatch"
             )
         swappings = _calculate_swappings(edge_ids_mapping)
         for edge_id1, edge_id2 in swappings.items():
             graph.swap_edges(edge_id1, edge_id2)
 
 
+def __get_initial_state_edge_ids(
+    graph: StateTransitionGraph[ParticleWithSpin],
+) -> Iterable[int]:
+    return graph.topology.incoming_edge_ids
+
+
+def __get_final_state_edge_ids(
+    graph: StateTransitionGraph[ParticleWithSpin],
+) -> Iterable[int]:
+    return graph.topology.outgoing_edge_ids
+
+
 def perform_external_edge_identical_particle_combinatorics(
     graph: StateTransitionGraph,
 ) -> List[StateTransitionGraph]:
     """Create combinatorics clones of the `.StateTransitionGraph`.
 
-    In case of identical particles in the initial or final state. Only
-    identical particles, which do not enter or exit the same node allow for
-    combinatorics!
+    In case of identical particles in the initial or final state. Only identical
+    particles, which do not enter or exit the same node allow for combinatorics!
     """
     if not isinstance(graph, StateTransitionGraph):
         raise TypeError(
             f"graph argument is not of type {StateTransitionGraph.__class__}"
         )
     temp_new_graphs = _external_edge_identical_particle_combinatorics(
         graph, __get_final_state_edge_ids
@@ -494,36 +446,32 @@
             )
         )
     return new_graphs
 
 
 def _external_edge_identical_particle_combinatorics(
     graph: StateTransitionGraph[ParticleWithSpin],
-    external_edge_getter_function: Callable[
-        [StateTransitionGraph], Iterable[int]
-    ],
+    external_edge_getter_function: Callable[[StateTransitionGraph], Iterable[int]],
 ) -> List[StateTransitionGraph]:
     # pylint: disable=too-many-locals
     new_graphs = [graph]
     edge_particle_mapping = _create_edge_id_particle_mapping(
         graph, external_edge_getter_function(graph)
     )
     identical_particle_groups: Dict[str, Set[int]] = {}
     for key, value in edge_particle_mapping.items():
         if value not in identical_particle_groups:
             identical_particle_groups[value] = set()
         identical_particle_groups[value].add(key)
     identical_particle_groups = {
-        key: value
-        for key, value in identical_particle_groups.items()
-        if len(value) > 1
+        key: value for key, value in identical_particle_groups.items() if len(value) > 1
     }
     # now for each identical particle group perform all permutations
     for edge_group in identical_particle_groups.values():
-        combinations = permutations(edge_group)
+        combinations = itertools.permutations(edge_group)
         graph_combinations = set()
         ext_edge_combinations = []
         ref_node_origin = get_originating_node_list(graph.topology, edge_group)
         for comb in combinations:
             temp_edge_node_mapping = tuple(sorted(zip(comb, ref_node_origin)))
             if temp_edge_node_mapping not in graph_combinations:
                 graph_combinations.add(temp_edge_node_mapping)
@@ -556,11 +504,9 @@
     return swappings
 
 
 def _create_edge_id_particle_mapping(
     graph: StateTransitionGraph[ParticleWithSpin], edge_ids: Iterable[int]
 ) -> Dict[int, str]:
     return {
-        i: graph.get_edge_props(i)[0].name
-        for i in edge_ids
-        if graph.get_edge_props(i)
+        i: graph.get_edge_props(i)[0].name for i in edge_ids if graph.get_edge_props(i)
     }
```

### Comparing `qrules-0.9.7/src/qrules/conservation_rules.py` & `qrules-0.9.8/src/qrules/conservation_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Collection of quantum number conservation rules for particle reactions.
 
-This module is the place where the 'expert' defines the rules that verify
-quantum numbers of the reaction.
+This module is the place where the 'expert' defines the rules that verify quantum
+numbers of the reaction.
 
-A rule is a function that takes quantum numbers as input and outputs a boolean.
-There are three different types of rules:
+A rule is a function that takes quantum numbers as input and outputs a boolean. There
+are three different types of rules:
 
 1. `GraphElementRule` that work on individual graph edges or nodes.
-2. `EdgeQNConservationRule` that work on the interaction level, which use
-   ingoing edges, outgoing edges as arguments.  E.g.: `.ChargeConservation`.
-3. `ConservationRule` that work on the interaction level, which use ingoing
-   edges, outgoing edges and a interaction node as arguments. E.g:
-   `.parity_conservation`.
-
-The arguments can be any type of quantum number. However a rule argument
-resembling edges only accepts `~.quantum_numbers.EdgeQuantumNumbers`. Similarly
-arguments that resemble a node only accept
-`~.quantum_numbers.NodeQuantumNumbers`. The argument types do not have to be
-limited to a single quantum number, but can be a composite (see
+2. `EdgeQNConservationRule` that work on the interaction level, which use ingoing edges,
+   outgoing edges as arguments.  E.g.: `.ChargeConservation`.
+3. `ConservationRule` that work on the interaction level, which use ingoing edges,
+   outgoing edges and a interaction node as arguments. E.g: `.parity_conservation`.
+
+The arguments can be any type of quantum number. However a rule argument resembling
+edges only accepts `~.quantum_numbers.EdgeQuantumNumbers`. Similarly arguments that
+resemble a node only accept `~.quantum_numbers.NodeQuantumNumbers`. The argument types
+do not have to be limited to a single quantum number, but can be a composite (see
 `.CParityEdgeInput`).
 
 .. warning::
     Besides the rule logic itself, a rule also has the responsibility of
     stating its run conditions. These run conditions **must** be stated by
     the type annotations of its :code:`__call__` method. The type annotations
     therefore are not just there for *static* type checking: they also
@@ -29,32 +27,32 @@
     by the :mod:`.solving` module.
 
 Generally, the conditions can be separated into two categories:
 
 * variable conditions
 * toplogical conditions
 
-Currently, only variable conditions are being used. Topological conditions
-could be created in the form of `~typing.Tuple` instead of `~typing.List`.
+Currently, only variable conditions are being used. Topological conditions could be
+created in the form of `~typing.Tuple` instead of `~typing.List`.
 
-For additive quantum numbers, the decorator `additive_quantum_number_rule`
-can be used to automatically generate the appropriate behavior.
+For additive quantum numbers, the decorator `additive_quantum_number_rule` can be used
+to automatically generate the appropriate behavior.
 
 
-The module is therefore strongly typed (both
-for the reader of the code and for type checking with :doc:`mypy
-<mypy:index>`). An example is `.HelicityParityEdgeInput`, which has been
-defined to provide type checks on `.parity_conservation_helicity`.
+The module is therefore strongly typed (both for the reader of the code and for type
+checking with :doc:`mypy <mypy:index>`). An example is `.HelicityParityEdgeInput`, which
+has been defined to provide type checks on `.parity_conservation_helicity`.
 
 .. seealso:: :doc:`/usage/conservation`
 """
 
 import sys
 from copy import deepcopy
 from functools import reduce
+from textwrap import dedent
 from typing import Any, Callable, List, Optional, Set, Tuple, Type, Union
 
 from attrs import define, field, frozen
 from attrs.converters import optional
 
 from .quantum_numbers import EdgeQuantumNumbers as EdgeQN
 from .quantum_numbers import NodeQuantumNumbers as NodeQN
@@ -102,39 +100,39 @@
 # __call__ method in a concrete version of the generic are still containing the
 # TypeVar types. See https://github.com/python/typing/issues/762
 def additive_quantum_number_rule(
     quantum_number: type,
 ) -> Callable[[Any], EdgeQNConservationRule]:
     r"""Class decorator for creating an additive conservation rule.
 
-    Use this decorator to create a `EdgeQNConservationRule` for a quantum number
-    to which an additive conservation rule applies:
+    Use this decorator to create a `EdgeQNConservationRule` for a quantum number to
+    which an additive conservation rule applies:
 
     .. math:: \sum q_{in} = \sum q_{out}
 
     Args:
         quantum_number: Quantum number to which you want to apply the additive
-            conservation check. An example would be
-            `.EdgeQuantumNumbers.charge`.
+            conservation check. An example would be `.EdgeQuantumNumbers.charge`.
     """
 
     def decorator(rule_class: Any) -> EdgeQNConservationRule:
         def new_call(
             # pylint: disable=unused-argument
             self: Type[EdgeQNConservationRule],
             ingoing_edge_qns: List[quantum_number],  # type: ignore[valid-type]
             outgoing_edge_qns: List[quantum_number],  # type: ignore[valid-type]
         ) -> bool:
             return sum(ingoing_edge_qns) == sum(outgoing_edge_qns)
 
         rule_class.__call__ = new_call
-        rule_class.__doc__ = (
-            f"""Decorated via `{additive_quantum_number_rule.__name__}`.\n\n"""
-            f"""Check for `~.EdgeQuantumNumbers.{quantum_number.__name__}` conservation."""
-        )
+        rule_class.__doc__ = dedent(f"""
+            Decorated via `{additive_quantum_number_rule.__name__}`.
+
+            Check for `~.EdgeQuantumNumbers.{quantum_number.__name__}` conservation.
+            """)
         return rule_class
 
     return decorator
 
 
 @additive_quantum_number_rule(EdgeQN.charge)
 class ChargeConservation(EdgeQNConservationRule):
@@ -178,30 +176,28 @@
 
 def parity_conservation(
     ingoing_edge_qns: List[EdgeQN.parity],
     outgoing_edge_qns: List[EdgeQN.parity],
     l_magnitude: NodeQN.l_magnitude,
 ) -> bool:
     r"""Implement :math:`P_{in} = P_{out} \cdot (-1)^L`."""
+    if any(p is None for p in [*ingoing_edge_qns, *outgoing_edge_qns]):
+        return False
     if len(ingoing_edge_qns) == 1 and len(outgoing_edge_qns) == 2:
         parity_in = reduce(lambda x, y: x * y.value, ingoing_edge_qns, 1)
         parity_out = reduce(lambda x, y: x * y.value, outgoing_edge_qns, 1)
         return parity_in == (parity_out * (-1) ** l_magnitude)
     return True
 
 
 @frozen
 class HelicityParityEdgeInput:
     parity: EdgeQN.parity = field(converter=EdgeQN.parity)
-    spin_magnitude: EdgeQN.spin_magnitude = field(
-        converter=EdgeQN.spin_magnitude
-    )
-    spin_projection: EdgeQN.spin_projection = field(
-        converter=EdgeQN.spin_projection
-    )
+    spin_magnitude: EdgeQN.spin_magnitude = field(converter=EdgeQN.spin_magnitude)
+    spin_projection: EdgeQN.spin_projection = field(converter=EdgeQN.spin_projection)
 
 
 def parity_conservation_helicity(
     ingoing_edge_qns: List[HelicityParityEdgeInput],
     outgoing_edge_qns: List[HelicityParityEdgeInput],
     parity_prefactor: NodeQN.parity_prefactor,
 ) -> bool:
@@ -210,48 +206,41 @@
     Check the following:
 
     .. math:: A_{-\lambda_1-\lambda_2} = P_1 P_2 P_3 (-1)^{S_2+S_3-S_1}
         A_{\lambda_1\lambda_2}
 
     .. math:: \mathrm{parity\,prefactor} = P_1 P_2 P_3 (-1)^{S_2+S_3-S_1}
 
-    .. note:: Only the special case :math:`\lambda_1=\lambda_2=0` may
-      return False independent on the parity prefactor.
+    .. note:: Only the special case :math:`\lambda_1=\lambda_2=0` may return `False`
+        independent on the parity prefactor.
     """
     if len(ingoing_edge_qns) == 1 and len(outgoing_edge_qns) == 2:
         out_spins = [x.spin_magnitude for x in outgoing_edge_qns]
         parity_product = reduce(
             lambda x, y: x * y.parity.value if y.parity else x,
             ingoing_edge_qns + outgoing_edge_qns,
             1,
         )
 
         prefactor = parity_product * (-1.0) ** (
             sum(out_spins) - ingoing_edge_qns[0].spin_magnitude
         )
 
-        if (
-            all(x.spin_projection == 0.0 for x in outgoing_edge_qns)
-            and prefactor == -1
-        ):
+        if all(x.spin_projection == 0.0 for x in outgoing_edge_qns) and prefactor == -1:
             return False
 
         return prefactor == parity_prefactor
     return True
 
 
 @frozen
 class CParityEdgeInput:
-    spin_magnitude: EdgeQN.spin_magnitude = field(
-        converter=EdgeQN.spin_magnitude
-    )
+    spin_magnitude: EdgeQN.spin_magnitude = field(converter=EdgeQN.spin_magnitude)
     pid: EdgeQN.pid = field(converter=EdgeQN.pid)
-    c_parity: Optional[EdgeQN.c_parity] = field(
-        converter=EdgeQN.c_parity, default=None
-    )
+    c_parity: Optional[EdgeQN.c_parity] = field(converter=EdgeQN.c_parity, default=None)
 
 
 @frozen
 class CParityNodeInput:
     l_magnitude: NodeQN.l_magnitude = field(converter=NodeQN.l_magnitude)
     s_magnitude: NodeQN.s_magnitude = field(converter=NodeQN.s_magnitude)
 
@@ -272,53 +261,43 @@
         c_parities_part = [x.c_parity.value for x in part_qns if x.c_parity]
         # if all states have C parity defined, then just multiply them
         if len(c_parities_part) == len(part_qns):
             return reduce(lambda x, y: x * y, c_parities_part, 1)
 
         # two particle case
         if len(part_qns) == 2:
-            if _is_particle_antiparticle_pair(
-                part_qns[0].pid, part_qns[1].pid
-            ):
+            if _is_particle_antiparticle_pair(part_qns[0].pid, part_qns[1].pid):
                 ang_mom = interaction_qns.l_magnitude
                 # if boson
                 if _is_boson(part_qns[0].spin_magnitude):
                     return (-1) ** int(ang_mom)
                 coupled_spin = interaction_qns.s_magnitude
                 if isinstance(coupled_spin, int) or coupled_spin.is_integer():
                     return (-1) ** int(ang_mom + coupled_spin)
         return None
 
-    c_parity_in = _get_c_parity_multiparticle(
-        ingoing_edge_qns, interaction_node_qns
-    )
+    c_parity_in = _get_c_parity_multiparticle(ingoing_edge_qns, interaction_node_qns)
     if c_parity_in is None:
         return True
 
-    c_parity_out = _get_c_parity_multiparticle(
-        outgoing_edge_qns, interaction_node_qns
-    )
+    c_parity_out = _get_c_parity_multiparticle(outgoing_edge_qns, interaction_node_qns)
     if c_parity_out is None:
         return True
 
     return c_parity_in == c_parity_out
 
 
 @frozen
 class GParityEdgeInput:
     isospin_magnitude: EdgeQN.isospin_magnitude = field(
         converter=EdgeQN.isospin_magnitude
     )
-    spin_magnitude: EdgeQN.spin_magnitude = field(
-        converter=EdgeQN.spin_magnitude
-    )
+    spin_magnitude: EdgeQN.spin_magnitude = field(converter=EdgeQN.spin_magnitude)
     pid: EdgeQN.pid = field(converter=EdgeQN.pid)
-    g_parity: Optional[EdgeQN.g_parity] = field(
-        converter=EdgeQN.g_parity, default=None
-    )
+    g_parity: Optional[EdgeQN.g_parity] = field(converter=EdgeQN.g_parity, default=None)
 
 
 @frozen
 class GParityNodeInput:
     l_magnitude: NodeQN.l_magnitude = field(converter=NodeQN.l_magnitude)
     s_magnitude: NodeQN.s_magnitude = field(converter=NodeQN.s_magnitude)
 
@@ -355,29 +334,23 @@
         couple_state: Tuple[GParityEdgeInput, GParityEdgeInput],
     ) -> bool:
         couple_state_g_parity = check_multistate_g_parity(
             single_state.isospin_magnitude,
             (couple_state[0], couple_state[1]),
         )
         single_state_g_parity = (
-            ingoing_edge_qns[0].g_parity.value
-            if ingoing_edge_qns[0].g_parity
-            else None
+            ingoing_edge_qns[0].g_parity.value if ingoing_edge_qns[0].g_parity else None
         )
 
         if not couple_state_g_parity or not single_state_g_parity:
             return True
         return couple_state_g_parity == single_state_g_parity
 
-    no_g_parity_in_part = [
-        True for x in ingoing_edge_qns if x.g_parity is None
-    ]
-    no_g_parity_out_part = [
-        True for x in outgoing_edge_qns if x.g_parity is None
-    ]
+    no_g_parity_in_part = [True for x in ingoing_edge_qns if x.g_parity is None]
+    no_g_parity_out_part = [True for x in outgoing_edge_qns if x.g_parity is None]
     # if all states have G parity defined, then just multiply them
     if not any(no_g_parity_in_part + no_g_parity_out_part):
         in_g_parity = reduce(
             lambda x, y: x * y.g_parity.value if y.g_parity else x,
             ingoing_edge_qns,
             1,
         )
@@ -402,39 +375,34 @@
             (ingoing_edge_qns[0], ingoing_edge_qns[1]),
         )
     return True
 
 
 @frozen
 class IdenticalParticleSymmetryOutEdgeInput:
-    spin_magnitude: EdgeQN.spin_magnitude = field(
-        converter=EdgeQN.spin_magnitude
-    )
-    spin_projection: EdgeQN.spin_projection = field(
-        converter=EdgeQN.spin_projection
-    )
+    spin_magnitude: EdgeQN.spin_magnitude = field(converter=EdgeQN.spin_magnitude)
+    spin_projection: EdgeQN.spin_projection = field(converter=EdgeQN.spin_projection)
     pid: EdgeQN.pid = field(converter=EdgeQN.pid)
 
 
 def identical_particle_symmetrization(
     ingoing_parities: List[EdgeQN.parity],
     outgoing_edge_qns: List[IdenticalParticleSymmetryOutEdgeInput],
 ) -> bool:
     """Verifies multi particle state symmetrization for identical particles.
 
-    In case of a multi particle state with identical particles, their exchange
-    symmetry has to follow the spin statistic theorem.
+    In case of a multi particle state with identical particles, their exchange symmetry
+    has to follow the spin statistic theorem.
+
+    For bosonic systems the total exchange symmetry (parity) has to be even (+1). For
+    fermionic systems the total exchange symmetry (parity) has to be odd (-1).
 
-    For bosonic systems the total exchange symmetry (parity) has to be even
-    (+1). For fermionic systems the total exchange symmetry (parity) has to be
-    odd (-1).
-
-    In case of a particle decaying into N identical particles (N>1), the
-    decaying particle has to have the same parity as required by the spin
-    statistic theorem of the multi body state.
+    In case of a particle decaying into N identical particles (N>1), the decaying
+    particle has to have the same parity as required by the spin statistic theorem of
+    the multi body state.
     """
 
     def _check_particles_identical(
         particles: List[IdenticalParticleSymmetryOutEdgeInput],
     ) -> bool:
         """Check if pids and spins match."""
         if len(particles) == 1:
@@ -519,25 +487,20 @@
 def _check_magnitude(
     in_part: List[float],
     out_part: List[float],
     interaction_qns: Optional[Union[SpinMagnitudeNodeInput, SpinNodeInput]],
 ) -> bool:
     def couple_mags(j_1: float, j_2: float) -> List[float]:
         return [
-            x / 2.0
-            for x in range(
-                int(2 * abs(j_1 - j_2)), int(2 * (j_1 + j_2 + 1)), 2
-            )
+            x / 2.0 for x in range(int(2 * abs(j_1 - j_2)), int(2 * (j_1 + j_2 + 1)), 2)
         ]
 
     def couple_magnitudes(
         magnitudes: List[float],
-        interaction_qns: Optional[
-            Union[SpinMagnitudeNodeInput, SpinNodeInput]
-        ],
+        interaction_qns: Optional[Union[SpinMagnitudeNodeInput, SpinNodeInput]],
     ) -> Set[float]:
         if len(magnitudes) == 1:
             return set(magnitudes)
 
         coupled_magnitudes = {magnitudes[0]}
         for mag in magnitudes[1:]:
             temp_set = coupled_magnitudes
@@ -583,23 +546,19 @@
     interaction_qns: Optional[SpinNodeInput] = None,
 ) -> Set[_Spin]:
     total_spins = set()
     if len(spins) == 1:
         return set(spins)
     total_spins = __create_coupled_spins(spins)
     if interaction_qns:
-        coupled_spin = _Spin(
-            interaction_qns.s_magnitude, interaction_qns.s_projection
-        )
+        coupled_spin = _Spin(interaction_qns.s_magnitude, interaction_qns.s_projection)
         if coupled_spin in total_spins:
             return __spin_couplings(
                 coupled_spin,
-                _Spin(
-                    interaction_qns.l_magnitude, interaction_qns.l_projection
-                ),
+                _Spin(interaction_qns.l_magnitude, interaction_qns.l_projection),
             )
         total_spins = set()
 
     return total_spins
 
 
 def __create_coupled_spins(spins: List[_Spin]) -> Set[_Spin]:
@@ -629,17 +588,15 @@
     s_2 = spin2.magnitude
 
     sum_proj = spin1.projection + spin2.projection
     return {
         _Spin(x, sum_proj)
         for x in arange(abs(s_1 - s_2), s_1 + s_2 + 1, 1.0)
         if x >= abs(sum_proj)
-        and not _is_clebsch_gordan_coefficient_zero(
-            spin1, spin2, _Spin(x, sum_proj)
-        )
+        and not _is_clebsch_gordan_coefficient_zero(spin1, spin2, _Spin(x, sum_proj))
     }
 
 
 @define
 class IsoSpinEdgeInput:
     isospin_magnitude: EdgeQN.isospin_magnitude = field(
         converter=EdgeQN.isospin_magnitude
@@ -671,53 +628,39 @@
     r"""Check for isospin conservation.
 
     Implements
 
     .. math::
         |I_1 - I_2| \leq I \leq |I_1 + I_2|
 
-    Also checks :math:`I_{1,z} + I_{2,z} = I_z` and if Clebsch-Gordan
-    coefficients are all 0.
+    Also checks :math:`I_{1,z} + I_{2,z} = I_z` and if Clebsch-Gordan coefficients are
+    all 0.
     """
     if not sum(x.isospin_projection for x in ingoing_isospins) == sum(
         x.isospin_projection for x in outgoing_isospins
     ):
         return False
-    if not all(
-        isospin_validity(x) for x in ingoing_isospins + outgoing_isospins
-    ):
+    if not all(isospin_validity(x) for x in ingoing_isospins + outgoing_isospins):
         return False
     return _check_spin_couplings(
-        [
-            _Spin(x.isospin_magnitude, x.isospin_projection)
-            for x in ingoing_isospins
-        ],
-        [
-            _Spin(x.isospin_magnitude, x.isospin_projection)
-            for x in outgoing_isospins
-        ],
+        [_Spin(x.isospin_magnitude, x.isospin_projection) for x in ingoing_isospins],
+        [_Spin(x.isospin_magnitude, x.isospin_projection) for x in outgoing_isospins],
         None,
     )
 
 
 @define
 class SpinEdgeInput:
-    spin_magnitude: EdgeQN.spin_magnitude = field(
-        converter=EdgeQN.spin_magnitude
-    )
-    spin_projection: EdgeQN.spin_projection = field(
-        converter=EdgeQN.spin_projection
-    )
+    spin_magnitude: EdgeQN.spin_magnitude = field(converter=EdgeQN.spin_magnitude)
+    spin_projection: EdgeQN.spin_projection = field(converter=EdgeQN.spin_projection)
 
 
 def spin_validity(spin: SpinEdgeInput) -> bool:
     r"""Check for valid spin magnitude and projection."""
-    return _check_spin_valid(
-        float(spin.spin_magnitude), float(spin.spin_projection)
-    )
+    return _check_spin_valid(float(spin.spin_magnitude), float(spin.spin_projection))
 
 
 def spin_conservation(
     ingoing_spins: List[SpinEdgeInput],
     outgoing_spins: List[SpinEdgeInput],
     interaction_qns: SpinNodeInput,
 ) -> bool:
@@ -729,43 +672,36 @@
         |S_1 - S_2| \leq S \leq |S_1 + S_2|
 
     and
 
     .. math::
         |L - S| \leq J \leq |L + S|
 
-    Also checks :math:`M_1 + M_2 = M` and if Clebsch-Gordan coefficients
-    are all 0.
+    Also checks :math:`M_1 + M_2 = M` and if Clebsch-Gordan coefficients are all 0.
 
     .. seealso:: /docs/usage/ls-coupling
     """
     # L and S can only be used if one side is a single state
     # and the other side contains of two states (isobar)
     # So do a full check if this is the case
     if (len(ingoing_spins) == 1 and len(outgoing_spins) == 2) or (
         len(ingoing_spins) == 2 and len(outgoing_spins) == 1
     ):
-
         return _check_spin_couplings(
-            [
-                _Spin(x.spin_magnitude, x.spin_projection)
-                for x in ingoing_spins
-            ],
-            [
-                _Spin(x.spin_magnitude, x.spin_projection)
-                for x in outgoing_spins
-            ],
+            [_Spin(x.spin_magnitude, x.spin_projection) for x in ingoing_spins],
+            [_Spin(x.spin_magnitude, x.spin_projection) for x in outgoing_spins],
             interaction_qns,
         )
 
     # otherwise don't use S and L and just check magnitude
     # are integral or non integral on both sides
+    # pylint: disable=line-too-long
     return (
-        sum(float(x.spin_magnitude) for x in ingoing_spins).is_integer()
-        == sum(float(x.spin_magnitude) for x in outgoing_spins).is_integer()
+        sum(float(x.spin_magnitude) for x in ingoing_spins).is_integer()  # type: ignore[union-attr]
+        == sum(float(x.spin_magnitude) for x in outgoing_spins).is_integer()  # type: ignore[union-attr]
     )
 
 
 def spin_magnitude_conservation(
     ingoing_spins: List[SpinEdgeInput],
     outgoing_spins: List[SpinEdgeInput],
     interaction_qns: SpinMagnitudeNodeInput,
@@ -792,33 +728,34 @@
             [x.spin_magnitude for x in ingoing_spins],
             [x.spin_magnitude for x in outgoing_spins],
             interaction_qns,
         )
 
     # otherwise don't use S and L and just check magnitude
     # are integral or non integral on both sides
+    # pylint: disable=line-too-long
     return (
-        sum(float(x.spin_magnitude) for x in ingoing_spins).is_integer()
-        == sum(float(x.spin_magnitude) for x in outgoing_spins).is_integer()
+        sum(float(x.spin_magnitude) for x in ingoing_spins).is_integer()  # type: ignore[union-attr]
+        == sum(float(x.spin_magnitude) for x in outgoing_spins).is_integer()  # type: ignore[union-attr]
     )
 
 
 def clebsch_gordan_helicity_to_canonical(
     ingoing_spins: List[SpinEdgeInput],
     outgoing_spins: List[SpinEdgeInput],
     interaction_qns: SpinNodeInput,
 ) -> bool:
     """Implement Clebsch-Gordan checks.
 
-    For :math:`S_1, S_2` to :math:`S` and the :math:`L,S` to :math:`J`
-    coupling based on the conversion of helicity to canonical amplitude sums.
+    For :math:`S_1, S_2` to :math:`S` and the :math:`L,S` to :math:`J` coupling based on
+    the conversion of helicity to canonical amplitude sums.
 
-    .. note:: This rule does not check that the spin magnitudes couple
-      correctly to :math:`L` and :math:`S`, as this is already performed by
-      `.spin_magnitude_conservation`.
+    .. note:: This rule does not check that the spin magnitudes couple correctly to
+        :math:`L` and :math:`S`, as this is already performed by
+        `.spin_magnitude_conservation`.
     """
     if len(ingoing_spins) == 1 and len(outgoing_spins) == 2:
         out_spin1 = _Spin(
             outgoing_spins[0].spin_magnitude,
             outgoing_spins[0].spin_projection,
         )
         out_spin2 = _Spin(
@@ -826,39 +763,29 @@
             -outgoing_spins[1].spin_projection,
         )
 
         helicity_diff = out_spin1.projection + out_spin2.projection
         if helicity_diff != interaction_qns.s_projection:
             return False
 
-        ang_mom = _Spin(
-            interaction_qns.l_magnitude, interaction_qns.l_projection
-        )
-        coupled_spin = _Spin(
-            interaction_qns.s_magnitude, interaction_qns.s_projection
-        )
+        ang_mom = _Spin(interaction_qns.l_magnitude, interaction_qns.l_projection)
+        coupled_spin = _Spin(interaction_qns.s_magnitude, interaction_qns.s_projection)
         parent_spin = ingoing_spins[0].spin_magnitude
 
         coupled_spin = _Spin(coupled_spin.magnitude, helicity_diff)
-        if not _check_spin_valid(
-            coupled_spin.magnitude, coupled_spin.projection
-        ):
+        if not _check_spin_valid(coupled_spin.magnitude, coupled_spin.projection):
             return False
         in_spin = _Spin(parent_spin, helicity_diff)
         if not _check_spin_valid(in_spin.magnitude, in_spin.projection):
             return False
 
-        if _is_clebsch_gordan_coefficient_zero(
-            out_spin1, out_spin2, coupled_spin
-        ):
+        if _is_clebsch_gordan_coefficient_zero(out_spin1, out_spin2, coupled_spin):
             return False
 
-        return not _is_clebsch_gordan_coefficient_zero(
-            ang_mom, coupled_spin, in_spin
-        )
+        return not _is_clebsch_gordan_coefficient_zero(ang_mom, coupled_spin, in_spin)
     return False
 
 
 def helicity_conservation(
     ingoing_spin_mags: List[EdgeQN.spin_magnitude],
     outgoing_helicities: List[EdgeQN.spin_projection],
 ) -> bool:
@@ -945,17 +872,15 @@
         or edge_qns.muon_lepton_number
         or edge_qns.tau_lepton_number
     ):
         return True
     isospin_3 = 0.0
     if edge_qns.isospin_projection:
         isospin_3 = edge_qns.isospin_projection
-    if float(edge_qns.charge) != (
-        isospin_3 + 0.5 * calculate_hypercharge(edge_qns)
-    ):
+    if float(edge_qns.charge) != (isospin_3 + 0.5 * calculate_hypercharge(edge_qns)):
         return False
     return True
 
 
 @frozen
 class MassEdgeInput:
     mass: EdgeQN.mass = field(converter=EdgeQN.mass)
@@ -973,17 +898,17 @@
         ingoing_edge_qns: List[MassEdgeInput],
         outgoing_edge_qns: List[MassEdgeInput],
     ) -> bool:
         r"""Implements mass conservation.
 
         :math:`M_{out} - N \cdot W_{out} < M_{in} + N \cdot W_{in}`
 
-        It makes sure that the net mass outgoing state :math:`M_{out}` is
-        smaller than the net mass of the ingoing state :math:`M_{in}`. Also the
-        width :math:`W` of the states is taken into account.
+        It makes sure that the net mass outgoing state :math:`M_{out}` is smaller than
+        the net mass of the ingoing state :math:`M_{in}`. Also the width :math:`W` of
+        the states is taken into account.
         """
         mass_in = sum(x.mass for x in ingoing_edge_qns)
         width_in = sum(x.width for x in ingoing_edge_qns if x.width)
         mass_out = sum(x.mass for x in outgoing_edge_qns)
         width_out = sum(x.width for x in outgoing_edge_qns if x.width)
 
         return (mass_out - self.__width_factor * width_out) < (
```

### Comparing `qrules-0.9.7/src/qrules/io/__init__.py` & `qrules-0.9.8/src/qrules/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=too-many-return-statements
 """Serialization module for the `qrules`.
 
-The `.io` module provides tools to export or import objects from `qrules` to
-and from disk, so that they can be used by external packages, or just to store
-(cache) the state of the system.
+The `.io` module provides tools to export or import objects from `qrules` to and from
+disk, so that they can be used by external packages, or just to store (cache) the state
+of the system.
 """
 
 import json
 from collections import abc
 from pathlib import Path
 from typing import Any, Dict, Optional
 
@@ -44,16 +44,15 @@
             value_serializer=_dict._value_serializer,
         )
     if isinstance(instance, StateTransitionGraph):
         return _dict.from_stg(instance)
     if isinstance(instance, Topology):
         return _dict.from_topology(instance)
     raise NotImplementedError(
-        "No conversion for dict available for class"
-        f" {instance.__class__.__name__}"
+        f"No conversion for dict available for class {instance.__class__.__name__}"
     )
 
 
 def fromdict(definition: dict) -> object:
     keys = set(definition.keys())
     if __REQUIRED_PARTICLE_FIELDS <= keys:
         return _dict.build_particle(definition)
@@ -68,21 +67,20 @@
     if keys == {"topology", "edge_props", "node_props"}:
         return _dict.build_stg(definition)
     if keys == __REQUIRED_TOPOLOGY_FIELDS:
         return _dict.build_topology(definition)
     raise NotImplementedError(f"Could not determine type from keys {keys}")
 
 
+# pylint: disable=line-too-long
 __REQUIRED_PARTICLE_FIELDS = {
-    field.name
-    for field in attrs.fields(Particle)
-    if field.default == attrs.NOTHING
+    field.name for field in attrs.fields(Particle) if field.default == attrs.NOTHING  # type: ignore[arg-type]
 }
 __REQUIRED_TOPOLOGY_FIELDS = {
-    field.name for field in attrs.fields(Topology) if field.init
+    field.name for field in attrs.fields(Topology) if field.init  # type: ignore[arg-type]
 }
 
 
 def asdot(
     instance: object,
     *,
     render_node: bool = False,
@@ -97,27 +95,26 @@
 ) -> str:
     """Convert a `object` to a DOT language `str`.
 
     Only works for objects that can be represented as a graph, particularly a
     `.StateTransitionGraph` or a `list` of `.StateTransitionGraph` instances.
 
     Args:
-        instance: the input `object` that is to be rendered as DOT (graphviz)
-            language.
+        instance: the input `object` that is to be rendered as DOT (graphviz) language.
 
-        strip_spin: Normally, each `.StateTransitionGraph` has a `.Particle`
-            with a spin projection on its edges. This option hides the
-            projections, leaving only `.Particle` names on edges.
-
-        collapse_graphs: Group all transitions by equivalent kinematic topology
-            and combine all allowed particles on each edge.
-
-        render_node: Whether or not to render node ID (in the case of a
-            `.Topology`) and/or node properties (in the case of a
-            `.StateTransitionGraph`). Meaning of the labels:
+        strip_spin: Normally, each `.StateTransitionGraph` has a `.Particle` with a spin
+            projection on its edges. This option hides the projections, leaving only
+            `.Particle` names on edges.
+
+        collapse_graphs: Group all transitions by equivalent kinematic topology and
+            combine all allowed particles on each edge.
+
+        render_node: Whether or not to render node ID (in the case of a `.Topology`)
+            and/or node properties (in the case of a `.StateTransitionGraph`). Meaning
+            of the labels:
 
             - :math:`P`: parity prefactor
             - :math:`s`: tuple of **coupled spin** magnitude and its
               projection
             - :math:`l`: tuple of **angular momentum** and its projection
 
             See `.InteractionProperties` for more info.
@@ -127,16 +124,16 @@
         render_initial_state_id: Add edge IDs for the initial state edges.
         edge_style: Styling of a Graphviz edge.
         node_style: Styling of a Graphviz node.
         figure_style: Styling of the whole figure.
 
     .. seealso::
 
-        See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_
-        for the available styling arguments.
+        See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_ for the
+        available styling arguments.
 
     .. seealso:: :doc:`/usage/visualize`
     """
     if edge_style is None:
         edge_style = {}
     if node_style is None:
         node_style = {}
@@ -178,24 +175,20 @@
         file_extension = _get_file_extension(filename)
         if file_extension == "json":
             definition = json.load(stream)
             return fromdict(definition)
         if file_extension in ["yaml", "yml"]:
             definition = yaml.load(stream, Loader=yaml.SafeLoader)
             return fromdict(definition)
-    raise NotImplementedError(
-        f'No loader defined for file type "{file_extension}"'
-    )
+    raise NotImplementedError(f'No loader defined for file type "{file_extension}"')
 
 
 class _IncreasedIndent(yaml.Dumper):
     # pylint: disable=too-many-ancestors
-    def increase_indent(
-        self, flow: bool = False, indentless: bool = False
-    ) -> None:
+    def increase_indent(self, flow: bool = False, indentless: bool = False) -> None:
         return super().increase_indent(flow, False)
 
     def write_line_break(self, data: Optional[str] = None) -> None:
         """See https://stackoverflow.com/a/44284819."""
         super().write_line_break(data)
         if len(self.indents) == 1:
             super().write_line_break()
@@ -220,17 +213,15 @@
             if isinstance(instance, str):  # direct output of asdot
                 output_str = instance
             else:
                 output_str = asdot(instance)
             with open(filename, "w") as stream:
                 stream.write(output_str)
             return
-    raise NotImplementedError(
-        f'No writer defined for file type "{file_extension}"'
-    )
+    raise NotImplementedError(f'No writer defined for file type "{file_extension}"')
 
 
 def _get_file_extension(filename: str) -> str:
     path = Path(filename)
     extension = path.suffix.lower()
     if not extension:
         raise ValueError(f'No file extension in file name "{filename}"')
```

### Comparing `qrules-0.9.7/src/qrules/io/_dict.py` & `qrules-0.9.8/src/qrules/io/_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 import json
 from collections import abc
 from os.path import dirname, realpath
 from typing import Any, Dict
 
 import attrs
 
-from qrules.particle import (
-    Parity,
-    Particle,
-    ParticleCollection,
-    ParticleWithSpin,
-    Spin,
-)
+from qrules.particle import Parity, Particle, ParticleCollection, ParticleWithSpin, Spin
 from qrules.quantum_numbers import InteractionProperties
 from qrules.topology import Edge, StateTransitionGraph, Topology
 from qrules.transition import (
     ReactionInfo,
     State,
     StateTransition,
     StateTransitionCollection,
@@ -71,15 +65,15 @@
     )
 
 
 def _value_serializer(  # pylint: disable=unused-argument
     inst: type, field: attrs.Attribute, value: Any
 ) -> Any:
     if isinstance(value, abc.Mapping):
-        if all(map(lambda p: isinstance(p, Particle), value.values())):
+        if all(isinstance(p, Particle) for p in value.values()):
             return {k: v.name for k, v in value.items()}
         return dict(value)
     if not isinstance(
         inst, (ReactionInfo, State, StateTransition, StateTransitionCollection)
     ) and isinstance(value, Particle):
         return value.name
     if isinstance(value, Parity):
@@ -93,17 +87,15 @@
 
 
 def build_particle_collection(
     definition: dict, do_validate: bool = True
 ) -> ParticleCollection:
     if do_validate:
         validate_particle_collection(definition)
-    return ParticleCollection(
-        build_particle(p) for p in definition["particles"]
-    )
+    return ParticleCollection(build_particle(p) for p in definition["particles"])
 
 
 def build_particle(definition: dict) -> Particle:
     isospin_def = definition.get("isospin", None)
     if isospin_def is not None:
         definition["isospin"] = Spin(**isospin_def)
     for parity in ["parity", "c_parity", "g_parity"]:
@@ -143,16 +135,15 @@
         edge_props=edge_props,
         node_props=node_props,
     )
 
 
 def build_stc(definition: dict) -> StateTransitionCollection:
     transitions = [
-        build_state_transition(graph_def)
-        for graph_def in definition["transitions"]
+        build_state_transition(graph_def) for graph_def in definition["transitions"]
     ]
     return StateTransitionCollection(transitions=transitions)
 
 
 def build_state_transition(definition: dict) -> StateTransition:
     topology = build_topology(definition["topology"])
     states = {
```

### Comparing `qrules-0.9.7/src/qrules/io/_dot.py` & `qrules-0.9.8/src/qrules/io/_dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,15 @@
 
 See :doc:`/usage/visualize` for more info.
 """
 
 import functools
 import re
 from collections import abc
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Union
 
 import attrs
 
 from qrules.combinatorics import InitialFacts
 from qrules.particle import Particle, ParticleCollection, ParticleWithSpin
 from qrules.quantum_numbers import InteractionProperties, _to_fraction
 from qrules.solving import EdgeSettings, GraphSettings, NodeSettings
@@ -68,17 +58,15 @@
         del updated_graphviz_attrs["label"]
     if label:
         updated_graphviz_attrs["label"] = label
     styling = __create_graphviz_edge_node_styling(updated_graphviz_attrs)
     return f'    "{from_node}" -> "{to_node}"{styling};\n'
 
 
-def _create_graphviz_node(
-    name: str, label: str, graphviz_attrs: Dict[str, Any]
-) -> str:
+def _create_graphviz_node(name: str, label: str, graphviz_attrs: Dict[str, Any]) -> str:
     updated_graphviz_attrs = {"shape": None, **graphviz_attrs, "label": label}
     styling = __create_graphviz_edge_node_styling(updated_graphviz_attrs)
     return f'    "{name}"{styling};\n'
 
 
 def __dot_kwargs_to_header(graphviz_attrs: Dict[str, Any]) -> str:
     r"""Create DOT-compatible header lines from Graphviz attributes.
@@ -95,16 +83,16 @@
     line_ending = ";\n"
     return indent + f"{line_ending}{indent}".join(assignments) + line_ending
 
 
 def __create_graphviz_edge_node_styling(graphviz_attrs: Dict[str, Any]) -> str:
     """Create a `str` of Graphviz attribute assignments for a node or edge.
 
-    See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_ for
-    the assignment syntax.
+    See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_ for the
+    assignment syntax.
 
     >>> __create_graphviz_edge_node_styling({"size": 12})
     ' [size=12]'
     >>> __create_graphviz_edge_node_styling({"color": "red", "size": 8})
     ' [color="red", size=8]'
     """
     if not graphviz_attrs:
@@ -112,16 +100,16 @@
     assignments = __create_graphviz_assignments(graphviz_attrs)
     return f" [{', '.join(assignments)}]"
 
 
 def __create_graphviz_assignments(graphviz_attrs: Dict[str, Any]) -> List[str]:
     """Create a `list` of graphviz attribute assignments.
 
-    See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_ for
-    the assignment syntax.
+    See `Graphviz attributes <https://graphviz.org/doc/info/attrs.html>`_ for the
+    assignment syntax.
 
     >>> __create_graphviz_assignments({"size": 12})
     ['size=12']
     >>> __create_graphviz_assignments({"color": "red", "size": 8})
     ['color="red"', 'size=8']
     >>> __create_graphviz_assignments({"shape": None})
     ['shape=none']
@@ -149,17 +137,15 @@
     edge_style: Dict[str, Any],
     node_style: Dict[str, Any],
 ) -> str:
     if strip_spin and collapse_graphs:
         raise ValueError("Cannot both strip spin and collapse graphs")
     if collapse_graphs:
         if render_node:
-            raise ValueError(
-                "Collapsed graphs cannot be rendered with node properties"
-            )
+            raise ValueError("Collapsed graphs cannot be rendered with node properties")
         graphs = _collapse_graphs(graphs)
     elif strip_spin:
         if render_node:
             stripped_graphs = []
             for graph in graphs:
                 if isinstance(graph, StateTransition):
                     graph = graph.to_graph()
@@ -243,17 +229,15 @@
     elif isinstance(graph, (StateTransition, StateTransitionGraph)):
         rendered_graph = graph
         topology = graph.topology
     elif isinstance(graph, Topology):
         rendered_graph = graph
         topology = graph
     else:
-        raise NotImplementedError(
-            f"Cannot render {graph.__class__.__name__} as dot"
-        )
+        raise NotImplementedError(f"Cannot render {graph.__class__.__name__} as dot")
     top = topology.incoming_edge_ids
     outs = topology.outgoing_edge_ids
     for edge_id in top | outs:
         if edge_id in top:
             render = render_initial_state_id
         else:
             render = render_final_state_id
@@ -266,17 +250,15 @@
     dot += __rank_string(top, prefix)
     dot += __rank_string(outs, prefix)
     for i, edge in topology.edges.items():
         j, k = edge.ending_node_id, edge.originating_node_id
         from_node = prefix + __node_name(i, k)
         to_node = prefix + __node_name(i, j)
         if j is None or k is None:
-            dot += _create_graphviz_edge(
-                from_node, to_node, graphviz_attrs=edge_style
-            )
+            dot += _create_graphviz_edge(from_node, to_node, graphviz_attrs=edge_style)
         else:
             label = __get_edge_label(rendered_graph, i, render_resonance_id)
             dot += _create_graphviz_edge(
                 from_node, to_node, label=label, graphviz_attrs=edge_style
             )
     if isinstance(graph, ProblemSet):
         node_props = graph.solving_settings.node_settings
@@ -287,17 +269,15 @@
             dot += _create_graphviz_node(
                 name=f"{prefix}node{node_id}",
                 label=node_label,
                 graphviz_attrs=node_style,
             )
     if isinstance(graph, (StateTransition, StateTransitionGraph)):
         if isinstance(graph, StateTransition):
-            interactions: Mapping[
-                int, InteractionProperties
-            ] = graph.interactions
+            interactions: Mapping[int, InteractionProperties] = graph.interactions
         else:
             interactions = {i: graph.get_node_props(i) for i in topology.nodes}
         for node_id, node_prop in interactions.items():
             node_label = ""
             if render_node:
                 node_label = __node_label(node_prop)
             dot += _create_graphviz_node(
@@ -363,17 +343,15 @@
     if isinstance(graph, StateTransitionGraph):
         edge_prop = graph.get_edge_props(edge_id)
         return ___render_edge_with_id(edge_id, edge_prop, render_edge_id)
     if isinstance(graph, Topology):
         if render_edge_id:
             return str(edge_id)
         return ""
-    raise NotImplementedError(
-        f"Cannot render {graph.__class__.__name__} as dot"
-    )
+    raise NotImplementedError(f"Cannot render {graph.__class__.__name__} as dot")
 
 
 def ___render_edge_with_id(
     edge_id: int,
     edge_prop: Optional[
         Union[EdgeSettings, ParticleCollection, Particle, ParticleWithSpin]
     ],
@@ -435,29 +413,28 @@
     raise NotImplementedError
 
 
 def __render_settings(settings: Union[EdgeSettings, NodeSettings]) -> str:
     output = ""
     if settings.rule_priorities:
         output += "RULE PRIORITIES\n"
-        rule_names = map(
-            lambda item: f"{item[0].__name__} - {item[1]}",  # type: ignore[union-attr]
-            settings.rule_priorities.items(),
+        rule_names = (
+            f"{item[0].__name__} - {item[1]}"  # type: ignore[union-attr]
+            for item in settings.rule_priorities.items()
         )
         sorted_names = sorted(rule_names, key=__extract_priority, reverse=True)
         output += "\n".join(sorted_names)
     if settings.qn_domains:
         if output:
             output += "\n"
-        domains = map(
-            lambda item: f"{item[0].__name__} ∊ {item[1]}",
-            settings.qn_domains.items(),
+        domains = sorted(
+            f"{item[0].__name__} ∊ {item[1]}" for item in settings.qn_domains.items()
         )
         output += "DOMAINS\n"
-        output += "\n".join(sorted(domains))
+        output += "\n".join(domains)
     return output
 
 
 def __extract_priority(description: str) -> int:
     matches = re.match(r".* \- ([0-9]+)$", description)
     if matches is None:
         raise ValueError(f"{description} does not contain a priority number")
@@ -476,17 +453,15 @@
     .. seealso:: :doc:`/usage/visualize`
     """
     inventory: List[StateTransitionGraph[Particle]] = []
     for transition in graphs:
         if isinstance(transition, StateTransition):
             transition = transition.to_graph()
         if any(
-            transition.compare(
-                other, edge_comparator=lambda e1, e2: e1[0] == e2
-            )
+            transition.compare(other, edge_comparator=lambda e1, e2: e1[0] == e2)
             for other in inventory
         ):
             continue
         stripped_graph = _strip_projections(transition)
         inventory.append(stripped_graph)
     inventory = sorted(
         inventory,
@@ -528,17 +503,15 @@
         graph: StateTransitionGraph[Particle],
         merged_graph: StateTransitionGraph[ParticleCollection],
     ) -> None:
         if (
             graph.topology.intermediate_edge_ids
             != merged_graph.topology.intermediate_edge_ids
         ):
-            raise ValueError(
-                "Cannot merge graphs that don't have the same edge IDs"
-            )
+            raise ValueError("Cannot merge graphs that don't have the same edge IDs")
         for i in graph.topology.edges:
             particle = graph.get_edge_props(i)
             other_particles = merged_graph.get_edge_props(i)
             if particle not in other_particles:
                 other_particles += particle
 
     def is_same_shape(
@@ -572,14 +545,13 @@
                 edge_id: ParticleCollection({graph.get_edge_props(edge_id)})
                 for edge_id in graph.topology.edges
             }
             inventory.append(
                 StateTransitionGraph[ParticleCollection](
                     topology=graph.topology,
                     node_props={
-                        i: graph.get_node_props(i)
-                        for i in graph.topology.nodes
+                        i: graph.get_node_props(i) for i in graph.topology.nodes
                     },
                     edge_props=new_edge_props,
                 )
             )
     return inventory
```

### Comparing `qrules-0.9.7/src/qrules/particle-validation.json` & `qrules-0.9.8/src/qrules/particle-validation.json`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/src/qrules/particle.py` & `qrules-0.9.8/src/qrules/particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pylint: disable=import-outside-toplevel
 """A collection of particle info containers.
 
-The :mod:`.particle` module is the starting point of `qrules`. Its main
-interface is the `ParticleCollection`, which is a collection of immutable
-`Particle` instances that are uniquely defined by their properties. As such, it
-can be used stand-alone as a database of quantum numbers (see
-:doc:`/usage/particle`).
+The :mod:`.particle` module is the starting point of `qrules`. Its main interface is the
+`ParticleCollection`, which is a collection of immutable `Particle` instances that are
+uniquely defined by their properties. As such, it can be used stand-alone as a database
+of quantum numbers (see :doc:`/usage/particle`).
 
 The `.transition` module uses the properties of `Particle` instances when it
 computes which `.StateTransitionGraph` s are allowed between an initial state
 and final state.
 """
 
 import logging
@@ -37,21 +36,19 @@
 from attrs.converters import optional
 from attrs.validators import instance_of
 
 from .conservation_rules import GellMannNishijimaInput, gellmann_nishijima
 from .quantum_numbers import Parity, _to_fraction
 
 if TYPE_CHECKING:
+    from IPython.lib.pretty import PrettyPrinter
     from particle import Particle as PdgDatabase
     from particle.particle import enums
 
-    try:
-        from IPython.lib.pretty import PrettyPrinter
-    except ImportError:
-        PrettyPrinter = Any
+_LOGGER = logging.getLogger(__name__)
 
 
 def _to_float(value: SupportsFloat) -> float:
     float_value = float(value)
     if float_value == -0.0:
         float_value = 0.0
     return float_value
@@ -69,16 +66,15 @@
         if self.magnitude % 0.5 != 0.0:
             raise ValueError(
                 f"Spin magnitude {self.magnitude} has to be a multitude of 0.5"
             )
         if abs(self.projection) > self.magnitude:
             if self.magnitude < 0.0:
                 raise ValueError(
-                    "Spin magnitude has to be positive, but is"
-                    f" {self.magnitude}"
+                    f"Spin magnitude has to be positive, but is {self.magnitude}"
                 )
             raise ValueError(
                 "Absolute value of spin projection cannot be larger than its "
                 "magnitude:\n"
                 f" abs({self.projection}) > {self.magnitude}"
             )
         if not (self.projection - self.magnitude).is_integer():
@@ -127,24 +123,23 @@
 
 
 @total_ordering
 @frozen(kw_only=True, order=False, repr=True)
 class Particle:  # pylint: disable=too-many-instance-attributes
     """Immutable container of data defining a physical particle.
 
-    A `Particle` is defined by the minimum set of the quantum numbers that
-    every possible instances of that particle have in common (the "static"
-    quantum numbers of the particle). A "non-static" quantum number is the spin
-    projection. Hence `Particle` instances do **not** contain spin projection
-    information.
-
-    `Particle` instances are uniquely defined by their quantum numbers and
-    properties like `~Particle.mass`. The `~Particle.name` and `~Particle.pid`
-    are therefore just labels that are not taken into account when checking if
-    two `Particle` instances are equal.
+    A `Particle` is defined by the minimum set of the quantum numbers that every
+    possible instances of that particle have in common (the "static" quantum numbers of
+    the particle). A "non-static" quantum number is the spin projection. Hence
+    `Particle` instances do **not** contain spin projection information.
+
+    `Particle` instances are uniquely defined by their quantum numbers and properties
+    like `~Particle.mass`. The `~Particle.name` and `~Particle.pid` are therefore just
+    labels that are not taken into account when checking if two `Particle` instances are
+    equal.
 
     .. note:: As opposed to classes such as `.EdgeQuantumNumbers` and
         `.NodeQuantumNumbers`, the `Particle` class serves as an interface to
         the user (see :doc:`/usage/particle`).
     """
 
     # Labels
@@ -161,31 +156,23 @@
     charmness: int = field(default=0, validator=instance_of(int))
     bottomness: int = field(default=0, validator=instance_of(int))
     topness: int = field(default=0, validator=instance_of(int))
     baryon_number: int = field(default=0, validator=instance_of(int))
     electron_lepton_number: int = field(default=0, validator=instance_of(int))
     muon_lepton_number: int = field(default=0, validator=instance_of(int))
     tau_lepton_number: int = field(default=0, validator=instance_of(int))
-    parity: Optional[Parity] = field(
-        converter=optional(_to_parity), default=None
-    )
-    c_parity: Optional[Parity] = field(
-        converter=optional(_to_parity), default=None
-    )
-    g_parity: Optional[Parity] = field(
-        converter=optional(_to_parity), default=None
-    )
+    parity: Optional[Parity] = field(converter=optional(_to_parity), default=None)
+    c_parity: Optional[Parity] = field(converter=optional(_to_parity), default=None)
+    g_parity: Optional[Parity] = field(converter=optional(_to_parity), default=None)
 
     def __attrs_post_init__(self) -> None:
         if self.isospin is not None and not gellmann_nishijima(
             GellMannNishijimaInput(
                 charge=self.charge,
-                isospin_projection=self.isospin.projection
-                if self.isospin
-                else None,
+                isospin_projection=self.isospin.projection if self.isospin else None,
                 strangeness=self.strangeness,
                 charmness=self.charmness,
                 bottomness=self.bottomness,
                 topness=self.topness,
                 baryon_number=self.baryon_number,
                 electron_lepton_number=self.electron_lepton_number,
                 muon_lepton_number=self.muon_lepton_number,
@@ -215,16 +202,15 @@
                     name_root,
                     particle.mass,
                     particle.charge,
                 )
 
             return sorting_key(self) > sorting_key(other)
         raise NotImplementedError(
-            f"Cannot compare {self.__class__.__name__} with"
-            f" {other.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with {other.__class__.__name__}"
         )
 
     def __neg__(self) -> "Particle":
         return create_antiparticle(self)
 
     def is_lepton(self) -> bool:
         return (
@@ -243,15 +229,15 @@
                     value = getattr(self, attribute.name)
                     if value != attribute.default:
                         p.breakable()
                         p.text(f"{attribute.name}=")
                         if isinstance(value, Parity):
                             p.text(_to_fraction(int(value), render_plus=True))
                         else:
-                            p.pretty(value)
+                            p.pretty(value)  # type: ignore[attr-defined]
                         p.text(",")
             p.breakable()
             p.text(")")
 
 
 def _get_name_root(name: str) -> str:
     """Strip a string (particularly the `.Particle.name`) of specifications."""
@@ -284,24 +270,21 @@
             f"Cannot search for type {instance.__class__.__name__}"
         )
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, abc.Iterable):
             return set(self) == set(other)
         raise NotImplementedError(
-            f"Cannot compare {self.__class__.__name__} with "
-            f" {self.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with  {self.__class__.__name__}"
         )
 
     def __getitem__(self, particle_name: str) -> Particle:
         if particle_name in self.__particles:
             return self.__particles[particle_name]
-        error_message = (
-            f"No particle with name '{particle_name}' in the database"
-        )
+        error_message = f"No particle with name '{particle_name}' in the database"
         candidates = [
             p.name
             for p in sorted(self, key=lambda p: p.mass)
             if p.name.startswith(particle_name)
         ]
         if not candidates:
             candidates = get_close_matches(particle_name, self.names, n=5)
@@ -339,31 +322,33 @@
         class_name = type(self).__name__
         if cycle:
             p.text(f"{class_name}(...)")
         else:
             with p.group(indent=2, open=f"{class_name}({{"):
                 for particle in self:
                     p.breakable()
-                    p.pretty(particle)
+                    p.pretty(particle)  # type: ignore[attr-defined]
                     p.text(",")
             p.breakable()
             p.text("})")
 
     def add(self, value: Particle) -> None:
         if value in self.__particles.values():
             equivalent_particles = {p for p in self if p == value}
             equivalent_particle = next(iter(equivalent_particles))
             raise ValueError(
-                f'Added particle "{value.name}" is equivalent to '
-                f'existing particle "{equivalent_particle.name}"',
+                (
+                    f'Added particle "{value.name}" is equivalent to '
+                    f'existing particle "{equivalent_particle.name}"'
+                ),
             )
         if value.name in self.__particles:
-            logging.warning(f'Overwriting particle with name "{value.name}"')
+            _LOGGER.warning(f'Overwriting particle with name "{value.name}"')
         if value.pid in self.__pid_to_name:
-            logging.warning(
+            _LOGGER.warning(
                 f"Particle with PID {value.pid} already exists:"
                 f' "{self.find(value.pid).name}"'
             )
         self.__particles[value.name] = value
         self.__pid_to_name[value.pid] = value.name
 
     def discard(self, value: Union[Particle, str]) -> None:
@@ -379,20 +364,20 @@
         del self.__pid_to_name[self[particle_name].pid]
         del self.__particles[particle_name]
 
     def find(self, search_term: Union[int, str]) -> Particle:
         """Search for a particle by either name (`str`) or PID (`int`)."""
         if isinstance(search_term, str):
             particle_name = search_term
-            return self.__getitem__(particle_name)
+            return self.__getitem__(particle_name)  # pylint: disable=C2801
         if isinstance(search_term, int):
             if search_term not in self.__pid_to_name:
                 raise KeyError(f"No particle with PID {search_term}")
             particle_name = self.__pid_to_name[search_term]
-            return self.__getitem__(particle_name)
+            return self.__getitem__(particle_name)  # pylint: disable=C2801
         raise NotImplementedError(
             f"Cannot search for a search term of type {type(search_term)}"
         )
 
     def filter(  # noqa: A003
         self, function: Callable[[Particle], bool]
     ) -> "ParticleCollection":
@@ -404,20 +389,18 @@
         >>> pdg = load_pdg()
         >>> subset = pdg.filter(
         ...     lambda p: p.mass > 1.8
         ...     and p.mass < 2.0
         ...     and p.spin == 2
         ...     and p.strangeness == 1
         ... )
-        >>> sorted(list(subset.names))
+        >>> sorted(subset.names)
         ['K(2)(1820)+', 'K(2)(1820)0', 'K(2)*(1980)+', 'K(2)*(1980)0']
         """
-        return ParticleCollection(
-            {particle for particle in self if function(particle)}
-        )
+        return ParticleCollection({particle for particle in self if function(particle)})
 
     def update(self, other: Iterable[Particle]) -> None:
         if not isinstance(other, abc.Iterable):
             raise TypeError(
                 f"Cannot update {self.__class__.__name__} from "
                 f"non-iterable class {self.__class__.__name__}"
             )
@@ -455,42 +438,40 @@
         name=name if name else template_particle.name,
         pid=pid if pid else template_particle.pid,
         latex=latex if latex else template_particle.latex,
         mass=mass if mass is not None else template_particle.mass,
         width=width if width else template_particle.width,
         spin=spin if spin else template_particle.spin,
         charge=charge if charge else template_particle.charge,
-        strangeness=strangeness
-        if strangeness
-        else template_particle.strangeness,
+        strangeness=strangeness if strangeness else template_particle.strangeness,
         charmness=charmness if charmness else template_particle.charmness,
         bottomness=bottomness if bottomness else template_particle.bottomness,
         topness=topness if topness else template_particle.topness,
-        baryon_number=baryon_number
-        if baryon_number
-        else template_particle.baryon_number,
-        electron_lepton_number=electron_lepton_number
-        if electron_lepton_number
-        else template_particle.electron_lepton_number,
-        muon_lepton_number=muon_lepton_number
-        if muon_lepton_number
-        else template_particle.muon_lepton_number,
-        tau_lepton_number=tau_lepton_number
-        if tau_lepton_number
-        else template_particle.tau_lepton_number,
-        isospin=template_particle.isospin
-        if isospin is None
-        else template_particle.isospin,
+        baryon_number=(
+            baryon_number if baryon_number else template_particle.baryon_number
+        ),
+        electron_lepton_number=(
+            electron_lepton_number
+            if electron_lepton_number
+            else template_particle.electron_lepton_number
+        ),
+        muon_lepton_number=(
+            muon_lepton_number
+            if muon_lepton_number
+            else template_particle.muon_lepton_number
+        ),
+        tau_lepton_number=(
+            tau_lepton_number
+            if tau_lepton_number
+            else template_particle.tau_lepton_number
+        ),
+        isospin=template_particle.isospin if isospin is None else isospin,
         parity=template_particle.parity if parity is None else Parity(parity),
-        c_parity=template_particle.c_parity
-        if c_parity is None
-        else Parity(c_parity),
-        g_parity=template_particle.g_parity
-        if g_parity is None
-        else Parity(g_parity),
+        c_parity=template_particle.c_parity if c_parity is None else Parity(c_parity),
+        g_parity=template_particle.g_parity if g_parity is None else Parity(g_parity),
     )
 
 
 def create_antiparticle(
     template_particle: Particle,
     new_name: Optional[str] = None,
     new_latex: Optional[str] = None,
@@ -503,17 +484,15 @@
         if template_particle.spin.is_integer():
             parity = template_particle.parity
         else:
             parity = -template_particle.parity
     return Particle(
         name=new_name if new_name else "anti-" + template_particle.name,
         pid=-template_particle.pid,
-        latex=new_latex
-        if new_latex
-        else Rf"\overline{{{template_particle.latex}}}",
+        latex=new_latex if new_latex else Rf"\overline{{{template_particle.latex}}}",
         mass=template_particle.mass,
         width=template_particle.width,
         charge=-template_particle.charge,
         spin=template_particle.spin,
         isospin=isospin,
         strangeness=-template_particle.strangeness,
         charmness=-template_particle.charmness,
@@ -669,18 +648,15 @@
     else:
         projection = 0.0
         if pdg_particle.pdgid.is_hadron:
             quark_content = __filter_quark_content(pdg_particle)
             projection += quark_content.count("u") + quark_content.count("D")
             projection -= quark_content.count("U") + quark_content.count("d")
             projection *= 0.5
-    if (
-        pdg_particle.I is not None
-        and not (pdg_particle.I - projection).is_integer()
-    ):
+    if pdg_particle.I is not None and not (pdg_particle.I - projection).is_integer():
         raise ValueError(f"Cannot have isospin {(pdg_particle.I, projection)}")
     return projection
 
 
 def __filter_quark_content(pdg_particle: "PdgDatabase") -> str:
     matches = re.search(r"([dDuUsScCbBtT+-]{2,})", pdg_particle.quarks)
     if matches is None:
```

### Comparing `qrules-0.9.7/src/qrules/quantum_numbers.py` & `qrules-0.9.8/src/qrules/quantum_numbers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Definitions used internally for type hints and signatures.
 
-`qrules` is strictly typed (enforced through :doc:`mypy <mypy:index>`). This
-module bundles structures and definitions that don't serve as data containers
-but only as type hints. `.EdgeQuantumNumbers` and `.NodeQuantumNumbers` are the
-main structures and serve as a bridge between the :mod:`.particle` and the
-:mod:`.conservation_rules` module.
+`qrules` is strictly typed (enforced through :doc:`mypy <mypy:index>`). This module
+bundles structures and definitions that don't serve as data containers but only as type
+hints. `.EdgeQuantumNumbers` and `.NodeQuantumNumbers` are the main structures and serve
+as a bridge between the :mod:`.particle` and the :mod:`.conservation_rules` module.
 """
 
 from decimal import Decimal
 from fractions import Fraction
 from functools import total_ordering
 from typing import Any, Generator, NewType, Optional, Union
 
@@ -61,21 +60,20 @@
     return label
 
 
 @frozen(init=False)
 class EdgeQuantumNumbers:  # pylint: disable=too-many-instance-attributes
     """Definition of quantum numbers for edges.
 
-    This class defines the types that are used in the
-    :mod:`.conservation_rules`, for instance in
-    `.additive_quantum_number_rule`. You can also create data classes (see
-    :func:`attrs.define`) with data members that are typed as the data members
-    of `.EdgeQuantumNumbers` (see for example `.HelicityParityEdgeInput`) and
-    use them in conservation rules that satisfy the appropriate rule protocol
-    (see `.ConservationRule`, `.EdgeQNConservationRule`).
+    This class defines the types that are used in the :mod:`.conservation_rules`, for
+    instance in `.additive_quantum_number_rule`. You can also create data classes (see
+    :func:`attrs.define`) with data members that are typed as the data members of
+    `.EdgeQuantumNumbers` (see for example `.HelicityParityEdgeInput`) and use them in
+    conservation rules that satisfy the appropriate rule protocol (see
+    `.ConservationRule`, `.EdgeQNConservationRule`).
     """
 
     pid = NewType("pid", int)
     mass = NewType("mass", float)
     width = NewType("width", float)
     spin_magnitude = NewType("spin_magnitude", float)
     spin_projection = NewType("spin_projection", float)
@@ -169,40 +167,32 @@
 class InteractionProperties:
     """Immutable data structure containing interaction properties.
 
     Interactions are represented by a node on a `.StateTransitionGraph`. This
     class represents the properties that are carried collectively by the edges
     that this node connects.
 
-    Interaction properties are in particular important in the canonical basis
-    of the helicity formalism. There, the *coupled spin* and angular momentum
-    of each interaction are used for the Clebsch-Gordan coefficients for each
-    term in a sequential amplitude.
+    Interaction properties are in particular important in the canonical basis of the
+    helicity formalism. There, the *coupled spin* and angular momentum of each
+    interaction are used for the Clebsch-Gordan coefficients for each term in a
+    sequential amplitude.
 
-    .. note:: As opposed to `NodeQuantumNumbers`, the `InteractionProperties`
-        class serves as an interface to the user.
+    .. note:: As opposed to `NodeQuantumNumbers`, the `InteractionProperties` class
+        serves as an interface to the user.
     """
 
     l_magnitude: Optional[int] = field(  # L cannot be half integer
         default=None, converter=_to_optional_int
     )
-    l_projection: Optional[int] = field(
-        default=None, converter=_to_optional_int
-    )
-    s_magnitude: Optional[float] = field(
-        default=None, converter=_to_optional_float
-    )
-    s_projection: Optional[float] = field(
-        default=None, converter=_to_optional_float
-    )
+    l_projection: Optional[int] = field(default=None, converter=_to_optional_int)
+    s_magnitude: Optional[float] = field(default=None, converter=_to_optional_float)
+    s_projection: Optional[float] = field(default=None, converter=_to_optional_float)
     parity_prefactor: Optional[float] = field(
         default=None, converter=_to_optional_float
     )
 
 
-def arange(
-    x_1: float, x_2: float, delta: float = 1.0
-) -> Generator[float, None, None]:
+def arange(x_1: float, x_2: float, delta: float = 1.0) -> Generator[float, None, None]:
     current = Decimal(x_1)
     while current < x_2:
         yield float(current)
         current += Decimal(delta)
```

### Comparing `qrules-0.9.7/src/qrules/settings.py` & `qrules-0.9.8/src/qrules/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,23 +51,23 @@
 ADDITIONAL_PARTICLES_DEFINITIONS_PATH: str = join(
     __QRULES_PATH, "additional_definitions.yml"
 )
 
 CONSERVATION_LAW_PRIORITIES: Dict[
     Union[GraphElementRule, EdgeQNConservationRule, ConservationRule], int
 ] = {
-    MassConservation: 10,
-    ElectronLNConservation: 45,
-    MuonLNConservation: 44,
-    TauLNConservation: 43,
-    BaryonNumberConservation: 90,
-    StrangenessConservation: 69,
-    CharmConservation: 70,
-    BottomnessConservation: 68,
-    ChargeConservation: 100,
+    MassConservation: 10,  # type: ignore[dict-item]
+    ElectronLNConservation: 45,  # type: ignore[dict-item]
+    MuonLNConservation: 44,  # type: ignore[dict-item]
+    TauLNConservation: 43,  # type: ignore[dict-item]
+    BaryonNumberConservation: 90,  # type: ignore[dict-item]
+    StrangenessConservation: 69,  # type: ignore[dict-item]
+    CharmConservation: 70,  # type: ignore[dict-item]
+    BottomnessConservation: 68,  # type: ignore[dict-item]
+    ChargeConservation: 100,  # type: ignore[dict-item]
     spin_conservation: 8,
     spin_magnitude_conservation: 8,
     parity_conservation: 6,
     c_parity_conservation: 5,
     g_parity_conservation: 3,
     isospin_conservation: 60,
     ls_spin_validity: 89,
@@ -98,17 +98,22 @@
         description_lower = description.lower()
         if description_lower.startswith("e"):
             return InteractionType.EM
         if description_lower.startswith("s"):
             return InteractionType.STRONG
         if description_lower.startswith("w"):
             return InteractionType.WEAK
-        raise ValueError(
-            f'Could not determine interaction type from "{description}"'
-        )
+        raise ValueError(f'Could not determine interaction type from "{description}"')
+
+
+DEFAULT_INTERACTION_TYPES = [
+    InteractionType.STRONG,
+    InteractionType.EM,
+    InteractionType.WEAK,
+]
 
 
 def create_interaction_settings(  # pylint: disable=too-many-locals,too-many-arguments
     formalism: str,
     particle_db: ParticleCollection,
     nbody_topology: bool = False,
     mass_conservation_factor: Optional[float] = 3.0,
@@ -121,37 +126,31 @@
             isospin_validity,
             gellmann_nishijima,
             spin_validity,
         },
         rule_priorities=EDGE_RULE_PRIORITIES,
         qn_domains=_create_domains(particle_db),
     )
-    formalism_node_settings = NodeSettings(
-        rule_priorities=CONSERVATION_LAW_PRIORITIES
-    )
+    formalism_node_settings = NodeSettings(rule_priorities=CONSERVATION_LAW_PRIORITIES)
 
     angular_momentum_domain = __get_ang_mom_magnitudes(
         nbody_topology, max_angular_momentum
     )
-    spin_magnitude_domain = __get_spin_magnitudes(
-        nbody_topology, max_spin_magnitude
-    )
+    spin_magnitude_domain = __get_spin_magnitudes(nbody_topology, max_spin_magnitude)
     if "helicity" in formalism:
         formalism_node_settings.conservation_rules = {
             spin_magnitude_conservation,
             helicity_conservation,
         }
         formalism_node_settings.qn_domains = {
             NodeQN.l_magnitude: angular_momentum_domain,
             NodeQN.s_magnitude: spin_magnitude_domain,
         }
     elif formalism == "canonical":
-        formalism_node_settings.conservation_rules = {
-            spin_magnitude_conservation
-        }
+        formalism_node_settings.conservation_rules = {spin_magnitude_conservation}
         if nbody_topology:
             formalism_node_settings.conservation_rules = {
                 spin_conservation,
                 ls_spin_validity,
             }
         formalism_node_settings.qn_domains = {
             NodeQN.l_magnitude: angular_momentum_domain,
@@ -177,36 +176,36 @@
             MassConservation(mass_conservation_factor)
         )
 
     interaction_type_settings = {}
     weak_node_settings = deepcopy(formalism_node_settings)
     weak_node_settings.conservation_rules.update(
         [
-            ChargeConservation(),
-            ElectronLNConservation(),
-            MuonLNConservation(),
-            TauLNConservation(),
-            BaryonNumberConservation(),
+            ChargeConservation(),  # type: ignore[abstract]
+            ElectronLNConservation(),  # type: ignore[abstract]
+            MuonLNConservation(),  # type: ignore[abstract]
+            TauLNConservation(),  # type: ignore[abstract]
+            BaryonNumberConservation(),  # type: ignore[abstract]
             identical_particle_symmetrization,
         ]
     )
     weak_node_settings.interaction_strength = 10 ** (-4)
     weak_edge_settings = deepcopy(formalism_edge_settings)
 
     interaction_type_settings[InteractionType.WEAK] = (
         weak_edge_settings,
         weak_node_settings,
     )
 
     em_node_settings = deepcopy(weak_node_settings)
     em_node_settings.conservation_rules.update(
         {
-            CharmConservation(),
-            StrangenessConservation(),
-            BottomnessConservation(),
+            CharmConservation(),  # type: ignore[abstract]
+            StrangenessConservation(),  # type: ignore[abstract]
+            BottomnessConservation(),  # type: ignore[abstract]
             parity_conservation,
             c_parity_conservation,
         }
     )
     if "helicity" in formalism:
         em_node_settings.conservation_rules.add(parity_conservation_helicity)
         em_node_settings.qn_domains.update({NodeQN.parity_prefactor: [-1, 1]})
@@ -229,25 +228,21 @@
         strong_edge_settings,
         strong_node_settings,
     )
 
     return interaction_type_settings
 
 
-def __get_ang_mom_magnitudes(
-    is_nbody: bool, max_angular_momentum: int
-) -> List[float]:
+def __get_ang_mom_magnitudes(is_nbody: bool, max_angular_momentum: int) -> List[float]:
     if is_nbody:
         return [0]
     return _int_domain(0, max_angular_momentum)  # type: ignore[return-value]
 
 
-def __get_spin_magnitudes(
-    is_nbody: bool, max_spin_magnitude: float
-) -> List[float]:
+def __get_spin_magnitudes(is_nbody: bool, max_spin_magnitude: float) -> List[float]:
     if is_nbody:
         return [0]
     return _halves_domain(0, max_spin_magnitude)
 
 
 def _create_domains(particle_db: ParticleCollection) -> Dict[Any, list]:
     domains: Dict[Any, list] = {
@@ -262,24 +257,20 @@
     for edge_qn, getter in {
         EdgeQN.charge: lambda p: p.charge,
         EdgeQN.baryon_number: lambda p: p.baryon_number,
         EdgeQN.strangeness: lambda p: p.strangeness,
         EdgeQN.charmness: lambda p: p.charmness,
         EdgeQN.bottomness: lambda p: p.bottomness,
     }.items():
-        domains[edge_qn] = __extend_negative(
-            __positive_int_domain(particle_db, getter)
-        )
+        domains[edge_qn] = __extend_negative(__positive_int_domain(particle_db, getter))
 
     domains[EdgeQN.spin_magnitude] = __positive_halves_domain(
         particle_db, lambda p: p.spin
     )
-    domains[EdgeQN.spin_projection] = __extend_negative(
-        domains[EdgeQN.spin_magnitude]
-    )
+    domains[EdgeQN.spin_projection] = __extend_negative(domains[EdgeQN.spin_magnitude])
     domains[EdgeQN.isospin_magnitude] = __positive_halves_domain(
         particle_db,
         lambda p: 0 if p.isospin is None else p.isospin.magnitude,
     )
     domains[EdgeQN.isospin_projection] = __extend_negative(
         domains[EdgeQN.isospin_magnitude]
     )
@@ -322,16 +313,15 @@
 
 def _halves_domain(start: float, stop: float) -> List[float]:
     if start % 0.5 != 0.0:
         raise ValueError(f"Start value {start} needs to be multiple of 0.5")
     if stop % 0.5 != 0.0:
         raise ValueError(f"Stop value {stop} needs to be multiple of 0.5")
     return [
-        int(v) if v.is_integer() else v
-        for v in arange(start, stop + 0.25, delta=0.5)
+        int(v) if v.is_integer() else v for v in arange(start, stop + 0.25, delta=0.5)
     ]
 
 
 def _int_domain(start: int, stop: int) -> List[int]:
     return list(range(start, stop + 1))
```

### Comparing `qrules-0.9.7/src/qrules/solving.py` & `qrules-0.9.8/src/qrules/solving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=too-many-lines
 """Functions to solve a particle reaction problem.
 
 This module is responsible for solving a particle reaction problem stated by a
-`.StateTransitionGraph` and corresponding `.GraphSettings`. The `.Solver`
-classes (e.g. :class:`.CSPSolver`) generate new quantum numbers (for example
-belonging to an intermediate state) and validate the decay processes with the
-rules formulated by the :mod:`.conservation_rules` module.
+`.StateTransitionGraph` and corresponding `.GraphSettings`. The `.Solver` classes (e.g.
+:class:`.CSPSolver`) generate new quantum numbers (for example belonging to an
+intermediate state) and validate the decay processes with the rules formulated by the
+:mod:`.conservation_rules` module.
 """
 
 
 import inspect
 import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict
@@ -27,40 +27,32 @@
     Type,
     TypeVar,
     Union,
 )
 
 import attrs
 from attrs import define, field, frozen
-from constraint import (
-    BacktrackingSolver,
-    Constraint,
-    Problem,
-    Unassigned,
-    Variable,
-)
+from constraint import BacktrackingSolver, Constraint, Problem, Unassigned, Variable
 
 from qrules._implementers import implement_pretty_repr
 
 from .argument_handling import (
     GraphEdgePropertyMap,
     GraphElementRule,
     GraphNodePropertyMap,
     Rule,
     RuleArgumentHandler,
     Scalar,
     get_required_qns,
 )
-from .quantum_numbers import (
-    EdgeQuantumNumber,
-    EdgeQuantumNumbers,
-    NodeQuantumNumber,
-)
+from .quantum_numbers import EdgeQuantumNumber, EdgeQuantumNumbers, NodeQuantumNumber
 from .topology import Topology
 
+_LOGGER = logging.getLogger(__name__)
+
 
 @implement_pretty_repr
 @define
 class EdgeSettings:
     """Solver settings for a specific edge of a graph."""
 
     conservation_rules: Set[GraphElementRule] = field(factory=set)
@@ -69,17 +61,17 @@
 
 
 @implement_pretty_repr
 @define
 class NodeSettings:
     """Container class for the interaction settings.
 
-    This class can be assigned to each node of a state transition graph. Hence,
-    these settings contain the complete configuration information which is
-    required for the solution finding, e.g:
+    This class can be assigned to each node of a state transition graph. Hence, these
+    settings contain the complete configuration information which is required for the
+    solution finding, e.g:
 
       - set of conservation rules
       - mapping of rules to priorities (optional)
       - mapping of quantum numbers to their domains
       - strength scale parameter (higher value means stronger force)
     """
 
@@ -179,31 +171,27 @@
 class QNResult:
     """Defines a result to a problem set processed by the solving code."""
 
     solutions: List[QuantumNumberSolution] = field(factory=list)
     not_executed_node_rules: Dict[int, Set[str]] = field(
         factory=lambda: defaultdict(set)
     )
-    violated_node_rules: Dict[int, Set[str]] = field(
-        factory=lambda: defaultdict(set)
-    )
+    violated_node_rules: Dict[int, Set[str]] = field(factory=lambda: defaultdict(set))
     not_executed_edge_rules: Dict[int, Set[str]] = field(
         factory=lambda: defaultdict(set)
     )
-    violated_edge_rules: Dict[int, Set[str]] = field(
-        factory=lambda: defaultdict(set)
-    )
+    violated_edge_rules: Dict[int, Set[str]] = field(factory=lambda: defaultdict(set))
 
     def __attrs_post_init__(self) -> None:
-        if self.solutions and (
-            self.violated_node_rules or self.violated_edge_rules
-        ):
+        if self.solutions and (self.violated_node_rules or self.violated_edge_rules):
             raise ValueError(
-                f"Invalid {self.__class__.__name__}! Found"
-                f" {len(self.solutions)} solutions, but also violated rules.",
+                (
+                    f"Invalid {self.__class__.__name__}! Found"
+                    f" {len(self.solutions)} solutions, but also violated rules."
+                ),
                 self.violated_node_rules,
                 self.violated_edge_rules,
             )
 
     def extend(self, other_result: "QNResult") -> None:
         if self.solutions or other_result.solutions:
             self.solutions.extend(other_result.solutions)
@@ -228,100 +216,92 @@
 class Solver(ABC):
     """Interface of a Solver."""
 
     @abstractmethod
     def find_solutions(self, problem_set: QNProblemSet) -> QNResult:
         """Find solutions for the given input.
 
-        It is expected that this function determines and returns all of the
-        found solutions. In case no solutions are found a partial list of
-        violated rules has to be given. This list of violated rules does not
-        have to be complete.
+        It is expected that this function determines and returns all of the found
+        solutions. In case no solutions are found a partial list of violated rules has
+        to be given. This list of violated rules does not have to be complete.
 
         Args:
-          problem_set (`.QNProblemSet`): states a problem set
+            problem_set (`.QNProblemSet`): states a problem set
 
         Returns:
-          QNResult: contains possible solutions, violated rules and not executed
-          rules due to requirement issues.
+            QNResult: contains possible solutions, violated rules and not executed
+                rules due to requirement issues.
         """
 
 
-def _merge_particle_candidates_with_solutions(
+def _insert_allowed_states(
     solutions: List[QuantumNumberSolution],
     topology: Topology,
-    allowed_particles: List[GraphEdgePropertyMap],
+    allowed_states: Iterable[GraphEdgePropertyMap],
 ) -> List[QuantumNumberSolution]:
-    merged_solutions = []
-
-    logging.debug("merging solutions with graph...")
-    intermediate_edges = topology.intermediate_edge_ids
+    _LOGGER.debug("Inserting allowed states into QN solution graphs...")
+    substituted_graphs: List[QuantumNumberSolution] = []
     for solution in solutions:
-        current_new_solutions = [solution]
-        for int_edge_id in intermediate_edges:
-            particle_edges = __get_particle_candidates_for_state(
-                solution.edge_quantum_numbers[int_edge_id],
-                allowed_particles,
-            )
-            if len(particle_edges) == 0:
-                logging.debug("Did not find any particle candidates for")
-                logging.debug("edge id: %d", int_edge_id)
-                logging.debug("edge properties:")
-                logging.debug(solution.edge_quantum_numbers[int_edge_id])
-            new_solutions_temp = []
-            for current_new_solution in current_new_solutions:
-                for particle_edge in particle_edges:
-                    # a "shallow" copy of the nested dicts is needed
-                    new_edge_qns = {
-                        k: copy(v)
-                        for k, v in current_new_solution.edge_quantum_numbers.items()
+        current_substituted_graphs = [solution]
+        for edge_id in topology.intermediate_edge_ids:
+            incomplete_state = solution.edge_quantum_numbers[edge_id]
+            candidate_states = __get_candidate_states(incomplete_state, allowed_states)
+            if len(candidate_states) == 0:
+                message = f"Did not find any QN state candidate for edge id: {edge_id}"
+                _LOGGER.debug(message)
+                _LOGGER.debug(
+                    f"State properties: {solution.edge_quantum_numbers[edge_id]}"
+                )
+            graphs_with_candidates = []
+            for new_solution in current_substituted_graphs:
+                for candidate in candidate_states:
+                    # need "shallow" copy of the nested dicts
+                    new_states = {
+                        i: copy(s) for i, s in new_solution.edge_quantum_numbers.items()
                     }
-                    new_edge_qns[int_edge_id].update(particle_edge)
-                    temp_solution = attrs.evolve(
-                        current_new_solution,
-                        edge_quantum_numbers=new_edge_qns,
+                    new_states[edge_id].update(candidate)  # keep spin_projection
+                    graph = attrs.evolve(
+                        new_solution,
+                        edge_quantum_numbers=new_states,
                     )
-                    new_solutions_temp.append(temp_solution)
-            current_new_solutions = new_solutions_temp
+                    graphs_with_candidates.append(graph)
+            current_substituted_graphs = graphs_with_candidates
 
-        merged_solutions.extend(current_new_solutions)
+        substituted_graphs.extend(current_substituted_graphs)
 
-    return merged_solutions
+    return substituted_graphs
 
 
-def __get_particle_candidates_for_state(
+def __get_candidate_states(
     state: GraphEdgePropertyMap,
-    allowed_particles: List[GraphEdgePropertyMap],
+    allowed_states: Iterable[GraphEdgePropertyMap],
 ) -> List[GraphEdgePropertyMap]:
-    particle_edges = []
-
-    for particle_qns in allowed_particles:
-        if __is_sub_mapping(state, particle_qns):
-            particle_edges.append(particle_qns)
-
-    return particle_edges
+    candidates = []
+    for candidate in allowed_states:
+        if __is_sub_mapping(state, candidate):
+            candidates.append(candidate)
+    return candidates
 
 
 def __is_sub_mapping(
-    qn_state: GraphEdgePropertyMap, reference_qn_state: GraphEdgePropertyMap
+    state: GraphEdgePropertyMap, reference_state: GraphEdgePropertyMap
 ) -> bool:
-    for qn_type, qn_value in qn_state.items():
+    for qn_type, qn_value in state.items():
         if qn_type is EdgeQuantumNumbers.spin_projection:
             continue
-        if qn_type not in reference_qn_state:
+        if qn_type not in reference_state:
             return False
-        if qn_value != reference_qn_state[qn_type]:
+        if qn_value != reference_state[qn_type]:
             return False
-
     return True
 
 
 def validate_full_solution(problem_set: QNProblemSet) -> QNResult:
     # pylint: disable=too-many-locals
-    logging.debug("validating graph...")
+    _LOGGER.debug("validating graph...")
 
     rule_argument_handler = RuleArgumentHandler()
 
     def _create_node_variables(
         node_id: int, qn_list: Set[Type[NodeQuantumNumber]]
     ) -> Dict[Type[NodeQuantumNumber], Scalar]:
         """Create variables for the quantum numbers of the specified node."""
@@ -336,17 +316,16 @@
 
     def _create_edge_variables(
         edge_ids: Iterable[int],
         qn_list: Set[Type[EdgeQuantumNumber]],
     ) -> List[dict]:
         """Create variables for the quantum numbers of the specified edges.
 
-        Initial and final state edges just get a single domain value.
-        Intermediate edges are initialized with the default domains of that
-        quantum number.
+        Initial and final state edges just get a single domain value. Intermediate edges
+        are initialized with the default domains of that quantum number.
         """
         variables = []
         for edge_id in edge_ids:
             if edge_id in problem_set.initial_facts.edge_props:
                 edge_props = problem_set.initial_facts.edge_props[edge_id]
                 edge_vars = {}
                 for qn_type in qn_list:
@@ -355,30 +334,26 @@
                 variables.append(edge_vars)
         return variables
 
     def _create_variable_containers(
         node_id: int, cons_law: Rule
     ) -> Tuple[List[dict], List[dict], dict]:
         in_edges = problem_set.topology.get_edge_ids_ingoing_to_node(node_id)
-        out_edges = problem_set.topology.get_edge_ids_outgoing_from_node(
-            node_id
-        )
+        out_edges = problem_set.topology.get_edge_ids_outgoing_from_node(node_id)
 
         edge_qns, node_qns = get_required_qns(cons_law)
         in_edges_vars = _create_edge_variables(in_edges, edge_qns)
         out_edges_vars = _create_edge_variables(out_edges, edge_qns)
 
         node_vars = _create_node_variables(node_id, node_qns)
 
         return (in_edges_vars, out_edges_vars, node_vars)
 
     edge_violated_rules: Dict[int, Set[GraphElementRule]] = defaultdict(set)
-    edge_not_executed_rules: Dict[int, Set[GraphElementRule]] = defaultdict(
-        set
-    )
+    edge_not_executed_rules: Dict[int, Set[GraphElementRule]] = defaultdict(set)
     node_violated_rules: Dict[int, Set[Rule]] = defaultdict(set)
     node_not_executed_rules: Dict[int, Set[Rule]] = defaultdict(set)
     for (
         edge_id,
         edge_settings,
     ) in problem_set.solving_settings.edge_settings.items():
         edge_rules = edge_settings.conservation_rules
@@ -461,69 +436,57 @@
 ) -> str:
     return str(element_id) + "-" + qn_type.__name__
 
 
 @define
 class _VariableContainer:
     ingoing_edge_variables: Set[_EdgeVariableInfo] = field(factory=set)
-    fixed_ingoing_edge_variables: Dict[int, GraphEdgePropertyMap] = field(
-        factory=dict
-    )
+    fixed_ingoing_edge_variables: Dict[int, GraphEdgePropertyMap] = field(factory=dict)
     outgoing_edge_variables: Set[_EdgeVariableInfo] = field(factory=set)
-    fixed_outgoing_edge_variables: Dict[int, GraphEdgePropertyMap] = field(
-        factory=dict
-    )
+    fixed_outgoing_edge_variables: Dict[int, GraphEdgePropertyMap] = field(factory=dict)
     node_variables: Set[_NodeVariableInfo] = field(factory=set)
     fixed_node_variables: GraphNodePropertyMap = field(factory=dict)
 
 
 class CSPSolver(Solver):
     """Solver reducing the task to a Constraint Satisfaction Problem.
 
     Solving this done with the python-constraint module.
 
-    The variables are the quantum numbers of particles/edges, but also some
-    composite quantum numbers which are attributed to the interaction nodes
-    (such as angular momentum :math:`L`). The conservation rules serve as the
-    constraints and a special wrapper class serves as an adapter.
+    The variables are the quantum numbers of particles/edges, but also some composite
+    quantum numbers which are attributed to the interaction nodes (such as angular
+    momentum :math:`L`). The conservation rules serve as the constraints and a special
+    wrapper class serves as an adapter.
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(
-        self, allowed_intermediate_particles: List[GraphEdgePropertyMap]
-    ):
-        self.__variables: Set[
-            Union[_EdgeVariableInfo, _NodeVariableInfo]
-        ] = set()
+    def __init__(self, allowed_intermediate_particles: List[GraphEdgePropertyMap]):
+        self.__variables: Set[Union[_EdgeVariableInfo, _NodeVariableInfo]] = set()
         self.__var_string_to_data: Dict[
             str, Union[_EdgeVariableInfo, _NodeVariableInfo]
         ] = {}
         self.__node_rules: Dict[int, Set[Rule]] = defaultdict(set)
-        self.__non_executable_node_rules: Dict[int, Set[Rule]] = defaultdict(
-            set
-        )
+        self.__non_executable_node_rules: Dict[int, Set[Rule]] = defaultdict(set)
         self.__edge_rules: Dict[int, Set[GraphElementRule]] = defaultdict(set)
-        self.__non_executable_edge_rules: Dict[
-            int, Set[GraphElementRule]
-        ] = defaultdict(set)
+        self.__non_executable_edge_rules: Dict[int, Set[GraphElementRule]] = (
+            defaultdict(set)
+        )
         self.__problem = Problem(BacktrackingSolver(True))
         self.__allowed_intermediate_particles = allowed_intermediate_particles
         self.__scoresheet = Scoresheet()
 
     def find_solutions(self, problem_set: QNProblemSet) -> QNResult:
         # pylint: disable=too-many-locals
         self.__initialize_constraints(problem_set)
         solutions = self.__problem.getSolutions()
 
         node_not_executed_rules = self.__non_executable_node_rules
         node_not_satisfied_rules: Dict[int, Set[Rule]] = defaultdict(set)
         edge_not_executed_rules = self.__non_executable_edge_rules
-        edge_not_satisfied_rules: Dict[
-            int, Set[GraphElementRule]
-        ] = defaultdict(set)
+        edge_not_satisfied_rules: Dict[int, Set[GraphElementRule]] = defaultdict(set)
         for node_id, rules in self.__node_rules.items():
             for rule in rules:
                 if self.__scoresheet.rule_calls[(node_id, rule)] == 0:
                     node_not_executed_rules[node_id].add(rule)
                 elif self.__scoresheet.rule_passes[(node_id, rule)] == 0:
                     node_not_satisfied_rules[node_id].add(rule)
 
@@ -534,44 +497,40 @@
                 elif self.__scoresheet.rule_passes[(edge_id, rule)] == 0:
                     edge_not_satisfied_rules[edge_id].add(rule)
 
         solutions = self.__convert_solution_keys(solutions)
 
         # insert particle instances
         if self.__node_rules or self.__edge_rules:
-            full_particle_solutions = (
-                _merge_particle_candidates_with_solutions(
-                    solutions,
-                    problem_set.topology,
-                    self.__allowed_intermediate_particles,
-                )
+            selected_solutions = _insert_allowed_states(
+                solutions,
+                problem_set.topology,
+                self.__allowed_intermediate_particles,
             )
         else:
-            full_particle_solutions = [
+            selected_solutions = [
                 QuantumNumberSolution(
                     node_quantum_numbers=problem_set.initial_facts.node_props,
                     edge_quantum_numbers=problem_set.initial_facts.edge_props,
                 )
             ]
 
-        if full_particle_solutions and (
-            node_not_executed_rules or edge_not_executed_rules
-        ):
-            # rerun solver on these graphs using not executed rules
-            # and combine results
+        if selected_solutions and (node_not_executed_rules or edge_not_executed_rules):
+            # rerun solver on these graphs using not executed rules and combine results
+            topology = problem_set.topology
             result = QNResult()
-            for full_particle_solution in full_particle_solutions:
+            for full_particle_solution in selected_solutions:
                 node_props = full_particle_solution.node_quantum_numbers
                 edge_props = full_particle_solution.edge_quantum_numbers
                 node_props.update(problem_set.initial_facts.node_props)
                 edge_props.update(problem_set.initial_facts.edge_props)
                 result.extend(
                     validate_full_solution(
                         QNProblemSet(
-                            topology=problem_set.topology,
+                            topology=topology,
                             initial_facts=GraphElementProperties(
                                 node_props=node_props,
                                 edge_props=edge_props,
                             ),
                             solving_settings=GraphSettings(
                                 node_settings={
                                     i: NodeSettings(conservation_rules=rules)
@@ -584,15 +543,15 @@
                             ),
                         )
                     )
                 )
             return result
 
         return QNResult(
-            full_particle_solutions,
+            selected_solutions,
             _convert_non_executed_rules_to_names(node_not_executed_rules),
             _convert_violated_rules_to_names(node_not_satisfied_rules),
             _convert_non_executed_rules_to_names(edge_not_executed_rules),
             _convert_violated_rules_to_names(edge_not_satisfied_rules),
         )
 
     def __clear(self) -> None:
@@ -602,111 +561,101 @@
         self.__edge_rules = defaultdict(set)
         self.__problem = Problem(BacktrackingSolver(True))
         self.__scoresheet = Scoresheet()
 
     def __initialize_constraints(self, problem_set: QNProblemSet) -> None:
         """Initialize all of the constraints for this graph.
 
-        For each interaction node a set of independent constraints/conservation
-        laws are created. For each conservation law a new CSP wrapper is
-        created. This wrapper needs all of the qn numbers/variables which enter
-        or exit the node and play a role for this conservation law. Hence
-        variables are also created within this method.
+        For each interaction node a set of independent constraints/conservation laws are
+        created. For each conservation law a new CSP wrapper is created. This wrapper
+        needs all of the qn numbers/variables which enter or exit the node and play a
+        role for this conservation law. Hence variables are also created within this
+        method.
         """
         # pylint: disable=too-many-locals
 
         self.__clear()
 
         def get_rules_by_priority(
             graph_element_settings: Union[
                 NodeSettings,
                 EdgeSettings,
             ]
         ) -> List[Rule]:
             # first add priorities to the entries
             priority_list = [
-                (x, graph_element_settings.rule_priorities[type(x)])
-                if type(x) in graph_element_settings.rule_priorities
-                else (x, 1)
+                (
+                    (x, graph_element_settings.rule_priorities[type(x)])  # type: ignore[index]
+                    if type(x) in graph_element_settings.rule_priorities
+                    else (x, 1)
+                )
                 for x in graph_element_settings.conservation_rules
             ]
             # then sort according to priority
-            sorted_list = sorted(
-                priority_list, key=lambda x: x[1], reverse=True
-            )
+            sorted_list = sorted(priority_list, key=lambda x: x[1], reverse=True)
             # and strip away the priorities again
             return [x[0] for x in sorted_list]
 
         arg_handler = RuleArgumentHandler()
 
         for edge_id in problem_set.topology.edges:
             edge_settings = problem_set.solving_settings.edge_settings[edge_id]
             for rule in get_rules_by_priority(edge_settings):
                 variable_mapping = _VariableContainer()
                 # from cons law and graph determine needed var lists
                 edge_qns, node_qns = get_required_qns(rule)
 
                 edge_vars, fixed_edge_vars = self.__create_edge_variables(
-                    [
-                        edge_id,
-                    ],
+                    [edge_id],
                     edge_qns,
                     problem_set,
                 )
 
                 score_callback = self.__scoresheet.register_rule(edge_id, rule)
                 constraint = _GraphElementConstraint[EdgeQuantumNumber](
                     rule,  # type: ignore[arg-type]
                     edge_vars,
                     fixed_edge_vars,
                     arg_handler,
                     score_callback,
                 )
 
                 if edge_vars:
-                    var_strings = [
-                        _create_variable_string(*x) for x in edge_vars
-                    ]
+                    var_strings = [_create_variable_string(*x) for x in edge_vars]
                     self.__edge_rules[edge_id].add(rule)  # type: ignore[arg-type]
                     self.__problem.addConstraint(constraint, var_strings)
                 else:
                     self.__non_executable_edge_rules[edge_id].add(rule)  # type: ignore[arg-type]
 
         for node_id in problem_set.topology.nodes:
             for rule in get_rules_by_priority(
                 problem_set.solving_settings.node_settings[node_id]
             ):
                 variable_mapping = _VariableContainer()
                 # from cons law and graph determine needed var lists
                 edge_qns, node_qns = get_required_qns(rule)
 
-                in_edges = problem_set.topology.get_edge_ids_ingoing_to_node(
-                    node_id
-                )
+                in_edges = problem_set.topology.get_edge_ids_ingoing_to_node(node_id)
                 in_edge_vars = self.__create_edge_variables(
                     in_edges, edge_qns, problem_set
                 )
                 variable_mapping.ingoing_edge_variables = in_edge_vars[0]
                 variable_mapping.fixed_ingoing_edge_variables = in_edge_vars[1]
-                var_list: List[
-                    Union[_EdgeVariableInfo, _NodeVariableInfo]
-                ] = list(variable_mapping.ingoing_edge_variables)
-
-                out_edges = (
-                    problem_set.topology.get_edge_ids_outgoing_from_node(
-                        node_id
-                    )
+                var_list: List[Union[_EdgeVariableInfo, _NodeVariableInfo]] = list(
+                    variable_mapping.ingoing_edge_variables
+                )
+
+                out_edges = problem_set.topology.get_edge_ids_outgoing_from_node(
+                    node_id
                 )
                 out_edge_vars = self.__create_edge_variables(
                     out_edges, edge_qns, problem_set
                 )
                 variable_mapping.outgoing_edge_variables = out_edge_vars[0]
-                variable_mapping.fixed_outgoing_edge_variables = out_edge_vars[
-                    1
-                ]
+                variable_mapping.fixed_outgoing_edge_variables = out_edge_vars[1]
                 var_list.extend(list(variable_mapping.outgoing_edge_variables))
 
                 # now create variables for node/interaction qns
                 int_node_vars = self.__create_node_variables(
                     node_id,
                     node_qns,
                     problem_set,
@@ -725,34 +674,31 @@
                         score_callback,
                     )
                 else:
                     constraint = _ConservationRuleConstraintWrapper(
                         rule, variable_mapping, arg_handler, score_callback
                     )
                 if var_list:
-                    var_strings = [
-                        _create_variable_string(*x) for x in var_list
-                    ]
+                    var_strings = [_create_variable_string(*x) for x in var_list]
                     self.__node_rules[node_id].add(rule)
                     self.__problem.addConstraint(constraint, var_strings)
                 else:
                     self.__non_executable_node_rules[node_id].add(rule)
 
     def __create_node_variables(
         self,
         node_id: int,
         qn_list: Set[Type[NodeQuantumNumber]],
         problem_set: QNProblemSet,
     ) -> Tuple[Set[_NodeVariableInfo], GraphNodePropertyMap]:
         """Create variables for the quantum numbers of the specified node.
 
-        If a quantum number is already defined for a node, then a fixed
-        variable is created, which cannot be changed by the csp solver.
-        Otherwise the node is initialized with the specified domain of that
-        quantum number.
+        If a quantum number is already defined for a node, then a fixed variable is
+        created, which cannot be changed by the csp solver. Otherwise the node is
+        initialized with the specified domain of that quantum number.
         """
         variables: Tuple[Set[_NodeVariableInfo], GraphNodePropertyMap] = (
             set(),
             {},
         )
 
         if node_id in problem_set.initial_facts.node_props:
@@ -774,18 +720,18 @@
         self,
         edge_ids: Iterable[int],
         qn_list: Set[Type[EdgeQuantumNumber]],
         problem_set: QNProblemSet,
     ) -> Tuple[Set[_EdgeVariableInfo], Dict[int, GraphEdgePropertyMap]]:
         """Create variables for the quantum numbers of the specified edges.
 
-        If a quantum number is already defined for an edge, then a fixed
-        variable is created, which cannot be changed by the csp solver. This is
-        the case for initial and final state edges. Otherwise the edges are
-        initialized with the specified domains of that quantum number.
+        If a quantum number is already defined for an edge, then a fixed variable is
+        created, which cannot be changed by the csp solver. This is the case for initial
+        and final state edges. Otherwise the edges are initialized with the specified
+        domains of that quantum number.
         """
         variables: Tuple[
             Set[_EdgeVariableInfo],
             Dict[int, GraphEdgePropertyMap],
         ] = (
             set(),
             {},
@@ -793,21 +739,17 @@
 
         for edge_id in edge_ids:
             variables[1][edge_id] = {}
             if edge_id in problem_set.initial_facts.edge_props:
                 edge_props = problem_set.initial_facts.edge_props[edge_id]
                 for qn_type in qn_list:
                     if qn_type in edge_props:
-                        variables[1][edge_id].update(
-                            {qn_type: edge_props[qn_type]}
-                        )
+                        variables[1][edge_id].update({qn_type: edge_props[qn_type]})
             else:
-                edge_settings = problem_set.solving_settings.edge_settings[
-                    edge_id
-                ]
+                edge_settings = problem_set.solving_settings.edge_settings[edge_id]
                 for qn_type in qn_list:
                     var_info = (edge_id, qn_type)
                     if qn_type in edge_settings.qn_domains:
                         qn_domain = edge_settings.qn_domains[qn_type]
                         self.__add_variable(var_info, qn_domain)
                         variables[0].add(var_info)
         return variables
@@ -824,35 +766,27 @@
             self.__problem.addVariable(var_string, domain)
 
     def __convert_solution_keys(
         self,
         solutions: List[Dict[str, Scalar]],
     ) -> List[QuantumNumberSolution]:
         """Convert keys of CSP solutions from `str` to quantum number types."""
-        converted_solutions = []
+        converted_solutions: List[QuantumNumberSolution] = []
         for solution in solutions:
-            edge_quantum_numbers: Dict[
-                int, GraphEdgePropertyMap
-            ] = defaultdict(dict)
-            node_quantum_numbers: Dict[
-                int, GraphNodePropertyMap
-            ] = defaultdict(dict)
+            edge_quantum_numbers: Dict[int, GraphEdgePropertyMap] = defaultdict(dict)
+            node_quantum_numbers: Dict[int, GraphNodePropertyMap] = defaultdict(dict)
             for var_string, value in solution.items():
                 ele_id, qn_type = self.__var_string_to_data[var_string]
 
-                if qn_type in getattr(  # noqa: B009
-                    EdgeQuantumNumber, "__args__"
-                ):
+                if qn_type in getattr(EdgeQuantumNumber, "__args__"):  # noqa: B009
                     edge_quantum_numbers[ele_id].update({qn_type: value})  # type: ignore[dict-item]
                 else:
                     node_quantum_numbers[ele_id].update({qn_type: value})  # type: ignore[dict-item]
             converted_solutions.append(
-                QuantumNumberSolution(
-                    node_quantum_numbers, edge_quantum_numbers
-                )
+                QuantumNumberSolution(node_quantum_numbers, edge_quantum_numbers)
             )
 
         return converted_solutions
 
 
 class Scoresheet:
     def __init__(self) -> None:
@@ -882,22 +816,26 @@
         return self.__rule_calls
 
     @property
     def rule_passes(self) -> Dict[Tuple[int, Rule], int]:
         return self.__rule_passes
 
 
-_QNType = TypeVar("_QNType", EdgeQuantumNumber, NodeQuantumNumber)
+_QNType = TypeVar(  # pylint: disable=invalid-name
+    "_QNType", EdgeQuantumNumber, NodeQuantumNumber
+)
 
 
-class _GraphElementConstraint(Generic[_QNType], Constraint):
+class _GraphElementConstraint(
+    Generic[_QNType], Constraint  # pyright: ignore[reportUntypedBaseClass]
+):
     """Wrapper class of the python-constraint Constraint class.
 
-    This allows a customized definition of conservation rules, and hence a
-    cleaner user interface.
+    This allows a customized definition of conservation rules, and hence a cleaner user
+    interface.
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         rule: GraphElementRule,
         variables: Set[Tuple[int, Type[_QNType]]],
@@ -926,40 +864,39 @@
     def __initialize_variable_containers(
         self,
         variables: Set[Tuple[int, Type[_QNType]]],
         fixed_variables: Dict[int, Dict[Type[_QNType], Scalar]],
     ) -> None:
         """Fill the name decoding map.
 
-        Also initialize the in and out particle lists. The variable names
-        follow the scheme edge_id(delimiter)qn_name. This method creates a dict
-        linking the var name to a list that consists of the particle list index
-        and the qn name.
+        Also initialize the in and out particle lists. The variable names follow the
+        scheme edge_id(delimiter)qn_name. This method creates a dict linking the var
+        name to a list that consists of the particle list index and the qn name.
         """
         self.__qns.update(list(fixed_variables.values())[0])
         for element_id, qn_type in variables:
-            self.__var_string_to_data[
-                _create_variable_string(element_id, qn_type)
-            ] = qn_type
+            self.__var_string_to_data[_create_variable_string(element_id, qn_type)] = (
+                qn_type
+            )
             self.__qns.update({qn_type: None})
 
     def __call__(
         self,
         variables: Set[str],
         domains: dict,
         assignments: dict,
         forwardcheck: bool = False,
         _unassigned: Variable = Unassigned,
     ) -> bool:
         """Perform the constraint checking.
 
-        If the forwardcheck parameter is not false, besides telling if the
-        constraint is currently broken or not, the constraint implementation
-        may choose to hide values from the domains of unassigned variables to
-        prevent them from being used, and thus prune the search space.
+        If the forwardcheck parameter is not false, besides telling if the constraint is
+        currently broken or not, the constraint implementation may choose to hide values
+        from the domains of unassigned variables to prevent them from being used, and
+        thus prune the search space.
 
         Args:
             variables: Variables affected by that constraint, in the same order
                 provided by the user.
 
             domains (dict): Dictionary mapping variables to their domains.
 
@@ -969,16 +906,15 @@
             forwardcheck (bool): Boolean value stating whether forward checking
                 should be performed or not.
 
             _unassigned: Can be left empty
 
         Return:
             bool:
-                Boolean value stating if this constraint is currently broken
-                or not.
+                Boolean value stating if this constraint is currently broken or not.
         """
         params = [(x, assignments.get(x, _unassigned)) for x in variables]
         missing = [name for (name, val) in params if val is _unassigned]
         if missing:
             return True
 
         self.__update_variable_lists(params)
@@ -1006,19 +942,21 @@
                 raise ValueError(
                     "The variable with name "
                     + qn_type.__name__
                     + "does not appear in the variable mapping"
                 )
 
 
-class _ConservationRuleConstraintWrapper(Constraint):
+class _ConservationRuleConstraintWrapper(
+    Constraint  # pyright: ignore[reportUntypedBaseClass]
+):
     """Wrapper class of the python-constraint Constraint class.
 
-    This allows a customized definition of conservation rules, and hence a
-    cleaner user interface.
+    This allows a customized definition of conservation rules, and hence a cleaner user
+    interface.
     """
 
     # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
         rule: Rule,
         variables: _VariableContainer,
@@ -1040,23 +978,20 @@
         ] = {}
         self.__in_edges_qns: Dict[int, GraphEdgePropertyMap] = {}
         self.__out_edges_qns: Dict[int, GraphEdgePropertyMap] = {}
         self.__node_qns: GraphNodePropertyMap = {}
 
         self.__initialize_variable_containers(variables)
 
-    def __initialize_variable_containers(
-        self, variables: _VariableContainer
-    ) -> None:
+    def __initialize_variable_containers(self, variables: _VariableContainer) -> None:
         """Fill the name decoding map.
 
-        Also initialize the in and out particle lists. The variable names
-        follow the scheme edge_id(delimiter)qn_name. This method creates a dict
-        linking the var name to a list that consists of the particle list index
-        and the qn name.
+        Also initialize the in and out particle lists. The variable names follow the
+        scheme edge_id(delimiter)qn_name. This method creates a dict linking the var
+        name to a list that consists of the particle list index and the qn name.
         """
 
         def _initialize_edge_container(
             variable_set: Set[_EdgeVariableInfo],
             fixed_variables: Dict[int, Dict[Type[EdgeQuantumNumber], Scalar]],
             container: Dict[int, GraphEdgePropertyMap],
         ) -> None:
@@ -1078,33 +1013,31 @@
             variables.outgoing_edge_variables,
             variables.fixed_outgoing_edge_variables,
             self.__out_edges_qns,
         )
         # and now interaction node variables
         for var_info in variables.node_variables:
             self.__node_qns[var_info[1]] = None  # type: ignore[assignment]
-            self.__var_string_to_data[
-                _create_variable_string(*var_info)
-            ] = var_info
+            self.__var_string_to_data[_create_variable_string(*var_info)] = var_info
         self.__node_qns.update(variables.fixed_node_variables)
 
     def __call__(
         self,
         variables: Set[str],
         domains: dict,
         assignments: dict,
         forwardcheck: bool = False,
         _unassigned: Variable = Unassigned,
     ) -> bool:
         """Perform the constraint checking.
 
-        If the forwardcheck parameter is not false, besides telling if the
-        constraint is currently broken or not, the constraint implementation
-        may choose to hide values from the domains of unassigned variables to
-        prevent them from being used, and thus prune the search space.
+        If the forwardcheck parameter is not false, besides telling if the constraint is
+        currently broken or not, the constraint implementation may choose to hide values
+        from the domains of unassigned variables to prevent them from being used, and
+        thus prune the search space.
 
         Args:
             variables: Variables affected by that constraint, in the same order
                 provided by the user.
 
             domains (dict): Dictionary mapping variables to their domains.
 
@@ -1114,16 +1047,15 @@
             forwardcheck (bool): Boolean value stating whether forward checking
                 should be performed or not.
 
             _unassigned: Can be left empty
 
         Return:
             bool:
-                Boolean value stating if this constraint is currently broken
-                or not.
+                Boolean value stating if this constraint is currently broken or not.
         """
         params = [(x, assignments.get(x, _unassigned)) for x in variables]
         missing = [name for (name, val) in params if val is _unassigned]
         if missing:
             return True
 
         self.__update_variable_lists(params)
@@ -1147,22 +1079,18 @@
 
     def __update_variable_lists(
         self,
         parameters: List[Tuple[str, Any]],
     ) -> None:
         for var_string, value in parameters:
             index, qn_type = self.__var_string_to_data[var_string]
-            if (
-                index in self.__in_edges_qns
-                and qn_type in self.__in_edges_qns[index]
-            ):
+            if index in self.__in_edges_qns and qn_type in self.__in_edges_qns[index]:
                 self.__in_edges_qns[index][qn_type] = value  # type: ignore[index]
             elif (
-                index in self.__out_edges_qns
-                and qn_type in self.__out_edges_qns[index]
+                index in self.__out_edges_qns and qn_type in self.__out_edges_qns[index]
             ):
                 self.__out_edges_qns[index][qn_type] = value  # type: ignore[index]
             elif qn_type in self.__node_qns:
                 self.__node_qns[qn_type] = value  # type: ignore[index]
             else:
                 raise ValueError(
                     f"The variable with name {qn_type.__name__} and a graph"
```

### Comparing `qrules-0.9.7/src/qrules/topology.py` & `qrules-0.9.8/src/qrules/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,26 @@
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
     from typing_extensions import Protocol
 
 if TYPE_CHECKING:
-    try:
-        from IPython.lib.pretty import PrettyPrinter
-    except ImportError:
-        PrettyPrinter = Any
+    from IPython.lib.pretty import PrettyPrinter
+
+_LOGGER = logging.getLogger(__name__)
 
 
 class Comparable(Protocol):
     @abstractmethod
     def __lt__(self, other: Any) -> bool:
         ...
 
 
+# pylint: disable=invalid-name
 KeyType = TypeVar("KeyType", bound=Comparable)
 """Type the keys of the `~typing.Mapping`, see `~typing.KeysView`."""
 ValueType = TypeVar("ValueType")
 """Type the value of the `~typing.Mapping`, see `~typing.ValuesView`."""
 
 
 @total_ordering
@@ -91,15 +91,15 @@
         if cycle:
             p.text(f"{class_name}(...)")
         else:
             with p.group(indent=2, open=f"{class_name}({{"):
                 for key, value in self.items():
                     p.breakable()
                     p.text(f"{key}: ")
-                    p.pretty(value)
+                    p.pretty(value)  # type: ignore[attr-defined]
                     p.text(",")
             p.breakable()
             p.text("})")
 
     def __iter__(self) -> Iterator[KeyType]:
         return iter(self.__mapping)
 
@@ -145,43 +145,38 @@
     return int(optional_int)
 
 
 @frozen(order=True)
 class Edge:
     """Struct-like definition of an edge, used in `Topology`."""
 
-    originating_node_id: Optional[int] = field(
-        default=None, converter=_to_optional_int
-    )
-    ending_node_id: Optional[int] = field(
-        default=None, converter=_to_optional_int
-    )
+    originating_node_id: Optional[int] = field(default=None, converter=_to_optional_int)
+    ending_node_id: Optional[int] = field(default=None, converter=_to_optional_int)
 
     def get_connected_nodes(self) -> Set[int]:
         connected_nodes = {self.ending_node_id, self.originating_node_id}
         connected_nodes.discard(None)
         return connected_nodes  # type: ignore[return-value]
 
 
 def _to_frozenset(iterable: Iterable[int]) -> FrozenSet[int]:
-    if not all(map(lambda i: isinstance(i, int), iterable)):
+    if any(not isinstance(i, int) for i in iterable):
         raise TypeError(f"Not all items in {iterable} are of type int")
     return frozenset(iterable)
 
 
 @implement_pretty_repr
 @frozen(order=True)
 class Topology:
     """Directed Feynman-like graph without edge or node properties.
 
-    Forms the underlying topology of `StateTransitionGraph`. The graphs are
-    directed, meaning the edges are ingoing and outgoing to specific nodes
-    (since feynman graphs also have a time axis). Note that a `Topology` is not
-    strictly speaking a graph from graph theory, because it allows open edges,
-    like a Feynman-diagram.
+    Forms the underlying topology of `StateTransitionGraph`. The graphs are directed,
+    meaning the edges are ingoing and outgoing to specific nodes (since feynman graphs
+    also have a time axis). Note that a `Topology` is not strictly speaking a graph from
+    graph theory, because it allows open edges, like a Feynman-diagram.
     """
 
     nodes: FrozenSet[int] = field(converter=_to_frozenset)
     edges: FrozenDict[int, Edge] = field(converter=FrozenDict)
 
     incoming_edge_ids: FrozenSet[int] = field(init=False, repr=False)
     outgoing_edge_ids: FrozenSet[int] = field(init=False, repr=False)
@@ -206,59 +201,54 @@
                 for edge_id, edge in self.edges.items()
                 if edge.ending_node_id is None
             ),
         )
         object.__setattr__(
             self,
             "intermediate_edge_ids",
-            frozenset(self.edges)
-            ^ self.incoming_edge_ids
-            ^ self.outgoing_edge_ids,
+            frozenset(self.edges) ^ self.incoming_edge_ids ^ self.outgoing_edge_ids,
         )
 
     def __verify(self) -> None:
         """Verify if there are no dangling edges or nodes."""
         for edge_id, edge in self.edges.items():
             connected_nodes = edge.get_connected_nodes()
             if not connected_nodes:
                 raise ValueError(
-                    f"Edge nr. {edge_id} is not connected to any other node"
-                    f" ({edge})"
+                    f"Edge nr. {edge_id} is not connected to any other node ({edge})"
                 )
             if not connected_nodes <= self.nodes:
                 raise ValueError(
                     f"{edge} (ID: {edge_id}) has non-existing node IDs.\n"
                     f"Available node IDs: {self.nodes}"
                 )
         self.__check_isolated_nodes()
 
     def __check_isolated_nodes(self) -> None:
         if len(self.nodes) < 2:
             return
         for node_id in self.nodes:
             surrounding_nodes = self.__get_surrounding_nodes(node_id)
             if not surrounding_nodes:
-                raise ValueError(
-                    f"Node {node_id} is not connected to any other node"
-                )
+                raise ValueError(f"Node {node_id} is not connected to any other node")
 
     def __get_surrounding_nodes(self, node_id: int) -> Set[int]:
         surrounding_nodes = set()
         for edge in self.edges.values():
             connected_nodes = edge.get_connected_nodes()
             if node_id in connected_nodes:
                 surrounding_nodes |= connected_nodes
         surrounding_nodes.discard(node_id)
         return surrounding_nodes
 
     def is_isomorphic(self, other: "Topology") -> bool:
         """Check if two graphs are isomorphic.
 
-        Returns `True` if the two graphs have a one-to-one mapping of the node
-        IDs and edge IDs.
+        Returns `True` if the two graphs have a one-to-one mapping of the node IDs and
+        edge IDs.
         """
         raise NotImplementedError
 
     def get_edge_ids_ingoing_to_node(self, node_id: int) -> Set[int]:
         return {
             edge_id
             for edge_id, edge in self.edges.items()
@@ -329,55 +319,48 @@
         )
         old_to_new_id = {j: i for i, j in new_to_old_id}
         return self.relabel_edges(old_to_new_id)
 
     def relabel_edges(self, old_to_new_id: Mapping[int, int]) -> "Topology":
         """Create a new `Topology` with new edge IDs.
 
-        This method is particularly useful when creating permutations of a
-        `Topology`, e.g.:
+        This method is particularly useful when creating permutations of a `Topology`,
+        e.g.:
 
         >>> topologies = create_isobar_topologies(3)
         >>> len(topologies)
         1
         >>> topology = topologies[0]
         >>> final_state_ids = topology.outgoing_edge_ids
         >>> permuted_topologies = {
         ...     topology.relabel_edges(dict(zip(final_state_ids, permutation)))
         ...     for permutation in itertools.permutations(final_state_ids)
         ... }
         >>> len(permuted_topologies)
         3
         """
-        new_edges = {
-            old_to_new_id.get(i, i): edge for i, edge in self.edges.items()
-        }
+        new_edges = {old_to_new_id.get(i, i): edge for i, edge in self.edges.items()}
         return attrs.evolve(self, edges=new_edges)
 
     def swap_edges(self, edge_id1: int, edge_id2: int) -> "Topology":
         return self.relabel_edges({edge_id1: edge_id2, edge_id2: edge_id1})
 
 
-def get_originating_node_list(
-    topology: Topology, edge_ids: Iterable[int]
-) -> List[int]:
+def get_originating_node_list(topology: Topology, edge_ids: Iterable[int]) -> List[int]:
     """Get list of node ids from which the supplied edges originate from.
 
     Args:
         topology: The `Topology` on which to perform the search.
-        edge_ids ([int]): A list of edge ids for which the origin node is
-            searched for.
+        edge_ids ([int]): A list of edge ids for which the origin node is searched for.
     """
 
     def __get_originating_node(edge_id: int) -> Optional[int]:
         return topology.edges[edge_id].originating_node_id
 
-    return [
-        node_id for node_id in map(__get_originating_node, edge_ids) if node_id
-    ]
+    return [node_id for node_id in map(__get_originating_node, edge_ids) if node_id]
 
 
 @define(kw_only=True)
 class _MutableTopology:
     edges: Dict[int, Edge] = field(factory=dict, converter=dict)
     nodes: Set[int] = field(factory=set, converter=set)
 
@@ -464,51 +447,42 @@
     """Helper class for the `.SimpleStateTransitionTopologyBuilder`."""
 
     number_of_ingoing_edges: int = field(validator=instance_of(int))
     number_of_outgoing_edges: int = field(validator=instance_of(int))
 
     def __attrs_post_init__(self) -> None:
         if self.number_of_ingoing_edges < 1:
-            raise ValueError(
-                "Number of incoming edges has to be larger than 0"
-            )
+            raise ValueError("Number of incoming edges has to be larger than 0")
         if self.number_of_outgoing_edges < 1:
-            raise ValueError(
-                "Number of outgoing edges has to be larger than 0"
-            )
+            raise ValueError("Number of outgoing edges has to be larger than 0")
 
 
 class SimpleStateTransitionTopologyBuilder:
     """Simple topology builder.
 
-    Recursively tries to add the interaction nodes to available open end
-    edges/lines in all combinations until the number of open end lines matches
-    the final state lines.
+    Recursively tries to add the interaction nodes to available open end edges/lines in
+    all combinations until the number of open end lines matches the final state lines.
     """
 
-    def __init__(
-        self, interaction_node_set: Iterable[InteractionNode]
-    ) -> None:
+    def __init__(self, interaction_node_set: Iterable[InteractionNode]) -> None:
         if not isinstance(interaction_node_set, list):
             raise TypeError("interaction_node_set must be a list")
-        self.interaction_node_set: List[InteractionNode] = list(
-            interaction_node_set
-        )
+        self.interaction_node_set: List[InteractionNode] = list(interaction_node_set)
 
     def build(
         self, number_of_initial_edges: int, number_of_final_edges: int
     ) -> Tuple[Topology, ...]:
         number_of_initial_edges = int(number_of_initial_edges)
         number_of_final_edges = int(number_of_final_edges)
         if number_of_initial_edges < 1:
             raise ValueError("number_of_initial_edges has to be larger than 0")
         if number_of_final_edges < 1:
             raise ValueError("number_of_final_edges has to be larger than 0")
 
-        logging.info("building topology graphs...")
+        _LOGGER.info("building topology graphs...")
         # result list
         graph_tuple_list: List[Tuple[_MutableTopology, List[int]]] = []
         # create seed graph
         seed_graph = _MutableTopology()
         current_open_end_edges = list(range(number_of_initial_edges))
         seed_graph.add_edges(current_open_end_edges)
         extendable_graph_list: List[Tuple[_MutableTopology, List[int]]] = [
@@ -526,15 +500,15 @@
                 ):
                     active_graph[0].freeze()  # verify
                     graph_tuple_list.append(active_graph)
                     continue
 
                 extendable_graph_list.extend(self._extend_graph(active_graph))
 
-        logging.info("finished building topology graphs...")
+        _LOGGER.info("finished building topology graphs...")
         # strip the current open end edges list from the result graph tuples
         topologies = []
         for graph_tuple in graph_tuple_list:
             topology = graph_tuple[0].freeze()
             topology = topology.organize_edge_ids()
             topologies.append(topology)
         return tuple(topologies)
@@ -545,17 +519,15 @@
         extended_graph_list: List[Tuple[_MutableTopology, List[int]]] = []
 
         topology, current_open_end_edges = pair
 
         # Try to extend the graph with interaction nodes
         # that have equal or less ingoing lines than active lines
         for interaction_node in self.interaction_node_set:
-            if interaction_node.number_of_ingoing_edges <= len(
-                current_open_end_edges
-            ):
+            if interaction_node.number_of_ingoing_edges <= len(current_open_end_edges):
                 # make all combinations
                 combis = list(
                     itertools.combinations(
                         current_open_end_edges,
                         interaction_node.number_of_ingoing_edges,
                     )
                 )
@@ -565,29 +537,25 @@
                         topology, comb1  # type: ignore[arg-type]
                     ) == get_originating_node_list(
                         topology, comb2  # type: ignore[arg-type]
                     ):  # type: ignore[arg-type]
                         combis.remove(comb2)
 
                 for combi in combis:
-                    new_graph = _attach_node_to_edges(
-                        pair, interaction_node, combi
-                    )
+                    new_graph = _attach_node_to_edges(pair, interaction_node, combi)
                     extended_graph_list.append(new_graph)
 
         return extended_graph_list
 
 
 def create_isobar_topologies(
     number_of_final_states: int,
 ) -> Tuple[Topology, ...]:
     if number_of_final_states < 2:
-        raise ValueError(
-            "At least two final states required for an isobar decay"
-        )
+        raise ValueError("At least two final states required for an isobar decay")
     builder = SimpleStateTransitionTopologyBuilder([InteractionNode(1, 2)])
     topologies = builder.build(
         number_of_initial_edges=1,
         number_of_final_edges=number_of_final_states,
     )
     return tuple(topologies)
 
@@ -655,18 +623,18 @@
 EdgeType = TypeVar("EdgeType")
 """A `~typing.TypeVar` representing the type of edge properties."""
 
 
 class StateTransitionGraph(Generic[EdgeType]):
     """Graph class that resembles a frozen `.Topology` with properties.
 
-    This class should contain the full information of a state transition from a
-    initial state to a final state. This information can be attached to the
-    nodes and edges via properties. In case not all information is provided,
-    error can be raised on property retrieval.
+    This class should contain the full information of a state transition from a initial
+    state to a final state. This information can be attached to the nodes and edges via
+    properties. In case not all information is provided, error can be raised on property
+    retrieval.
     """
 
     def __init__(
         self,
         topology: Topology,
         node_props: Mapping[int, InteractionProperties],
         edge_props: Mapping[int, EdgeType],
@@ -690,16 +658,15 @@
                 if self.get_edge_props(i) != other.get_edge_props(i):
                     return False
             for i in self.topology.nodes:
                 if self.get_node_props(i) != other.get_node_props(i):
                     return False
             return True
         raise NotImplementedError(
-            f"Cannot compare {self.__class__.__name__}"
-            f" with {other.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with {other.__class__.__name__}"
         )
 
     def get_node_props(self, node_id: int) -> InteractionProperties:
         return self.__node_props[node_id]
 
     def get_edge_props(self, edge_id: int) -> EdgeType:
         return self.__edge_props[edge_id]
@@ -707,16 +674,16 @@
     def evolve(
         self,
         node_props: Optional[Dict[int, InteractionProperties]] = None,
         edge_props: Optional[Dict[int, EdgeType]] = None,
     ) -> "StateTransitionGraph[EdgeType]":
         """Changes the node and edge properties of a graph instance.
 
-        Since a `.StateTransitionGraph` is frozen (cannot be modified), the
-        evolve function will also create a shallow copy the properties.
+        Since a `.StateTransitionGraph` is frozen (cannot be modified), the evolve
+        function will also create a shallow copy the properties.
         """
         new_node_props = copy.copy(self.__node_props)
         if node_props:
             _assert_over_defined(self.topology.nodes, node_props)
             for node_id, node_prop in node_props.items():
                 new_node_props[node_id] = node_prop
 
@@ -740,23 +707,19 @@
             Callable[[InteractionProperties, InteractionProperties], bool]
         ] = None,
     ) -> bool:
         if self.topology != other.topology:
             return False
         if edge_comparator is not None:
             for i in self.topology.edges:
-                if not edge_comparator(
-                    self.get_edge_props(i), other.get_edge_props(i)
-                ):
+                if not edge_comparator(self.get_edge_props(i), other.get_edge_props(i)):
                     return False
         if node_comparator is not None:
             for i in self.topology.nodes:
-                if not node_comparator(
-                    self.get_node_props(i), other.get_node_props(i)
-                ):
+                if not node_comparator(self.get_node_props(i), other.get_node_props(i)):
                     return False
         return True
 
     def swap_edges(self, edge_id1: int, edge_id2: int) -> None:
         self.topology = self.topology.swap_edges(edge_id1, edge_id2)
         value1: Optional[EdgeType] = None
         value2: Optional[EdgeType] = None
```

### Comparing `qrules-0.9.7/src/qrules/transition.py` & `qrules-0.9.8/src/qrules/transition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=too-many-lines
 """Find allowed transitions between an initial and final state."""
 
 import logging
+import re
 from collections import abc, defaultdict
 from copy import copy, deepcopy
 from enum import Enum, auto
 from itertools import zip_longest
 from multiprocessing import Pool
 from typing import (
     TYPE_CHECKING,
@@ -36,23 +37,25 @@
 from ._system_control import (
     GammaCheck,
     InteractionDeterminator,
     LeptonCheck,
     create_edge_properties,
     create_interaction_properties,
     create_node_properties,
-    create_particle,
     filter_interaction_types,
+    find_particle,
     remove_duplicate_solutions,
 )
 from .combinatorics import (
     InitialFacts,
     StateDefinition,
     create_initial_facts,
+    ensure_nested_list,
     match_external_edges,
+    permutate_topology_kinematically,
 )
 from .particle import (
     Particle,
     ParticleCollection,
     ParticleWithSpin,
     _to_float,
     load_pdg,
@@ -61,14 +64,15 @@
     EdgeQuantumNumber,
     EdgeQuantumNumbers,
     InteractionProperties,
     NodeQuantumNumber,
     NodeQuantumNumbers,
 )
 from .settings import (
+    DEFAULT_INTERACTION_TYPES,
     InteractionType,
     NumberOfThreads,
     create_interaction_settings,
 )
 from .solving import (
     CSPSolver,
     EdgeSettings,
@@ -87,15 +91,17 @@
     create_n_body_topology,
 )
 
 if TYPE_CHECKING:
     try:
         from IPython.lib.pretty import PrettyPrinter
     except ImportError:
-        PrettyPrinter = Any
+        PrettyPrinter = Any  # type: ignore[assignment,misc]
+
+_LOGGER = logging.getLogger(__name__)
 
 
 class SolvingMode(Enum):
     """Types of modes for solving."""
 
     FAST = auto()
     """Find "likeliest" solutions only."""
@@ -105,23 +111,19 @@
 
 @implement_pretty_repr
 @define(on_setattr=attrs.setters.frozen)
 class ExecutionInfo:
     not_executed_node_rules: Dict[int, Set[str]] = field(
         factory=lambda: defaultdict(set)
     )
-    violated_node_rules: Dict[int, Set[str]] = field(
-        factory=lambda: defaultdict(set)
-    )
+    violated_node_rules: Dict[int, Set[str]] = field(factory=lambda: defaultdict(set))
     not_executed_edge_rules: Dict[int, Set[str]] = field(
         factory=lambda: defaultdict(set)
     )
-    violated_edge_rules: Dict[int, Set[str]] = field(
-        factory=lambda: defaultdict(set)
-    )
+    violated_edge_rules: Dict[int, Set[str]] = field(factory=lambda: defaultdict(set))
 
     def extend(
         self, other_result: "ExecutionInfo", intersect_violations: bool = False
     ) -> None:
         for key, rules in other_result.not_executed_node_rules.items():
             self.not_executed_node_rules[key].update(rules)
 
@@ -147,41 +149,39 @@
         self.violated_edge_rules.clear()
 
 
 @frozen
 class _SolutionContainer:
     """Defines a result of a `.ProblemSet`."""
 
-    solutions: List[StateTransitionGraph[ParticleWithSpin]] = field(
-        factory=list
-    )
+    solutions: List[StateTransitionGraph[ParticleWithSpin]] = field(factory=list)
     execution_info: ExecutionInfo = field(default=ExecutionInfo())
 
     def __attrs_post_init__(self) -> None:
         if self.solutions and (
             self.execution_info.violated_node_rules
             or self.execution_info.violated_edge_rules
         ):
             raise ValueError(
-                f"Invalid {self.__class__.__name__}! Found"
-                f" {len(self.solutions)} solutions, but also violated rules.",
+                (
+                    f"Invalid {self.__class__.__name__}! Found"
+                    f" {len(self.solutions)} solutions, but also violated rules."
+                ),
                 self.execution_info.violated_node_rules,
                 self.execution_info.violated_edge_rules,
             )
 
     def extend(
         self, other: "_SolutionContainer", intersect_violations: bool = False
     ) -> None:
         if self.solutions or other.solutions:
             self.solutions.extend(other.solutions)
             self.execution_info.clear()
         else:
-            self.execution_info.extend(
-                other.execution_info, intersect_violations
-            )
+            self.execution_info.extend(other.execution_info, intersect_violations)
 
 
 @implement_pretty_repr
 @define
 class ProblemSet:
     """Particle reaction problem set, defined as a graph like data structure.
 
@@ -214,29 +214,23 @@
             solving_settings=self.solving_settings,
         )
 
 
 def _group_by_strength(
     problem_sets: List[ProblemSet],
 ) -> Dict[float, List[ProblemSet]]:
-    def calculate_strength(
-        node_interaction_settings: Dict[int, NodeSettings]
-    ) -> float:
+    def calculate_strength(node_interaction_settings: Dict[int, NodeSettings]) -> float:
         strength = 1.0
         for int_setting in node_interaction_settings.values():
             strength *= int_setting.interaction_strength
         return strength
 
-    strength_sorted_problem_sets: Dict[float, List[ProblemSet]] = defaultdict(
-        list
-    )
+    strength_sorted_problem_sets: Dict[float, List[ProblemSet]] = defaultdict(list)
     for problem_set in problem_sets:
-        strength = calculate_strength(
-            problem_set.solving_settings.node_settings
-        )
+        strength = calculate_strength(problem_set.solving_settings.node_settings)
         strength_sorted_problem_sets[strength].append(problem_set)
     return strength_sorted_problem_sets
 
 
 class StateTransitionManager:  # pylint: disable=too-many-instance-attributes
     """Main handler for decay topologies.
 
@@ -247,15 +241,15 @@
         self,
         initial_state: Sequence[StateDefinition],
         final_state: Sequence[StateDefinition],
         particle_db: Optional[ParticleCollection] = None,
         allowed_intermediate_particles: Optional[List[str]] = None,
         interaction_type_settings: Dict[
             InteractionType, Tuple[EdgeSettings, NodeSettings]
-        ] = None,
+        ] = None,  # type: ignore[assignment]
         formalism: str = "helicity",
         topology_building: str = "isobar",
         solving_mode: SolvingMode = SolvingMode.FAST,
         reload_pdg: bool = False,
         mass_conservation_factor: Optional[float] = 3.0,
         max_angular_momentum: int = 1,
         max_spin_magnitude: float = 2.0,
@@ -277,28 +271,27 @@
                 f" Use one of {allowed_formalisms} instead."
             )
         self.__formalism = str(formalism)
         self.__particles = ParticleCollection()
         if particle_db is not None:
             self.__particles = particle_db
         self.reaction_mode = str(solving_mode)
-        self.initial_state = initial_state
-        self.final_state = final_state
+        self.initial_state = list(initial_state)
+        self.final_state = list(final_state)
         self.interaction_type_settings = interaction_type_settings
 
         self.interaction_determinators: List[InteractionDeterminator] = [
             LeptonCheck(),
             GammaCheck(),
         ]
         self.final_state_groupings: Optional[List[List[List[str]]]] = None
-        self.allowed_interaction_types: List[InteractionType] = [
-            InteractionType.STRONG,
-            InteractionType.EM,
-            InteractionType.WEAK,
-        ]
+        self.__allowed_interaction_types: Union[
+            List[InteractionType],
+            Dict[int, List[InteractionType]],
+        ] = DEFAULT_INTERACTION_TYPES
         self.filter_remove_qns: Set[Type[NodeQuantumNumber]] = set()
         self.filter_ignore_qns: Set[Type[NodeQuantumNumber]] = set()
         if formalism == "helicity":
             self.filter_remove_qns = {
                 NodeQuantumNumbers.l_magnitude,
                 NodeQuantumNumbers.l_projection,
                 NodeQuantumNumbers.s_magnitude,
@@ -332,197 +325,196 @@
                 particle_db=self.__particles,
                 nbody_topology=use_nbody_topology,
                 mass_conservation_factor=mass_conservation_factor,
                 max_angular_momentum=max_angular_momentum,
                 max_spin_magnitude=max_spin_magnitude,
             )
 
-        self.__user_allowed_intermediate_particles = (
-            allowed_intermediate_particles
-        )
-        self.__allowed_intermediate_particles: List[GraphEdgePropertyMap] = []
-        if allowed_intermediate_particles is not None:
-            self.set_allowed_intermediate_particles(
-                allowed_intermediate_particles
-            )
-        else:
-            self.__allowed_intermediate_particles = [
+        self.__intermediate_particle_filters = allowed_intermediate_particles
+        if allowed_intermediate_particles is None:
+            self.__allowed_intermediate_states: List[GraphEdgePropertyMap] = [
                 create_edge_properties(x) for x in self.__particles
             ]
+        else:
+            self.set_allowed_intermediate_particles(allowed_intermediate_particles)
 
     def set_allowed_intermediate_particles(
-        self, particle_names: List[str]
+        self, name_patterns: Union[Iterable[str], str], regex: bool = False
     ) -> None:
-        self.__allowed_intermediate_particles = []
-        for particle_name in particle_names:
-            matches = self.__particles.filter(
-                lambda p: particle_name  # pylint: disable=cell-var-from-loop
-                in p.name
-            )
+        if isinstance(name_patterns, str):
+            name_patterns = [name_patterns]
+        selected_particles = ParticleCollection()
+        for pattern in name_patterns:
+            # pylint: disable=cell-var-from-loop
+            matches = _filter_by_name_pattern(self.__particles, pattern, regex)
             if len(matches) == 0:
                 raise LookupError(
                     "Could not find any matches for allowed intermediate"
-                    f' particle "{particle_name}"'
+                    f' particle pattern "{pattern}"'
                 )
-            self.__allowed_intermediate_particles += [
-                create_edge_properties(x) for x in matches
-            ]
+            selected_particles.update(matches)
+        self.__allowed_intermediate_states = [
+            create_edge_properties(x)
+            for x in sorted(selected_particles, key=lambda p: p.name)
+        ]
 
     @property
     def formalism(self) -> str:
         return self.__formalism
 
     def add_final_state_grouping(
         self, fs_group: Union[List[str], List[List[str]]]
     ) -> None:
         if not isinstance(fs_group, list):
-            raise ValueError(
-                "The final state grouping has to be of type list."
-            )
+            raise ValueError("The final state grouping has to be of type list.")
         if len(fs_group) > 0:
             if self.final_state_groupings is None:
                 self.final_state_groupings = []
-            nested_list = _safe_wrap_list(fs_group)
+            nested_list = ensure_nested_list(fs_group)
             self.final_state_groupings.append(nested_list)
 
+    @overload
+    def get_allowed_interaction_types(
+        self,
+    ) -> Union[List[InteractionType], Dict[int, List[InteractionType]]]:
+        ...
+
+    @overload
+    def get_allowed_interaction_types(self, node_id: int) -> List[InteractionType]:
+        ...
+
+    def get_allowed_interaction_types(self, node_id=None):  # type: ignore[no-untyped-def]
+        if node_id is None:
+            return self.__allowed_interaction_types
+        if isinstance(self.__allowed_interaction_types, list):
+            return self.__allowed_interaction_types
+        return self.__allowed_interaction_types.get(node_id, DEFAULT_INTERACTION_TYPES)
+
     def set_allowed_interaction_types(
-        self, allowed_interaction_types: Iterable[InteractionType]
+        self,
+        allowed_interaction_types: Iterable[InteractionType],
+        node_id: Optional[int] = None,
     ) -> None:
         # verify order
         for allowed_types in allowed_interaction_types:
             if not isinstance(allowed_types, InteractionType):
                 raise TypeError(
-                    "allowed interaction types must be of type"
-                    "[InteractionType]"
+                    "Allowed interaction types must be of type[InteractionType]"
                 )
             if allowed_types not in self.interaction_type_settings:
-                logging.info(self.interaction_type_settings.keys())
-                raise ValueError(
-                    f"interaction {allowed_types} not found in settings"
-                )
-        self.allowed_interaction_types = list(allowed_interaction_types)
+                _LOGGER.info(self.interaction_type_settings.keys())
+                raise ValueError(f"Interaction {allowed_types} not found in settings")
+        allowed_interaction_types = list(allowed_interaction_types)
+        if node_id is None:
+            self.__allowed_interaction_types = allowed_interaction_types
+        else:
+            if not isinstance(self.__allowed_interaction_types, dict):
+                self.__allowed_interaction_types = {}
+            self.__allowed_interaction_types[node_id] = allowed_interaction_types
 
     def create_problem_sets(self) -> Dict[float, List[ProblemSet]]:
-        problem_sets = []
-        for topology in self.topologies:
+        problem_sets = [
+            ProblemSet(permutation, initial_facts, settings)
             for initial_facts in create_initial_facts(
-                topology=topology,
-                particle_db=self.__particles,
-                initial_state=self.initial_state,
-                final_state=self.final_state,
-                final_state_groupings=self.final_state_groupings,
-            ):
-                problem_sets.extend(
-                    [
-                        ProblemSet(
-                            topology=topology,
-                            initial_facts=initial_facts,
-                            solving_settings=x,
-                        )
-                        for x in self.__determine_graph_settings(
-                            topology, initial_facts
-                        )
-                    ]
-                )
-        # create groups of settings ordered by "probability"
+                self.initial_state, self.final_state, self.__particles
+            )
+            for topology in self.topologies
+            for permutation in permutate_topology_kinematically(
+                topology,
+                self.initial_state,
+                self.final_state,
+                self.final_state_groupings,
+            )
+            for settings in self.__determine_graph_settings(permutation, initial_facts)
+        ]
         return _group_by_strength(problem_sets)
 
     def __determine_graph_settings(
         self, topology: Topology, initial_facts: InitialFacts
     ) -> List[GraphSettings]:
         # pylint: disable=too-many-locals
+        weak_edge_settings, _ = self.interaction_type_settings[InteractionType.WEAK]
+
         def create_intermediate_edge_qn_domains() -> Dict:
+            if self.__intermediate_particle_filters is None:
+                return weak_edge_settings.qn_domains
+
             # if a list of intermediate states is given by user,
             # built a domain based on these states
-            if self.__user_allowed_intermediate_particles:
-                intermediate_edge_domains: Dict[
-                    Type[EdgeQuantumNumber], Set
-                ] = defaultdict(set)
-                intermediate_edge_domains[
-                    EdgeQuantumNumbers.spin_projection
-                ].update(
-                    self.interaction_type_settings[InteractionType.WEAK][
-                        0
-                    ].qn_domains[EdgeQuantumNumbers.spin_projection]
-                )
-                for particle_props in self.__allowed_intermediate_particles:
-                    for edge_qn, qn_value in particle_props.items():
-                        intermediate_edge_domains[edge_qn].add(qn_value)
-
-                return {
-                    k: list(v)
-                    for k, v in intermediate_edge_domains.items()
-                    if k is not EdgeQuantumNumbers.pid
-                    and k is not EdgeQuantumNumbers.mass
-                    and k is not EdgeQuantumNumbers.width
-                }
+            intermediate_edge_domains: Dict[Type[EdgeQuantumNumber], Set] = defaultdict(
+                set
+            )
+            intermediate_edge_domains[EdgeQuantumNumbers.spin_projection].update(
+                weak_edge_settings.qn_domains[EdgeQuantumNumbers.spin_projection]
+            )
+            for particle_props in self.__allowed_intermediate_states:
+                for edge_qn, qn_value in particle_props.items():
+                    if edge_qn in {
+                        EdgeQuantumNumbers.pid,
+                        EdgeQuantumNumbers.mass,
+                        EdgeQuantumNumbers.width,
+                    }:
+                        continue
+                    intermediate_edge_domains[edge_qn].add(qn_value)
 
-            return self.interaction_type_settings[InteractionType.WEAK][
-                0
-            ].qn_domains
+            return {k: list(v) for k, v in intermediate_edge_domains.items()}
 
         intermediate_state_edges = topology.intermediate_edge_ids
         int_edge_domains = create_intermediate_edge_qn_domains()
 
         def create_edge_settings(edge_id: int) -> EdgeSettings:
-            settings = copy(
-                self.interaction_type_settings[InteractionType.WEAK][0]
-            )
+            settings = copy(weak_edge_settings)
             if edge_id in intermediate_state_edges:
                 settings.qn_domains = int_edge_domains
             else:
                 settings.qn_domains = {}
             return settings
 
         final_state_edges = topology.outgoing_edge_ids
         initial_state_edges = topology.incoming_edge_ids
 
         graph_settings: List[GraphSettings] = [
             GraphSettings(
                 edge_settings={
-                    edge_id: create_edge_settings(edge_id)
-                    for edge_id in topology.edges
+                    edge_id: create_edge_settings(edge_id) for edge_id in topology.edges
                 },
                 node_settings={},
             )
         ]
 
         for node_id in topology.nodes:
             interaction_types: List[InteractionType] = []
             out_edge_ids = topology.get_edge_ids_outgoing_from_node(node_id)
             in_edge_ids = topology.get_edge_ids_outgoing_from_node(node_id)
             in_edge_props = [
                 initial_facts.edge_props[edge_id]
-                for edge_id in [
-                    x for x in in_edge_ids if x in initial_state_edges
-                ]
+                for edge_id in [x for x in in_edge_ids if x in initial_state_edges]
             ]
             out_edge_props = [
                 initial_facts.edge_props[edge_id]
-                for edge_id in [
-                    x for x in out_edge_ids if x in final_state_edges
-                ]
+                for edge_id in [x for x in out_edge_ids if x in final_state_edges]
             ]
             node_props = InteractionProperties()
             if node_id in initial_facts.node_props:
                 node_props = initial_facts.node_props[node_id]
             for int_det in self.interaction_determinators:
                 determined_interactions = int_det.check(
                     in_edge_props, out_edge_props, node_props
                 )
                 if interaction_types:
                     interaction_types = list(
                         set(determined_interactions) & set(interaction_types)
                     )
                 else:
                     interaction_types = determined_interactions
+            allowed_interaction_types = self.get_allowed_interaction_types(node_id)
             interaction_types = filter_interaction_types(
-                interaction_types, self.allowed_interaction_types
+                interaction_types, allowed_interaction_types
             )
-            logging.debug(
+            _LOGGER.debug(
                 "using %s interaction order for node: %s",
                 str(interaction_types),
                 str(node_id),
             )
 
             temp_graph_settings: List[GraphSettings] = graph_settings
             graph_settings = []
@@ -539,44 +531,41 @@
     def find_solutions(  # pylint: disable=too-many-branches
         self,
         problem_sets: Dict[float, List[ProblemSet]],
     ) -> "ReactionInfo":
         # pylint: disable=too-many-locals
         """Check for solutions for a specific set of interaction settings."""
         results: Dict[float, _SolutionContainer] = {}
-        logging.info(
+        _LOGGER.info(
             "Number of interaction settings groups being processed: %d",
             len(problem_sets),
         )
         total = sum(map(len, problem_sets.values()))
         progress_bar = tqdm(
             total=total,
             desc="Propagating quantum numbers",
-            disable=logging.getLogger().level > logging.WARNING,
+            disable=_LOGGER.level > logging.WARNING,
         )
         for strength, problems in sorted(problem_sets.items(), reverse=True):
-            logging.info(
-                "processing interaction settings group with "
-                f"strength {strength}",
+            _LOGGER.info(
+                f"processing interaction settings group with strength {strength}",
             )
-            logging.info(f"{len(problems)} entries in this group")
-            logging.info(f"running with {self.__number_of_threads} threads...")
+            _LOGGER.info(f"{len(problems)} entries in this group")
+            _LOGGER.info(f"running with {self.__number_of_threads} threads...")
 
             qn_problems = [x.to_qn_problem_set() for x in problems]
 
             # Because of pickling problems of Generic classes (in this case
             # StateTransitionGraph), multithreaded code has to work with
             # QNProblemSet's and QNResult's. So the appropriate conversions
             # have to be done before and after
             temp_qn_results: List[Tuple[QNProblemSet, QNResult]] = []
             if self.__number_of_threads > 1:
                 with Pool(self.__number_of_threads) as pool:
-                    for qn_result in pool.imap_unordered(
-                        self._solve, qn_problems, 1
-                    ):
+                    for qn_result in pool.imap_unordered(self._solve, qn_problems, 1):
                         temp_qn_results.append(qn_result)
                         progress_bar.update()
             else:
                 for problem in qn_problems:
                     temp_qn_results.append(self._solve(problem))
                     progress_bar.update()
             for temp_qn_result in temp_qn_results:
@@ -584,43 +573,42 @@
                     temp_qn_result[0].topology,
                     temp_qn_result[1],
                 )
                 if strength not in results:
                     results[strength] = temp_result
                 else:
                     results[strength].extend(temp_result, True)
-            if (
-                results[strength].solutions
-                and self.reaction_mode == SolvingMode.FAST
-            ):
+            if results[strength].solutions and self.reaction_mode == SolvingMode.FAST:
                 break
         progress_bar.close()
 
         for key, result in results.items():
-            logging.info(
-                f"number of solutions for strength ({key}) "
-                f"after qn solving: {len(result.solutions)}",
+            _LOGGER.info(
+                (
+                    f"number of solutions for strength ({key}) "
+                    f"after qn solving: {len(result.solutions)}"
+                ),
             )
 
         final_result = _SolutionContainer()
         for temp_result in results.values():
             final_result.extend(temp_result)
 
         # remove duplicate solutions, which only differ in the interaction qns
         final_solutions = remove_duplicate_solutions(
             final_result.solutions,
             self.filter_remove_qns,
             self.filter_ignore_qns,
         )
 
+        execution_info = final_result.execution_info
         if (
             final_result.execution_info.violated_edge_rules
             or final_result.execution_info.violated_node_rules
         ):
-            execution_info = final_result.execution_info
             violated_rules: Set[str] = set()
             for rules in execution_info.violated_edge_rules.values():
                 violated_rules |= rules
             for rules in execution_info.violated_node_rules.values():
                 violated_rules |= rules
             if violated_rules:
                 raise RuntimeError(
@@ -641,44 +629,41 @@
                 + ", ".join(not_executed_rules)
             )
         if not final_solutions:
             raise ValueError("No solutions were found")
 
         match_external_edges(final_solutions)
         final_solutions = [
-            _match_final_state_ids(graph, self.final_state)
-            for graph in final_solutions
+            _match_final_state_ids(graph, self.final_state) for graph in final_solutions
         ]
         return ReactionInfo.from_graphs(final_solutions, self.formalism)
 
-    def _solve(
-        self, qn_problem_set: QNProblemSet
-    ) -> Tuple[QNProblemSet, QNResult]:
-        solver = CSPSolver(self.__allowed_intermediate_particles)
-
-        return (qn_problem_set, solver.find_solutions(qn_problem_set))
+    def _solve(self, qn_problem_set: QNProblemSet) -> Tuple[QNProblemSet, QNResult]:
+        solver = CSPSolver(self.__allowed_intermediate_states)
+        solutions = solver.find_solutions(qn_problem_set)
+        return qn_problem_set, solutions
 
     def __convert_result(
         self, topology: Topology, qn_result: QNResult
     ) -> _SolutionContainer:
         """Converts a `.QNResult` with a `.Topology` into `.ReactionInfo`.
 
-        The ParticleCollection is used to retrieve a particle instance
-        reference to lower the memory footprint.
+        The ParticleCollection is used to retrieve a particle instance reference to
+        lower the memory footprint.
         """
         solutions = []
         for solution in qn_result.solutions:
             graph = StateTransitionGraph[ParticleWithSpin](
                 topology=topology,
                 node_props={
                     i: create_interaction_properties(x)
                     for i, x in solution.node_quantum_numbers.items()
                 },
                 edge_props={
-                    i: create_particle(x, self.__particles)
+                    i: find_particle(x, self.__particles)  # type: ignore[misc]
                     for i, x in solution.edge_quantum_numbers.items()
                 },
             )
             solutions.append(graph)
 
         return _SolutionContainer(
             solutions,
@@ -687,25 +672,26 @@
                 violated_node_rules=qn_result.violated_node_rules,
                 not_executed_node_rules=qn_result.not_executed_node_rules,
                 not_executed_edge_rules=qn_result.not_executed_edge_rules,
             ),
         )
 
 
-def _safe_wrap_list(
-    nested_list: Union[List[str], List[List[str]]]
-) -> List[List[str]]:
-    if all(map(lambda i: isinstance(i, list), nested_list)):
-        return nested_list  # type: ignore[return-value]
-    if all(map(lambda i: isinstance(i, str), nested_list)):
-        return [nested_list]  # type: ignore[list-item]
-    raise TypeError(
-        f"Input final state grouping {nested_list} is not a list of lists of"
-        " strings"
-    )
+def _filter_by_name_pattern(
+    particles: ParticleCollection, pattern: str, regex: bool
+) -> ParticleCollection:
+    def match_regex(particle: Particle) -> bool:
+        return re.match(pattern, particle.name) is not None
+
+    def match_substring(particle: Particle) -> bool:
+        return pattern in particle.name
+
+    if regex:
+        return particles.filter(match_regex)
+    return particles.filter(match_substring)
 
 
 def _match_final_state_ids(
     graph: StateTransitionGraph[ParticleWithSpin],
     state_definition: Sequence[StateDefinition],
 ) -> StateTransitionGraph[ParticleWithSpin]:
     """Temporary fix to https://github.com/ComPWA/qrules/issues/143."""
@@ -746,33 +732,28 @@
 @implement_pretty_repr
 @frozen(order=True)
 class StateTransition:
     """Frozen instance of a `.StateTransitionGraph` of a particle with spin."""
 
     topology: Topology = field(validator=instance_of(Topology))
     states: FrozenDict[int, State] = field(converter=FrozenDict)
-    interactions: FrozenDict[int, InteractionProperties] = field(
-        converter=FrozenDict
-    )
+    interactions: FrozenDict[int, InteractionProperties] = field(converter=FrozenDict)
 
     def __attrs_post_init__(self) -> None:
         _assert_defined(self.topology.edges, self.states)
         _assert_defined(self.topology.nodes, self.interactions)
 
     @staticmethod
     def from_graph(
         graph: StateTransitionGraph[ParticleWithSpin],
     ) -> "StateTransition":
         return StateTransition(
             topology=graph.topology,
             states=FrozenDict(
-                {
-                    i: State(*graph.get_edge_props(i))
-                    for i in graph.topology.edges
-                }
+                {i: State(*graph.get_edge_props(i)) for i in graph.topology.edges}
             ),
             interactions=FrozenDict(
                 {i: graph.get_node_props(i) for i in graph.topology.nodes}
             ),
         )
 
     def to_graph(self) -> StateTransitionGraph[ParticleWithSpin]:
@@ -814,38 +795,34 @@
             f" Available items: {existing}, items with property: {defined}"
         )
 
 
 def _to_sorted_tuple(
     iterable: Iterable[StateTransition],
 ) -> Tuple[StateTransition, ...]:
-    if not all(map(lambda t: isinstance(t, StateTransition), iterable)):
-        raise TypeError(
-            f"Not all instances are of type {StateTransition.__name__}"
-        )
+    if any(not isinstance(t, StateTransition) for t in iterable):
+        raise TypeError(f"Not all instances are of type {StateTransition.__name__}")
     return tuple(sorted(iterable))
 
 
 @frozen
 class StateTransitionCollection(abc.Sequence):
     """`.StateTransition` instances with the same `.Topology` and edge IDs."""
 
-    transitions: Tuple[StateTransition, ...] = field(
-        converter=_to_sorted_tuple
-    )
+    transitions: Tuple[StateTransition, ...] = field(converter=_to_sorted_tuple)
     topology: Topology = field(init=False, repr=False)
     initial_state: FrozenDict[int, Particle] = field(init=False, repr=False)
     final_state: FrozenDict[int, Particle] = field(init=False, repr=False)
 
     def __attrs_post_init__(self) -> None:
-        if not any(self.transitions):
-            ValueError(f"At least one {StateTransition.__name__} required")
+        if len(self.transitions) == 0:
+            raise ValueError(f"At least one {StateTransition.__name__} required")
         some_transition = next(iter(self.transitions))
         topology = some_transition.topology
-        if not all(map(lambda t: t.topology == topology, self.transitions)):
+        if any(t.topology != topology for t in self.transitions):
             raise TypeError(
                 f"Not all {StateTransition.__name__} items have the same"
                 f" underlying topology. Expecting: {topology}"
             )
         object.__setattr__(self, "topology", topology)
         object.__setattr__(
             self,
@@ -874,15 +851,15 @@
         class_name = type(self).__name__
         if cycle:
             p.text(f"{class_name}(...)")
         else:
             with p.group(indent=2, open=f"{class_name}(transitions=("):
                 for transition in self:
                     p.breakable()
-                    p.pretty(transition)
+                    p.pretty(transition)  # type: ignore[attr-defined]
                     p.text(",")
             p.breakable()
             p.text("))")
 
     def __contains__(self, item: object) -> bool:
         return item in self.transitions
 
@@ -922,41 +899,36 @@
                     intermediate_states.add(state.particle)
         return intermediate_states
 
 
 def _to_tuple(
     iterable: Iterable[StateTransitionCollection],
 ) -> Tuple[StateTransitionCollection, ...]:
-    if not all(
-        map(lambda t: isinstance(t, StateTransitionCollection), iterable)
-    ):
+    if any(not isinstance(t, StateTransitionCollection) for t in iterable):
         raise TypeError(
-            "Not all instances are of type"
-            f" {StateTransitionCollection.__name__}"
+            f"Not all instances are of type {StateTransitionCollection.__name__}"
         )
     return tuple(iterable)
 
 
 @frozen(eq=False, hash=True)
 class ReactionInfo:
     """`StateTransitionCollection` instances, grouped by `.Topology`."""
 
     transition_groups: Tuple[StateTransitionCollection, ...] = field(
         converter=_to_tuple
     )
-    transitions: Tuple[StateTransition, ...] = field(
-        init=False, repr=False, eq=False
-    )
+    transitions: Tuple[StateTransition, ...] = field(init=False, repr=False, eq=False)
     initial_state: FrozenDict[int, Particle] = field(init=False, repr=False)
     final_state: FrozenDict[int, Particle] = field(init=False, repr=False)
     formalism: str = field(validator=instance_of(str))
 
     def __attrs_post_init__(self) -> None:
         if len(self.transition_groups) == 0:
-            ValueError(
+            raise ValueError(
                 f"At least one {StateTransitionCollection.__name__} required"
             )
         transitions: List[StateTransition] = []
         for grouping in self.transition_groups:
             transitions.extend(sorted(grouping))
         first_grouping = self.transition_groups[0]
         object.__setattr__(self, "transitions", tuple(transitions))
@@ -968,36 +940,35 @@
             for own_grouping, other_grouping in zip_longest(
                 self.transition_groups, other.transition_groups
             ):
                 if own_grouping != other_grouping:
                     return False
             return True
         raise NotImplementedError(
-            f"Cannot compare {self.__class__.__name__} with "
-            f" {other.__class__.__name__}"
+            f"Cannot compare {self.__class__.__name__} with  {other.__class__.__name__}"
         )
 
     def _repr_pretty_(self, p: "PrettyPrinter", cycle: bool) -> None:
         class_name = type(self).__name__
         if cycle:
             p.text(f"{class_name}(...)")
         else:
             with p.group(indent=2, open=f"{class_name}("):
                 p.breakable()
                 p.text("transition_groups=")
                 with p.group(indent=2, open="("):
                     for transition_grouping in self.transition_groups:
                         p.breakable()
-                        p.pretty(transition_grouping)
+                        p.pretty(transition_grouping)  # type: ignore[attr-defined]
                         p.text(",")
                 p.breakable()
                 p.text("),")
                 p.breakable()
                 p.text("formalism=")
-                p.pretty(self.formalism)
+                p.pretty(self.formalism)  # type: ignore[attr-defined]
                 p.text(",")
             p.breakable()
             p.text(")")
 
     def get_intermediate_particles(self) -> ParticleCollection:
         """Extract the names of the intermediate state particles."""
         return ParticleCollection(
@@ -1010,21 +981,19 @@
         )
 
     @staticmethod
     def from_graphs(
         graphs: Iterable[StateTransitionGraph[ParticleWithSpin]],
         formalism: str,
     ) -> "ReactionInfo":
-        transition_mapping: DefaultDict[
-            Topology, List[StateTransition]
-        ] = defaultdict(list)
+        transition_mapping: DefaultDict[Topology, List[StateTransition]] = defaultdict(
+            list
+        )
         for graph in graphs:
-            transition_mapping[graph.topology].append(
-                StateTransition.from_graph(graph)
-            )
+            transition_mapping[graph.topology].append(StateTransition.from_graph(graph))
         transition_groups = tuple(
             StateTransitionCollection(transitions)
             for transitions in transition_mapping.values()
         )
         return ReactionInfo(transition_groups, formalism)
 
     def to_graphs(self) -> List[StateTransitionGraph[ParticleWithSpin]]:
```

### Comparing `qrules-0.9.7/src/qrules.egg-info/PKG-INFO` & `qrules-0.9.8/src/qrules.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrules
-Version: 0.9.7
+Version: 0.9.8
 Summary: Rule-based particle reaction problem solver on a quantum number level
 Home-page: UNKNOWN
 Author: Common Partial Wave Analysis
 Author-email: compwa-admin@ep1.rub.de
 Maintainer-email: compwa-admin@ep1.rub.de
 License: GPLv3 or later
 Project-URL: Tracker, https://github.com/ComPWA/qrules/issues
@@ -18,39 +18,38 @@
         
         [![PyPI package](https://badge.fury.io/py/qrules.svg)](https://pypi.org/project/qrules)
         [![Conda package](https://anaconda.org/conda-forge/qrules/badges/version.svg)](https://anaconda.org/conda-forge/qrules)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/qrules)](https://pypi.org/project/qrules)
         
         [![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ComPWA/qrules/stable?filepath=docs/usage)
         [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ComPWA/qrules/blob/stable)
-        [![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/ComPWA/qrules)
-        [![GitPod](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
+        [![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/qrules)
+        [![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/qrules)
         
         [![Documentation](https://readthedocs.org/projects/qrules/badge/?version=latest)](https://qrules.readthedocs.io)
         [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/qrules/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/qrules/main)
         [![pytest](https://github.com/ComPWA/qrules/workflows/pytest/badge.svg)](https://github.com/ComPWA/qrules/actions?query=branch%3Amain+workflow%3Apytest)
         [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
         [![Test coverage](https://codecov.io/gh/ComPWA/qrules/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/qrules)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/deeee5b9e2bb4b3daa655942c71e17da)](https://www.codacy.com/gh/ComPWA/qrules)
         [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
         [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort)
         
-        QRules is a Python package for **validating and generating particle reactions**
-        using quantum number conservation rules. The user only has to provide a certain
-        set of boundary conditions (initial and final state, allowed interaction types,
-        expected decay topologies, etc.). QRules will then span the space of allowed
-        quantum numbers over all allowed decay topologies and particle instances that
-        correspond with the sets of allowed quantum numbers it has found.
-        
-        The resulting state transition objects are particularly useful for **amplitude
-        analysis / Partial Wave Analysis** as they contain all information (such as
-        expected masses, widths, and spin projections) that is needed to formulate an
-        amplitude model.
+        QRules is a Python package for **validating and generating particle reactions** using
+        quantum number conservation rules. The user only has to provide a certain set of
+        boundary conditions (initial and final state, allowed interaction types, expected decay
+        topologies, etc.). QRules will then span the space of allowed quantum numbers over all
+        allowed decay topologies and particle instances that correspond with the sets of allowed
+        quantum numbers it has found.
+        
+        The resulting state transition objects are particularly useful for **amplitude analysis
+        / Partial Wave Analysis** as they contain all information (such as expected masses,
+        widths, and spin projections) that is needed to formulate an amplitude model.
         
         Visit [qrules.rtfd.io](https://qrules.readthedocs.io) for more information!
         
         For an overview of **upcoming releases and planned functionality**, see
         [here](https://github.com/ComPWA/qrules/milestones?direction=asc&sort=title&state=open).
         
         ## Available features
@@ -67,16 +66,15 @@
           - Large set of predefined rules
             - Spin/Angular momentum conservation
             - Quark and Lepton flavor conservation (incl. isospin)
             - Baryon number conservation
             - EM-charge conservation
             - Parity, C-Parity, G-Parity conservation
             - Mass conservation
-          - Predefined sets of conservation rules representing Strong, EM, Weak
-            interactions
+          - Predefined sets of conservation rules representing Strong, EM, Weak interactions
         
         ## Contribute
         
         See [`CONTRIBUTING.md`](./CONTRIBUTING.md)
         
 Keywords: HEP,PWA,amplitude analysis,partial wave analysis,particle physics,particles,physics
 Platform: UNKNOWN
@@ -89,22 +87,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: format
 Provides-Extra: flake8
 Provides-Extra: mypy
 Provides-Extra: lint
 Provides-Extra: sty
+Provides-Extra: jupyter
 Provides-Extra: dev
```

### Comparing `qrules-0.9.7/src/qrules.egg-info/SOURCES.txt` & `qrules-0.9.8/src/qrules.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,52 +7,50 @@
 .mypy.ini
 .pre-commit-config.yaml
 .prettierignore
 .prettierrc
 .pydocstyle
 .pylintrc
 .readthedocs.yml
+.taplo.toml
 .zenodo.json
 CONTRIBUTING.md
 LICENSE
 README.md
 codecov.yml
 commitlint.config.js
 environment.yml
 pyproject.toml
 pyrightconfig.json
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
 .constraints/py3.10.txt
+.constraints/py3.11.txt
 .constraints/py3.6.txt
 .constraints/py3.7.txt
 .constraints/py3.8.txt
 .constraints/py3.9.txt
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/cd.yml
-.github/workflows/ci-docs.yml
-.github/workflows/ci-style.yml
-.github/workflows/ci-tests.yml
-.github/workflows/linkcheck.yml
-.github/workflows/milestone.yml
+.github/workflows/ci.yml
+.github/workflows/clean-caches.yml
 .github/workflows/pr-linting.yml
 .github/workflows/release-drafter.yml
-.github/workflows/requirements-cron.yml
-.github/workflows/requirements-pr.yml
+.github/workflows/requirements.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 docs/.gitignore
 docs/.pydocstyle
-docs/Makefile
 docs/_relink_references.py
 docs/bibliography.bib
 docs/conf.py
 docs/index.md
 docs/install.md
 docs/references.md
 docs/usage.ipynb
@@ -99,20 +97,23 @@
 src/qrules/io/_dot.py
 tests/.pydocstyle
 tests/__init__.py
 tests/conftest.py
 tests/channels/__init__.py
 tests/channels/test_d0_to_ks_kp_km.py
 tests/channels/test_jpsi_to_gamma_pi0_pi0.py
+tests/channels/test_lc_to_p_km_pip.py
 tests/channels/test_nbody_reactions.py
+tests/channels/test_psi2s_to_eta_k_kstar.py
 tests/channels/test_y_to_d0_d0bar_pi0_pi0.py
 tests/output/.gitignore
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_combinatorics.py
+tests/unit/test_final_state_permutations.py
 tests/unit/test_parity_prefactor.py
 tests/unit/test_particle.py
 tests/unit/test_pdg.py
 tests/unit/test_qrules.py
 tests/unit/test_quantum_numbers.py
 tests/unit/test_settings.py
 tests/unit/test_system_control.py
```

### Comparing `qrules-0.9.7/src/qrules.egg-info/requires.txt` & `qrules-0.9.8/src/qrules.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,190 +1,212 @@
 attrs>=20.1.0
 jsonschema
 particle
 python-constraint
 PyYAML
 tqdm>=4.24.0
 
-[:python_version < "3.8.0"]
+[:python_version < "3.10.0"]
 typing-extensions
 
 [all]
 graphviz
 
 [dev]
 graphviz
 graphviz
-jupyter
-myst-nb>=0.11
-nbclient>=0.5.5
+myst-nb
 Sphinx>=3
 sphinx-book-theme
 sphinx-codeautolink[ipython]
 sphinx-comments
 sphinx-copybutton
-sphinx-panels
+sphinx-design
 sphinx-thebe
 sphinx-togglebutton
 sphinxcontrib-bibtex>=2
 sphinxcontrib-hep-pdgref
 sphobjinv
+aquirdturtle-collapsible-headings
+jupyterlab
+jupyterlab-code-formatter
 black
 isort
-flake8>=4
-flake8-blind-except
-flake8-bugbear
-flake8-builtins
-flake8-comprehensions
-flake8-pytest-style
-flake8-rst-docstrings
-flake8-use-fstring
-pep8-naming
 mypy>=0.730
 types-docutils
 types-pkg-resources
 types-PyYAML
 types-requests
 types-setuptools
 pydocstyle
 pylint>=2.5
 ipython
 nbmake
+nbmake!=1.3.*
+nbmake!=1.4.*
 pydot
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist
 pre-commit>=1.4.0
 ipython
 nbmake
+nbmake!=1.3.*
+nbmake!=1.4.*
 pydot
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist
-aquirdturtle-collapsible-headings
-jupyterlab
-jupyterlab-code-formatter
-pip-tools>=6.1.0
 sphinx-autobuild
 tox>=1.9
 
+[dev:python_version < "3.7.0"]
+virtualenv!=20.16.*
+virtualenv!=20.17.*
+
 [dev:python_version < "3.8.0"]
-Sphinx<4.4
+importlib-metadata
+tox!=4.*
 
 [dev:python_version >= "3.7.0"]
 jupyterlab-myst
+ypy-websocket<0.8.3
 
 [dev:python_version >= "3.8.0"]
+flake8>=4
+flake8-blind-except
+flake8-bugbear
+flake8-builtins
+flake8-comprehensions
+flake8-future-import
+flake8-pytest-style
+flake8-rst-docstrings
 flake8-type-ignore
+flake8-use-fstring
+pep8-naming
 
 [doc]
 graphviz
-jupyter
-myst-nb>=0.11
-nbclient>=0.5.5
+myst-nb
 Sphinx>=3
 sphinx-book-theme
 sphinx-codeautolink[ipython]
 sphinx-comments
 sphinx-copybutton
-sphinx-panels
+sphinx-design
 sphinx-thebe
 sphinx-togglebutton
 sphinxcontrib-bibtex>=2
 sphinxcontrib-hep-pdgref
 sphobjinv
 
 [doc:python_version < "3.8.0"]
-Sphinx<4.4
+importlib-metadata
 
 [flake8]
+
+[flake8:python_version >= "3.8.0"]
 flake8>=4
 flake8-blind-except
 flake8-bugbear
 flake8-builtins
 flake8-comprehensions
+flake8-future-import
 flake8-pytest-style
 flake8-rst-docstrings
+flake8-type-ignore
 flake8-use-fstring
 pep8-naming
 
-[flake8:python_version >= "3.8.0"]
-flake8-type-ignore
-
 [format]
 black
 isort
 
+[jupyter]
+aquirdturtle-collapsible-headings
+jupyterlab
+jupyterlab-code-formatter
+
+[jupyter:python_version >= "3.7.0"]
+jupyterlab-myst
+ypy-websocket<0.8.3
+
 [lint]
-flake8>=4
-flake8-blind-except
-flake8-bugbear
-flake8-builtins
-flake8-comprehensions
-flake8-pytest-style
-flake8-rst-docstrings
-flake8-use-fstring
-pep8-naming
 mypy>=0.730
 types-docutils
 types-pkg-resources
 types-PyYAML
 types-requests
 types-setuptools
 pydocstyle
 pylint>=2.5
 
 [lint:python_version >= "3.8.0"]
+flake8>=4
+flake8-blind-except
+flake8-bugbear
+flake8-builtins
+flake8-comprehensions
+flake8-future-import
+flake8-pytest-style
+flake8-rst-docstrings
 flake8-type-ignore
+flake8-use-fstring
+pep8-naming
 
 [mypy]
 mypy>=0.730
 types-docutils
 types-pkg-resources
 types-PyYAML
 types-requests
 types-setuptools
 
 [sty]
 black
 isort
-flake8>=4
-flake8-blind-except
-flake8-bugbear
-flake8-builtins
-flake8-comprehensions
-flake8-pytest-style
-flake8-rst-docstrings
-flake8-use-fstring
-pep8-naming
 mypy>=0.730
 types-docutils
 types-pkg-resources
 types-PyYAML
 types-requests
 types-setuptools
 pydocstyle
 pylint>=2.5
 ipython
 nbmake
+nbmake!=1.3.*
+nbmake!=1.4.*
 pydot
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist
 pre-commit>=1.4.0
 
 [sty:python_version >= "3.8.0"]
+flake8>=4
+flake8-blind-except
+flake8-bugbear
+flake8-builtins
+flake8-comprehensions
+flake8-future-import
+flake8-pytest-style
+flake8-rst-docstrings
 flake8-type-ignore
+flake8-use-fstring
+pep8-naming
 
 [test]
 ipython
 nbmake
+nbmake!=1.3.*
+nbmake!=1.4.*
 pydot
 pytest
 pytest-cov
 pytest-profiling
 pytest-xdist
 
 [viz]
```

### Comparing `qrules-0.9.7/tests/channels/test_d0_to_ks_kp_km.py` & `qrules-0.9.8/tests/channels/test_d0_to_ks_kp_km.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/channels/test_jpsi_to_gamma_pi0_pi0.py` & `qrules-0.9.8/tests/channels/test_jpsi_to_gamma_pi0_pi0.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,15 @@
         particle_db=particle_database,
         allowed_interaction_types=["strong", "EM"],
         allowed_intermediate_particles=allowed_intermediate_particles,
         formalism="helicity",
     )
     assert len(reaction.transition_groups) == n_topologies
     assert len(reaction.transitions) == number_of_solutions
-    assert (
-        reaction.get_intermediate_particles().names
-        == allowed_intermediate_particles
-    )
+    assert reaction.get_intermediate_particles().names == allowed_intermediate_particles
 
 
 def test_id_to_particle_mappings(particle_database):
     reaction = qrules.generate_transitions(
         initial_state=("J/psi(1S)", [-1, +1]),
         final_state=["gamma", "pi0", "pi0"],
         particle_db=particle_database,
```

### Comparing `qrules-0.9.7/tests/channels/test_nbody_reactions.py` & `qrules-0.9.8/tests/channels/test_nbody_reactions.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/channels/test_y_to_d0_d0bar_pi0_pi0.py` & `qrules-0.9.8/tests/channels/test_y_to_d0_d0bar_pi0_pi0.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,7 +41,27 @@
     )
     stm.set_allowed_interaction_types([InteractionType.STRONG])
     stm.add_final_state_grouping([["D0", "pi0"], ["D~0", "pi0"]])
     problem_sets = stm.create_problem_sets()
     reaction = stm.find_solutions(problem_sets)
     assert len(reaction.transition_groups) == 1
     assert len(reaction.transitions) == n_solutions
+
+
+def test_resonance_filter(particle_database):
+    # https://github.com/ComPWA/qrules/issues/33
+    stm = StateTransitionManager(
+        initial_state=[("Y(4260)", [-1, +1])],
+        final_state=["D0", "D~0", "pi0", "pi0"],
+        allowed_intermediate_particles=["D"],
+        particle_db=particle_database,
+    )
+    stm.set_allowed_interaction_types([InteractionType.STRONG])
+    stm.add_final_state_grouping([["D0", "pi0"], ["D~0", "pi0"]])
+    problem_sets = stm.create_problem_sets()
+    result = stm.find_solutions(problem_sets)
+    assert set(result.get_intermediate_particles().names) == {
+        "D*(2007)0",
+        "D*(2007)~0",
+        "D(0)*(2300)0",
+        "D(0)*(2300)~0",
+    }
```

### Comparing `qrules-0.9.7/tests/conftest.py` & `qrules-0.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_c_parity.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_c_parity.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,45 +11,29 @@
 
 
 @pytest.mark.parametrize(
     ("rule_input", "expected"),
     [
         (
             (
+                [CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(-1))],
                 [
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(-1)
-                    )
-                ],
-                [
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(-1)
-                    ),
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(1)
-                    ),
+                    CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(-1)),
+                    CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(1)),
                 ],
                 None,
             ),
             True,
         ),
         (
             (
+                [CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(1))],
                 [
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(1)
-                    )
-                ],
-                [
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(-1)
-                    ),
-                    CParityEdgeInput(
-                        spin_magnitude=0.0, pid=1, c_parity=Parity(1)
-                    ),
+                    CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(-1)),
+                    CParityEdgeInput(spin_magnitude=0.0, pid=1, c_parity=Parity(1)),
                 ],
                 None,
             ),
             False,
         ),
     ],
 )
@@ -92,17 +76,15 @@
                         spin_magnitude=0, pid=123, c_parity=Parity(c_parity)
                     )
                 ],
                 [
                     CParityEdgeInput(spin_magnitude=0.5, pid=100),
                     CParityEdgeInput(spin_magnitude=0.5, pid=-100),
                 ],
-                CParityNodeInput(
-                    l_magnitude=l_magnitude, s_magnitude=s_magnitude
-                ),
+                CParityNodeInput(l_magnitude=l_magnitude, s_magnitude=s_magnitude),
             ),
             (s_magnitude + l_magnitude) % 2 == abs(c_parity - 1) / 2,
         )
         for c_parity, s_magnitude, l_magnitude in product(
             [-1, 1], range(0, 5), range(0, 5)
         )
     ],
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_clebsch_gordan.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_clebsch_gordan.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     isospin_conservation,
     spin_conservation,
 )
 from qrules.particle import Spin
 
 from .test_spin import __create_two_body_decay_spin_data
 
-_SpinRuleInputType = Tuple[
-    List[SpinEdgeInput], List[SpinEdgeInput], SpinNodeInput
-]
+_SpinRuleInputType = Tuple[List[SpinEdgeInput], List[SpinEdgeInput], SpinNodeInput]
 
 
 @pytest.mark.parametrize(
     ("rule_input", "expected"),
     [
         (
             __create_two_body_decay_spin_data(
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_duck_typing.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_duck_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Check duck typing.
 
-Ideally, the rule input classes use a `~typing.Protocol`. This is not possible,
-however, because of https://github.com/python/mypy/issues/6850. Duck typing is
-therefore checked through functions defined in this test.
+Ideally, the rule input classes use a `~typing.Protocol`. This is not possible, however,
+because of https://github.com/python/mypy/issues/6850. Duck typing is therefore checked
+through functions defined in this test.
 """
 
 import inspect
 from typing import Set, Type
 
 import attrs
 
@@ -58,17 +58,15 @@
 def __get_duck_types(instance: Type) -> Set[Type]:
     """Get a `set` of rule input classes that this instance can duck type."""
     return {c for c in RULE_INPUT_CLASSES if __is_duck_type(c, instance)}
 
 
 def test_is_duck_type():
     assert __is_duck_type(NodeQuantumNumbers, InteractionProperties)
-    assert __is_duck_type(
-        conservation_rules.CParityNodeInput, NodeQuantumNumbers
-    )
+    assert __is_duck_type(conservation_rules.CParityNodeInput, NodeQuantumNumbers)
     assert __is_duck_type(conservation_rules.MassEdgeInput, Particle)
 
 
 def __is_duck_type(duck_type: Type, class_type: Type) -> bool:
     """See https://github.com/python/mypy/issues/6850."""
     return __get_members(duck_type) <= __get_members(class_type)
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_g_parity.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_g_parity.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,12 @@
                         pid=-100,
                     ),
                 ],
                 GParityNodeInput(l_magnitude=l_magnitude, s_magnitude=0),
             ),
             (-1) ** (l_magnitude + isospin) == g_parity,
         )
-        for g_parity, isospin, l_magnitude in product(
-            [-1, 1], [0, 1], range(0, 5)
-        )
+        for g_parity, isospin, l_magnitude in product([-1, 1], [0, 1], range(0, 5))
     ],
 )
 def test_g_parity_multiparticle_boson(rule_input, expected):
     assert g_parity_conservation(*rule_input) is expected
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_gellmann_nishijima.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_gellmann_nishijima.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from itertools import product
 
 import pytest
 
-from qrules.conservation_rules import (
-    GellMannNishijimaInput,
-    gellmann_nishijima,
-)
+from qrules.conservation_rules import GellMannNishijimaInput, gellmann_nishijima
 
 
 @pytest.mark.parametrize(
     ("particle", "expected"),
     [
         (
             GellMannNishijimaInput(
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_helicity_conservation.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_helicity_conservation.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_identical_particle_symmetrization.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_identical_particle_symmetrization.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_mass.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_mass.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_parity_conservation.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_parity_conservation.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,15 @@
         )
         for parity_in, parity_out1, l_magnitude in product(
             [-1, 1], [-1, 1], range(0, 5)
         )
     ],
 )
 def test_parity_conservation(in_parities, out_parities, l_magnitude, expected):
-    assert (
-        parity_conservation(in_parities, out_parities, l_magnitude) is expected
-    )
+    assert parity_conservation(in_parities, out_parities, l_magnitude) is expected
 
 
 @pytest.mark.parametrize(
     ("in_parities", "out_parities", "l_magnitude", "expected"),
     [
         (
             [
@@ -57,28 +55,26 @@
                 HelicityParityEdgeInput(
                     parity=Parity(out_parity2),
                     spin_magnitude=1,
                     spin_projection=-1,
                 ),
             ],
             NodeQuantumNumbers.parity_prefactor(1),
-            in_parity * out_parity1 * out_parity2 * (-1) ** (in_spin_mag % 2)
-            == 1,
+            in_parity * out_parity1 * out_parity2 * (-1) ** (in_spin_mag % 2) == 1,
         )
         for in_spin_mag, in_parity, out_parity1, out_parity2 in product(
             range(0, 4), [-1, 1], [-1, 1], [-1, 1]
         )
     ],
 )
 def test_parity_conservation_helicity_prefactor(
     in_parities, out_parities, l_magnitude, expected
 ):
     assert (
-        parity_conservation_helicity(in_parities, out_parities, l_magnitude)
-        is expected
+        parity_conservation_helicity(in_parities, out_parities, l_magnitude) is expected
     )
 
 
 @pytest.mark.parametrize(
     ("in_parities", "out_parities", "l_magnitude", "expected"),
     [
         (
@@ -98,22 +94,18 @@
                 HelicityParityEdgeInput(
                     parity=Parity(1),
                     spin_magnitude=1,
                     spin_projection=0,
                 ),
             ],
             NodeQuantumNumbers.parity_prefactor(parity_prefactor),
-            in_parity * (-1) ** (in_spin_mag % 2) == 1
-            and parity_prefactor == 1,
+            in_parity * (-1) ** (in_spin_mag % 2) == 1 and parity_prefactor == 1,
         )
         for in_spin_mag, in_parity, parity_prefactor in product(
             range(0, 4), [-1, 1], [-1, 1]
         )
     ],
 )
-def test_parity_conservation_helicity(
-    in_parities, out_parities, l_magnitude, expected
-):
+def test_parity_conservation_helicity(in_parities, out_parities, l_magnitude, expected):
     assert (
-        parity_conservation_helicity(in_parities, out_parities, l_magnitude)
-        is expected
+        parity_conservation_helicity(in_parities, out_parities, l_magnitude) is expected
     )
```

### Comparing `qrules-0.9.7/tests/unit/conservation_rules/test_spin.py` & `qrules-0.9.8/tests/unit/conservation_rules/test_spin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
     SpinEdgeInput,
     SpinNodeInput,
     spin_conservation,
     spin_magnitude_conservation,
 )
 from qrules.particle import Spin
 
-_SpinRuleInputType = Tuple[
-    List[SpinEdgeInput], List[SpinEdgeInput], SpinNodeInput
-]
+_SpinRuleInputType = Tuple[List[SpinEdgeInput], List[SpinEdgeInput], SpinNodeInput]
 
 
 def __create_two_body_decay_spin_data(
     in_spin: Optional[Spin] = None,
     out_spin1: Optional[Spin] = None,
     out_spin2: Optional[Spin] = None,
     angular_momentum: Optional[Spin] = None,
@@ -48,17 +46,15 @@
     )
 
 
 @pytest.mark.parametrize(
     ("rule_input", "expected"),
     [
         (
-            __create_two_body_decay_spin_data(
-                angular_momentum=Spin(ang_mom_mag, 0)
-            ),
+            __create_two_body_decay_spin_data(angular_momentum=Spin(ang_mom_mag, 0)),
             expected,
         )
         for ang_mom_mag, expected in [
             (0, True),
             (1, False),
             (2, False),
             (3, False),
@@ -109,17 +105,15 @@
                 angular_momentum=Spin(1, 0),
                 coupled_spin=Spin(2, 0),
             ),
             True,
         ),
     ],
 )
-def test_spin_all_defined(
-    rule_input: _SpinRuleInputType, expected: bool
-) -> None:
+def test_spin_all_defined(rule_input: _SpinRuleInputType, expected: bool) -> None:
     assert spin_conservation(*rule_input) is expected
 
 
 @pytest.mark.parametrize(
     ("rule_input", "expected"),
     [
         (
```

### Comparing `qrules-0.9.7/tests/unit/io/conftest.py` & `qrules-0.9.8/tests/unit/io/conftest.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/io/test_dict.py` & `qrules-0.9.8/tests/unit/io/test_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
         io.write(particle_selection, output_dir + "test.py")
     with pytest.raises(ValueError, match=r"No file extension in file name"):
         io.write(particle_selection, output_dir + "no_file_extension")
     with pytest.raises(NotImplementedError):
         io.write(666, output_dir + "wont_work_anyway.yml")
 
 
-def test_serialization(
-    output_dir: str, particle_selection: ParticleCollection
-):
+def test_serialization(output_dir: str, particle_selection: ParticleCollection):
     io.write(particle_selection, output_dir + "particle_selection.yml")
     assert len(particle_selection) == 193
     asdict = io.asdict(particle_selection)
     imported_collection = io.fromdict(asdict)
     assert isinstance(imported_collection, ParticleCollection)
     assert len(particle_selection) == len(imported_collection)
     for particle in particle_selection:
```

### Comparing `qrules-0.9.7/tests/unit/io/test_dot.py` & `qrules-0.9.8/tests/unit/io/test_dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-# pylint: disable=no-self-use
 import pydot
 import pytest
 
 import qrules
 from qrules import io
-from qrules.io._dot import (
-    _collapse_graphs,
-    _get_particle_graphs,
-    _strip_projections,
-)
+from qrules.io._dot import _collapse_graphs, _get_particle_graphs, _strip_projections
 from qrules.particle import ParticleCollection
 from qrules.topology import (
     Edge,
     Topology,
     create_isobar_topologies,
     create_n_body_topology,
 )
@@ -97,20 +92,16 @@
         transition,
         edge_style={"fontcolor": "blue"},
         node_style={"fontcolor": "darkgreen", "shape": "ellipse"},
     )
     assert pydot.graph_from_dot_data(dot) is not None
     with open(output_dir + f"styled_{reaction.formalism}.gv", "w") as stream:
         stream.write(dot)
-    assert (
-        '"edge0" [shape=none, fontcolor="blue", label="0: gamma[-1]"];' in dot
-    )
-    assert (
-        '"node0" -> "node1" [fontcolor="blue", label="f(0)(980)[0]"];' in dot
-    )
+    assert '"edge0" [shape=none, fontcolor="blue", label="0: gamma[-1]"];' in dot
+    assert '"node0" -> "node1" [fontcolor="blue", label="f(0)(980)[0]"];' in dot
     assert '"node0" [shape="ellipse", fontcolor="darkgreen", label=""];' in dot
 
 
 def test_asdot_no_label_overwriting(reaction: ReactionInfo):
     transition = reaction.transitions[0]
     label = "should be ignored"
     dot_data = io.asdot(
```

### Comparing `qrules-0.9.7/tests/unit/io/test_io.py` & `qrules-0.9.8/tests/unit/io/test_io.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/test_combinatorics.py` & `qrules-0.9.8/tests/unit/test_combinatorics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,148 @@
-# pylint: disable=no-self-use, redefined-outer-name
-from math import factorial
+# pylint: disable=redefined-outer-name
+from typing import List
 
 import pytest
 
 from qrules.combinatorics import (
     _generate_kinematic_permutations,
-    _generate_outer_edge_permutations,
-    _generate_spin_permutations,
     _get_kinematic_representation,
     _KinematicRepresentation,
-    _safe_set_spin_projections,
+    _permutate_outer_edges,
     create_initial_facts,
+    permutate_topology_kinematically,
 )
-from qrules.particle import ParticleCollection
 from qrules.topology import Topology, create_isobar_topologies
 
 
 @pytest.fixture(scope="session")
 def three_body_decay() -> Topology:
     topologies = create_isobar_topologies(3)
     topology = next(iter(topologies))
     return topology
 
 
+def test_create_initial_facts(particle_database):
+    initial_facts = create_initial_facts(
+        initial_state=[("J/psi(1S)", [-1, +1])],
+        final_state=["gamma", "pi0", "pi0"],
+        particle_db=particle_database,
+    )
+    assert len(initial_facts) == 4
+
+    for fact in initial_facts:
+        edge_ids = sorted(fact.edge_props)
+        assert edge_ids == [-1, 0, 1, 2]
+        particle_names = [fact.edge_props[i][0].name for i in edge_ids]
+        assert particle_names == ["J/psi(1S)", "gamma", "pi0", "pi0"]
+        _, initial_polarization = fact.edge_props[-1]
+        assert initial_polarization in {-1, +1}
+
+
+def test_generate_kinematic_permutations_groupings(three_body_decay: Topology):
+    topology = three_body_decay
+    particle_names = {
+        -1: "J/psi(1S)",
+        0: "gamma",
+        1: "pi0",
+        2: "pi0",
+    }
+    allowed_kinematic_groupings = [_KinematicRepresentation(["pi0", "pi0"])]
+    permutations = _generate_kinematic_permutations(
+        topology, particle_names, allowed_kinematic_groupings
+    )
+    assert len(permutations) == 1
+
+    permutations = _generate_kinematic_permutations(topology, particle_names)
+    assert len(permutations) == 2
+    assert permutations[0].get_originating_final_state_edge_ids(1) == {1, 2}
+    assert permutations[1].get_originating_final_state_edge_ids(1) == {0, 2}
+
+
+@pytest.mark.parametrize(
+    ("n_permutations", "decay_type"),
+    [
+        (3, "two_to_three_decay"),
+        (3, "three_body_decay"),
+    ],
+)
+def test_permutate_outer_edges(
+    n_permutations: int,
+    decay_type: str,
+    three_body_decay: Topology,
+    two_to_three_decay: Topology,
+):
+    if decay_type == "two_to_three_decay":
+        topology = two_to_three_decay
+    elif decay_type == "three_body_decay":
+        topology = three_body_decay
+    else:
+        raise NotImplementedError(decay_type)
+    permutations = _permutate_outer_edges(topology)
+    assert len(permutations) == n_permutations
+
+
 @pytest.mark.parametrize(
     "final_state_groupings",
     [
         ["pi0", "pi0"],
         [["pi0", "pi0"]],
         [[["pi0", "pi0"]]],
         ["gamma", "pi0"],
         [["gamma", "pi0"]],
         [[["gamma", "pi0"]]],
+        None,
     ],
 )
-def test_initialize_graph(
+def test_permutate_topology_kinematically(
     final_state_groupings,
     three_body_decay: Topology,
-    particle_database: ParticleCollection,
 ):
-    initial_facts = create_initial_facts(
-        three_body_decay,
+    permutations = permutate_topology_kinematically(
+        topology=three_body_decay,
         initial_state=[("J/psi(1S)", [-1, +1])],
         final_state=["gamma", "pi0", "pi0"],
-        particle_db=particle_database,
         final_state_groupings=final_state_groupings,
     )
-    assert len(initial_facts) == 4
+    if final_state_groupings is None:
+        assert len(permutations) == 2
+    else:
+        assert len(permutations) == 1
 
 
 @pytest.mark.parametrize(
-    ("initial_state", "final_state"),
+    ("n_permutations", "initial_state", "final_state"),
     [
-        (["J/psi(1S)"], ["gamma", "pi0", "pi0"]),
-        (["J/psi(1S)"], ["K+", "K-", "pi+", "pi-"]),
-        (["e+", "e-"], ["gamma", "pi-", "pi+"]),
-        (["e+", "e-"], ["K+", "K-", "pi+", "pi-"]),
+        (2, ["J/psi(1S)"], ["gamma", "pi0", "pi0"]),
+        (3, ["J/psi(1S)"], ["gamma", "pi-", "pi+"]),
+        (2, ["e+", "e-"], ["gamma", "pi0", "pi0"]),
+        (3, ["e+", "e-"], ["gamma", "pi-", "pi+"]),
     ],
 )
-def test_generate_outer_edge_permutations(
-    initial_state,
-    final_state,
+def test_generate_kinematic_permutations(
+    n_permutations: int,
+    initial_state: List[str],
+    final_state: List[str],
     three_body_decay: Topology,
-    particle_database: ParticleCollection,
+    two_to_three_decay: Topology,
 ):
-    initial_state_with_spins = _safe_set_spin_projections(
-        initial_state, particle_database
-    )
-    final_state_with_spins = _safe_set_spin_projections(
-        final_state, particle_database
-    )
-    list_of_permutations = list(
-        _generate_outer_edge_permutations(
-            three_body_decay,
-            initial_state_with_spins,
-            final_state_with_spins,
+    if len(initial_state) == 1:
+        topology = three_body_decay
+    elif len(initial_state) == 2:
+        topology = two_to_three_decay
+    else:
+        raise NotImplementedError
+    particle_names = dict(
+        zip(
+            sorted(topology.incoming_edge_ids) + sorted(topology.outgoing_edge_ids),
+            list(initial_state) + list(final_state),
         )
     )
-    n_permutations_final_state = factorial(len(final_state))
-    n_permutations_initial_state = factorial(len(initial_state))
-    n_permutations = n_permutations_final_state * n_permutations_initial_state
-    assert len(list_of_permutations) == n_permutations
+    permutations = _generate_kinematic_permutations(topology, particle_names)
+    assert len(permutations) == n_permutations
 
 
 class TestKinematicRepresentation:
     def test_constructor(self):
         representation = _KinematicRepresentation(
             initial_state=["J/psi"],
             final_state=["gamma", "pi0"],
@@ -92,21 +150,19 @@
         assert representation.initial_state == [["J/psi"]]
         assert representation.final_state == [["gamma", "pi0"]]
         representation = _KinematicRepresentation([["gamma", "pi0"]])
         assert representation.initial_state is None
         assert representation.final_state == [["gamma", "pi0"]]
 
     def test_from_topology(self, three_body_decay: Topology):
-        pi0 = ("pi0", [0])
-        gamma = ("gamma", [-1, 1])
         edge_props = {
-            -1: ("J/psi", [-1, +1]),
-            0: pi0,
-            1: pi0,
-            2: gamma,
+            -1: "J/psi",
+            0: "pi0",
+            1: "pi0",
+            2: "gamma",
         }
         kinematic_representation1 = _get_kinematic_representation(
             three_body_decay, edge_props
         )
         assert kinematic_representation1.initial_state == [
             ["J/psi"],
             ["J/psi"],
@@ -114,30 +170,30 @@
         assert kinematic_representation1.final_state == [
             ["gamma", "pi0"],
             ["gamma", "pi0", "pi0"],
         ]
 
         kinematic_representation2 = _get_kinematic_representation(
             topology=three_body_decay,
-            initial_facts={
-                -1: ("J/psi", [-1, +1]),
-                0: pi0,
-                1: gamma,
-                2: pi0,
+            particle_names={
+                -1: "J/psi",
+                0: "pi0",
+                1: "gamma",
+                2: "pi0",
             },
         )
         assert kinematic_representation1 == kinematic_representation2
 
         kinematic_representation3 = _get_kinematic_representation(
             topology=three_body_decay,
-            initial_facts={
-                -1: ("J/psi", [-1, +1]),
-                0: pi0,
-                1: gamma,
-                2: gamma,
+            particle_names={
+                -1: "J/psi",
+                0: "pi0",
+                1: "gamma",
+                2: "gamma",
             },
         )
         assert kinematic_representation2 != kinematic_representation3
 
     def test_repr_and_equality(self):
         kinematic_representation = _KinematicRepresentation(
             initial_state=[["J/psi"]],
@@ -161,56 +217,7 @@
         with pytest.raises(ValueError, match=r"Cannot compare "):
             assert float() in kinematic_representation
         with pytest.raises(
             ValueError,
             match=r"Comparison representation needs to be a list of lists",
         ):
             assert ["should be nested list"] in kinematic_representation
-
-
-def test_generate_permutations(
-    three_body_decay: Topology, particle_database: ParticleCollection
-):
-    permutations = _generate_kinematic_permutations(
-        three_body_decay,
-        initial_state=[("J/psi(1S)", [-1, +1])],
-        final_state=["gamma", "pi0", "pi0"],
-        particle_db=particle_database,
-        allowed_kinematic_groupings=[_KinematicRepresentation(["pi0", "pi0"])],
-    )
-    assert len(permutations) == 1
-
-    permutations = _generate_kinematic_permutations(
-        three_body_decay,
-        initial_state=[("J/psi(1S)", [-1, +1])],
-        final_state=["gamma", "pi0", "pi0"],
-        particle_db=particle_database,
-    )
-    assert len(permutations) == 2
-    graph0_final_state_node1 = [
-        permutations[0][edge_id]
-        for edge_id in three_body_decay.get_originating_final_state_edge_ids(1)
-    ]
-    graph1_final_state_node1 = [
-        permutations[1][edge_id]
-        for edge_id in three_body_decay.get_originating_final_state_edge_ids(1)
-    ]
-    assert graph0_final_state_node1 == [
-        ("pi0", [0]),
-        ("pi0", [0]),
-    ]
-    assert graph1_final_state_node1 == [
-        ("gamma", [-1, 1]),
-        ("pi0", [0]),
-    ]
-
-    permutation0 = permutations[0]
-    spin_permutations = _generate_spin_permutations(
-        permutation0, particle_database
-    )
-    assert len(spin_permutations) == 4
-    assert spin_permutations[0][-1][1] == -1
-    assert spin_permutations[0][0][1] == -1
-    assert spin_permutations[1][-1][1] == -1
-    assert spin_permutations[1][0][1] == +1
-    assert spin_permutations[2][-1][1] == +1
-    assert spin_permutations[3][-1][1] == +1
```

### Comparing `qrules-0.9.7/tests/unit/test_parity_prefactor.py` & `qrules-0.9.8/tests/unit/test_parity_prefactor.py`

 * *Files identical despite different names*

### Comparing `qrules-0.9.7/tests/unit/test_particle.py` & `qrules-0.9.8/tests/unit/test_particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# pylint: disable=eval-used, no-self-use, redefined-outer-name
+# pylint: disable=eval-used redefined-outer-name
 # pyright: reportUnusedImport=false
 import logging
+import sys
 from copy import deepcopy
 
 import pytest
 from attrs.exceptions import FrozenInstanceError
 from IPython.lib.pretty import pretty
 
 from qrules.particle import (
@@ -35,17 +36,15 @@
             ("e+", True),
             ("e-", True),
             ("nu(e)", True),
             ("nu(tau)~", True),
             ("tau+", True),
         ],
     )
-    def test_is_lepton(
-        self, name, is_lepton, particle_database: ParticleCollection
-    ):
+    def test_is_lepton(self, name, is_lepton, particle_database: ParticleCollection):
         assert particle_database[name].is_lepton() == is_lepton
 
     def test_exceptions(self):
         test_state = Particle(
             name="MyParticle",
             pid=123,
             mass=1.2,
@@ -124,17 +123,15 @@
         pim = particle_database.find(-211)
         assert pip == -pim
 
     def test_total_ordering(self, particle_database: ParticleCollection):
         pdg = particle_database
         assert [
             particle.name
-            for particle in sorted(
-                pdg.filter(lambda p: p.name.startswith("f(0)"))
-            )
+            for particle in sorted(pdg.filter(lambda p: p.name.startswith("f(0)")))
         ] == [
             "f(0)(500)",
             "f(0)(980)",
             "f(0)(1370)",
             "f(0)(1500)",
             "f(0)(1710)",
         ]
@@ -156,20 +153,16 @@
     @pytest.mark.parametrize("repr_method", [repr, pretty])
     def test_repr(self, particle_database: ParticleCollection, repr_method):
         instance = particle_database
         from_repr = eval(repr_method(instance))
         assert from_repr == instance
 
     def test_add(self, particle_database: ParticleCollection):
-        subset_copy = particle_database.filter(
-            lambda p: p.name.startswith("omega")
-        )
-        subset_copy += particle_database.filter(
-            lambda p: p.name.startswith("pi")
-        )
+        subset_copy = particle_database.filter(lambda p: p.name.startswith("omega"))
+        subset_copy += particle_database.filter(lambda p: p.name.startswith("pi"))
         n_subset = len(subset_copy)
 
         new_particle = create_particle(
             particle_database.find(443),
             pid=666,
             name="EpEm",
             mass=1.0,
@@ -257,15 +250,19 @@
             (666, None),
             ("non-existing", None),
             # cspell:disable
             ("gamm", "'gamma'"),
             ("gama", "'gamma', 'Sigma0', 'Sigma-', 'Sigma+', 'Lambda'"),
             (
                 "omega",
-                "'omega(782)', 'omega(1420)', 'omega(3)(1670)', 'omega(1650)'",
+                (
+                    "'omega(782)', 'omega(1420)', 'omega(3)(1670)', 'omega(1650)'"
+                    if sys.version_info < (3, 7)
+                    else "'omega(782)', 'omega(3)(1670)', 'omega(1650)'"
+                ),
             ),
             ("p~~", "'p~'"),
             ("~", "'p~', 'n~'"),
             ("lambda", "'Lambda', 'Lambda~', 'Lambda(c)+', 'Lambda(b)0'"),
             # cspell:enable
         ],
     )
@@ -281,16 +278,15 @@
             assert message.endswith(expected)
 
     def test_exceptions(self, particle_database: ParticleCollection):
         gamma = particle_database["gamma"]
         with pytest.raises(
             ValueError,
             match=(
-                'Added particle "gamma_new" is equivalent to existing particle'
-                ' "gamma"'
+                'Added particle "gamma_new" is equivalent to existing particle "gamma"'
             ),
         ):
             particle_database += create_particle(gamma, name="gamma_new")
         with pytest.raises(NotImplementedError):
             particle_database.find(3.14)  # type: ignore[arg-type]
         with pytest.raises(NotImplementedError):
             particle_database += 3.14  # type: ignore[arg-type]
@@ -369,17 +365,15 @@
 )
 def test_create_antiparticle(
     particle_database: ParticleCollection,
     particle_name,
     anti_particle_name,
 ):
     template_particle = particle_database[particle_name]
-    anti_particle = create_antiparticle(
-        template_particle, new_name=anti_particle_name
-    )
+    anti_particle = create_antiparticle(template_particle, new_name=anti_particle_name)
     comparison_particle = particle_database[anti_particle_name]
 
     assert anti_particle == comparison_particle
 
 
 def test_create_antiparticle_tilde(particle_database: ParticleCollection):
     anti_particles = particle_database.filter(lambda p: "~" in p.name)
@@ -398,17 +392,17 @@
 
         assert created_particle == particle_database[particle_name]
 
 
 def test_create_antiparticle_by_pid(particle_database: ParticleCollection):
     n_particles_with_neg_pid = 0
     for particle in particle_database:
+        # pylint: disable=cell-var-from-loop
         anti_particles_by_pid = particle_database.filter(
-            lambda p: p.pid
-            == -particle.pid  # pylint: disable=cell-var-from-loop
+            lambda p: p.pid == -particle.pid  # noqa: B023
         )
         if len(anti_particles_by_pid) != 1:
             continue
         n_particles_with_neg_pid += 1
         anti_particle = next(iter(anti_particles_by_pid))
         particle_from_anti = -anti_particle
         assert particle == particle_from_anti
@@ -419,17 +413,15 @@
     ]
 
 
 @pytest.mark.parametrize(
     "particle_name",
     ["p", "phi(1020)", "W-", "gamma"],
 )
-def test_create_particle(
-    particle_database: ParticleCollection, particle_name: str
-):
+def test_create_particle(particle_database: ParticleCollection, particle_name: str):
     template_particle = particle_database[particle_name]
     new_particle = create_particle(
         template_particle,
         name="testparticle",
         pid=89,
         mass=1.5,
         width=0.5,
@@ -440,14 +432,30 @@
     assert new_particle.spin == template_particle.spin
     assert new_particle.mass == 1.5
     assert new_particle.width == 0.5
     assert new_particle.baryon_number == template_particle.baryon_number
     assert new_particle.strangeness == template_particle.strangeness
 
 
+def test_create_particle_isospin():
+    template_particle = Particle(
+        name="some particle",
+        pid=0,
+        spin=0,
+        mass=3.14,
+    )
+    new_isospin = Spin(0, 0)
+    new_particle = create_particle(
+        template_particle,
+        isospin=new_isospin,
+    )
+    assert template_particle.isospin != new_isospin
+    assert new_particle.isospin == new_isospin
+
+
 def test_get_name_root(particle_database: ParticleCollection):
     name_roots = {_get_name_root(p.name) for p in particle_database}
     assert name_roots == {
         "a",
         "B",
         "b",
         "chi",
```

### Comparing `qrules-0.9.7/tests/unit/test_pdg.py` & `qrules-0.9.8/tests/unit/test_pdg.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     )
     assert expected_maybe_qq == {item.name for item in maybe_qq_search_results}
 
 
 def test_pdg_size(pdg: ParticleCollection):
     assert len(pdg) in {
         512,  # particle==0.13
-        519,  # particle==0.14, 0.15
-        531,  # particle==0.16
+        519,  # particle==0.14-0.15
+        531,  # particle==0.16-0.20
+        530,  # particle==0.21
     }
     assert len(pdg.filter(lambda p: "~" in p.name)) in {
         165,  # particle==0.13
         172,  # particle==0.14, 0.15
         175,  # particle==0.16
     }
```

### Comparing `qrules-0.9.7/tests/unit/test_qrules.py` & `qrules-0.9.8/tests/unit/test_qrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,10 @@
         allowed_intermediate_particles=resonance_names,
         allowed_interaction_types="strong",
     )
     assert len(reaction.transition_groups) == len(resonance_names)
     final_state = dict(enumerate(final_state_names))
     for transition in reaction.transitions:
         this_final_state = {
-            i: state.particle.name
-            for i, state in transition.final_states.items()
+            i: state.particle.name for i, state in transition.final_states.items()
         }
         assert final_state == this_final_state
```

### Comparing `qrules-0.9.7/tests/unit/test_quantum_numbers.py` & `qrules-0.9.8/tests/unit/test_quantum_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=eval-used, no-self-use
+# pylint: disable=eval-used
 import typing
 from copy import deepcopy
 
 import pytest
 
 from qrules.quantum_numbers import Parity, _to_fraction
 
@@ -43,17 +43,15 @@
         parity = Parity(value)
         from_repr = eval(repr(parity))
         assert from_repr == parity
 
     def test_exceptions(self):
         with pytest.raises(TypeError):
             Parity(1.2)  # type: ignore[arg-type]
-        with pytest.raises(
-            ValueError, match=r"Parity can only be \+1 or -1, not 0"
-        ):
+        with pytest.raises(ValueError, match=r"Parity can only be \+1 or -1, not 0"):
             Parity(0)
 
 
 @pytest.mark.parametrize(
     ("value", "render_plus", "expected"),
     [
         (0, False, "0"),
```

### Comparing `qrules-0.9.7/tests/unit/test_settings.py` & `qrules-0.9.8/tests/unit/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-self-use
 import pytest
 
 from qrules.particle import ParticleCollection
 from qrules.quantum_numbers import EdgeQuantumNumbers as EdgeQN
 from qrules.settings import (
     InteractionType,
     _create_domains,
@@ -52,17 +51,15 @@
     )
     assert domains[EdgeQN.isospin_magnitude] == [0, 0.5, 1]
     assert domains[EdgeQN.isospin_projection] == [-1, -0.5, 0, 0.5, 1]
 
 
 @pytest.mark.parametrize("interaction_type", list(InteractionType))
 @pytest.mark.parametrize("nbody_topology", [False, True])
-@pytest.mark.parametrize(
-    "formalism", ["canonical", "canonical-helicity", "helicity"]
-)
+@pytest.mark.parametrize("formalism", ["canonical", "canonical-helicity", "helicity"])
 def test_create_interaction_settings(
     particle_database: ParticleCollection,
     interaction_type: InteractionType,
     nbody_topology: bool,
     formalism: str,
 ):
     settings = create_interaction_settings(
@@ -70,16 +67,15 @@
         particle_db=particle_database,
         nbody_topology=nbody_topology,
     )
     assert set(settings) == set(InteractionType)
 
     edge_settings, node_settings = settings[interaction_type]
     edge_qn_domains_str = {  # strings are easier to compare with pytest
-        qn_type.__name__: domain
-        for qn_type, domain in edge_settings.qn_domains.items()
+        qn_type.__name__: domain for qn_type, domain in edge_settings.qn_domains.items()
     }
     assert edge_qn_domains_str == {
         "baryon_number": [-1, 0, +1],
         "electron_lepton_number": [-1, 0, +1],
         "muon_lepton_number": [-1, 0, +1],
         "tau_lepton_number": [-1, 0, +1],
         "parity": [-1, +1],
@@ -110,16 +106,15 @@
         expected["l_magnitude"] = [0]
         expected["s_magnitude"] = [0]
     if nbody_topology and formalism != "helicity":
         expected["l_projection"] = [0]
         expected["s_projection"] = [0]
 
     node_qn_domains_str = {  # strings are easier to compare with pytest
-        qn_type.__name__: domain
-        for qn_type, domain in node_settings.qn_domains.items()
+        qn_type.__name__: domain for qn_type, domain in node_settings.qn_domains.items()
     }
     assert node_qn_domains_str == expected
 
 
 @pytest.mark.parametrize(
     ("start", "stop", "expected"),
     [
```

### Comparing `qrules-0.9.7/tests/unit/test_system_control.py` & `qrules-0.9.8/tests/unit/test_system_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pylint: disable=protected-access
+import sys
 from copy import deepcopy
 from typing import List
 
 import pytest
 
 from qrules import InteractionType, ProblemSet, StateTransitionManager
 from qrules._system_control import (
@@ -143,15 +144,17 @@
         ),
         (
             "D+",  # no g and c parity
             0,
             {
                 EdgeQuantumNumbers.pid: 411,
                 EdgeQuantumNumbers.mass: 1.86966,
-                EdgeQuantumNumbers.width: 6.33e-13,
+                EdgeQuantumNumbers.width: (
+                    6.33e-13 if sys.version_info < (3, 7) else 6.37e-13
+                ),
                 EdgeQuantumNumbers.spin_magnitude: 0.0,
                 EdgeQuantumNumbers.spin_projection: 0,
                 EdgeQuantumNumbers.charge: 1,
                 EdgeQuantumNumbers.isospin_magnitude: 0.5,
                 EdgeQuantumNumbers.isospin_projection: 0.5,
                 EdgeQuantumNumbers.strangeness: 0,
                 EdgeQuantumNumbers.charmness: 1,
@@ -194,23 +197,18 @@
     ],
 )
 def test_create_edge_properties(
     particle_name, spin_projection, expected_properties, particle_database
 ):
     particle = particle_database[particle_name]
 
-    assert (
-        create_edge_properties(particle, spin_projection)
-        == expected_properties
-    )
+    assert create_edge_properties(particle, spin_projection) == expected_properties
 
 
-def make_ls_test_graph(
-    angular_momentum_magnitude, coupled_spin_magnitude, particle
-):
+def make_ls_test_graph(angular_momentum_magnitude, coupled_spin_magnitude, particle):
     graph = StateTransitionGraph[ParticleWithSpin](
         topology=Topology(
             nodes={0},
             edges={0: Edge(None, 0)},
         ),
         node_props={
             0: InteractionProperties(
@@ -238,15 +236,15 @@
             )
         },
         edge_props={0: (particle, 0)},
     )
     return graph
 
 
-class TestSolutionFilter:  # pylint: disable=no-self-use
+class TestSolutionFilter:
     @pytest.mark.parametrize(
         ("ls_pairs", "result"),
         [
             ([(1, 0), (1, 1)], 2),
             ([(1, 0), (1, 0)], 1),
         ],
     )
@@ -256,17 +254,15 @@
         for ls_pair in ls_pairs:
             graphs.append(make_ls_test_graph(ls_pair[0], ls_pair[1], pi0))
 
         results = remove_duplicate_solutions(graphs)
         assert len(results) == result
 
         for ls_pair in ls_pairs:
-            graphs.append(
-                make_ls_test_graph_scrambled(ls_pair[0], ls_pair[1], pi0)
-            )
+            graphs.append(make_ls_test_graph_scrambled(ls_pair[0], ls_pair[1], pi0))
         results = remove_duplicate_solutions(graphs)
         assert len(results) == result
 
     @pytest.mark.parametrize(
         ("input_values", "filter_parameters", "result"),
         [
             (
```

### Comparing `qrules-0.9.7/tests/unit/test_topology.py` & `qrules-0.9.8/tests/unit/test_topology.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=eval-used, no-self-use, redefined-outer-name, too-many-arguments
+# pylint: disable=eval-used redefined-outer-name too-many-arguments
 # pyright: reportUnusedImport=false
 import typing
 
 import pytest
 from attrs.exceptions import FrozenInstanceError
 from IPython.lib.pretty import pretty
 
@@ -15,41 +15,14 @@
     _MutableTopology,
     create_isobar_topologies,
     create_n_body_topology,
     get_originating_node_list,
 )
 
 
-@pytest.fixture(scope="session")
-def two_to_three_decay() -> Topology:
-    r"""Create a dummy `Topology`.
-
-    Has the following shape:
-
-    .. code-block::
-
-        e0 -- (N0) -- e2 -- (N1) -- e3 -- (N2) -- e6
-              /               \             \
-            e1                 e4            e5
-    """
-    topology = Topology(
-        nodes={0, 1, 2},
-        edges={
-            0: Edge(None, 0),
-            1: Edge(None, 0),
-            2: Edge(0, 1),
-            3: Edge(1, 2),
-            4: Edge(1, None),
-            5: Edge(2, None),
-            6: Edge(2, None),
-        },
-    )
-    return topology
-
-
 class TestEdge:
     def test_get_connected_nodes(self):
         edge = Edge(1, 2)
         assert edge.get_connected_nodes() == {1, 2}
         edge = Edge(originating_node_id=3)
         assert edge.get_connected_nodes() == {3}
         edge = Edge(ending_node_id=4)
@@ -137,17 +110,15 @@
         with pytest.raises(ValueError, match=r"Edge nr. 7 does not exist"):
             topology.attach_edges_to_node_outgoing([7], 2)
 
 
 class TestSimpleStateTransitionTopologyBuilder:
     def test_two_body_states(self):
         two_body_decay_node = InteractionNode(1, 2)
-        simple_builder = SimpleStateTransitionTopologyBuilder(
-            [two_body_decay_node]
-        )
+        simple_builder = SimpleStateTransitionTopologyBuilder([two_body_decay_node])
         all_graphs = simple_builder.build(1, 3)
         assert len(all_graphs) == 1
 
 
 class TestTopology:
     @pytest.mark.parametrize(
         ("nodes", "edges"),
@@ -194,17 +165,15 @@
             ([], {0: Edge(1, None)}),
             ({0, 1}, {0: Edge(0, None), 1: Edge(None, 1)}),
         ],
     )
     def test_constructor_exceptions(self, nodes, edges):
         with pytest.raises(
             ValueError,
-            match=(
-                r"(not connected to any other node|has non-existing node IDs)"
-            ),
+            match=r"(not connected to any other node|has non-existing node IDs)",
         ):
             assert Topology(nodes=nodes, edges=edges)
 
     @pytest.mark.parametrize("repr_method", [repr, pretty])
     def test_repr_and_eq(self, repr_method, two_to_three_decay: Topology):
         topology = eval(repr_method(two_to_three_decay))
         assert topology == two_to_three_decay
```

### Comparing `qrules-0.9.7/tests/unit/test_transition.py` & `qrules-0.9.8/tests/unit/test_transition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # pyright: reportUnusedImport=false
-# pylint: disable=eval-used, no-self-use
+# pylint: disable=eval-used
 from operator import itemgetter
 from typing import List
 
 import pytest
 from IPython.lib.pretty import pretty
 
 from qrules.particle import (  # noqa: F401
     Parity,
     Particle,
     ParticleCollection,
     ParticleWithSpin,
     Spin,
 )
 from qrules.quantum_numbers import InteractionProperties  # noqa: F401
+from qrules.settings import InteractionType
 from qrules.topology import (  # noqa: F401
     Edge,
     FrozenDict,
     StateTransitionGraph,
     Topology,
 )
 from qrules.transition import State  # noqa: F401
@@ -82,17 +83,15 @@
         state1 = create_state(state_def_1)
         state2 = create_state(state_def_2)
         assert state2 >= state1
 
 
 class TestStateTransition:
     def test_ordering(self, reaction: ReactionInfo):
-        sorted_transitions: List[StateTransition] = sorted(
-            reaction.transitions
-        )
+        sorted_transitions: List[StateTransition] = sorted(reaction.transitions)
         if reaction.formalism.startswith("cano"):
             first = sorted_transitions[0]
             second = sorted_transitions[1]
             assert first.interactions[0].l_magnitude == 0.0
             assert second.interactions[0].l_magnitude == 2.0
             assert first.interactions[1] == second.interactions[1]
             transition_selection = sorted_transitions[::2]
@@ -199,12 +198,37 @@
         stm = StateTransitionManager(
             initial_state=[("J/psi(1S)", [-1, +1])],
             final_state=["p", "p~", "eta"],
         )
         particle_name = "N(753)"
         with pytest.raises(
             LookupError,
-            match=(
-                r"Could not find any matches for allowed intermediate particle"
-            ),
+            match=r"Could not find any matches for allowed intermediate particle",
         ):
-            stm.set_allowed_intermediate_particles([particle_name])
+            stm.set_allowed_intermediate_particles(particle_name)
+
+    def test_regex_pattern(self):
+        stm = StateTransitionManager(
+            initial_state=["Lambda(c)+"],
+            final_state=["p", "K-", "pi+"],
+            allowed_intermediate_particles=["Delta"],
+        )
+        stm.set_allowed_interaction_types([InteractionType.STRONG], node_id=1)
+        problem_sets = stm.create_problem_sets()
+        reaction = stm.find_solutions(problem_sets)
+        assert reaction.get_intermediate_particles().names == [
+            "Delta(1232)++",
+            "Delta(1600)++",
+            "Delta(1620)++",
+            "Delta(1900)++",
+            "Delta(1910)++",
+            "Delta(1920)++",
+        ]
+
+        stm.set_allowed_intermediate_particles(r"^Delta\(\d(60|9[02])0\)", regex=True)
+        problem_sets = stm.create_problem_sets()
+        reaction = stm.find_solutions(problem_sets)
+        assert reaction.get_intermediate_particles().names == [
+            "Delta(1600)++",
+            "Delta(1900)++",
+            "Delta(1920)++",
+        ]
```

