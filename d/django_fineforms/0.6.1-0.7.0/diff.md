# Comparing `tmp/django_fineforms-0.6.1.tar.gz` & `tmp/django_fineforms-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_fineforms-0.6.1.tar", last modified: Wed Feb 17 08:13:09 2021, max compression
+gzip compressed data, was "django_fineforms-0.7.0.tar", last modified: Thu Apr 13 17:49:13 2023, max compression
```

## Comparing `django_fineforms-0.6.1.tar` & `django_fineforms-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2735 2021-02-16 14:08:26.000000 django_fineforms-0.6.1/CHANGELOG.rst
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      133 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6145 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3899 2021-02-16 14:05:29.000000 django_fineforms-0.6.1/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/django_fineforms.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6145 2021-02-17 08:13:08.000000 django_fineforms-0.6.1/django_fineforms.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1004 2021-02-17 08:13:09.000000 django_fineforms-0.6.1/django_fineforms.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2021-02-17 08:13:08.000000 django_fineforms-0.6.1/django_fineforms.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2021-02-16 14:01:21.000000 django_fineforms-0.6.1/django_fineforms.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       18 2021-02-17 08:13:08.000000 django_fineforms-0.6.1/django_fineforms.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       10 2021-02-17 08:13:08.000000 django_fineforms-0.6.1/django_fineforms.egg-info/top_level.txt
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2021-02-17 08:12:53.000000 django_fineforms-0.6.1/fineforms/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      525 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      855 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/packages/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/packages/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/fineforms/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      401 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/fineforms/errors.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      667 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/fineforms/field.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      168 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/fineforms/submit.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/templates/fineforms/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      386 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templates/fineforms/errors.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       55 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templates/fineforms/field-plain.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      665 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templates/fineforms/field.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templates/fineforms/fields.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      188 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templates/fineforms/submit.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/fineforms/templatetags/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templatetags/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1249 2021-02-16 13:55:46.000000 django_fineforms-0.6.1/fineforms/templatetags/fineforms.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3982 2021-02-17 08:12:42.000000 django_fineforms-0.6.1/fineforms/wrappers.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1536 2021-02-17 08:13:09.010000 django_fineforms-0.6.1/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2021-02-16 14:00:49.000000 django_fineforms-0.6.1/setup.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.709193 django_fineforms-0.7.0/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3042 2023-04-13 17:48:43.000000 django_fineforms-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1548 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/LICENSE
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      133 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/MANIFEST.in
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5205 2023-04-13 17:49:13.709193 django_fineforms-0.7.0/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4073 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/README.rst
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.707193 django_fineforms-0.7.0/django_fineforms.egg-info/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5205 2023-04-13 17:49:13.000000 django_fineforms-0.7.0/django_fineforms.egg-info/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1088 2023-04-13 17:49:13.000000 django_fineforms-0.7.0/django_fineforms.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-04-13 17:49:13.000000 django_fineforms-0.7.0/django_fineforms.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-04-13 17:45:21.000000 django_fineforms-0.7.0/django_fineforms.egg-info/not-zip-safe
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       30 2023-04-13 17:49:13.000000 django_fineforms-0.7.0/django_fineforms.egg-info/requires.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       10 2023-04-13 17:49:13.000000 django_fineforms-0.7.0/django_fineforms.egg-info/top_level.txt
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.707193 django_fineforms-0.7.0/fineforms/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       62 2023-04-13 17:48:53.000000 django_fineforms-0.7.0/fineforms/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.706193 django_fineforms-0.7.0/fineforms/locale/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.706193 django_fineforms-0.7.0/fineforms/locale/de/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.707193 django_fineforms-0.7.0/fineforms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      525 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      855 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.706193 django_fineforms-0.7.0/fineforms/locale/rm/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.708192 django_fineforms-0.7.0/fineforms/locale/rm/LC_MESSAGES/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      474 2023-04-13 17:47:14.000000 django_fineforms-0.7.0/fineforms/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1005 2023-04-13 17:46:49.000000 django_fineforms-0.7.0/fineforms/locale/rm/LC_MESSAGES/django.po
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.708192 django_fineforms-0.7.0/fineforms/packages/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/packages/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.708192 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.706193 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.708192 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/fineforms/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      401 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/fineforms/errors.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      667 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/fineforms/field.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      168 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/fineforms/submit.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.706193 django_fineforms-0.7.0/fineforms/templates/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.708192 django_fineforms-0.7.0/fineforms/templates/fineforms/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      386 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templates/fineforms/errors.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       55 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templates/fineforms/field-plain.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      665 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templates/fineforms/field.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       62 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templates/fineforms/fields.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      188 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templates/fineforms/submit.html
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:49:13.709193 django_fineforms-0.7.0/fineforms/templatetags/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templatetags/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1191 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/templatetags/fineforms.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3900 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/fineforms/wrappers.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1345 2023-04-13 17:49:13.709193 django_fineforms-0.7.0/setup.cfg
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)       62 2023-04-13 17:44:23.000000 django_fineforms-0.7.0/setup.py
```

### Comparing `django_fineforms-0.6.1/CHANGELOG.rst` & `django_fineforms-0.7.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 ==========
 Change log
 ==========
 
 `Next version`_
 ===============
 
+.. _Next version: https://github.com/matthiask/django-fineforms/compare/0.7...main
+
+
+`0.7`_ (2023-04-13)
+===================
+
+.. _0.7: https://github.com/matthiask/django-fineforms/compare/0.6...0.7
+
+- Dropped support for Python < 3.8, Django < 3.2.
+- Added Django 4.1 and 4.2.
+- Added Romansh translations.
+
 
 `0.6`_ (2021-02-16)
 ===================
 
 - Added ``forms`` to the context of ``fineforms/errors.html``, ``form`` to the
   context of ``fineforms/fields.html``.
 - Switched from Travis CI to GitHub actions.
@@ -72,8 +84,8 @@
 
 .. _0.1: https://github.com/matthiask/django-fineforms/commit/06f30791f3d
 .. _0.2: https://github.com/matthiask/django-fineforms/compare/0.1...0.2
 .. _0.3: https://github.com/matthiask/django-fineforms/compare/0.2...0.3
 .. _0.4: https://github.com/matthiask/django-fineforms/compare/0.3...0.4
 .. _0.5: https://github.com/matthiask/django-fineforms/compare/0.4...0.5
 .. _0.6: https://github.com/matthiask/django-fineforms/compare/0.5...0.6
-.. _Next version: https://github.com/matthiask/django-fineforms/compare/0.6...master
+.. _Next version: https://github.com/matthiask/django-fineforms/compare/0.6...main
```

### Comparing `django_fineforms-0.6.1/LICENSE` & `django_fineforms-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_fineforms-0.6.1/PKG-INFO` & `django_fineforms-0.7.0/django_fineforms.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,164 @@
 Metadata-Version: 2.1
-Name: django_fineforms
-Version: 0.6.1
+Name: django-fineforms
+Version: 0.7.0
 Summary: Form rendering for Django
 Home-page: http://github.com/matthiask/django-fineforms/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
-Description: ============================================
-        django-fineforms - Form rendering for Django
-        ============================================
-        
-        .. image:: https://github.com/matthiask/django-fineforms/workflows/Tests/badge.svg
-            :target: https://github.com/matthiask/django-fineforms
-        
-        This library offers an improved replacement for Django's own form
-        rendering methods (``as_p``, ``as_table`` etc.) while staying simple
-        and extensible but without introducing a whole new framework.
-        
-        django-fineforms consists of a template tag library and a few
-        opinionated default templates.
-        
-        
-        Goals
-        =====
-        
-        - Stay simple and extensible
-        - Avoid options, settings and customizability as much as possible
-        
-        
-        Non-goals
-        =========
-        
-        - Compete with django-crispy-forms or any of the more flexible libraries
-          out there
-        
-        
-        Installation
-        ============
-        
-        Simply ``pip install django-fineforms``, and add ``fineforms`` to your
-        ``INSTALLED_APPS``.
-        
-        
-        High-level overview
-        ===================
-        
-        The template tags mostly wrap their arguments in wrapper classes that do
-        the real work. For example, ``{% ff_field %}`` simply wraps the passed
-        field in a wrapper defined in the ``FINEFORMS_WRAPPERS`` setting. All
-        wrappers use a template to render their output. The default wrapper
-        types are as follows::
-        
-            {
-                "errors": ErrorsWrapper,
-                "field": FieldWrapper,
-                "field-plain": PlainFieldWrapper,
-                "fields": FieldsWrapper,
-            }
-        
-        The wrappers themselves mostly aren't configurable, but you can replace
-        individual wrappers (or all of them) by adding a ``FINEFORMS_WRAPPERS``
-        setting. You do not have to override all of them; if you only want to
-        add another wrapper for a specific field type you could just set::
-        
-            FINEFORMS_WRAPPERS = {
-                "specific": "app.wrappers.SpecificWrapper",
-            }
-        
-        ... and use this wrapper as ``{% ff_field some_field type='specific' %}``
-        somewhere in your templates.
-        
-        
-        Template tags
-        =============
-        
-        All template tags are contained in the ``fineforms`` library.
-        
-        ``{% ff_field field [type=field] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/field.html``
-        
-        Render a single field. The wrapper can be optionally overridden by
-        passing a different type. The key has to exist in the
-        ``FINEFORMS_WRAPPERS`` dictionary.
-        
-        The default implementation renders the label, the widget, help text and
-        errors related to the field. It is recommended to also set the
-        ``error_css_class`` and ``required_css_class`` form attributes; those
-        classes are also added to the output.
-        
-        The ``field-plain`` type can be used if the widget should be rendered
-        alone. A wrapping ``<span>`` tag still contains the CSS classes
-        mentioned above.
-        
-        
-        ``{% ff_fields form [fields='a,b,c' | exclude='a,b,c'] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/fields.html``
-        
-        Render fields of a form. ``fields`` and ``exclude`` are
-        comma-separated strings that can be used to only render a selection of
-        fields. The ``fields`` parameter takes precedence if both are given.
-        
-        Hidden fields are rendered separately at the end, all other fields are
-        wrapped using ``FINEFORMS_WRAPPERS["field"]`` and rendered as well.
-        
-        
-        ``{% ff_errors form1 [form2 ...] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/errors.html``
-        
-        Render form errors at the top. The default implementation renders all
-        non-field errors, and all errors from hidden fields.  Falsy parameters
-        (i.e. ``None``) are filtered out for you. If there aren't any errors at
-        all nothing is rendered.
-        
-        
-        ``{% ff_hidden_fields form1 [form2 ...] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This template tag is the outlier in that it does not use a template at
-        all. The return value is the concatenated result of rendering all hidden
-        fields of all passed forms. Falsy parameters (i.e. ``None``) are
-        filtered out for you.
-        
-        Please note that ``{% ff_fields %}`` adds hidden fields to the output
-        automatically.
-        
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
+License-File: LICENSE
+
+============================================
+django-fineforms - Form rendering for Django
+============================================
+
+.. image:: https://github.com/matthiask/django-fineforms/workflows/Tests/badge.svg
+    :target: https://github.com/matthiask/django-fineforms
+
+This library offers an improved replacement for Django's own form
+rendering methods (``as_p``, ``as_table`` etc.) while staying simple
+and extensible but without introducing a whole new framework.
+
+django-fineforms consists of a template tag library and a few
+opinionated default templates.
+
+
+Goals
+=====
+
+- Stay simple and extensible
+- Avoid options, settings and customizability as much as possible
+
+
+Non-goals
+=========
+
+- Compete with django-crispy-forms or any of the more flexible libraries
+  out there
+
+
+Installation
+============
+
+Simply ``pip install django-fineforms``, and add ``fineforms`` to your
+``INSTALLED_APPS``.
+
+
+High-level overview
+===================
+
+The template tags mostly wrap their arguments in wrapper classes that do
+the real work. For example, ``{% ff_field %}`` simply wraps the passed
+field in a wrapper defined in the ``FINEFORMS_WRAPPERS`` setting. All
+wrappers use a template to render their output. The default wrapper
+types are as follows:
+
+.. code-block:: python
+
+    {
+        "errors": ErrorsWrapper,
+        "field": FieldWrapper,
+        "field-plain": PlainFieldWrapper,
+        "fields": FieldsWrapper,
+    }
+
+The wrappers themselves mostly aren't configurable, but you can replace
+individual wrappers (or all of them) by adding a ``FINEFORMS_WRAPPERS``
+setting. You do not have to override all of them; if you only want to
+add another wrapper for a specific field type you could just set:
+
+.. code-block:: python
+
+    FINEFORMS_WRAPPERS = {
+        "specific": "app.wrappers.SpecificWrapper",
+    }
+
+... and use this wrapper as ``{% ff_field some_field type='specific' %}``
+somewhere in your templates.
+
+
+Template tags
+=============
+
+All template tags are contained in the ``fineforms`` library.
+
+``{% ff_field field [type=field] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/field.html``
+
+Render a single field. The wrapper can be optionally overridden by
+passing a different type. The key has to exist in the
+``FINEFORMS_WRAPPERS`` dictionary.
+
+The default implementation renders the label, the widget, help text and
+errors related to the field. It is recommended to also set the
+``error_css_class`` and ``required_css_class`` form attributes; those
+classes are also added to the output.
+
+The ``field-plain`` type can be used if the widget should be rendered
+alone. A wrapping ``<span>`` tag still contains the CSS classes
+mentioned above.
+
+
+``{% ff_fields form [fields='a,b,c' | exclude='a,b,c'] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/fields.html``
+
+Render fields of a form. ``fields`` and ``exclude`` are
+comma-separated strings that can be used to only render a selection of
+fields. The ``fields`` parameter takes precedence if both are given.
+
+Hidden fields are rendered separately at the end, all other fields are
+wrapped using ``FINEFORMS_WRAPPERS["field"]`` and rendered as well.
+
+
+``{% ff_errors form1 [form2 ...] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/errors.html``
+
+Render form errors at the top. The default implementation renders all
+non-field errors, and all errors from hidden fields.  Falsy parameters
+(i.e. ``None``) are filtered out for you. If there aren't any errors at
+all nothing is rendered.
+
+
+``{% ff_hidden_fields form1 [form2 ...] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This template tag is the outlier in that it does not use a template at
+all. The return value is the concatenated result of rendering all hidden
+fields of all passed forms. Falsy parameters (i.e. ``None``) are
+filtered out for you.
+
+Please note that ``{% ff_fields %}`` adds hidden fields to the output
+automatically.
+
+
+``{% ff_submit [_("label")] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/submit.html``
+
+Show a submit button.
```

### Comparing `django_fineforms-0.6.1/README.rst` & `django_fineforms-0.7.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -37,27 +37,31 @@
 High-level overview
 ===================
 
 The template tags mostly wrap their arguments in wrapper classes that do
 the real work. For example, ``{% ff_field %}`` simply wraps the passed
 field in a wrapper defined in the ``FINEFORMS_WRAPPERS`` setting. All
 wrappers use a template to render their output. The default wrapper
-types are as follows::
+types are as follows:
+
+.. code-block:: python
 
     {
         "errors": ErrorsWrapper,
         "field": FieldWrapper,
         "field-plain": PlainFieldWrapper,
         "fields": FieldsWrapper,
     }
 
 The wrappers themselves mostly aren't configurable, but you can replace
 individual wrappers (or all of them) by adding a ``FINEFORMS_WRAPPERS``
 setting. You do not have to override all of them; if you only want to
-add another wrapper for a specific field type you could just set::
+add another wrapper for a specific field type you could just set:
+
+.. code-block:: python
 
     FINEFORMS_WRAPPERS = {
         "specific": "app.wrappers.SpecificWrapper",
     }
 
 ... and use this wrapper as ``{% ff_field some_field type='specific' %}``
 somewhere in your templates.
@@ -117,7 +121,15 @@
 This template tag is the outlier in that it does not use a template at
 all. The return value is the concatenated result of rendering all hidden
 fields of all passed forms. Falsy parameters (i.e. ``None``) are
 filtered out for you.
 
 Please note that ``{% ff_fields %}`` adds hidden fields to the output
 automatically.
+
+
+``{% ff_submit [_("label")] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/submit.html``
+
+Show a submit button.
```

### Comparing `django_fineforms-0.6.1/django_fineforms.egg-info/PKG-INFO` & `django_fineforms-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,164 @@
 Metadata-Version: 2.1
-Name: django-fineforms
-Version: 0.6.1
+Name: django_fineforms
+Version: 0.7.0
 Summary: Form rendering for Django
 Home-page: http://github.com/matthiask/django-fineforms/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
-Description: ============================================
-        django-fineforms - Form rendering for Django
-        ============================================
-        
-        .. image:: https://github.com/matthiask/django-fineforms/workflows/Tests/badge.svg
-            :target: https://github.com/matthiask/django-fineforms
-        
-        This library offers an improved replacement for Django's own form
-        rendering methods (``as_p``, ``as_table`` etc.) while staying simple
-        and extensible but without introducing a whole new framework.
-        
-        django-fineforms consists of a template tag library and a few
-        opinionated default templates.
-        
-        
-        Goals
-        =====
-        
-        - Stay simple and extensible
-        - Avoid options, settings and customizability as much as possible
-        
-        
-        Non-goals
-        =========
-        
-        - Compete with django-crispy-forms or any of the more flexible libraries
-          out there
-        
-        
-        Installation
-        ============
-        
-        Simply ``pip install django-fineforms``, and add ``fineforms`` to your
-        ``INSTALLED_APPS``.
-        
-        
-        High-level overview
-        ===================
-        
-        The template tags mostly wrap their arguments in wrapper classes that do
-        the real work. For example, ``{% ff_field %}`` simply wraps the passed
-        field in a wrapper defined in the ``FINEFORMS_WRAPPERS`` setting. All
-        wrappers use a template to render their output. The default wrapper
-        types are as follows::
-        
-            {
-                "errors": ErrorsWrapper,
-                "field": FieldWrapper,
-                "field-plain": PlainFieldWrapper,
-                "fields": FieldsWrapper,
-            }
-        
-        The wrappers themselves mostly aren't configurable, but you can replace
-        individual wrappers (or all of them) by adding a ``FINEFORMS_WRAPPERS``
-        setting. You do not have to override all of them; if you only want to
-        add another wrapper for a specific field type you could just set::
-        
-            FINEFORMS_WRAPPERS = {
-                "specific": "app.wrappers.SpecificWrapper",
-            }
-        
-        ... and use this wrapper as ``{% ff_field some_field type='specific' %}``
-        somewhere in your templates.
-        
-        
-        Template tags
-        =============
-        
-        All template tags are contained in the ``fineforms`` library.
-        
-        ``{% ff_field field [type=field] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/field.html``
-        
-        Render a single field. The wrapper can be optionally overridden by
-        passing a different type. The key has to exist in the
-        ``FINEFORMS_WRAPPERS`` dictionary.
-        
-        The default implementation renders the label, the widget, help text and
-        errors related to the field. It is recommended to also set the
-        ``error_css_class`` and ``required_css_class`` form attributes; those
-        classes are also added to the output.
-        
-        The ``field-plain`` type can be used if the widget should be rendered
-        alone. A wrapping ``<span>`` tag still contains the CSS classes
-        mentioned above.
-        
-        
-        ``{% ff_fields form [fields='a,b,c' | exclude='a,b,c'] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/fields.html``
-        
-        Render fields of a form. ``fields`` and ``exclude`` are
-        comma-separated strings that can be used to only render a selection of
-        fields. The ``fields`` parameter takes precedence if both are given.
-        
-        Hidden fields are rendered separately at the end, all other fields are
-        wrapped using ``FINEFORMS_WRAPPERS["field"]`` and rendered as well.
-        
-        
-        ``{% ff_errors form1 [form2 ...] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Template: ``fineforms/errors.html``
-        
-        Render form errors at the top. The default implementation renders all
-        non-field errors, and all errors from hidden fields.  Falsy parameters
-        (i.e. ``None``) are filtered out for you. If there aren't any errors at
-        all nothing is rendered.
-        
-        
-        ``{% ff_hidden_fields form1 [form2 ...] %}``
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This template tag is the outlier in that it does not use a template at
-        all. The return value is the concatenated result of rendering all hidden
-        fields of all passed forms. Falsy parameters (i.e. ``None``) are
-        filtered out for you.
-        
-        Please note that ``{% ff_fields %}`` adds hidden fields to the output
-        automatically.
-        
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
+License-File: LICENSE
+
+============================================
+django-fineforms - Form rendering for Django
+============================================
+
+.. image:: https://github.com/matthiask/django-fineforms/workflows/Tests/badge.svg
+    :target: https://github.com/matthiask/django-fineforms
+
+This library offers an improved replacement for Django's own form
+rendering methods (``as_p``, ``as_table`` etc.) while staying simple
+and extensible but without introducing a whole new framework.
+
+django-fineforms consists of a template tag library and a few
+opinionated default templates.
+
+
+Goals
+=====
+
+- Stay simple and extensible
+- Avoid options, settings and customizability as much as possible
+
+
+Non-goals
+=========
+
+- Compete with django-crispy-forms or any of the more flexible libraries
+  out there
+
+
+Installation
+============
+
+Simply ``pip install django-fineforms``, and add ``fineforms`` to your
+``INSTALLED_APPS``.
+
+
+High-level overview
+===================
+
+The template tags mostly wrap their arguments in wrapper classes that do
+the real work. For example, ``{% ff_field %}`` simply wraps the passed
+field in a wrapper defined in the ``FINEFORMS_WRAPPERS`` setting. All
+wrappers use a template to render their output. The default wrapper
+types are as follows:
+
+.. code-block:: python
+
+    {
+        "errors": ErrorsWrapper,
+        "field": FieldWrapper,
+        "field-plain": PlainFieldWrapper,
+        "fields": FieldsWrapper,
+    }
+
+The wrappers themselves mostly aren't configurable, but you can replace
+individual wrappers (or all of them) by adding a ``FINEFORMS_WRAPPERS``
+setting. You do not have to override all of them; if you only want to
+add another wrapper for a specific field type you could just set:
+
+.. code-block:: python
+
+    FINEFORMS_WRAPPERS = {
+        "specific": "app.wrappers.SpecificWrapper",
+    }
+
+... and use this wrapper as ``{% ff_field some_field type='specific' %}``
+somewhere in your templates.
+
+
+Template tags
+=============
+
+All template tags are contained in the ``fineforms`` library.
+
+``{% ff_field field [type=field] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/field.html``
+
+Render a single field. The wrapper can be optionally overridden by
+passing a different type. The key has to exist in the
+``FINEFORMS_WRAPPERS`` dictionary.
+
+The default implementation renders the label, the widget, help text and
+errors related to the field. It is recommended to also set the
+``error_css_class`` and ``required_css_class`` form attributes; those
+classes are also added to the output.
+
+The ``field-plain`` type can be used if the widget should be rendered
+alone. A wrapping ``<span>`` tag still contains the CSS classes
+mentioned above.
+
+
+``{% ff_fields form [fields='a,b,c' | exclude='a,b,c'] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/fields.html``
+
+Render fields of a form. ``fields`` and ``exclude`` are
+comma-separated strings that can be used to only render a selection of
+fields. The ``fields`` parameter takes precedence if both are given.
+
+Hidden fields are rendered separately at the end, all other fields are
+wrapped using ``FINEFORMS_WRAPPERS["field"]`` and rendered as well.
+
+
+``{% ff_errors form1 [form2 ...] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/errors.html``
+
+Render form errors at the top. The default implementation renders all
+non-field errors, and all errors from hidden fields.  Falsy parameters
+(i.e. ``None``) are filtered out for you. If there aren't any errors at
+all nothing is rendered.
+
+
+``{% ff_hidden_fields form1 [form2 ...] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This template tag is the outlier in that it does not use a template at
+all. The return value is the concatenated result of rendering all hidden
+fields of all passed forms. Falsy parameters (i.e. ``None``) are
+filtered out for you.
+
+Please note that ``{% ff_fields %}`` adds hidden fields to the output
+automatically.
+
+
+``{% ff_submit [_("label")] %}``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Template: ``fineforms/submit.html``
+
+Show a submit button.
```

### Comparing `django_fineforms-0.6.1/django_fineforms.egg-info/SOURCES.txt` & `django_fineforms-0.7.0/django_fineforms.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 django_fineforms.egg-info/not-zip-safe
 django_fineforms.egg-info/requires.txt
 django_fineforms.egg-info/top_level.txt
 fineforms/__init__.py
 fineforms/wrappers.py
 fineforms/locale/de/LC_MESSAGES/django.mo
 fineforms/locale/de/LC_MESSAGES/django.po
+fineforms/locale/rm/LC_MESSAGES/django.mo
+fineforms/locale/rm/LC_MESSAGES/django.po
 fineforms/packages/__init__.py
 fineforms/packages/foundation_xy_grid/__init__.py
 fineforms/packages/foundation_xy_grid/templates/fineforms/errors.html
 fineforms/packages/foundation_xy_grid/templates/fineforms/field.html
 fineforms/packages/foundation_xy_grid/templates/fineforms/submit.html
 fineforms/templates/fineforms/errors.html
 fineforms/templates/fineforms/field-plain.html
```

### Comparing `django_fineforms-0.6.1/fineforms/locale/de/LC_MESSAGES/django.mo` & `django_fineforms-0.7.0/fineforms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_fineforms-0.6.1/fineforms/locale/de/LC_MESSAGES/django.po` & `django_fineforms-0.7.0/fineforms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_fineforms-0.6.1/fineforms/packages/foundation_xy_grid/templates/fineforms/field.html` & `django_fineforms-0.7.0/fineforms/packages/foundation_xy_grid/templates/fineforms/field.html`

 * *Files identical despite different names*

### Comparing `django_fineforms-0.6.1/fineforms/templates/fineforms/field.html` & `django_fineforms-0.7.0/fineforms/templates/fineforms/field.html`

 * *Files identical despite different names*

### Comparing `django_fineforms-0.6.1/fineforms/wrappers.py` & `django_fineforms-0.7.0/fineforms/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from __future__ import absolute_import, unicode_literals
-
 from django import forms
 from django.conf import settings
 from django.template.loader import render_to_string
 from django.utils.html import html_safe, mark_safe
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
 
 
 # TODO aria-describedby etc.
 
 
 @html_safe
-class ErrorsWrapper(object):
+class ErrorsWrapper:
     template_name = "fineforms/errors.html"
 
     def __init__(self, forms):
         self.forms = forms
         self.top_errors = []
         self.has_field_errors = False
         for form in self.forms:
@@ -43,15 +41,15 @@
                 "top_errors": self.top_errors,
                 "has_field_errors": self.has_field_errors,
             },
         )
 
 
 @html_safe
-class FieldWrapper(object):
+class FieldWrapper:
     template_name = "fineforms/field.html"
     label_suffix = ""
     error_css_class = "error"
     required_css_class = "required"
 
     def __init__(self, field):
         self.field = field
@@ -90,15 +88,15 @@
 
 
 class PlainFieldWrapper(FieldWrapper):
     template_name = "fineforms/field-plain.html"
 
 
 @html_safe
-class FieldsWrapper(object):
+class FieldsWrapper:
     template_name = "fineforms/fields.html"
 
     def __init__(self, form, fields):
         self.form = form
         self.fields = fields
 
     def __str__(self):
```

### Comparing `django_fineforms-0.6.1/setup.cfg` & `django_fineforms-0.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,38 @@
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries :: Application Frameworks
 
 [options]
 packages = find:
-python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+install_requires = 
+	Django>=3.2
+python_requires = >=3.8
 include_package_data = True
 zip_safe = False
 
-[options.extras_require]
-tests = 
-	coverage
-
 [options.packages.find]
 exclude = tests
 
-[flake8]
-exclude = venv,build,docs,.tox
-ignore = E203,W503
-max-complexity = 10
-max-line-length = 88
+[options.extras_require]
+tests = 
+	coverage
 
 [coverage:run]
 branch = True
 include = 
 	*fineforms*
 omit = 
 	*migrations*
```

