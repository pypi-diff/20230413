# Comparing `tmp/ansible-compat-3.0.1.tar.gz` & `tmp/ansible-compat-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-3.0.1.tar", last modified: Wed Feb  1 12:13:45 2023, max compression
+gzip compressed data, was "ansible-compat-3.0.2.tar", last modified: Thu Apr 13 17:14:09 2023, max compression
```

## Comparing `ansible-compat-3.0.1.tar` & `ansible-compat-3.0.2.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.639363 ansible-compat-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.623363 ansible-compat-3.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 12:13:45.639363 ansible-compat-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.623363 ansible-compat-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26445 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/src/ansible_compat/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.631363 ansible-compat-3.0.1/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-01 12:13:45.000000 ansible-compat-3.0.1/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-01 12:13:45.000000 ansible-compat-3.0.1/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 12:13:45.000000 ansible-compat-3.0.1/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-01 12:13:45.000000 ansible-compat-3.0.1/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 12:13:45.000000 ansible-compat-3.0.1/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.623363 ansible-compat-3.0.1/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.623363 ansible-compat-3.0.1/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/collections/acme.goodies/roles/baz/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.627363 ansible-compat-3.0.1/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:13:45.635363 ansible-compat-3.0.1/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-02-01 12:13:27.000000 ansible-compat-3.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.272825 ansible-compat-3.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.264825 ansible-compat-3.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.264825 ansible-compat-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.280825 ansible-compat-3.0.2/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27606 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.280825 ansible-compat-3.0.2/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/tox.ini
```

### Comparing `ansible-compat-3.0.1/.flake8` & `ansible-compat-3.0.2/.flake8`

 * *Files 12% similar despite different names*

```diff
@@ -53,16 +53,14 @@
   W503,
   H
 
 # Allow certain violations in certain files:
 # per-file-ignores =
 
 # flake8-pytest-style
-# PT001:
-pytest-fixture-no-parentheses = true
 # PT006:
 pytest-parametrize-names-type = tuple
 # PT007:
 pytest-parametrize-values-type = tuple
 pytest-parametrize-values-row-type = tuple
 
 # flake8-rst-docstrings
```

### Comparing `ansible-compat-3.0.1/.github/dependabot.yml` & `ansible-compat-3.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/.github/workflows/release.yml` & `ansible-compat-3.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/.github/workflows/tox.yml` & `ansible-compat-3.0.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/.gitignore` & `ansible-compat-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/.pre-commit-config.yaml` & `ansible-compat-3.0.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,33 @@
     for more information, see https://pre-commit.ci
   skip:
     # https://github.com/pre-commit-ci/issues/issues/55
     - pip-compile
 default_language_version:
   # Needed in order to make pip-compile output predictable.
   python: python3.9
+exclude: |
+  (?x)^(
+    test/assets/.*
+  )$
 repos:
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.261"
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.6"
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
+          - prettier-plugin-sort-json
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
         exclude: >
           (?x)^(
@@ -35,33 +45,33 @@
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
         language_version: python3
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args:
           # https://github.com/pre-commit/mirrors-isort/issues/9#issuecomment-624404082
           - --filter-files
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/flake8.git
     rev: 6.0.0
     hooks:
       - id: flake8
@@ -69,15 +79,15 @@
         additional_dependencies:
           - flake8-2020>=1.6.0
           - flake8-docstrings>=1.5.0
           - flake8-pytest-style>=1.2.2
           - flake8-rst-docstrings>=0.2.3
           - flake8-rst>=0.8.0
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.1.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
           - ansible-core
           - cached_property
@@ -85,36 +95,36 @@
           - pytest
           - pytest-mock
           - subprocess-tee>=0.4.1
           - types-PyYAML
           - types-pkg_resources
           - types-jsonschema>=4.4.9
   - repo: https://github.com/pycqa/pylint
-    rev: v2.16.0b1
+    rev: v3.0.0a6
     hooks:
       - id: pylint
         additional_dependencies:
           - PyYAML
           - pytest
           - typing_extensions
   # Keep last due to being considerably slower than the others:
   - repo: local
     hooks:
       - id: pip-compile-upgrade
         # To run it execute: `pre-commit run pip-compile-upgrade --hook-stage manual`
         name: Upgrade constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking --upgrade -q --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
+        entry: python -m piptools compile --resolver=backtracking --upgrade -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
         pass_filenames: false
         stages:
           - manual
         additional_dependencies:
           - pip-tools>=6.11.0
       - id: pip-compile
         name: Check constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking -q --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
+        entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
         pass_filenames: false
         additional_dependencies:
           - pip-tools>=6.11.0
```

### Comparing `ansible-compat-3.0.1/.readthedocs.yml` & `ansible-compat-3.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/LICENSE` & `ansible-compat-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/PKG-INFO` & `ansible-compat-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 3.0.1
+Version: 3.0.2
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
@@ -33,15 +33,16 @@
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # ansible-compat
 
 [![pypi](https://img.shields.io/pypi/v/ansible-compat.svg)](https://pypi.org/project/ansible-compat/)
-[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/en/latest/)
+[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/)
 [![gh](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml)
 [![codecov.io](https://codecov.io/github/ansible/ansible-compat/coverage.svg?branch=main)](https://codecov.io/github/ansible/ansible-compat?branch=main)
 
 A python package contains functions that facilitate working with various
 versions of Ansible 2.12 and newer.
 
-Documentation is available at [ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/en/latest/).
+Documentation is available at
+[ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/).
```

### Comparing `ansible-compat-3.0.1/README.md` & `ansible-compat-3.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ansible-compat
 
 [![pypi](https://img.shields.io/pypi/v/ansible-compat.svg)](https://pypi.org/project/ansible-compat/)
-[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/en/latest/)
+[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/)
 [![gh](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml)
 [![codecov.io](https://codecov.io/github/ansible/ansible-compat/coverage.svg?branch=main)](https://codecov.io/github/ansible/ansible-compat?branch=main)
 
 A python package contains functions that facilitate working with various
 versions of Ansible 2.12 and newer.
 
-Documentation is available at [ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/en/latest/).
+Documentation is available at
+[ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/).
```

### Comparing `ansible-compat-3.0.1/docs/images/favicon.ico` & `ansible-compat-3.0.2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/docs/images/logo.png` & `ansible-compat-3.0.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/docs/images/logo.svg` & `ansible-compat-3.0.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-3.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/mkdocs.yml` & `ansible-compat-3.0.2/mkdocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,54 @@
+---
 site_name: Ansible Compat Library
 site_url: https://ansible-compat.readthedocs.io/
 repo_url: https://github.com/ansible/ansible-compat
 edit_uri: blob/main/docs/
 copyright: Copyright © 2023 Red Hat, Inc.
-
-strict: true
+docs_dir: docs
+# strict: true
 watch:
   - mkdocs.yml
   - src
   - docs
 
 theme:
-  name: "material"
-  logo: images/logo.svg
-  favicon: images/favicon.ico
+  name: ansible
   features:
     - content.code.copy
     - content.action.edit
-    # - navigation.expand
-    - navigation.instant
-    - navigation.tracking
+    - navigation.expand
     - navigation.sections
+    - navigation.instant
     - navigation.indexes
+    - navigation.tracking
     - toc.integrate
-  palette:
-    - media: "(prefers-color-scheme: light)"
-      primary: teal
-      accent: blue
-      scheme: default
-      toggle:
-        icon: material/brightness-7
-        name: Switch to dark mode
-    - media: "(prefers-color-scheme: dark)"
-      scheme: slate
-      primary: teal
-      accent: blue
-      toggle:
-        icon: material/brightness-4
-        name: Switch to light mode
 extra:
   social:
     - icon: fontawesome/brands/github-alt
       link: https://github.com/ansible/ansible-compat
 nav:
   - examples: index.md
   - api: api.md
 plugins:
   - autorefs
   - search
-  - social
+  - material/social
+  - material/tags
   - mkdocstrings:
       handlers:
         python:
           import:
             - https://docs.python.org/3/objects.inv
           options:
             # heading_level: 2
             docstring_style: sphinx
             docstring_options:
               ignore_init_summary: yes
+
             show_submodules: no
             docstring_section_style: list
             members_order: alphabetical
             show_category_heading: no
             # cannot merge init into class due to parse error...
             # merge_init_into_class: yes
             # separate_signature: yes
@@ -71,33 +57,34 @@
             separate_signature: yes
             # show_bases: false
     # options:
     #   show_root_heading: true
     #   docstring_style: sphinx
 
 markdown_extensions:
+  - markdown_include.include:
+      base_path: docs
   - admonition
   - def_list
   - footnotes
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite
-  - pymdownx.snippets:
-      check_paths: true
   - pymdownx.superfences
   - pymdownx.magiclink:
       repo_url_shortener: true
       repo_url_shorthand: true
       social_url_shorthand: true
       social_url_shortener: true
       user: facelessuser
       repo: pymdown-extensions
       normalize_issue_symbols: true
   - pymdownx.tabbed:
       alternate_style: true
   - toc:
+      toc_depth: 2
       permalink: true
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: !!python/name:pymdownx.superfences.fence_code_format
```

### Comparing `ansible-compat-3.0.1/pyproject.toml` & `ansible-compat-3.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -48,29 +48,15 @@
 [project.urls]
 homepage = "https://github.com/ansible/ansible-compat"
 documentation = "https://ansible-compat.readthedocs.io/"
 repository = "https://github.com/ansible/ansible-compat"
 changelog = "https://github.com/ansible/ansible-compat/releases"
 
 [project.optional-dependencies]
-docs = [
-  "argparse-manpage",
-  "black",
-  "cairosvg",
-  "markdown-include",
-  "mkdocs",
-  "mkdocs-exclude",
-  "mkdocs-material",
-  "mkdocs-material-extensions",
-  "mkdocstrings",
-  "mkdocstrings-python",
-  "pillow",
-  "pymdown-extensions",
-  "slugify",
-]
+docs = ["argparse-manpage", "black", "mkdocs-ansible[lock]>=0.1.2"]
 test = ["coverage", "pip-tools", "pytest>=7.2.0", "pytest-mock", "pytest-plus"]
 
 [tool.coverage.run]
 source = ["src"]
 branch = true
 
 [tool.coverage.report]
@@ -124,9 +110,20 @@
   "duplicate-code",
 ]
 
 [tool.pytest.ini_options]
 # ensure we treat warnings as error
 filterwarnings = ["error"]
 
+[tool.ruff]
+select = ["PT"]
+ignore = [
+  "E501", # we use black
+
+]
+target-version = "py39"
+
+[tool.ruff.flake8-pytest-style]
+parametrize-values-type = "tuple"
+
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `ansible-compat-3.0.1/src/ansible_compat/config.py` & `ansible-compat-3.0.2/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat/constants.py` & `ansible-compat-3.0.2/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat/errors.py` & `ansible-compat-3.0.2/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat/loaders.py` & `ansible-compat-3.0.2/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat/prerun.py` & `ansible-compat-3.0.2/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat/runtime.py` & `ansible-compat-3.0.2/src/ansible_compat/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Ansible runtime environment maanger."""
+"""Ansible runtime environment manager."""
 import importlib
 import json
 import logging
 import os
 import pathlib
 import re
 import shutil
@@ -125,31 +125,34 @@
                 f" ({ansible_module_version}) versions do not match. This "
                 "indicates a broken execution environment."
             )
 
         # For ansible 2.15+ we need to initialize the plugin loader
         # https://github.com/ansible/ansible-lint/issues/2945
         if not Runtime.initialized:  # noqa: F823
+            col_path = [f"{self.cache_dir}/collections"]
             if self.version >= Version("2.15.0.dev0"):
                 # pylint: disable=import-outside-toplevel,no-name-in-module
                 from ansible.plugins.loader import init_plugin_loader
 
-                init_plugin_loader([])
+                init_plugin_loader(col_path)
             else:
                 # noinspection PyProtectedMember
                 from ansible.utils.collection_loader._collection_finder import (  # pylint: disable=import-outside-toplevel
                     _AnsibleCollectionFinder,
                 )
 
                 # noinspection PyProtectedMember
                 # pylint: disable=protected-access
+                col_path += self.config.collections_paths
+                col_path += os.path.dirname(
+                    os.environ.get(ansible_collections_path(), ".")
+                ).split(":")
                 _AnsibleCollectionFinder(
-                    paths=[
-                        os.path.dirname(os.environ.get(ansible_collections_path(), "."))
-                    ]
+                    paths=col_path
                 )._install()  # pylint: disable=protected-access
             Runtime.initialized = True
 
     def clean(self) -> None:
         """Remove content of cache_dir."""
         if self.cache_dir:
             shutil.rmtree(self.cache_dir, ignore_errors=True)
@@ -246,22 +249,27 @@
         # As ansible-galaxy install is not able to automatically determine
         # if the range requires a pre-release, we need to manuall add the --pre
         # flag when needed.
         matches = version_re.search(collection)
         if matches and Version(matches[1]).is_prerelease:
             cmd.append("--pre")
 
-        if destination:
-            cmd.extend(["-p", str(destination)])
+        cpaths: List[str] = self.config.collections_paths
+        if destination and str(destination) not in cpaths:
+            # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
+            # we hack ansible_collections_path instead and inject our own path there.
+            # pylint: disable=no-member
+            cpaths.insert(0, str(destination))
         cmd.append(f"{collection}")
 
         _logger.info("Running from %s : %s", os.getcwd(), " ".join(cmd))
         run = self.exec(
             cmd,
             retry=True,
+            env={**self.environ, ansible_collections_path(): ":".join(cpaths)},
         )
         if run.returncode != 0:
             msg = f"Command returned {run.returncode} code:\n{run.stdout}\n{run.stderr}"
             _logger.error(msg)
             raise InvalidPrerequisiteError(msg)
 
     def install_collection_from_disk(
@@ -289,14 +297,15 @@
             for archive_file in os.listdir(tmp_dir):
                 self.install_collection(
                     os.path.join(tmp_dir, archive_file),
                     destination=destination,
                     force=True,
                 )
 
+    # pylint: disable=too-many-branches
     def install_requirements(
         self, requirement: str, retry: bool = False, offline: bool = False
     ) -> None:
         """Install dependencies from a requirements.yml.
 
         :param requirement: path to requirements.yml file
         :param retry: retry network operations on failures
@@ -331,31 +340,40 @@
                 result = self.exec(cmd, retry=retry)
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     raise AnsibleCommandError(result)
 
         # Run galaxy collection install works on v2 requirements.yml
         if "collections" in reqs_yaml:
-
             cmd = [
                 "ansible-galaxy",
                 "collection",
                 "install",
                 "-v",
             ]
             if offline:
                 _logger.warning(
                     "Skipped installing collection dependencies due to running in offline mode."
                 )
             else:
                 cmd.extend(["-r", requirement])
+                cpaths = self.config.collections_paths
                 if self.cache_dir:
-                    cmd.extend(["-p", f"{self.cache_dir}/collections"])
+                    # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
+                    # we hack ansible_collections_path instead and inject our own path there.
+                    dest_path = f"{self.cache_dir}/collections"
+                    if dest_path not in cpaths:
+                        # pylint: disable=no-member
+                        cpaths.insert(0, dest_path)
                 _logger.info("Running %s", " ".join(cmd))
-                result = self.exec(cmd, retry=retry)
+                result = self.exec(
+                    cmd,
+                    retry=retry,
+                    env={**os.environ, "ANSIBLE_COLLECTIONS_PATH": ":".join(cpaths)},
+                )
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     _logger.error(result.stderr)
                     raise AnsibleCommandError(result)
 
     def prepare_environment(  # noqa: C901
         self,
```

### Comparing `ansible-compat-3.0.1/src/ansible_compat/schema.py` & `ansible-compat-3.0.2/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-3.0.2/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 3.0.1
+Version: 3.0.2
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
@@ -33,15 +33,16 @@
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # ansible-compat
 
 [![pypi](https://img.shields.io/pypi/v/ansible-compat.svg)](https://pypi.org/project/ansible-compat/)
-[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/en/latest/)
+[![docs](https://readthedocs.org/projects/ansible-compat/badge/?version=latest)](https://ansible-compat.readthedocs.io/)
 [![gh](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible/ansible-compat/actions/workflows/tox.yml)
 [![codecov.io](https://codecov.io/github/ansible/ansible-compat/coverage.svg?branch=main)](https://codecov.io/github/ansible/ansible-compat?branch=main)
 
 A python package contains functions that facilitate working with various
 versions of Ansible 2.12 and newer.
 
-Documentation is available at [ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/en/latest/).
+Documentation is available at
+[ansible-compat.readthedocs.io](https://ansible-compat.readthedocs.io/).
```

### Comparing `ansible-compat-3.0.1/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-3.0.2/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.prettierignore
+.prettierrc.yaml
 .readthedocs.yml
 .yamllint
 LICENSE
 README.md
 codecov.yml
 mkdocs.yml
 pyproject.toml
```

### Comparing `ansible-compat-3.0.1/test/assets/validate0_expected.json` & `ansible-compat-3.0.2/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/test/conftest.py` & `ansible-compat-3.0.2/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from typing import Generator
 
 import pytest
 
 from ansible_compat.runtime import Runtime
 
 
-@pytest.fixture
+@pytest.fixture()
 # pylint: disable=unused-argument
 def runtime(scope: str = "session") -> Generator[Runtime, None, None]:
     """Isolated runtime fixture."""
     instance = Runtime(isolated=True)
     yield instance
     instance.clean()
 
 
-@pytest.fixture
+@pytest.fixture()
 # pylint: disable=unused-argument
 def runtime_tmp(
     tmp_path: pathlib.Path, scope: str = "session"
 ) -> Generator[Runtime, None, None]:
     """Isolated runtime fixture using a temp directory."""
     instance = Runtime(project_dir=str(tmp_path), isolated=True)
     yield instance
```

### Comparing `ansible-compat-3.0.1/test/test_config.py` & `ansible-compat-3.0.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/test/test_runtime.py` & `ansible-compat-3.0.2/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/test/test_runtime_example.py` & `ansible-compat-3.0.2/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/test/test_schema.py` & `ansible-compat-3.0.2/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.1/tox.ini` & `ansible-compat-3.0.2/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 commands =
   sh -c "ansible --version | head -n 1"
   # We add coverage options but not making them mandatory as we do not want to force
   # pytest users to run coverage when they just want to run a single test with `pytest -k test`
   coverage run -m pytest {posargs:}
   sh -c "coverage xml || true && coverage report"
+  # We fail if files are modified at the end
+  git diff --exit-code
 commands_pre =
   # safety measure to assure we do not accidentally run tests with broken dependencies
   {envpython} -m pip check
 passenv =
   CURL_CA_BUNDLE  # https proxies, https://github.com/tox-dev/tox/issues/1437
   FORCE_COLOR
   HOME
@@ -59,14 +61,15 @@
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
   py38: PIP_CONSTRAINT = /dev/null
   PRE_COMMIT_COLOR = always
   PYTEST_REQPASS = 80
   FORCE_COLOR = 1
 allowlist_externals =
   ansible
+  git
   sh
 
 [testenv:lint]
 description = Run all linters
 # locked basepython is needed because to keep constrains.txt predictable
 basepython = python3.9
 deps =
@@ -86,15 +89,16 @@
 [testenv:deps]
 description = Bump all test dependencies
 basepython = {[testenv:lint]basepython}
 envdir = {toxworkdir}/lint
 deps = {[testenv:lint]deps}
 skip_install = true
 commands =
-  {[testenv:lint]commands} --hook-stage manual
+  pre-commit run -a --hook-stage manual pip-compile-upgrade
+  {[testenv:lint]commands}
 setenv =
   {[testenv]setenv}
   PIP_CONSTRAINT = /dev/null
 
 [testenv:pkg]
 description =
   Build package, verify metadata, install package and assert behavior when ansible is missing.
```

