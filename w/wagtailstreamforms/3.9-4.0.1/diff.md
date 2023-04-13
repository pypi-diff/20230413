# Comparing `tmp/wagtailstreamforms-3.9.tar.gz` & `tmp/wagtailstreamforms-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtailstreamforms-3.9.tar", last modified: Wed Mar 18 12:54:48 2020, max compression
+gzip compressed data, was "wagtailstreamforms-4.0.1.tar", last modified: Thu Apr 13 14:27:52 2023, max compression
```

## Comparing `wagtailstreamforms-3.9.tar` & `wagtailstreamforms-4.0.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/
--rw-r--r--   0 runner    (1001) docker     (115)     1066 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)       80 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     5411 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     3549 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (115)      103 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1997 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/
--rw-r--r--   0 runner    (1001) docker     (115)      212 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3234 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/blocks.py
--rw-r--r--   0 runner    (1001) docker     (115)      863 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)     5039 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (115)     2334 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/forms.py
--rw-r--r--   0 runner    (1001) docker     (115)     1611 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (115)     5217 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (115)     7797 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (115)     5391 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (115)    11218 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (115)      379 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (115)     5948 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/management/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      898 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/management/commands/prunesubmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/migrations/
--rw-r--r--   0 runner    (1001) docker     (115)    26213 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (115)      554 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/migrations/0002_form_site.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/
--rw-r--r--   0 runner    (1001) docker     (115)     1361 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      318 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (115)     1007 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/file.py
--rw-r--r--   0 runner    (1001) docker     (115)     5752 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/form.py
--rw-r--r--   0 runner    (1001) docker     (115)      744 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/models/submission.py
--rw-r--r--   0 runner    (1001) docker     (115)      307 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (115)     1752 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/streamfield.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/
--rw-r--r--   0 runner    (1001) docker     (115)     1005 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/advanced_settings.html
--rw-r--r--   0 runner    (1001) docker     (115)     1057 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/confirm_copy.html
--rw-r--r--   0 runner    (1001) docker     (115)     1039 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (115)      471 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/form_block.html
--rw-r--r--   0 runner    (1001) docker     (115)     5002 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/index_submissions.html
--rw-r--r--   0 runner    (1001) docker     (115)     1801 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/list_submissions.html
--rw-r--r--   0 runner    (1001) docker     (115)       71 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/non_existent_form.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/partials/
--rw-r--r--   0 runner    (1001) docker     (115)      181 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/partials/form_field.html
--rw-r--r--   0 runner    (1001) docker     (115)      692 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/wagtailadmin/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
--rw-r--r--   0 runner    (1001) docker     (115)     1183 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/templatetags/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1250 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/templatetags/streamforms_tags.py
--rw-r--r--   0 runner    (1001) docker     (115)      789 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      685 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (115)      152 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (115)      989 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/loading.py
--rw-r--r--   0 runner    (1001) docker     (115)      353 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (115)      533 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/
--rw-r--r--   0 runner    (1001) docker     (115)      183 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1527 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     2729 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/copy.py
--rw-r--r--   0 runner    (1001) docker     (115)     2159 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/submission_delete.py
--rw-r--r--   0 runner    (1001) docker     (115)     4057 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/views/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (115)     8519 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (115)     6830 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/wagtailstreamforms_fields.py
--rw-r--r--   0 runner    (1001) docker     (115)     1123 2020-03-18 12:54:43.000000 wagtailstreamforms-3.9/wagtailstreamforms/wagtailstreamforms_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     5411 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2613 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      227 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       19 2020-03-18 12:54:48.000000 wagtailstreamforms-3.9/wagtailstreamforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 14:27:52.654876 wagtailstreamforms-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.638875 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/prunesubmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0002_form_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/models/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/streamfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/advanced_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/form_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/index_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/list_submissions.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/non_existent_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/form_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.642876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/streamforms_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.650876 wagtailstreamforms-4.0.1/wagtailstreamforms/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-13 14:27:50.000000 wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:27:52.646876 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 14:27:52.000000 wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtailstreamforms-3.9/LICENSE` & `wagtailstreamforms-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/PKG-INFO` & `wagtailstreamforms-4.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 3.9
+Version: 4.0.1
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
         ===================
         
-        |CircleCI| |Codecov|
+        |tests| |Codecov| |pypi| |github|
         
         Allows you to build forms in the CMS admin area and add them to any StreamField in your site.
         You can add your own fields along with the vast array of default fields which include the likes
         of file fields. Form submissions are controlled by hooks that you can add that process the forms cleaned data.
         Templates can be created which will then appear as choices when you build your form,
         allowing you to display and submit a form however you want.
         
@@ -77,15 +77,15 @@
         Example site with docker
         ------------------------
         
         Clone the repo
         
         .. code:: bash
         
-            $ git clone https://github.com/AccentDesign/wagtailstreamforms.git
+            $ git clone https://github.com/labd/wagtailstreamforms.git
         
         Run the docker container
         
         .. code:: bash
         
             $ cd wagtailstreamforms
             $ docker-compose up
@@ -95,31 +95,38 @@
         .. code:: bash
         
             $ docker-compose exec app bash
             $ python manage.py createsuperuser
         
         Go to http://127.0.0.1:8000
         
-        .. |CircleCI| image:: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev.svg?style=svg
-           :target: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev
-        .. |Codecov| image:: https://codecov.io/gh/AccentDesign/wagtailstreamforms/branch/3-dev/graph/badge.svg
-           :target: https://codecov.io/gh/AccentDesign/wagtailstreamforms
+        .. |tests| image:: https://github.com/labd/wagtailstreamforms/workflows/Python%20Tests/badge.svg
+           :target: https://github.com/labd/wagtailstreamforms/actions?query=workflow%3A%22Python+Tests%22
+        .. |Codecov| image:: https://codecov.io/gh/labd/wagtailstreamforms/branch/master/graph/badge.svg
+           :target: https://codecov.io/gh/labd/wagtailstreamforms
+        .. |pypi| image:: https://img.shields.io/pypi/v/wagtailstreamforms.svg
+           :target: https://pypi.org/project/wagtailstreamforms/
+        .. |github| image:: https://img.shields.io/github/stars/labd/wagtailstreamforms.svg?style=social&logo=github
+           :target: https://github.com/labd/wagtailstreamforms/stargazers
+        
         
 Keywords: wagtail,streamfield,forms,accent,design
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 4
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `wagtailstreamforms-3.9/README.rst` & `wagtailstreamforms-4.0.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Wagtail StreamForms
 ===================
 
-|CircleCI| |Codecov|
+|tests| |Codecov| |pypi| |github|
 
 Allows you to build forms in the CMS admin area and add them to any StreamField in your site.
 You can add your own fields along with the vast array of default fields which include the likes
 of file fields. Form submissions are controlled by hooks that you can add that process the forms cleaned data.
 Templates can be created which will then appear as choices when you build your form,
 allowing you to display and submit a form however you want.
 
@@ -68,15 +68,15 @@
 Example site with docker
 ------------------------
 
 Clone the repo
 
 .. code:: bash
 
-    $ git clone https://github.com/AccentDesign/wagtailstreamforms.git
+    $ git clone https://github.com/labd/wagtailstreamforms.git
 
 Run the docker container
 
 .. code:: bash
 
     $ cd wagtailstreamforms
     $ docker-compose up
@@ -86,11 +86,16 @@
 .. code:: bash
 
     $ docker-compose exec app bash
     $ python manage.py createsuperuser
 
 Go to http://127.0.0.1:8000
 
-.. |CircleCI| image:: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev.svg?style=svg
-   :target: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev
-.. |Codecov| image:: https://codecov.io/gh/AccentDesign/wagtailstreamforms/branch/3-dev/graph/badge.svg
-   :target: https://codecov.io/gh/AccentDesign/wagtailstreamforms
+.. |tests| image:: https://github.com/labd/wagtailstreamforms/workflows/Python%20Tests/badge.svg
+   :target: https://github.com/labd/wagtailstreamforms/actions?query=workflow%3A%22Python+Tests%22
+.. |Codecov| image:: https://codecov.io/gh/labd/wagtailstreamforms/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/labd/wagtailstreamforms
+.. |pypi| image:: https://img.shields.io/pypi/v/wagtailstreamforms.svg
+   :target: https://pypi.org/project/wagtailstreamforms/
+.. |github| image:: https://img.shields.io/github/stars/labd/wagtailstreamforms.svg?style=social&logo=github
+   :target: https://github.com/labd/wagtailstreamforms/stargazers
+
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/blocks.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/blocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 import uuid
 
-from django import forms
+from django.utils.functional import cached_property
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _
-from wagtail.core import blocks
+from django.utils.translation import gettext_lazy as _
+from wagtail import blocks
+
 from wagtailstreamforms.models import Form
+from wagtailstreamforms.wagtail_hooks import WagtailStreamFormsChooser
 
 
 class InfoBlock(blocks.CharBlock):
     def render_form(self, value, prefix="", errors=None):
         field = self.field
         shown_value = value if value else field.help_text
         return mark_safe(
             '<div style="margin-top:5px;padding:0.9em 1.2em;">%s</div>' % shown_value
         )
 
 
 class FormChooserBlock(blocks.ChooserBlock):
-    target_model = Form
-    widget = forms.Select
+    @cached_property
+    def target_model(self):
+        return Form
+
+    @cached_property
+    def widget(self):
+        return WagtailStreamFormsChooser()
 
-    def value_for_form(self, value):
-        if isinstance(value, self.target_model):
-            return value.pk
-        return value
-
-    def value_from_form(self, value):
-        if value == "":
-            return None
-        return super().value_from_form(value)
-
-    def to_python(self, value):
-        if value is None:
-            return value
-        else:
-            try:
-                return self.target_model.objects.get(pk=value)
-            except self.target_model.DoesNotExist:
-                return None
+    def get_form_state(self, value):
+        return self.widget.get_value_data(value)
 
 
 class WagtailFormBlock(blocks.StructBlock):
     form = FormChooserBlock()
     form_action = blocks.CharBlock(
         required=False,
         help_text=_('The form post action. "" or "." for the current page or a url'),
@@ -70,15 +61,14 @@
     def get_context(self, value, parent_context=None):
         context = super().get_context(value, parent_context)
 
         form = value.get("form")
         form_reference = value.get("form_reference")
 
         if form:
-
             # check the context for an invalid form submitted to the page.
             # Use that instead if it has the same unique form_reference number
             invalid_form_reference = context.get("invalid_stream_form_reference")
             invalid_form = context.get("invalid_stream_form")
 
             if (
                 invalid_form_reference
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/conf.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 SETTINGS_PREFIX = "WAGTAILSTREAMFORMS"
 SETTINGS_DEFAULTS = {
     "ADMIN_MENU_LABEL": _("Streamforms"),
     "ADMIN_MENU_ORDER": None,
     "ADVANCED_SETTINGS_MODEL": None,
     "ENABLE_FORM_PROCESSING": True,
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/forms.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict
 
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
+
 from wagtailstreamforms.fields import get_fields
-from wagtailstreamforms.utils.general import get_slug_from_string
 
 
 class BaseForm(forms.Form):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("label_suffix", "")
 
         self.user = kwargs.pop("user", None)
@@ -18,15 +18,15 @@
 
 class FormBuilder:
     def __init__(self, fields):
         self.fields = fields
 
     @property
     def formfields(self):
-        """ Return a list of form fields from the registered fields. """
+        """Return a list of form fields from the registered fields."""
 
         formfields = OrderedDict()
 
         registered_fields = get_fields()
 
         for field in self.fields:
             field_type = field.get("type")
@@ -34,26 +34,17 @@
 
             # check we have the field
             if field_type not in registered_fields:
                 raise AttributeError(
                     "Could not find a registered field of type %s" % field_type
                 )
 
-            # check there is a label
-            if "label" not in field_value:
-                raise AttributeError(
-                    "The block for %s must contain a label of type blocks.CharBlock(required=True)"
-                    % field_type
-                )
-
-            # slugify the label for the field name
-            field_name = get_slug_from_string(field_value.get("label"))
-
             # get the field
             registered_cls = registered_fields[field_type]()
+            field_name = registered_cls.get_formfield_name(field_value)
             field_cls = registered_cls.get_formfield(field_value)
             formfields[field_name] = field_cls
 
         # add fields to uniquely identify the form
         formfields["form_id"] = forms.CharField(widget=forms.HiddenInput)
         formfields["form_reference"] = forms.CharField(widget=forms.HiddenInput)
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/hooks.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     global _searched_for_hooks
     if not _searched_for_hooks:
         list(get_app_submodules("wagtailstreamforms_hooks"))
         _searched_for_hooks = True
 
 
 def get_hooks(hook_name):
-    """ Return the hooks function sorted by their order. """
+    """Return the hooks function sorted by their order."""
 
     search_for_hooks()
     hooks = _hooks.get(hook_name, [])
     hooks = sorted(hooks, key=itemgetter(1))
     fncs = []
     builtin_hook_modules = ["wagtailstreamforms.wagtailstreamforms_hooks"]
     builtin_enabled = get_setting("ENABLE_BUILTIN_HOOKS")
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/locale/es/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo` & `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -298,19 +298,19 @@
 
 #: templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html:22
 msgid "Tuesday"
 msgstr "Dinsdag"
 
 #: templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html:23
 msgid "Wednesday"
-msgstr ""
+msgstr "Woensdag"
 
 #: templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html:24
 msgid "Thursday"
-msgstr "Woensdag"
+msgstr "Donderdag"
 
 #: templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html:25
 msgid "Friday"
 msgstr "Vrijdag"
 
 #: templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html:26
 msgid "Saturday"
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po` & `wagtailstreamforms-4.0.1/wagtailstreamforms/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/management/commands/prunesubmissions.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/management/commands/prunesubmissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
 
 from django.core.management.base import BaseCommand
+
 from wagtailstreamforms.models import FormSubmission
 
 
 class Command(BaseCommand):
     help = "Deletes form submissions older than the provided number of days"
 
     def add_arguments(self, parser):
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/migrations/0001_initial.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Generated by Django 2.0.5 on 2018-05-30 23:03
 
 import django.db.models.deletion
 import wagtail.core.blocks
+from django.db import migrations, models
+
 import wagtailstreamforms.conf
 import wagtailstreamforms.fields
 import wagtailstreamforms.streamfield
-from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [("wagtailcore", "0040_page_draft_title")]
 
     operations = [
         migrations.CreateModel(
             name="Form",
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/migrations/0002_form_site.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/migrations/0002_form_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.6 on 2019-11-22 10:27
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("wagtailstreamforms", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="form",
             name="site",
             field=models.ForeignKey(
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/models/__init__.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
-from .abstract import AbstractFormSetting
-from .file import FormSubmissionFile
-from .form import Form
-from .submission import FormSubmission
+from .abstract import AbstractFormSetting  # noqa
+from .file import FormSubmissionFile  # noqa
+from .form import Form  # noqa
+from .submission import FormSubmission  # noqa
 
 
 def get_form_model_string():
     """
     Get the dotted ``app.Model`` name for the form model as a string.
     Useful for developers making Wagtail plugins that need to refer to the
     form model, such as in foreign keys, but the model itself is not required.
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/models/file.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/models/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models, transaction
 from django.db.models.signals import post_delete
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class FormSubmissionFile(models.Model):
-    """ Data for a form submission file. """
+    """Data for a form submission file."""
 
     submission = models.ForeignKey(
         "FormSubmission",
         verbose_name=_("Submission"),
         on_delete=models.CASCADE,
         related_name="files",
     )
@@ -24,12 +24,12 @@
 
     @property
     def url(self):
         return self.file.url
 
 
 def delete_file_from_storage(instance, **kwargs):
-    """ Cleanup deleted files from disk """
+    """Cleanup deleted files from disk"""
     transaction.on_commit(lambda: instance.file.delete(False))
 
 
 post_delete.connect(delete_file_from_storage, sender=FormSubmissionFile)
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/models/form.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/models/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import uuid
 
+from django.conf import settings
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
-from wagtail.admin.edit_handlers import (
+from django.utils.translation import gettext_lazy as _
+from wagtail import VERSION as WAGTAIL_VERSION
+from wagtail.admin.panels import (
     FieldPanel,
     MultiFieldPanel,
     ObjectList,
     PageChooserPanel,
-    StreamFieldPanel,
     TabbedInterface,
 )
-from wagtail.core.models import Site
+from wagtail.models import Site
+
 from wagtailstreamforms import hooks
 from wagtailstreamforms.conf import get_setting
 from wagtailstreamforms.fields import HookSelectField
 from wagtailstreamforms.forms import FormBuilder
 from wagtailstreamforms.streamfield import FormFieldsStreamField
 from wagtailstreamforms.utils.general import get_slug_from_string
 from wagtailstreamforms.utils.loading import get_advanced_settings_model
@@ -37,15 +39,15 @@
         max_length=255,
         unique=True,
         help_text=_("Used to identify the form in template tags"),
     )
     template_name = models.CharField(
         _("Template"), max_length=255, choices=get_setting("FORM_TEMPLATES")
     )
-    fields = FormFieldsStreamField([], verbose_name=_("Fields"))
+    fields = FormFieldsStreamField([], use_json_field=True, verbose_name=_("Fields"))
     submit_button_text = models.CharField(
         _("Submit button text"), max_length=100, default="Submit"
     )
     success_message = models.CharField(
         _("Success message"),
         blank=True,
         max_length=255,
@@ -84,15 +86,15 @@
         MultiFieldPanel(
             [FieldPanel("success_message"), FieldPanel("error_message")], _("Messages")
         ),
         FieldPanel("process_form_submission_hooks", classname="choice_field"),
         PageChooserPanel("post_redirect_page"),
     ]
 
-    field_panels = [StreamFieldPanel("fields")]
+    field_panels = [FieldPanel("fields")]
 
     edit_handler = TabbedInterface(
         [
             ObjectList(settings_panels, heading=_("General")),
             ObjectList(field_panels, heading=_("Fields")),
         ]
     )
@@ -103,15 +105,15 @@
     class Meta:
         abstract = True
         ordering = ["title"]
         verbose_name = _("Form")
         verbose_name_plural = _("Forms")
 
     def copy(self):
-        """ Copy this form and its fields. """
+        """Copy this form and its fields."""
 
         form_copy = Form(
             site=self.site,
             title=self.title,
             slug=uuid.uuid4(),
             template_name=self.template_name,
             fields=self.fields,
@@ -136,50 +138,54 @@
                 pass
 
         return form_copy
 
     copy.alters_data = True
 
     def get_data_fields(self):
-        """ Returns a list of tuples with (field_name, field_label). """
+        """Returns a list of tuples with (field_name, field_label)."""
 
         data_fields = [("submit_time", _("Submission date"))]
         data_fields += [
             (get_slug_from_string(field["value"]["label"]), field["value"]["label"])
             for field in self.get_form_fields()
         ]
-
+        if getattr(settings, "WAGTAILSTREAMFORMS_SHOW_FORM_REFERENCE", False):
+            data_fields += [("form_reference", _("Form reference"))]
         return data_fields
 
     def get_form(self, *args, **kwargs):
-        """ Returns the form. """
+        """Returns the form."""
 
         form_class = self.get_form_class()
         return form_class(*args, **kwargs)
 
     def get_form_class(self):
-        """ Returns the form class. """
+        """Returns the form class."""
 
         return FormBuilder(self.get_form_fields()).get_form_class()
 
     def get_form_fields(self):
-        """ Returns the form fields stream_data. """
+        """Returns the form field's stream data."""
 
-        form_fields = self.fields.stream_data
+        if WAGTAIL_VERSION >= (2, 12):
+            form_fields = self.fields.raw_data
+        else:
+            form_fields = self.fields.stream_data
         for fn in hooks.get_hooks("construct_submission_form_fields"):
             form_fields = fn(form_fields)
         return form_fields
 
     def get_submission_class(self):
-        """ Returns submission class. """
+        """Returns submission class."""
 
         return FormSubmission
 
     def process_form_submission(self, form):
-        """ Runs each hook if selected in the form. """
+        """Runs each hook if selected in the form."""
 
         for fn in hooks.get_hooks("process_form_submission"):
             if fn.__name__ in self.process_form_submission_hooks:
                 fn(self, form)
 
 
 class Form(AbstractForm):
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/models/submission.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/models/submission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class FormSubmission(models.Model):
-    """ Data for a form submission. """
+    """Data for a form submission."""
 
     form_data = models.TextField(_("Form data"))
     form = models.ForeignKey("Form", verbose_name=_("Form"), on_delete=models.CASCADE)
     submit_time = models.DateTimeField(_("Submit time"), auto_now_add=True)
 
     def get_data(self):
-        """ Returns dict with form data. """
+        """Returns dict with form data."""
         form_data = json.loads(self.form_data)
 
         form_data.update({"submit_time": self.submit_time})
 
         return form_data
 
     def __str__(self):
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/streamfield.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/streamfield.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from django.core.exceptions import ImproperlyConfigured
-from wagtail.core import blocks
-from wagtail.core.fields import StreamField
+from wagtail import blocks
+from wagtail.fields import StreamField
+
 from wagtailstreamforms.fields import BaseField, get_fields
 
 
 class FormFieldStreamBlock(blocks.StreamBlock):
-    """ Add all registered instances of BaseField's get_form_block method to the streamfield. """
+    """Add all registered instances of BaseField's get_form_block method to the streamfield."""
 
     def __init__(self, local_blocks=None, **kwargs):
         self._constructor_kwargs = kwargs
 
         # Note, this is calling BaseStreamBlock's super __init__, not FormFieldStreamBlock's.
-        # We don't want BaseStreamBlock.__init__() to run, because it tries to assign to self.child_blocks,
-        # which we've overridden with a @property. But we DO want Block.__init__() to run.
+        # We don't want BaseStreamBlock.__init__() to run, because it tries to assign to
+        # self.child_blocks, which we've overridden with a @property. But we DO want
+        # Block.__init__() to run.
         super(blocks.BaseStreamBlock, self).__init__()
 
         self._child_blocks = self.base_blocks.copy()
 
         for name, field_class in get_fields().items():
-
             # ensure the field is a subclass of BaseField.
             if not issubclass(field_class, BaseField):
                 raise ImproperlyConfigured(
                     "'%s' must be a subclass of '%s'" % (field_class, BaseField)
                 )
 
             # assign the block
@@ -38,10 +39,10 @@
 
     @property
     def dependencies(self):
         return self._dependencies
 
 
 class FormFieldsStreamField(StreamField):
-    def __init__(self, block_types, **kwargs):
+    def __init__(self, block_types, use_json_field=None, **kwargs):
         super().__init__(block_types, **kwargs)
         self.stream_block = FormFieldStreamBlock(block_types, required=not self.blank)
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/advanced_settings.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/advanced_settings.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/confirm_copy.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_copy.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/confirm_delete.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/index_submissions.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/list_submissions.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/partials/pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templates/streamforms/wagtailadmin/shared/datetimepicker_translations.html`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/templatetags/streamforms_tags.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/templatetags/streamforms_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from urllib.parse import urlencode
 
 from django.template import Library
 from django.utils.safestring import mark_safe
+
 from wagtailstreamforms.blocks import WagtailFormBlock
 from wagtailstreamforms.models import Form
 
 register = Library()
 
 
 @register.simple_tag(takes_context=True)
 def url_replace(context, **kwargs):
-    """ will append kwargs to the existing url replacing any passed in """
+    """will append kwargs to the existing url replacing any passed in"""
 
     query = context["request"].GET.dict()
     query.update(kwargs)
     return urlencode(query)
 
 
 @register.simple_tag(takes_context=True)
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/urls.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.urls import path
+
 from wagtailstreamforms import views
 from wagtailstreamforms.utils.loading import get_advanced_settings_model
 
 SettingsModel = get_advanced_settings_model()
 
 
 urlpatterns = [
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/utils/apps.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/utils/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/utils/loading.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/utils/loading.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.apps import apps
 from django.core.exceptions import ImproperlyConfigured
+
 from wagtailstreamforms.conf import get_setting
 from wagtailstreamforms.models import AbstractFormSetting
 
 
 def get_advanced_settings_model():
     """
     Returns the advanced form settings model if one is defined
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/views/advanced_settings.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/views/advanced_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django import forms
 from django.contrib import messages
 from django.shortcuts import get_object_or_404
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.generic import UpdateView
+
 from wagtailstreamforms.models import Form
 from wagtailstreamforms.utils.loading import get_advanced_settings_model
 from wagtailstreamforms.wagtail_hooks import FormURLHelper
 
 SettingsModel = get_advanced_settings_model()
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/views/copy.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/views/copy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from django import forms
 from django.contrib import messages
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponseRedirect
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.views.generic.detail import (
     BaseDetailView,
     SingleObjectTemplateResponseMixin,
 )
 from wagtail.contrib.modeladmin.helpers import PermissionHelper
+
 from wagtailstreamforms.models import Form
 from wagtailstreamforms.wagtail_hooks import FormURLHelper
 
 
 class CopyForm(forms.Form):
     title = forms.CharField(label=_("New title"))
     slug = forms.SlugField(label=_("New slug"))
@@ -46,15 +47,14 @@
         obj = super().get_object(queryset)
         return obj
 
     def copy(self, request, *args, **kwargs):
         form = CopyForm(request.POST)
 
         if form.is_valid():
-
             copied = self.object.copy()
             copied.title = form.cleaned_data["title"]
             copied.slug = form.cleaned_data["slug"]
 
             copied.save()
 
             self.create_success_message(copied)
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/views/submission_delete.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.contrib import messages
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponseRedirect
 from django.urls import reverse
-from django.utils.translation import ungettext
+from django.utils.translation import ngettext
 from django.views.generic import DeleteView
 from wagtail.contrib.modeladmin.helpers import PermissionHelper
+
 from wagtailstreamforms.models import Form
 
 
 class SubmissionDeleteView(DeleteView):
     model = Form
     template_name = "streamforms/confirm_delete.html"
 
@@ -35,25 +36,38 @@
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["submissions"] = self.get_submissions()
         return context
 
     def delete(self, request, *args, **kwargs):
+        """
+        Django 4.0 uses FormMixin, so this logic has been moved to form_valid.
+
+        This can be removed once Django 3.2 is no longer supported.
+        """
+        success_url = self.get_success_url()
+        submissions = self.get_submissions()
+        count = submissions.count()
+        submissions.delete()
+        self.create_success_message(count)
+        return HttpResponseRedirect(success_url)
+
+    def form_valid(self, request, *args, **kwargs):
         success_url = self.get_success_url()
         submissions = self.get_submissions()
         count = submissions.count()
         submissions.delete()
         self.create_success_message(count)
         return HttpResponseRedirect(success_url)
 
     def create_success_message(self, count):
         messages.success(
             self.request,
-            ungettext(
+            ngettext(
                 "One submission has been deleted.",
                 "%(count)d submissions have been deleted.",
                 count,
             )
             % {"count": count},
         )
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/views/submission_list.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/views/submission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import csv
 import datetime
 
 from django.core.exceptions import PermissionDenied
 from django.http import Http404, HttpResponse
 from django.utils.encoding import smart_str
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.generic import ListView
 from django.views.generic.detail import SingleObjectMixin
 from wagtail.contrib.modeladmin.helpers import PermissionHelper
+
 from wagtailstreamforms import hooks
 from wagtailstreamforms.forms import SelectDateForm
 from wagtailstreamforms.models import Form
 
 
 class SubmissionListView(SingleObjectMixin, ListView):
     paginate_by = 25
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/wagtail_hooks.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtail_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django.conf.urls import include
 from django.contrib import messages
 from django.contrib.admin.utils import quote
-from django.contrib.auth.decorators import login_required
 from django.shortcuts import redirect
 from django.template.response import TemplateResponse
-from django.urls import path, reverse
-from django.utils.decorators import method_decorator
-from django.utils.translation import ugettext_lazy as _
+from django.urls import include, path, reverse
+from django.utils.translation import gettext_lazy as _
+from generic_chooser.views import ModelChooserViewSet
+from generic_chooser.widgets import AdminChooser
 from wagtail.admin import messages as wagtail_messages
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper, ButtonHelper
 from wagtail.contrib.modeladmin.options import ModelAdmin, modeladmin_register
 from wagtail.contrib.modeladmin.views import (
     CreateView,
     DeleteView,
     EditView,
     InspectView,
 )
-from wagtail.core import hooks
+from wagtail import hooks
+
 from wagtailstreamforms import hooks as form_hooks
 from wagtailstreamforms.conf import get_setting
 from wagtailstreamforms.models import Form
 from wagtailstreamforms.utils.loading import get_advanced_settings_model
 from wagtailstreamforms.utils.requests import get_form_instance_from_request
 
 SettingsModel = get_advanced_settings_model()
@@ -83,15 +83,15 @@
                     _("Copy"),
                     _("Copy this form"),
                     classnames_add,
                     classnames_exclude,
                 )
             )
 
-        # users that can do any form actions can vies submissions
+        # users that can do any form actions can view submissions
         buttons.append(
             self.button(
                 pk,
                 "submissions",
                 _("Submissions"),
                 _("Submissions of this form"),
                 classnames_add,
@@ -140,15 +140,15 @@
 @modeladmin_register
 class FormModelAdmin(ModelAdmin):
     model = Form
     list_display = ("title", "slug", "latest_submission", "saved_submissions")
     list_filter = None
     menu_label = _(get_setting("ADMIN_MENU_LABEL"))
     menu_order = get_setting("ADMIN_MENU_ORDER")
-    menu_icon = "icon icon-form"
+    menu_icon = "form"
     search_fields = ("title", "slug")
     button_helper_class = FormButtonHelper
     inspect_view_class = InspectFormView
     create_view_class = CreateFormView
     edit_view_class = EditFormView
     delete_view_class = DeleteFormView
     url_helper_class = FormURLHelper
@@ -193,15 +193,15 @@
     from wagtailstreamforms import urls
 
     return [path("wagtailstreamforms/", include((urls, "wagtailstreamforms")))]
 
 
 @hooks.register("before_serve_page")
 def process_form(page, request, *args, **kwargs):
-    """ Process the form if there is one, if not just continue. """
+    """Process the form if there is one, if not just continue."""
 
     # only process if settings.WAGTAILSTREAMFORMS_ENABLE_FORM_PROCESSING is True
     if not get_setting("ENABLE_FORM_PROCESSING"):
         return
 
     if request.method == "POST":
         form_def = get_form_instance_from_request(request)
@@ -219,15 +219,16 @@
                 # create success message
                 if form_def.success_message:
                     messages.success(
                         request, form_def.success_message, fail_silently=True
                     )
 
                 # redirect to the page defined in the form
-                # or the current page as a fallback - this will avoid refreshing and submitting again
+                # or the current page as a fallback - this will avoid refreshing
+                # and submitting again
                 redirect_page = form_def.post_redirect_page or page
 
                 return redirect(redirect_page.get_url(request), context=context)
 
             else:
                 # update the context with the invalid form and serve the page
                 context.update(
@@ -242,7 +243,30 @@
                 # create error message
                 if form_def.error_message:
                     messages.error(request, form_def.error_message, fail_silently=True)
 
                 return TemplateResponse(
                     request, page.get_template(request, *args, **kwargs), context
                 )
+
+
+class WagtailStreamFormsChooserViewSet(ModelChooserViewSet):
+    icon = "form"
+    model = Form
+    page_title = _("Choose a form")
+    per_page = 10
+
+
+class WagtailStreamFormsChooser(AdminChooser):
+    choose_one_text = _("Choose a form")
+    choose_another_text = _("Choose another form")
+    link_to_chosen_text = _("Edit this form")
+    model = Form
+    choose_modal_url_name = "wagtailstreamforms_chooser:choose"
+    icon = "form"
+
+
+@hooks.register("register_admin_viewset")
+def register_wagtailstreamforms_chooser_viewset():
+    return WagtailStreamFormsChooserViewSet(
+        "wagtailstreamforms_chooser", url_prefix="wagtailstreamforms-chooser"
+    )
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/wagtailstreamforms_fields.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from typing import List, Tuple
+
 from django import forms
-from django.utils.translation import ugettext_lazy as _
-from wagtail.core import blocks
+from django.utils.translation import gettext_lazy as _
+from wagtail import blocks
+
 from wagtailstreamforms.conf import get_setting
 from wagtailstreamforms.fields import BaseField, register
 
 
 class SingleLineTextField(BaseField):
     field_class = forms.CharField
     label = _("Text field (single line)")
@@ -48,15 +51,21 @@
 class DropdownField(BaseField):
     field_class = forms.ChoiceField
     icon = "arrow-down-big"
     label = _("Dropdown field")
 
     def get_options(self, block_value):
         options = super().get_options(block_value)
-        choices = [(c.strip(), c.strip()) for c in block_value.get("choices")]
+        choices: List[Tuple[str, str]] = []
+        for c in block_value.get("choices"):
+            if isinstance(c, dict) and c.get("value"):
+                choices.append((c["value"].strip(), c["value"].strip()))
+            else:
+                choices.append((c.strip(), c.strip()))
+
         if block_value.get("empty_label"):
             choices.insert(0, ("", block_value.get("empty_label")))
         options.update({"choices": choices})
         return options
 
     def get_form_block(self):
         return blocks.StructBlock(
@@ -75,15 +84,20 @@
 class MultiSelectField(BaseField):
     field_class = forms.MultipleChoiceField
     icon = "list-ul"
     label = _("Multiselect field")
 
     def get_options(self, block_value):
         options = super().get_options(block_value)
-        choices = [(c.strip(), c.strip()) for c in block_value.get("choices")]
+        choices: List[Tuple[str, str]] = []
+        for c in block_value.get("choices"):
+            if isinstance(c, dict) and c.get("value"):
+                choices.append((c["value"].strip(), c["value"].strip()))
+            else:
+                choices.append((c.strip(), c.strip()))
         options.update({"choices": choices})
         return options
 
     def get_form_block(self):
         return blocks.StructBlock(
             [
                 ("label", blocks.CharBlock()),
@@ -100,15 +114,20 @@
     field_class = forms.ChoiceField
     widget = forms.widgets.RadioSelect
     icon = "radio-empty"
     label = _("Radio buttons")
 
     def get_options(self, block_value):
         options = super().get_options(block_value)
-        choices = [(c.strip(), c.strip()) for c in block_value.get("choices")]
+        choices: List[Tuple[str, str]] = []
+        for c in block_value.get("choices"):
+            if isinstance(c, dict) and c.get("value"):
+                choices.append((c["value"].strip(), c["value"].strip()))
+            else:
+                choices.append((c.strip(), c.strip()))
         options.update({"choices": choices})
         return options
 
     def get_form_block(self):
         return blocks.StructBlock(
             [
                 ("label", blocks.CharBlock()),
@@ -125,15 +144,20 @@
     field_class = forms.MultipleChoiceField
     widget = forms.widgets.CheckboxSelectMultiple
     icon = "tick-inverse"
     label = _("Checkboxes")
 
     def get_options(self, block_value):
         options = super().get_options(block_value)
-        choices = [(c.strip(), c.strip()) for c in block_value.get("choices")]
+        choices: List[Tuple[str, str]] = []
+        for c in block_value.get("choices"):
+            if isinstance(c, dict) and c.get("value"):
+                choices.append((c["value"].strip(), c["value"].strip()))
+            else:
+                choices.append((c.strip(), c.strip()))
         options.update({"choices": choices})
         return options
 
     def get_form_block(self):
         return blocks.StructBlock(
             [
                 ("label", blocks.CharBlock()),
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms/wagtailstreamforms_hooks.py` & `wagtailstreamforms-4.0.1/wagtailstreamforms/wagtailstreamforms_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 
 from django.template.defaultfilters import pluralize
+
 from wagtailstreamforms.hooks import register
 from wagtailstreamforms.models import FormSubmissionFile
 from wagtailstreamforms.serializers import FormSubmissionSerializer
 
 
 @register("process_form_submission")
 def save_form_submission_data(instance, form):
-    """ saves the form submission data """
+    """saves the form submission data"""
 
     # copy the cleaned_data so we dont mess with the original
     submission_data = form.cleaned_data.copy()
 
     # change the submission data to a count of the files
     for field in form.files.keys():
         count = len(form.files.getlist(field))
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms.egg-info/PKG-INFO` & `wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: wagtailstreamforms
-Version: 3.9
+Version: 4.0.1
 Summary: Wagtail forms in a streamfield
 Home-page: https://github.com/AccentDesign/wagtailstreamforms/
 Author: Stuart George
 Author-email: stuart@accentdesign.co.uk
 License: MIT
 Download-URL: https://pypi.python.org/pypi/wagtailstreamforms
 Description: Wagtail StreamForms
         ===================
         
-        |CircleCI| |Codecov|
+        |tests| |Codecov| |pypi| |github|
         
         Allows you to build forms in the CMS admin area and add them to any StreamField in your site.
         You can add your own fields along with the vast array of default fields which include the likes
         of file fields. Form submissions are controlled by hooks that you can add that process the forms cleaned data.
         Templates can be created which will then appear as choices when you build your form,
         allowing you to display and submit a form however you want.
         
@@ -77,15 +77,15 @@
         Example site with docker
         ------------------------
         
         Clone the repo
         
         .. code:: bash
         
-            $ git clone https://github.com/AccentDesign/wagtailstreamforms.git
+            $ git clone https://github.com/labd/wagtailstreamforms.git
         
         Run the docker container
         
         .. code:: bash
         
             $ cd wagtailstreamforms
             $ docker-compose up
@@ -95,31 +95,38 @@
         .. code:: bash
         
             $ docker-compose exec app bash
             $ python manage.py createsuperuser
         
         Go to http://127.0.0.1:8000
         
-        .. |CircleCI| image:: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev.svg?style=svg
-           :target: https://circleci.com/gh/AccentDesign/wagtailstreamforms/tree/3-dev
-        .. |Codecov| image:: https://codecov.io/gh/AccentDesign/wagtailstreamforms/branch/3-dev/graph/badge.svg
-           :target: https://codecov.io/gh/AccentDesign/wagtailstreamforms
+        .. |tests| image:: https://github.com/labd/wagtailstreamforms/workflows/Python%20Tests/badge.svg
+           :target: https://github.com/labd/wagtailstreamforms/actions?query=workflow%3A%22Python+Tests%22
+        .. |Codecov| image:: https://codecov.io/gh/labd/wagtailstreamforms/branch/master/graph/badge.svg
+           :target: https://codecov.io/gh/labd/wagtailstreamforms
+        .. |pypi| image:: https://img.shields.io/pypi/v/wagtailstreamforms.svg
+           :target: https://pypi.org/project/wagtailstreamforms/
+        .. |github| image:: https://img.shields.io/github/stars/labd/wagtailstreamforms.svg?style=social&logo=github
+           :target: https://github.com/labd/wagtailstreamforms/stargazers
+        
         
 Keywords: wagtail,streamfield,forms,accent,design
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 4
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `wagtailstreamforms-3.9/wagtailstreamforms.egg-info/SOURCES.txt` & `wagtailstreamforms-4.0.1/wagtailstreamforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

