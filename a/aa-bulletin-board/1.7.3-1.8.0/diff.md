# Comparing `tmp/aa_bulletin_board-1.7.3.tar.gz` & `tmp/aa_bulletin_board-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_bulletin_board-1.7.3.tar", last modified: Sun Sep 18 02:04:09 2022, max compression
+gzip compressed data, was "aa_bulletin_board-1.8.0.tar", last modified: Thu Apr 13 14:00:02 2023, max compression
```

## Comparing `aa_bulletin_board-1.7.3.tar` & `aa_bulletin_board-1.8.0.tar`

### file list

```diff
@@ -1,66 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.309538 aa_bulletin_board-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14077 2022-09-18 02:04:09.309538 aa_bulletin_board-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12778 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/0003_group_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)    34280 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0 runner    (1001) docker     (121)    22226 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     7610 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bundles/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.301538 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/partials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/partials/header/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.309538 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6952 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_bulletins.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_user_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/aa_bulletin_board/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 02:04:09.305538 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14077 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-18 02:04:09.000000 aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-18 02:03:53.000000 aa_bulletin_board-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-09-18 02:04:09.309538 aa_bulletin_board-1.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0003_group_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34280 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.033726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_bulletins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/aa_bulletin_board/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:00:02.037726 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:00:01.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 14:00:02.000000 aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 13:59:46.000000 aa_bulletin_board-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-13 14:00:02.041726 aa_bulletin_board-1.8.0/setup.cfg
```

### Comparing `aa_bulletin_board-1.7.3/LICENSE` & `aa_bulletin_board-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/PKG-INFO` & `aa_bulletin_board-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_bulletin_board
-Version: 1.7.3
+Version: 1.8.0
 Summary: A simple bulletin board for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-bulletin-board
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_bulletin_board-1.7.3/README.md` & `aa_bulletin_board-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/auth_hooks.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/forms.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/forms.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/helpers.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/managers.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/managers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/0001_initial.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/migrations/0003_group_restrictions.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/migrations/0003_group_restrictions.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/models.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/models.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css` & `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css` & `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_bulletin_board-1.8.0/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html` & `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html` & `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html` & `aa_bulletin_board-1.8.0/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/templatetags/aa_bulletin_board_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_access.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_auth_hooks.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_auth_hooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 # Standard Library
 from http import HTTPStatus
 
 # Django
 from django.test import TestCase
 from django.urls import reverse
 
-# Alliance Auth
-from allianceauth.tests.auth_utils import AuthUtils
-
 # AA Bulletin Board
 from aa_bulletin_board.tests.utils import create_fake_user
 
 
 class TestHooks(TestCase):
     """
     Test the app hook into allianceauth
@@ -48,19 +45,15 @@
     def test_render_hook_success(self):
         """
         Test should show the link to the app in the navigation to user with access
         :return:
         :rtype:
         """
 
-        self.testuser = AuthUtils.add_permissions_to_user_by_name(
-            ["aa_bulletin_board.basic_access"], self.user_1002
-        )
-
-        self.client.force_login(self.testuser)
+        self.client.force_login(self.user_1002)
 
         response = self.client.get(reverse("authentication:dashboard"))
 
         self.assertEqual(response.status_code, HTTPStatus.OK)
         self.assertContains(response, self.html_menu, html=True)
 
     def test_render_hook_fail(self):
```

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_bulletins.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_bulletins.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_templatetags.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/test_user_interface.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/tests/utils.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/urls.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/urls.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board/views.py` & `aa_bulletin_board-1.8.0/aa_bulletin_board/views.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/PKG-INFO` & `aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-bulletin-board
-Version: 1.7.3
+Version: 1.8.0
 Summary: A simple bulletin board for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-bulletin-board
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_bulletin_board-1.7.3/aa_bulletin_board.egg-info/SOURCES.txt` & `aa_bulletin_board-1.8.0/aa_bulletin_board.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 aa_bulletin_board/views.py
 aa_bulletin_board.egg-info/PKG-INFO
 aa_bulletin_board.egg-info/SOURCES.txt
 aa_bulletin_board.egg-info/dependency_links.txt
 aa_bulletin_board.egg-info/not-zip-safe
 aa_bulletin_board.egg-info/requires.txt
 aa_bulletin_board.egg-info/top_level.txt
+aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
+aa_bulletin_board/locale/de/LC_MESSAGES/django.po
+aa_bulletin_board/locale/es/LC_MESSAGES/django.po
+aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
+aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
+aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
+aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
+aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
+aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
+aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
 aa_bulletin_board/migrations/0001_initial.py
 aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
 aa_bulletin_board/migrations/0003_group_restrictions.py
 aa_bulletin_board/migrations/__init__.py
 aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.css
 aa_bulletin_board/static/aa_bulletin_board/css/aa-bootstrap-fix.min.css
 aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
```

### Comparing `aa_bulletin_board-1.7.3/setup.cfg` & `aa_bulletin_board-1.8.0/setup.cfg`

 * *Files identical despite different names*

