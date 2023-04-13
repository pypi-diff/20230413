# Comparing `tmp/aa_fleetfinder-1.0.0.tar.gz` & `tmp/aa_fleetfinder-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_fleetfinder-1.0.0.tar", last modified: Thu Apr 13 16:45:57 2023, max compression
+gzip compressed data, was "aa_fleetfinder-1.0.0b1.tar", last modified: Tue Jan 10 18:32:50 2023, max compression
```

## Comparing `aa_fleetfinder-1.0.0.tar` & `aa_fleetfinder-1.0.0b1.tar`

### file list

```diff
@@ -1,106 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.114890 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-13 16:45:57.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-13 16:45:57.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:45:57.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:45:56.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 16:45:57.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 16:45:57.000000 aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.114890 aa_fleetfinder-1.0.0/fleetfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.102890 aa_fleetfinder-1.0.0/fleetfinder/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.114890 aa_fleetfinder-1.0.0/fleetfinder/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.102890 aa_fleetfinder-1.0.0/fleetfinder/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.114890 aa_fleetfinder-1.0.0/fleetfinder/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.118890 aa_fleetfinder-1.0.0/fleetfinder/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/multi-select/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.106890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35554 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.110890 aa_fleetfinder-1.0.0/fleetfinder/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.110890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.122890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/css/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/js/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/create-fleet.html
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/edit-fleet.html
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/fleet-details.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/join-fleet.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.110890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/fleetfinder/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/fleetfinder/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/fleetfinder/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 16:45:33.000000 aa_fleetfinder-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 16:45:57.126890 aa_fleetfinder-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.618713 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-10 18:32:50.000000 aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.css
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/multi-select/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.622713 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35554 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.614713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/create-fleet.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/edit-fleet.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/fleet-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/join-fleet.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.618713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/templatetags/fleetfinder_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 18:32:50.626713 aa_fleetfinder-1.0.0b1/fleetfinder/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/fleetfinder/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-10 18:32:34.000000 aa_fleetfinder-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-10 18:32:50.630713 aa_fleetfinder-1.0.0b1/setup.cfg
```

### Comparing `aa_fleetfinder-1.0.0/CHANGELOG.md` & `aa_fleetfinder-1.0.0b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 
 ## [In Development] - Unreleased
 
 
-## [1.0.0] - 2023-04-13
-
-### Added
-
-- German translation
-
-
 ## [1.0.0-beta.1] - 2023-01-10
 
 ### Changed
 
 - Migrations reset
```

### Comparing `aa_fleetfinder-1.0.0/LICENSE` & `aa_fleetfinder-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/aa_fleetfinder.egg-info/SOURCES.txt` & `aa_fleetfinder-1.0.0b1/aa_fleetfinder.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,14 @@
 fleetfinder/auth_hooks.py
 fleetfinder/constants.py
 fleetfinder/models.py
 fleetfinder/providers.py
 fleetfinder/tasks.py
 fleetfinder/urls.py
 fleetfinder/views.py
-fleetfinder/locale/de/LC_MESSAGES/django.mo
-fleetfinder/locale/de/LC_MESSAGES/django.po
-fleetfinder/locale/es/LC_MESSAGES/django.po
-fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
-fleetfinder/locale/it_IT/LC_MESSAGES/django.po
-fleetfinder/locale/ja/LC_MESSAGES/django.po
-fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
-fleetfinder/locale/ru/LC_MESSAGES/django.mo
-fleetfinder/locale/ru/LC_MESSAGES/django.po
-fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
 fleetfinder/migrations/0001_initial.py
 fleetfinder/migrations/__init__.py
 fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
 fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
 fleetfinder/static/fleetfinder/css/fleetfinder.css
 fleetfinder/static/fleetfinder/css/fleetfinder.min.css
 fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
```

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/auth_hooks.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/constants.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/constants.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/migrations/0001_initial.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/models.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/css/fleetfinder.css` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js` & `aa_fleetfinder-1.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/tasks.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/create-fleet.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/create-fleet.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
-{% block page_title %}{% translate "Create Fleet" %}{% endblock %}
+{% block page_title %}{% translate "Create fleet" %}{% endblock %}
 
 {% block fleetfinder_block %}
     {% if error %}
         <div class="alert alert-danger" role="alert">{{ error }}</div>
     {%endif%}
 
     <div class="panel panel-primary">
```

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/dashboard.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/edit-fleet.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/edit-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/fleet-details.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/join-fleet.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/join-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html` & `aa_fleetfinder-1.0.0b1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/templatetags/fleetfinder_versioned_static.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/templatetags/fleetfinder_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/tests/test_access.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/tests/test_auth_hooks.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/tests/test_templatetags.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/tests/utils.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/urls.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/fleetfinder/views.py` & `aa_fleetfinder-1.0.0b1/fleetfinder/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.0.0/setup.cfg` & `aa_fleetfinder-1.0.0b1/setup.cfg`

 * *Files identical despite different names*

