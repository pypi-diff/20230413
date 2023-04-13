# Comparing `tmp/swh.deposit-1.2.0.tar.gz` & `tmp/swh.deposit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.deposit-1.2.0.tar", last modified: Mon Aug  1 09:57:14 2022, max compression
+gzip compressed data, was "dist/swh.deposit-1.2.1.tar", last modified: Thu Apr 13 09:27:38 2023, max compression
```

## Comparing `swh.deposit-1.2.0.tar` & `swh.deposit-1.2.1.tar`

### file list

```diff
@@ -1,343 +1,344 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      926 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      375 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      831 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     4315 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3366 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/bin/
--rw-r--r--   0 jenkins    (115) docker     (999)      959 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/Makefile
--rwxr-xr-x   0 jenkins    (115) docker     (999)      130 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/content.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      322 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/create_deposit.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      381 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/create_deposit_atom.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      492 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/create_deposit_with_metadata.sh
--rw-r--r--   0 jenkins    (115) docker     (999)       94 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/default-setup
--rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/download-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)       60 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/home.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      551 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/replace-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)       91 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/service-document.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      256 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/status.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      582 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/update-deposit-with-another-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      252 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/bin/update-status.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      569 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       25 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      240 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3366 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/api/
--rw-r--r--   0 jenkins    (115) docker     (999)     3230 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/api-documentation.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      181 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     8815 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/metadata.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1598 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/register-account.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     8033 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/use-cases.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    14875 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/api/user-manual.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      653 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      169 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/endpoints/
--rw-r--r--   0 jenkins    (115) docker     (999)     3371 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/collection.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1864 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/content.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2342 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/service-document.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3488 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/status.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      996 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/update-media.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      884 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/endpoints/update-metadata.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      179 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      687 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-authentication-basic.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      977 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-authentication-keycloak.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      929 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-create-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1151 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-delete-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1460 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-update-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1005 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-workflow-checking.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1208 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-workflow-loading.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1139 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/deposit-workflow-reception.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      542 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/images/status.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      254 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/index.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/internals/
--rw-r--r--   0 jenkins    (115) docker     (999)     1646 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/internals/authentication.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3613 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/internals/dev-environment.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      299 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/internals/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3534 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/internals/loading-workflow.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4191 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/internals/prod-environment.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       60 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/metadata.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       69 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/spec-api.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/docs/specs/
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/blueprint.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      179 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1216 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/metadata_example.xml
--rw-r--r--   0 jenkins    (115) docker     (999)    11354 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/protocol-reference.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    19155 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/spec-loading.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/specs/spec-meta-deposit.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/docs/user-manual.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      846 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      396 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       73 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/requirements-server.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      138 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/requirements-swh-server.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       41 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      336 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       33 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/resources/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/resources/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)       46 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/resources/deposit/server.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2648 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)      414 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/api/
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9451 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/checks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6034 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/collection.py
--rw-r--r--   0 jenkins    (115) docker     (999)    45841 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1337 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1827 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5267 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/edit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3085 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/edit_media.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/api/private/
--rw-r--r--   0 jenkins    (115) docker     (999)     2606 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7310 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/deposit_check.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7257 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/deposit_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7593 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/deposit_read.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3822 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/deposit_update_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2606 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/private/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1455 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/service_document.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1575 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/state.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2987 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/sword_edit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2322 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1119 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/api/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      362 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/apps.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6072 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/auth.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     1187 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8380 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/cli/admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20150 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/cli/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    28542 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3895 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6080 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1345 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/exception.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/fixtures/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/fixtures/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      194 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/fixtures/deposit_data.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      456 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/gunicorn_config.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/loader/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1397 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/loader/checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)      657 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/loader/tasks.py
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1748 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/manage.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/migrations/
--rw-r--r--   0 jenkins    (115) docker     (999)     5260 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (115) docker     (999)      552 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0002_depositrequest_archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      705 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0003_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      368 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0004_delete_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      909 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0005_auto_20171019_1436.py
--rw-r--r--   0 jenkins    (115) docker     (999)      519 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0006_depositclient_url.py
--rw-r--r--   0 jenkins    (115) docker     (999)      451 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0007_auto_20171129_1609.py
--rw-r--r--   0 jenkins    (115) docker     (999)      918 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0008_auto_20171130_1513.py
--rw-r--r--   0 jenkins    (115) docker     (999)      610 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0009_deposit_parent.py
--rw-r--r--   0 jenkins    (115) docker     (999)      633 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0010_auto_20180110_0953.py
--rw-r--r--   0 jenkins    (115) docker     (999)      884 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0011_auto_20180115_1510.py
--rw-r--r--   0 jenkins    (115) docker     (999)      520 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0012_deposit_status_detail.py
--rw-r--r--   0 jenkins    (115) docker     (999)      463 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)      818 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0014_auto_20180720_1221.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1360 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0015_depositrequest_typemigration.py
--rw-r--r--   0 jenkins    (115) docker     (999)      879 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0016_auto_20190507_1408.py
--rw-r--r--   0 jenkins    (115) docker     (999)      613 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0017_auto_20190925_0906.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12150 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0018_migrate_swhids.py
--rw-r--r--   0 jenkins    (115) docker     (999)      517 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0019_auto_20200519_1035.py
--rw-r--r--   0 jenkins    (115) docker     (999)      583 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0020_auto_20200929_0855.py
--rw-r--r--   0 jenkins    (115) docker     (999)      859 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1858 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/0022_auto_20220223_1542.py
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/migrations/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8440 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/models.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2367 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/parsers.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/settings/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/settings/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3446 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/settings/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1845 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/settings/development.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3115 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/settings/production.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1481 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/settings/testing.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/static/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/static/css/
--rw-r--r--   0 jenkins    (115) docker     (999)    16840 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/css/bootstrap-responsive.min.css
--rw-r--r--   0 jenkins    (115) docker     (999)     8833 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/css/style.css
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/static/img/
--rw-r--r--   0 jenkins    (115) docker     (999)      868 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/arrow-up-small.png
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/static/img/icons/
--rw-r--r--   0 jenkins    (115) docker     (999)     1961 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-32x32.png
--rw-r--r--   0 jenkins    (115) docker     (999)    16114 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
--rw-r--r--   0 jenkins    (115) docker     (999)    17138 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
--rw-r--r--   0 jenkins    (115) docker     (999)    23808 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
--rw-r--r--   0 jenkins    (115) docker     (999)    45250 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/swh-logo-deposit.png
--rw-r--r--   0 jenkins    (115) docker     (999)    11585 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/img/swh-logo-deposit.svg
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/static/robots.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      505 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/api.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      492 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/collection_list.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      840 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/content.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      274 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/deposit_info.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1249 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/deposit_receipt.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      414 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/error.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1357 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/service_document.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1501 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/deposit/state.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1507 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/homepage.html
--rw-r--r--   0 jenkins    (115) docker     (999)     3170 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/layout.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/templates/rest_framework/
--rw-r--r--   0 jenkins    (115) docker     (999)      168 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/templates/rest_framework/api.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2730 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)      921 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_basic_auth.py
--rw-r--r--   0 jenkins    (115) docker     (999)    39027 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_checks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3499 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5097 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_add_to_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5083 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29034 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_atom.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10077 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_binary.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12498 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_multipart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9575 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_reuse_slug.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3860 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4364 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_delete.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7680 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_check.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12966 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4051 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_read_archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17497 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_read_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6857 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_update_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4175 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_schedule.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5193 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_state.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4695 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update.py
--rw-r--r--   0 jenkins    (115) docker     (999)    19861 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update_atom.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13738 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update_binary.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1781 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2435 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_get_file.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_keycloak_auth.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3586 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_parsers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3051 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/api/test_service_document.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/cli/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10494 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/cli/test_admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    38630 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/cli/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6908 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17893 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/archives/
--rw-r--r--   0 jenkins    (115) docker     (999)      102 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/
--rw-r--r--   0 jenkins    (115) docker     (999)     3613 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/codemeta-sample.xml
--rw-r--r--   0 jenkins    (115) docker     (999)       73 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1349 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
--rw-r--r--   0 jenkins    (115) docker     (999)       74 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-empty-body.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      220 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      208 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-ko.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      111 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-minimal.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      421 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1107 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      158 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      501 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      639 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      515 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      601 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      449 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      459 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      413 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      463 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      630 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1229 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data0.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      998 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data2.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      617 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data3.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      695 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1021 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1469 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      449 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-only-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      263 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-update-in-place.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      346 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-cli.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     2060 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-decimal.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-external-identifier.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      527 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1538 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/atom/metadata.xml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.swh.test/
--rw-r--r--   0 jenkins    (115) docker     (999)     1209 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1164 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_test
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.list/
--rw-r--r--   0 jenkins    (115) docker     (999)     1212 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1469 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1240 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test
--rw-r--r--   0 jenkins    (115) docker     (999)     1196 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
--rw-r--r--   0 jenkins    (115) docker     (999)     1196 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
--rw-r--r--   0 jenkins    (115) docker     (999)      792 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/
--rw-r--r--   0 jenkins    (115) docker     (999)     1218 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)      812 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.status/
--rw-r--r--   0 jenkins    (115) docker     (999)     1212 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1636 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/
--rw-r--r--   0 jenkins    (115) docker     (999)     1217 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1634 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
--rw-r--r--   0 jenkins    (115) docker     (999)     1635 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
--rw-r--r--   0 jenkins    (115) docker     (999)      750 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4190 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)      601 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/http_example.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/http_example.org/hello.json
--rw-r--r--   0 jenkins    (115) docker     (999)       13 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/http_example.org/hello_you
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
--rw-r--r--   0 jenkins    (115) docker     (999)     2146 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
--rw-r--r--   0 jenkins    (115) docker     (999)   725946 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
--rw-r--r--   0 jenkins    (115) docker     (999)        5 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_nowhere.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) docker     (999)       21 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
--rw-r--r--   0 jenkins    (115) docker     (999)     1233 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/test_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7064 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2387 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/loader/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2466 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7253 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_client_module.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1050 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2031 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_gunicorn_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)      762 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5134 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_migrations.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7679 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests/test_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/tests_migration/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/tests_migration/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1360 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7713 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh/deposit/xsd/
--rw-r--r--   0 jenkins    (115) docker     (999)     3808 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/xsd/codemeta.xsd
--rw-r--r--   0 jenkins    (115) docker     (999)     2699 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/swh/deposit/xsd/swh.xsd
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     4315 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)    11768 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      162 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      696 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-08-01 09:57:14.000000 swh.deposit-1.2.0/swh.deposit.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1825 2022-08-01 09:57:12.000000 swh.deposit-1.2.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      970 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      375 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/bin/
+-rw-r--r--   0 jenkins    (115) docker     (999)      959 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/Makefile
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      130 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/content.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      322 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      381 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit_atom.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      492 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit_with_metadata.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)       94 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/default-setup
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/download-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)       60 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/home.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      551 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/replace-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)       91 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/service-document.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      256 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/status.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      582 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/update-deposit-with-another-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      252 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/update-status.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      569 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       25 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      240 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3230 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/api-documentation.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      181 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     8816 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/metadata.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1504 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/register-account.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     8033 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/use-cases.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    14875 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/user-manual.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      169 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/endpoints/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3371 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/collection.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1864 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/content.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2342 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/service-document.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3488 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/status.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      996 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/update-media.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/update-metadata.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      687 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-authentication-basic.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      977 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-authentication-keycloak.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      929 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-create-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1151 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-delete-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1460 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-update-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1005 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-checking.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1208 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-loading.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1139 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-reception.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      542 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/status.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      372 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/index.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/internals/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1646 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/authentication.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/dev-environment.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      299 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3534 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/loading-workflow.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4191 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/prod-environment.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       60 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/metadata.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       69 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/spec-api.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/specs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/blueprint.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1216 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/metadata_example.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)    13782 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/protocol-reference.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    26174 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/spec-loading.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/spec-meta-deposit.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/user-manual.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      846 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-server.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-swh-server.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       55 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      336 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       33 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/resources/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/resources/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)       46 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/resources/deposit/server.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2648 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9451 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/checks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6034 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/collection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    46093 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1337 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5267 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/edit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3085 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/edit_media.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/api/private/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2606 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7310 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_check.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7257 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7593 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_read.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_update_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1455 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/service_document.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/state.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2987 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/sword_edit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2328 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1119 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/apps.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/auth.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1187 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8348 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20150 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    28542 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4025 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6080 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1345 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/exception.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/fixtures/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/fixtures/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/fixtures/deposit_data.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/gunicorn_config.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1397 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      657 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/tasks.py
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1748 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/manage.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/migrations/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5260 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0002_depositrequest_archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      705 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0003_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      368 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0004_delete_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      519 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0006_depositclient_url.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      451 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0007_auto_20171129_1609.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      918 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      610 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0009_deposit_parent.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      520 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0012_deposit_status_detail.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      818 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1360 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      879 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12150 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0018_migrate_swhids.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      517 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1858 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8440 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/models.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2367 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/parsers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/settings/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3446 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/development.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3115 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/production.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1481 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/testing.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/css/
+-rw-r--r--   0 jenkins    (115) docker     (999)    16840 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/css/bootstrap-responsive.min.css
+-rw-r--r--   0 jenkins    (115) docker     (999)     8833 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/css/style.css
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/img/
+-rw-r--r--   0 jenkins    (115) docker     (999)      868 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/arrow-up-small.png
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1961 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    16114 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    17138 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    23808 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    45250 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    11585 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.svg
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/robots.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      505 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/api.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/collection_list.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      840 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/content.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      274 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_info.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1249 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_receipt.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/error.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/service_document.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1501 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/state.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1507 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/homepage.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     3170 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/layout.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/rest_framework/
+-rw-r--r--   0 jenkins    (115) docker     (999)      168 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/rest_framework/api.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      921 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_basic_auth.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    39027 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_checks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3499 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5097 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5083 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    29034 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_atom.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10077 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_binary.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14940 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_multipart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9575 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3860 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_delete.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7680 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_check.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12966 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4051 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17497 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6857 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4175 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_schedule.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5193 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_state.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4695 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    19861 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_atom.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13738 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_binary.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1781 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2435 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_get_file.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_keycloak_auth.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3586 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_parsers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_service_document.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10494 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/test_admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    38630 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6908 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17877 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) docker     (999)      102 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1349 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-empty-body.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      220 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      208 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-ko.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      111 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-minimal.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      421 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1107 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      501 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      639 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      459 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      630 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1229 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data0.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      998 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data2.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      617 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data3.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      695 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1021 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-only-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-update-in-place.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      346 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-cli.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2060 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1538 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/metadata.xml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1164 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1240 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test
+-rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
+-rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
+-rw-r--r--   0 jenkins    (115) docker     (999)      792 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)      812 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1636 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1217 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1634 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
+-rw-r--r--   0 jenkins    (115) docker     (999)     1635 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
+-rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4190 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/hello.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       13 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/hello_you
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
+-rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
+-rw-r--r--   0 jenkins    (115) docker     (999)   725946 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
+-rw-r--r--   0 jenkins    (115) docker     (999)        5 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
+-rw-r--r--   0 jenkins    (115) docker     (999)     1233 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7064 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2387 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2466 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7253 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_client_module.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1050 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1258 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2031 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      762 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5134 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_migrations.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7679 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests_migration/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests_migration/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1394 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7713 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/xsd/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3808 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/xsd/codemeta.xsd
+-rw-r--r--   0 jenkins    (115) docker     (999)     2699 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/xsd/swh.xsd
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)    11801 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      162 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      690 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1872 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/tox.ini
```

### Comparing `swh.deposit-1.2.0/.pre-commit-config.yaml` & `swh.deposit-1.2.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+exclude: ^swh/deposit/tests/data/atom/.*$
+
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.3.0
     hooks:
       - id: trailing-whitespace
       - id: check-json
       - id: check-yaml
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8
+    rev: 5.0.4
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-bugbear==22.3.23]
+        additional_dependencies: [flake8-bugbear==22.9.23]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.2
     hooks:
       - id: codespell
         name: Check source code spelling
         args: [-L sur]
         stages: [commit]
 
   - repo: local
@@ -27,15 +29,15 @@
         entry: env DJANGO_SETTINGS_MODULE=swh.deposit.settings.testing mypy
         args: [swh]
         pass_filenames: false
         language: system
         types: [python]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
 
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
       - id: black
```

### Comparing `swh.deposit-1.2.0/CODE_OF_CONDUCT.md` & `swh.deposit-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/LICENSE` & `swh.deposit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/Makefile.local` & `swh.deposit-1.2.1/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/PKG-INFO` & `swh.deposit-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Software Heritage Deposit Server
 Home-page: https://forge.softwareheritage.org/source/swh-deposit/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-deposit
@@ -33,15 +33,15 @@
 This implementation allows interaction between a client (a repository) and a server (SWH
 repository) to deposit software source code archives and associated metadata.
 
 Description
 -----------
 
 Most of the software source code artifacts present in the SWH Archive are gathered by
-the mean of :term:`loader <loader>` workers run by the SWH project from sourve code
+the mean of :term:`loader <loader>` workers run by the SWH project from source code
 origins identified by :term:`lister <lister>` workers. This is a pull mechanism: it's
 the responsibility of the SWH project to gather and collect source code artifacts that
 way.
 
 Alternatively, SWH allows its partners to push source code artifacts and metadata
 directly into the Archive with a push-based mechanism. By using this possibility
 different actors, holding software artifacts or metadata, can preserve their assets
```

### Comparing `swh.deposit-1.2.0/README.rst` & `swh.deposit-1.2.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This implementation allows interaction between a client (a repository) and a server (SWH
 repository) to deposit software source code archives and associated metadata.
 
 Description
 -----------
 
 Most of the software source code artifacts present in the SWH Archive are gathered by
-the mean of :term:`loader <loader>` workers run by the SWH project from sourve code
+the mean of :term:`loader <loader>` workers run by the SWH project from source code
 origins identified by :term:`lister <lister>` workers. This is a pull mechanism: it's
 the responsibility of the SWH project to gather and collect source code artifacts that
 way.
 
 Alternatively, SWH allows its partners to push source code artifacts and metadata
 directly into the Archive with a push-based mechanism. By using this possibility
 different actors, holding software artifacts or metadata, can preserve their assets
```

### Comparing `swh.deposit-1.2.0/bin/Makefile` & `swh.deposit-1.2.1/bin/Makefile`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/bin/replace-deposit-archive.sh` & `swh.deposit-1.2.1/bin/replace-deposit-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/bin/update-deposit-with-another-archive.sh` & `swh.deposit-1.2.1/bin/update-deposit-with-another-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/conftest.py` & `swh.deposit-1.2.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/README.rst` & `swh.deposit-1.2.1/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This implementation allows interaction between a client (a repository) and a server (SWH
 repository) to deposit software source code archives and associated metadata.
 
 Description
 -----------
 
 Most of the software source code artifacts present in the SWH Archive are gathered by
-the mean of :term:`loader <loader>` workers run by the SWH project from sourve code
+the mean of :term:`loader <loader>` workers run by the SWH project from source code
 origins identified by :term:`lister <lister>` workers. This is a pull mechanism: it's
 the responsibility of the SWH project to gather and collect source code artifacts that
 way.
 
 Alternatively, SWH allows its partners to push source code artifacts and metadata
 directly into the Archive with a push-based mechanism. By using this possibility
 different actors, holding software artifacts or metadata, can preserve their assets
```

### Comparing `swh.deposit-1.2.0/docs/api/api-documentation.rst` & `swh.deposit-1.2.1/docs/api/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/api/metadata.rst` & `swh.deposit-1.2.1/docs/api/metadata.rst`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             <codemeta:datePublished>publication date</codemeta:datePublished>
             <codemeta:releaseNotes>comment</codemeta:releaseNotes>
             <codemeta:referencePublication>
               <codemeta:name> article name</codemeta:name>
               <codemeta:identifier> article id </codemeta:identifier>
             </codemeta:referencePublication>
             <codemeta:isPartOf>
-                <codemeta:type> Collaboration/Projet </codemeta:type>
+                <codemeta:type> Collaboration/Project </codemeta:type>
                 <codemeta:name> project name</codemeta:name>
                 <codemeta:identifier> id </codemeta:identifier>
             </codemeta:isPartOf>
             <codemeta:relatedLink>see also </codemeta:relatedLink>
             <codemeta:funding>Sponsor A  </codemeta:funding>
             <codemeta:funding>Sponsor B</codemeta:funding>
             <codemeta:operatingSystem>Platform/OS </codemeta:operatingSystem>
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 -------- Using only Atom ^^^^^^^^^^^^^^^ .. code:: xml <?xml version="1.0"?>
 urn:uuid:1225c695-cfb8-4ebb-aaaa-80da344efa6a 2017-10-07T15:17:08Z some awesome
 author       Using Atom with CodeMeta ^^^^^^^^^^^^^^^^^^^^^^^^ .. code:: xml
 <?xml version="1.0"?>
 urn:uuid:1225c695-cfb8-4ebb-aaaa-80da344efa6a      1785io25c695 origin url
 other identifier, DOI, ARK Domain description key-word 1 key-word 2 creation
 date publication date comment   article name  article id     Collaboration/
-Projet   project name  id   see also  Sponsor A  Sponsor B Platform/OS
+Project   project name  id   see also  Sponsor A  Sponsor B Platform/OS
 dependencies  Version active   license url spdx  .Net Framework 3.0  Python2.3
 author1   Inria   UPMC     author2   Inria   UPMC   http://code.com language 1
 language 2 http://issuetracker.com  Using Atom with DublinCore and CodeMeta
 (multi-schema entry)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ .. code:: xml
 <?xml version="1.0"?>
 urn:uuid:1225c695-cfb8-4ebb-aaaa-80da344efa6a      hal-01587361 doi:10.5281/
```

### Comparing `swh.deposit-1.2.0/docs/api/register-account.rst` & `swh.deposit-1.2.1/docs/api/register-account.rst`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 .. _swh-deposit-register-account-as-deposit-client:
 
 As a deposit client
 -------------------
 
 For this, as a client, you need to register an account on the swh keycloak `production
-<https://archive.softwareheritage.org/oidc/login/?next_path=https://archive.softwareheritage.org/>`_
+<https://archive.softwareheritage.org/oidc/login/>`_
 or `staging
-<https://webapp.staging.swh.network/oidc/login/?next_path=https://webapp.staging.swh.network/>`_
+<https://webapp.staging.swh.network/oidc/login/>`_
 instance.
 
 .. _swh-deposit-register-account-as-sysadm:
 
 As a sysadm
 -----------
```

### Comparing `swh.deposit-1.2.0/docs/api/use-cases.rst` & `swh.deposit-1.2.1/docs/api/use-cases.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/api/user-manual.rst` & `swh.deposit-1.2.1/docs/api/user-manual.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/cli.rst` & `swh.deposit-1.2.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/collection.rst` & `swh.deposit-1.2.1/docs/endpoints/collection.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/content.rst` & `swh.deposit-1.2.1/docs/endpoints/content.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/service-document.rst` & `swh.deposit-1.2.1/docs/endpoints/service-document.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/status.rst` & `swh.deposit-1.2.1/docs/endpoints/status.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/update-media.rst` & `swh.deposit-1.2.1/docs/endpoints/update-media.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/endpoints/update-metadata.rst` & `swh.deposit-1.2.1/docs/endpoints/update-metadata.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-authentication-basic.uml` & `swh.deposit-1.2.1/docs/images/deposit-authentication-basic.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-authentication-keycloak.uml` & `swh.deposit-1.2.1/docs/images/deposit-authentication-keycloak.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-create-chart.uml` & `swh.deposit-1.2.1/docs/images/deposit-create-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-delete-chart.uml` & `swh.deposit-1.2.1/docs/images/deposit-delete-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-update-chart.uml` & `swh.deposit-1.2.1/docs/images/deposit-update-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-workflow-checking.uml` & `swh.deposit-1.2.1/docs/images/deposit-workflow-checking.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-workflow-loading.uml` & `swh.deposit-1.2.1/docs/images/deposit-workflow-loading.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/deposit-workflow-reception.uml` & `swh.deposit-1.2.1/docs/images/deposit-workflow-reception.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/images/status.uml` & `swh.deposit-1.2.1/docs/images/status.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/internals/authentication.rst` & `swh.deposit-1.2.1/docs/internals/authentication.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/internals/dev-environment.rst` & `swh.deposit-1.2.1/docs/internals/dev-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/internals/loading-workflow.rst` & `swh.deposit-1.2.1/docs/internals/loading-workflow.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/internals/prod-environment.rst` & `swh.deposit-1.2.1/docs/internals/prod-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/specs/metadata_example.xml` & `swh.deposit-1.2.1/docs/specs/metadata_example.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/docs/specs/protocol-reference.rst` & `swh.deposit-1.2.1/docs/specs/protocol-reference.rst`

 * *Files 17% similar despite different names*

```diff
@@ -140,19 +140,38 @@
 While the SWORDv2 specification recommends the use of DublinCore_,
 we prefer the CodeMeta_ vocabulary, as we already use it in other components
 of Software Heritage.
 
 While CodeMeta is designed for use in JSON-LD, it is easy to reuse its vocabulary
 and embed it in an XML document, in three steps:
 
-1. use the JSON-LD compact representation of the CodeMeta document
-2. replace ``@context`` declarations with XML namespaces
-3. unfold JSON lists to sibling XML subtrees
+1. use the `JSON-LD compact representation`_ of the CodeMeta document with
+   ``@context: "https://doi.org/10.5063/SCHEMA/CODEMETA-2.0"`` and no other context;
+   which implies that:
+
+   1. Codemeta properties (whether in the ``https://codemeta.github.io/terms/``
+      or ``http://schema.org/`` namespaces) are unprefixed terms
+   2. other properties in the ``http://schema.org/`` namespace use `compact IRIs`_
+      with the ``schema`` prefix
+   3. other properties are absolute
+2. replace ``@context`` declarations with a XMLNS declaration with
+   ``https://doi.org/10.5063/SCHEMA/CODEMETA-2.0`` as namespace
+   (eg. ``xmlns="https://doi.org/10.5063/SCHEMA/CODEMETA-2.0"``
+   or ``xmlns:codemeta="https://doi.org/10.5063/SCHEMA/CODEMETA-2.0"``)
+3. if using a non-default namespace, apply its prefix to any unprefixed term
+   (ie. any term defined in https://doi.org/10.5063/SCHEMA/CODEMETA-2.0 )
+4. add XMLNS declarations for any other prefix (eg. ``xmlns:schema="http://schema.org/"``
+   if any property in that namespace is used)
+5. unfold JSON lists to sibling XML subtrees
 
-For example, this CodeMeta document:
+.. _JSON-LD compact representation: https://www.w3.org/TR/json-ld11/#compacted-document-form
+.. _compact IRIs: https://www.w3.org/TR/json-ld11/#compact-iris
+
+Example Codemeta document
+"""""""""""""""""""""""""
 
 .. code:: json
 
    {
       "@context": "https://doi.org/10.5063/SCHEMA/CODEMETA-2.0",
       "name": "My Software",
       "author": [
@@ -197,14 +216,64 @@
      </codemeta:author>
      <codemeta:author>
        <codemeta:name>Author 2</codemeta:name>
      </codemeta:author>
    </entry>
 
 
+Note that in both these examples, ``codemeta:name`` is used even though
+the property is actually ``http://schema.org/name``.
+
+Example generic JSON-LD document
+""""""""""""""""""""""""""""""""
+
+Another example using properties not part of Codemeta:
+
+.. code:: json
+
+   {
+      "@context": "https://doi.org/10.5063/SCHEMA/CODEMETA-2.0",
+      "name": "My Software",
+      "schema:sameAs": "http://example.org/my-software"
+   }
+
+which is equivalent to:
+
+.. code:: json
+
+   {
+      "@context": "https://doi.org/10.5063/SCHEMA/CODEMETA-2.0",
+      "name": "My Software",
+      "http://schema.org/sameAs": "http://example.org/my-software"
+   }
+
+becomes this XML document:
+
+.. code:: xml
+
+   <?xml version="1.0"?>
+   <atom:entry xmlns:atom="http://www.w3.org/2005/Atom"
+               xmlns="https://doi.org/10.5063/SCHEMA/CODEMETA-2.0"
+               xmlns:schema="http://schema.org/">
+     <name>My Software</name>
+     <schema:sameAs>http://example.org/my-software</schema:sameAs>
+   </atom:entry>
+
+Or, equivalently:
+
+.. code:: xml
+
+   <?xml version="1.0"?>
+   <entry xmlns="http://www.w3.org/2005/Atom"
+          xmlns:codemeta="https://doi.org/10.5063/SCHEMA/CODEMETA-2.0"
+          xmlns:schema="http://schema.org/">
+     <codemeta:name>My Software</codemeta:name>
+     <schema:sameAs>http://example.org/my-software</schema:sameAs>
+   </entry>
+
 .. _mandatory-attributes:
 
 Mandatory attributes
 ^^^^^^^^^^^^^^^^^^^^
 
 All deposits must include:
```

### Comparing `swh.deposit-1.2.0/docs/specs/spec-meta-deposit.rst` & `swh.deposit-1.2.1/docs/specs/spec-meta-deposit.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/mypy.ini` & `swh.deposit-1.2.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/setup.py` & `swh.deposit-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/checks.py` & `swh.deposit-1.2.1/swh/deposit/api/checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/collection.py` & `swh.deposit-1.2.1/swh/deposit/api/collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/common.py` & `swh.deposit-1.2.1/swh/deposit/api/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,23 +580,32 @@
                 "application/x-tar) and 1 atom+xml entry for multipart "
                 "deposit",
                 "You need to provide only 1 application/(zip|x-tar) "
                 "and 1 application/atom+xml content-disposition header "
                 "in the multipart deposit",
             )
 
-        filehandler = data["application/zip"]
-        if not filehandler:
-            filehandler = data["application/x-tar"]
+        filehandler = data["application/zip"] or data["application/x-tar"]
 
+        if filehandler is None:
+            raise DepositError(
+                BAD_REQUEST,
+                "You must provide an archive, either as application/zip or "
+                "application/x-tar",
+            )
         assert isinstance(filehandler, UploadedFile), filehandler
 
         self._check_file_length(filehandler)
         self._check_file_md5sum(filehandler, headers.content_md5sum)
 
+        if data["application/atom+xml"] is None:
+            raise DepositError(
+                BAD_REQUEST, "You must provide an application/atom+xml entry."
+            )
+
         try:
             raw_metadata, metadata_tree = self._read_metadata(
                 data["application/atom+xml"]
             )
         except ParserError:
             raise DepositError(
                 PARSING_ERROR,
@@ -616,15 +625,14 @@
             ARCHIVE_KEY: filehandler,
             RAW_METADATA_KEY: raw_metadata,
         }
         self._deposit_request_put(
             deposit, deposit_request_data, replace_metadata, replace_archives
         )
 
-        assert filehandler is not None
         return Receipt(
             deposit_id=deposit.id,
             deposit_date=deposit.reception_date,
             archive=filehandler.name,
             status=deposit.status,
         )
 
@@ -1006,17 +1014,15 @@
         # This class depends on AuthenticatedAPIView, so request.user.username
         # is always set
         username = request.user.username
         assert username is not None
 
         if self._client is None:
             try:
-                self._client = DepositClient.objects.get(  # type: ignore
-                    username=username
-                )
+                self._client = DepositClient.objects.get(username=username)
             except DepositClient.DoesNotExist:
                 raise DepositError(NOT_FOUND, f"Unknown client name {username}")
 
         assert self._client.username == username
 
         return self._client
```

### Comparing `swh.deposit-1.2.0/swh/deposit/api/content.py` & `swh.deposit-1.2.1/swh/deposit/api/content.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/converters.py` & `swh.deposit-1.2.1/swh/deposit/api/converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/edit.py` & `swh.deposit-1.2.1/swh/deposit/api/edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/edit_media.py` & `swh.deposit-1.2.1/swh/deposit/api/edit_media.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/__init__.py` & `swh.deposit-1.2.1/swh/deposit/api/private/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/deposit_check.py` & `swh.deposit-1.2.1/swh/deposit/api/private/deposit_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/deposit_list.py` & `swh.deposit-1.2.1/swh/deposit/api/private/deposit_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/deposit_read.py` & `swh.deposit-1.2.1/swh/deposit/api/private/deposit_read.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/deposit_update_status.py` & `swh.deposit-1.2.1/swh/deposit/api/private/deposit_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/private/urls.py` & `swh.deposit-1.2.1/swh/deposit/api/private/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Copyright (C) 2017-2022  The Software Heritage developers
+# Copyright (C) 2017-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from django.conf.urls import url
+from django.urls import re_path as url
 
 from ...config import (
     PRIVATE_CHECK_DEPOSIT,
     PRIVATE_GET_DEPOSIT_METADATA,
     PRIVATE_GET_RAW_CONTENT,
     PRIVATE_LIST_DEPOSITS,
     PRIVATE_LIST_DEPOSITS_DATATABLES,
```

### Comparing `swh.deposit-1.2.0/swh/deposit/api/service_document.py` & `swh.deposit-1.2.1/swh/deposit/api/service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/state.py` & `swh.deposit-1.2.1/swh/deposit/api/state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/sword_edit.py` & `swh.deposit-1.2.1/swh/deposit/api/sword_edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/api/urls.py` & `swh.deposit-1.2.1/swh/deposit/api/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (C) 2017-2021  The Software Heritage developers
+# Copyright (C) 2017-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """SWH's deposit api URL Configuration
 
 """
 
-from django.conf.urls import url
 from django.shortcuts import render
+from django.urls import re_path as url
 
 from ..config import COL_IRI, CONT_FILE_IRI, EDIT_IRI, EM_IRI, SD_IRI, SE_IRI, STATE_IRI
 from .collection import CollectionAPI
 from .content import ContentAPI
 from .edit import EditAPI
 from .edit_media import EditMediaAPI
 from .service_document import ServiceDocumentAPI
```

### Comparing `swh.deposit-1.2.0/swh/deposit/api/utils.py` & `swh.deposit-1.2.1/swh/deposit/api/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/auth.py` & `swh.deposit-1.2.1/swh/deposit/auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/cli/__init__.py` & `swh.deposit-1.2.1/swh/deposit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/cli/admin.py` & `swh.deposit-1.2.1/swh/deposit/cli/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     if not collection:
         collection = username
     # create the collection if it does not exist
     collection_ = _create_collection(collection)
 
     # user create/update
     try:
-        user = DepositClient.objects.get(username=username)  # type: ignore
+        user = DepositClient.objects.get(username=username)
         click.echo(f"Update user '{username}'.")
         action_done = "updated"
     except DepositClient.DoesNotExist:
         click.echo(f"Create user '{username}'.")
         user = DepositClient(username=username)
         user.save()
         action_done = "created"
@@ -162,15 +162,15 @@
 @click.pass_context
 def user_exists(ctx, username: str):
     """Check if user exists."""
     # to avoid loading too early django namespaces
     from swh.deposit.models import DepositClient
 
     try:
-        DepositClient.objects.get(username=username)  # type: ignore
+        DepositClient.objects.get(username=username)
         click.echo(f"User {username} exists.")
         ctx.exit(0)
     except DepositClient.DoesNotExist:
         click.echo(f"User {username} does not exist.")
         ctx.exit(1)
```

### Comparing `swh.deposit-1.2.0/swh/deposit/cli/client.py` & `swh.deposit-1.2.1/swh/deposit/cli/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/client.py` & `swh.deposit-1.2.1/swh/deposit/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/config.py` & `swh.deposit-1.2.1/swh/deposit/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2017-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from swh.core import config
 from swh.deposit import __version__
 from swh.model.model import MetadataAuthority, MetadataAuthorityType, MetadataFetcher
 from swh.scheduler import get_scheduler
 from swh.scheduler.interface import SchedulerInterface
 from swh.storage import get_storage
@@ -54,44 +54,45 @@
 
 DEFAULT_CONFIG = {
     "max_upload_size": 209715200,
     "checks": True,
 }
 
 
-def setup_django_for(platform=None, config_file=None):
-    """Setup function for command line tools (swh.deposit.create_user) to
-       initialize the needed db access.
+def setup_django_for(platform: Optional[str] = None, config_file: Optional[str] = None):
+    """Setup function for command line tools (e.g. swh.deposit.create_user) to
+    initialize the needed db access.
 
     Note:
         Do not import any django related module prior to this function
-        call. Otherwise, this will raise an
-        django.core.exceptions.ImproperlyConfigured error message.
+        call. Otherwise, this will raise a django.core.exceptions.ImproperlyConfigured
+        error message.
 
     Args:
-        platform (str): the platform the scheduling is running
-        config_file (str): Extra configuration file (typically for the
-                           production platform)
+        platform: the platform to use when running program (e.g. cli, ...)
+        config_file: Extra configuration file (typically for the production platform)
 
     Raises:
-        ValueError in case of wrong platform inputs.
+        ValueError in case of wrong platform inputs
 
     """
     if platform is not None:
         if platform not in AUTHORIZED_PLATFORMS:
-            raise ValueError("Platform should be one of %s" % AUTHORIZED_PLATFORMS)
+            raise ValueError(f"Platform should be one of {AUTHORIZED_PLATFORMS}")
         if "DJANGO_SETTINGS_MODULE" not in os.environ:
-            os.environ["DJANGO_SETTINGS_MODULE"] = "swh.deposit.settings.%s" % platform
+            os.environ["DJANGO_SETTINGS_MODULE"] = f"swh.deposit.settings.{platform}"
 
     if config_file:
+        # Hack to set the environment variable which in some cases is required (e.g.
+        # production)
         os.environ.setdefault("SWH_CONFIG_FILENAME", config_file)
 
-    import django
+    from django import setup
 
-    django.setup()
+    setup()
 
 
 class APIConfig:
     """API Configuration centralized class. This loads explicitly the configuration file out
     of the SWH_CONFIG_FILENAME environment variable.
 
     """
```

### Comparing `swh.deposit-1.2.0/swh/deposit/errors.py` & `swh.deposit-1.2.1/swh/deposit/errors.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/exception.py` & `swh.deposit-1.2.1/swh/deposit/exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/loader/checker.py` & `swh.deposit-1.2.1/swh/deposit/loader/checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/loader/tasks.py` & `swh.deposit-1.2.1/swh/deposit/loader/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/manage.py` & `swh.deposit-1.2.1/swh/deposit/manage.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0001_initial.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0002_depositrequest_archive.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0002_depositrequest_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0003_temporaryarchive.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0003_temporaryarchive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0005_auto_20171019_1436.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0006_depositclient_url.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0006_depositclient_url.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0008_auto_20171130_1513.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0009_deposit_parent.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0009_deposit_parent.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0010_auto_20180110_0953.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0011_auto_20180115_1510.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0012_deposit_status_detail.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0012_deposit_status_detail.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0014_auto_20180720_1221.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0015_depositrequest_typemigration.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0016_auto_20190507_1408.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0017_auto_20190925_0906.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0018_migrate_swhids.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0018_migrate_swhids.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0019_auto_20200519_1035.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0020_auto_20200929_0855.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/migrations/0022_auto_20220223_1542.py` & `swh.deposit-1.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/models.py` & `swh.deposit-1.2.1/swh/deposit/models.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/parsers.py` & `swh.deposit-1.2.1/swh/deposit/parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/settings/common.py` & `swh.deposit-1.2.1/swh/deposit/settings/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/settings/development.py` & `swh.deposit-1.2.1/swh/deposit/settings/development.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/settings/production.py` & `swh.deposit-1.2.1/swh/deposit/settings/production.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/settings/testing.py` & `swh.deposit-1.2.1/swh/deposit/settings/testing.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/css/bootstrap-responsive.min.css` & `swh.deposit-1.2.1/swh/deposit/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/css/style.css` & `swh.deposit-1.2.1/swh/deposit/static/css/style.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/arrow-up-small.png` & `swh.deposit-1.2.1/swh/deposit/static/img/arrow-up-small.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-32x32.png` & `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png` & `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png` & `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png` & `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/swh-logo-deposit.png` & `swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/static/img/swh-logo-deposit.svg` & `swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.svg`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/deposit/content.xml` & `swh.deposit-1.2.1/swh/deposit/templates/deposit/content.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/deposit/deposit_receipt.xml` & `swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_receipt.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/deposit/service_document.xml` & `swh.deposit-1.2.1/swh/deposit/templates/deposit/service_document.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/deposit/state.xml` & `swh.deposit-1.2.1/swh/deposit/templates/deposit/state.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/homepage.html` & `swh.deposit-1.2.1/swh/deposit/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/templates/layout.html` & `swh.deposit-1.2.1/swh/deposit/templates/layout.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/conftest.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_basic_auth.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_checks.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_add_to_origin.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_list.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_atom.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_binary.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_post_multipart.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_multipart.py`

 * *Files 12% similar despite different names*

```diff
@@ -267,15 +267,15 @@
                 == atom_dataset["entry-data-deposit-binary"]
             )
 
 
 # FAILURE scenarios
 
 
-def test_post_deposit_multipart_only_archive_and_atom_entry(
+def test_post_deposit_multipart_only_one_archive_and_atom_entry(
     authenticated_client, deposit_collection
 ):
     """Multipart deposit only accepts one archive and one atom+xml"""
     # given
     url = reverse(COL_IRI, args=[deposit_collection.name])
 
     archive_content = b"some content representing archive"
@@ -387,7 +387,85 @@
 
     # then
     assert response.status_code == status.HTTP_413_REQUEST_ENTITY_TOO_LARGE
     assert b"Upload size limit exceeded" in response.content
 
     with pytest.raises(Deposit.DoesNotExist):
         Deposit.objects.get(external_id=external_id)
+
+
+def test_post_deposit_atom_400_multipart_no_atom(
+    authenticated_client, deposit_collection, atom_dataset, deposit_user, sample_archive
+):
+    """Posting without an atom body should return a 400 response"""
+    origin_url = "http://example.org/foo"
+
+    archive = InMemoryUploadedFile(
+        BytesIO(sample_archive["data"]),
+        field_name=sample_archive["name"],
+        name=sample_archive["name"],
+        content_type="application/x-tar",
+        size=sample_archive["length"],
+        charset=None,
+    )
+
+    atom_data = atom_dataset["entry-data0"] % origin_url
+
+    atom_entry = InMemoryUploadedFile(
+        BytesIO(atom_data.encode("utf-8")),
+        field_name="atom0",
+        name="atom0",
+        content_type="application/x-foobar",  # should be application/atom+xml
+        size=len(atom_data),
+        charset="utf-8",
+    )
+
+    response = authenticated_client.post(
+        reverse(COL_IRI, args=[deposit_collection.name]),
+        format="multipart",
+        data={
+            "archive": archive,
+            "atom_entry": atom_entry,
+        },
+    )
+
+    assert response.status_code == status.HTTP_400_BAD_REQUEST
+    assert "provide an application/atom+xml entry" in response.content.decode()
+
+
+def test_post_deposit_atom_400_multipart_no_archive(
+    authenticated_client, deposit_collection, atom_dataset, deposit_user, sample_archive
+):
+    """Posting without an atom body should return a 400 response"""
+    origin_url = "http://example.org/foo"
+
+    archive = InMemoryUploadedFile(
+        BytesIO(sample_archive["data"]),
+        field_name=sample_archive["name"],
+        name=sample_archive["name"],
+        content_type="application/x-foobar",  # should be application/x-tar
+        size=sample_archive["length"],
+        charset=None,
+    )
+
+    atom_data = atom_dataset["entry-data0"] % origin_url
+
+    atom_entry = InMemoryUploadedFile(
+        BytesIO(atom_data.encode("utf-8")),
+        field_name="atom0",
+        name="atom0",
+        content_type="application/atom+xml",
+        size=len(atom_data),
+        charset="utf-8",
+    )
+
+    response = authenticated_client.post(
+        reverse(COL_IRI, args=[deposit_collection.name]),
+        format="multipart",
+        data={
+            "archive": archive,
+            "atom_entry": atom_entry,
+        },
+    )
+
+    assert response.status_code == status.HTTP_400_BAD_REQUEST
+    assert "provide an archive" in response.content.decode()
```

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_collection_reuse_slug.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_converters.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_delete.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_delete.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_check.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_list.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_read_archive.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_read_metadata.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_private_update_status.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_schedule.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_schedule.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_state.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update_atom.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_deposit_update_binary.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_exception.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_get_file.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_get_file.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_keycloak_auth.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_keycloak_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_parsers.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/api/test_service_document.py` & `swh.deposit-1.2.1/swh/deposit/tests/api/test_service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/cli/test_admin.py` & `swh.deposit-1.2.1/swh/deposit/tests/cli/test_admin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/cli/test_client.py` & `swh.deposit-1.2.1/swh/deposit/tests/cli/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/common.py` & `swh.deposit-1.2.1/swh/deposit/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/conftest.py` & `swh.deposit-1.2.1/swh/deposit/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
     """
     from swh.deposit.models import DepositClient
 
     user_data_d = deepcopy(user_data)
     user_data_d.pop("collection", None)
     passwd = user_data_d.pop("password", None)
-    user, _ = DepositClient.objects.get_or_create(  # type: ignore
+    user, _ = DepositClient.objects.get_or_create(
         username=user_data_d["username"],
         defaults={**user_data_d, "collections": [collection.id]},
     )
     if passwd:
         user.set_password(passwd)
         user.save()
```

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/codemeta-sample.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data-with-swhid.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data0.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data0.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data1.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data1.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data2.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-data3.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data3.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/entry-list-deposits.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-decimal.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/atom/metadata.xml` & `swh.deposit-1.2.1/swh/deposit/tests/data/atom/metadata.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.swh.test/1_test` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status` & `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/common.py` & `swh.deposit-1.2.1/swh/deposit/tests/loader/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/conftest.py` & `swh.deposit-1.2.1/swh/deposit/tests/loader/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta` & `swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw` & `swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/test_checker.py` & `swh.deposit-1.2.1/swh/deposit/tests/loader/test_checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/test_client.py` & `swh.deposit-1.2.1/swh/deposit/tests/loader/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/loader/test_tasks.py` & `swh.deposit-1.2.1/swh/deposit/tests/loader/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_backend.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_client_module.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_client_module.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_common.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_gunicorn_config.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_init.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_migrations.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/tests/test_utils.py` & `swh.deposit-1.2.1/swh/deposit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/urls.py` & `swh.deposit-1.2.1/swh/deposit/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright (C) 2017-2021  The Software Heritage developers
+# Copyright (C) 2017-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """SWH's main deposit URL Configuration
 
 """
 from __future__ import annotations
 
 from typing import Sequence, Union
 
-from django.conf.urls import include, url
+from django.conf.urls import include
 from django.shortcuts import render
+from django.urls import re_path as url
 from django.views.generic.base import RedirectView
 from rest_framework.urlpatterns import format_suffix_patterns
 
 try:
     from django.urls import URLPattern, URLResolver
 except ImportError:
     # retro-compatibility workaround, django 1.11.29 [1] does not expose the previous
```

### Comparing `swh.deposit-1.2.0/swh/deposit/utils.py` & `swh.deposit-1.2.1/swh/deposit/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/xsd/codemeta.xsd` & `swh.deposit-1.2.1/swh/deposit/xsd/codemeta.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh/deposit/xsd/swh.xsd` & `swh.deposit-1.2.1/swh/deposit/xsd/swh.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.0/swh.deposit.egg-info/PKG-INFO` & `swh.deposit-1.2.1/swh.deposit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Software Heritage Deposit Server
 Home-page: https://forge.softwareheritage.org/source/swh-deposit/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-deposit
@@ -33,15 +33,15 @@
 This implementation allows interaction between a client (a repository) and a server (SWH
 repository) to deposit software source code archives and associated metadata.
 
 Description
 -----------
 
 Most of the software source code artifacts present in the SWH Archive are gathered by
-the mean of :term:`loader <loader>` workers run by the SWH project from sourve code
+the mean of :term:`loader <loader>` workers run by the SWH project from source code
 origins identified by :term:`lister <lister>` workers. This is a pull mechanism: it's
 the responsibility of the SWH project to gather and collect source code artifacts that
 way.
 
 Alternatively, SWH allows its partners to push source code artifacts and metadata
 directly into the Archive with a push-based mechanism. By using this possibility
 different actors, holding software artifacts or metadata, can preserve their assets
```

### Comparing `swh.deposit-1.2.0/swh.deposit.egg-info/SOURCES.txt` & `swh.deposit-1.2.1/swh.deposit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 swh/deposit/templates/rest_framework/api.html
 swh/deposit/tests/__init__.py
 swh/deposit/tests/common.py
 swh/deposit/tests/conftest.py
 swh/deposit/tests/test_backend.py
 swh/deposit/tests/test_client_module.py
 swh/deposit/tests/test_common.py
+swh/deposit/tests/test_config.py
 swh/deposit/tests/test_gunicorn_config.py
 swh/deposit/tests/test_init.py
 swh/deposit/tests/test_migrations.py
 swh/deposit/tests/test_utils.py
 swh/deposit/tests/api/__init__.py
 swh/deposit/tests/api/conftest.py
 swh/deposit/tests/api/test_basic_auth.py
```

### Comparing `swh.deposit-1.2.0/tox.ini` & `swh.deposit-1.2.1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [tox]
+requires =
+  tox>4
 envlist=flake8,mypy,py3-django2,py3-django3
 
 [testenv]
 extras =
   testing
 deps =
   # the dependency below is needed for now as a workaround for
@@ -18,66 +20,64 @@
   !dev: --cov {envsitepackagesdir}/swh/deposit --cov-branch \
         {envsitepackagesdir}/swh/deposit \
         {posargs}
 
 [testenv:black]
 skip_install = true
 deps =
-  black==22.3.0
+  black==22.10.0
 commands =
   {envpython} -m black --check swh
 
 [testenv:flake8]
 skip_install = true
 deps =
-  flake8==4.0.1
-  flake8-bugbear==22.3.23
+  flake8==5.0.4
+  flake8-bugbear==22.9.23
+  pycodestyle==2.9.1
 commands =
   {envpython} -m flake8 \
     --exclude=.tox,.git,__pycache__,.tox,.eggs,*.egg,swh/deposit/migrations
 
 [testenv:mypy]
 setenv = DJANGO_SETTINGS_MODULE=swh.deposit.settings.testing
 extras =
   testing
 deps =
-  mypy==0.942
+  mypy==1.0.1
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

