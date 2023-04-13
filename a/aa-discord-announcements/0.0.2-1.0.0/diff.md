# Comparing `tmp/aa_discord_announcements-0.0.2.tar.gz` & `tmp/aa_discord_announcements-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_discord_announcements-0.0.2.tar", last modified: Sun Sep 18 11:28:53 2022, max compression
+gzip compressed data, was "aa_discord_announcements-1.0.0.tar", last modified: Thu Apr 13 15:56:46 2023, max compression
```

## Comparing `aa_discord_announcements-0.0.2.tar` & `aa_discord_announcements-1.0.0.tar`

### file list

```diff
@@ -1,71 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.910353 aa_discord_announcements-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-09-18 11:28:53.910353 aa_discord_announcements-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/helper/
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/helper/discord_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5384 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5883 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.902353 aa_discord_announcements-0.0.2/aa_discord_announcements/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.902353 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/css/
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.902353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.902353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/header/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.910353 aa_discord_announcements-0.0.2/aa_discord_announcements/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.910353 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/aa_discord_announcements/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 11:28:53.906353 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-18 11:28:53.000000 aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-18 11:28:34.000000 aa_discord_announcements-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-09-18 11:28:53.910353 aa_discord_announcements-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/discord_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.641008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.641008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/setup.cfg
```

### Comparing `aa_discord_announcements-0.0.2/LICENSE` & `aa_discord_announcements-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/PKG-INFO` & `aa_discord_announcements-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_discord_announcements
-Version: 0.0.2
+Version: 1.0.0
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Home-page: https://github.com/ppfeufer/aa-discord-announcements
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_discord_announcements-0.0.2/README.md` & `aa_discord_announcements-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,68 +24,52 @@
     )
 
     filter_horizontal = ("restricted_to_group",)
     readonly_fields = ("discord_id",)
     ordering = ("name",)
 
     @classmethod
+    @admin.display(description="Ping Target", ordering="name")
     def _name(cls, obj):
         return obj.name
 
-    _name.short_description = "Ping Target"
-    _name.admin_order_field = "name"
-
     @classmethod
+    @admin.display(description="Restricted to", ordering="restricted_to_group__name")
     def _restricted_to_group(cls, obj):
         names = [x.name for x in obj.restricted_to_group.all().order_by("name")]
 
         if names:
             return ", ".join(names)
 
         return None
 
-    _restricted_to_group.short_description = "Restricted to"
-    _restricted_to_group.admin_order_field = "restricted_to_group__name"
-
 
 @admin.register(Webhook)
 class WebhookAdmin(admin.ModelAdmin):
     """
     WebhookAdmin
     """
 
-    list_display = (
-        "_name",
-        "_url",
-        "_restricted_to_group",
-        "notes",
-        "is_enabled",
-    )
+    list_display = ("_name", "_url", "_restricted_to_group", "notes", "is_enabled")
 
     filter_horizontal = ("restricted_to_group",)
     ordering = ("name",)
 
     @classmethod
+    @admin.display(description="Channel Name", ordering="name")
     def _name(cls, obj):
         return obj.name
 
-    _name.short_description = "Channel Name"
-    _name.admin_order_field = "name"
-
     @classmethod
+    @admin.display(description="Webhook URL", ordering="url")
     def _url(cls, obj):
         return obj.url
 
-    _url.short_description = "Webhook URL"
-    _url.admin_order_field = "url"
-
     @classmethod
+    @admin.display(description="Restricted to", ordering="restricted_to_group__name")
     def _restricted_to_group(cls, obj):
         names = [x.name for x in obj.restricted_to_group.all().order_by("name")]
 
         if names:
             return ", ".join(names)
 
         return None
-
-    _restricted_to_group.short_description = "Restricted to"
-    _restricted_to_group.admin_order_field = "restricted_to_group__name"
```

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/forms.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/forms.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/models.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements/views.py` & `aa_discord_announcements-1.0.0/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/PKG-INFO` & `aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discord-announcements
-Version: 0.0.2
+Version: 1.0.0
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Home-page: https://github.com/ppfeufer/aa-discord-announcements
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_discord_announcements-0.0.2/aa_discord_announcements.egg-info/SOURCES.txt` & `aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,24 @@
 aa_discord_announcements.egg-info/SOURCES.txt
 aa_discord_announcements.egg-info/dependency_links.txt
 aa_discord_announcements.egg-info/not-zip-safe
 aa_discord_announcements.egg-info/requires.txt
 aa_discord_announcements.egg-info/top_level.txt
 aa_discord_announcements/helper/announcement_context.py
 aa_discord_announcements/helper/discord_webhook.py
+aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
 aa_discord_announcements/migrations/0001_initial.py
 aa_discord_announcements/migrations/__init__.py
 aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
 aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
 aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
 aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
 aa_discord_announcements/templates/aa_discord_announcements/base.html
```

### Comparing `aa_discord_announcements-0.0.2/setup.cfg` & `aa_discord_announcements-1.0.0/setup.cfg`

 * *Files identical despite different names*

