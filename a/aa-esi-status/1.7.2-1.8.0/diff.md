# Comparing `tmp/aa_esi_status-1.7.2.tar.gz` & `tmp/aa_esi_status-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_esi_status-1.7.2.tar", last modified: Sun Sep 18 12:26:56 2022, max compression
+gzip compressed data, was "aa_esi_status-1.8.0.tar", last modified: Thu Apr 13 16:12:22 2023, max compression
```

## Comparing `aa_esi_status-1.7.2.tar` & `aa_esi_status-1.8.0.tar`

### file list

```diff
@@ -1,52 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/aa_esi_status.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-18 12:26:56.000000 aa_esi_status-1.7.2/aa_esi_status.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/docs/
--rw-r--r--   0 runner    (1001) docker     (121)   229003 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/docs/aa-esi-status.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/locale/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/locale/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.562635 aa_esi_status-1.7.2/esistatus/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.562635 aa_esi_status-1.7.2/esistatus/static/esistatus/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/static/esistatus/css/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/static/esistatus/css/esistatus.css
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/static/esistatus/css/esistatus.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.562635 aa_esi_status-1.7.2/esistatus/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/templates/esistatus/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templates/esistatus/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templates/esistatus/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/templates/esistatus/partials/
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templates/esistatus/partials/endpoints.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/templates/esistatus/partials/header/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templates/esistatus/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/templatetags/esistatus_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 12:26:56.566635 aa_esi_status-1.7.2/esistatus/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/esistatus/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-18 12:26:41.000000 aa_esi_status-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-18 12:26:56.570635 aa_esi_status-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/aa_esi_status.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   229003 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/docs/aa-esi-status.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/static/esistatus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/static/esistatus/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/static/esistatus/css/esistatus.css
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/static/esistatus/css/esistatus.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/endpoints.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templatetags/esistatus_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/setup.cfg
```

### Comparing `aa_esi_status-1.7.2/CHANGELOG.md` & `aa_esi_status-1.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 
 ## [In Development] - Unreleased
 
 
+## [1.8.0] - 2023-04-13
+
+### Added
+
+- German translation
+
+
 ## [1.7.2] - 2022-09-18
 
 ### Change
 
 - Internal code changes/improvements
 - Minimum dependencies:
   - Alliance Auth>=3.0.0
```

### Comparing `aa_esi_status-1.7.2/LICENSE` & `aa_esi_status-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/PKG-INFO` & `aa_esi_status-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_esi_status
-Version: 1.7.2
+Version: 1.8.0
 Summary: A simple status monitor for ESI
 Home-page: https://github.com/ppfeufer/aa-esi-status
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_esi_status-1.7.2/README.md` & `aa_esi_status-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/aa_esi_status.egg-info/PKG-INFO` & `aa_esi_status-1.8.0/aa_esi_status.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-esi-status
-Version: 1.7.2
+Version: 1.8.0
 Summary: A simple status monitor for ESI
 Home-page: https://github.com/ppfeufer/aa-esi-status
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_esi_status-1.7.2/esistatus/auth_hooks.py` & `aa_esi_status-1.8.0/esistatus/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/docs/aa-esi-status.jpg` & `aa_esi_status-1.8.0/esistatus/docs/aa-esi-status.jpg`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/migrations/0001_initial.py` & `aa_esi_status-1.8.0/esistatus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/templates/esistatus/index.html` & `aa_esi_status-1.8.0/esistatus/templates/esistatus/index.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/templates/esistatus/partials/endpoints.html` & `aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/endpoints.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/templatetags/esistatus_versioned_static.py` & `aa_esi_status-1.8.0/esistatus/templatetags/esistatus_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/tests/test_access.py` & `aa_esi_status-1.8.0/esistatus/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/tests/test_auth_hooks.py` & `aa_esi_status-1.8.0/esistatus/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/tests/test_templatetags.py` & `aa_esi_status-1.8.0/esistatus/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/tests/utils.py` & `aa_esi_status-1.8.0/esistatus/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/esistatus/views.py` & `aa_esi_status-1.8.0/esistatus/views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.7.2/setup.cfg` & `aa_esi_status-1.8.0/setup.cfg`

 * *Files identical despite different names*

