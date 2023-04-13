# Comparing `tmp/easys-ordermanager-2.1.1.tar.gz` & `tmp/easys-ordermanager-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easys-ordermanager-2.1.1.tar", last modified: Tue Mar 21 16:23:08 2023, max compression
+gzip compressed data, was "easys-ordermanager-2.1.2.tar", last modified: Thu Apr 13 15:08:47 2023, max compression
```

## Comparing `easys-ordermanager-2.1.1.tar` & `easys-ordermanager-2.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/
--rw-r--r--   0 root         (0) root         (0)    12032 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     8773 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/CHANGELOG_SERIALIZER.md
--rw-r--r--   0 root         (0) root         (0)    34940 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      106 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    21584 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/management/commands/i18n.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/tests/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/tests/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/tests/v1/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/tests/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/tests/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/dev/tests/v2/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/dev/tests/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 10:47:37.000000 easys-ordermanager-2.1.1/dev/tests/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/dev/tests/v3/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/easys_ordermanager/
--rw-r--r--   0 root         (0) root         (0)      300 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/easys_ordermanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/easys_ordermanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      519 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      829 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/easys_ordermanager/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.506067 easys-ordermanager-2.1.1/easys_ordermanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.506067 easys-ordermanager-2.1.1/easys_ordermanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/easys_ordermanager/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    13139 2023-03-16 14:57:55.000000 easys-ordermanager-2.1.1/easys_ordermanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/easys_ordermanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/easys_ordermanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93490 2023-03-16 14:57:55.000000 easys-ordermanager-2.1.1/easys_ordermanager/v1/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/easys_ordermanager/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/easys_ordermanager/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93525 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/easys_ordermanager/v2/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/easys_ordermanager/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 10:47:37.000000 easys-ordermanager-2.1.1/easys_ordermanager/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95739 2023-03-21 14:23:25.000000 easys-ordermanager-2.1.1/easys_ordermanager/v3/serializer.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/easys_ordermanager/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 16:23:08.510067 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21584 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-21 16:23:08.000000 easys-ordermanager-2.1.1/easys_ordermanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      331 2023-03-21 16:23:08.514067 easys-ordermanager-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1249 2023-02-17 14:18:12.000000 easys-ordermanager-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)    12147 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     9321 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/CHANGELOG_SERIALIZER.md
+-rw-r--r--   0 root         (0) root         (0)    34940 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22247 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/management/commands/i18n.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v1/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v2/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/dev/tests/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/dev/tests/v3/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.220855 easys-ordermanager-2.1.2/easys_ordermanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.220855 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93490 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v1/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93525 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v2/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94662 2023-04-13 14:49:23.000000 easys-ordermanager-2.1.2/easys_ordermanager/v3/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/easys_ordermanager/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22247 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:08:47.000000 easys-ordermanager-2.1.2/easys_ordermanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-13 15:08:47.224856 easys-ordermanager-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-04-13 10:28:08.000000 easys-ordermanager-2.1.2/setup.py
```

### Comparing `easys-ordermanager-2.1.1/CHANGELOG.md` & `easys-ordermanager-2.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 2.1.2 (2023-04-12)
+* Updates to Serializer v3, see serializer changelog
+* Fixed missing development dependency
+
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
 
 ## 2.1.0 (2023-03-16)
 * Introduction of serializer v3, see serializer changelog
 * `easys-ordermanager/easys_ordermanager/v3/serializer.Serializer` is considered WIP until integration in EasyS starts
```

### Comparing `easys-ordermanager-2.1.1/CHANGELOG_SERIALIZER.md` & `easys-ordermanager-2.1.2/CHANGELOG_SERIALIZER.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Serializer changes
 
+## 2.1.2
+
+#### `OrderLineGoogleAdsPremiumSerializer`
+* Made `target_page_type` required.
+* Removed fields:
+  - `expected_clicks`
+  - `expected_conversions`
+  - `expected_impression_share`
+  - `expected_impressions`
+  - `keywords_with_zero_search_volume`
+  - `branch_codes`
+  - `call_to_action`
+  - `is_generic_campaign`
+  - `generic_topics`
+  - `remarketing_setup_fee`
+  - `remarketing_budget`
+
+#### `OrderLineLandingpageSerializer`
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
 * Change constant value from 3 to 4, to prevent clashes with `NEW_LANDINGPAGE` constant.
```

### Comparing `easys-ordermanager-2.1.1/LICENSE.md` & `easys-ordermanager-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/PKG-INFO` & `easys-ordermanager-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.1
+Version: 2.1.2
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -30,14 +30,18 @@
 ### Django 4.1
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.1.2 (2023-04-12)
+* Updates to Serializer v3, see serializer changelog
+* Fixed missing development dependency
+
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
 
 ## 2.1.0 (2023-03-16)
 * Introduction of serializer v3, see serializer changelog
 * `easys-ordermanager/easys_ordermanager/v3/serializer.Serializer` is considered WIP until integration in EasyS starts
@@ -422,14 +426,34 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.1.2
+
+#### `OrderLineGoogleAdsPremiumSerializer`
+* Made `target_page_type` required.
+* Removed fields:
+  - `expected_clicks`
+  - `expected_conversions`
+  - `expected_impression_share`
+  - `expected_impressions`
+  - `keywords_with_zero_search_volume`
+  - `branch_codes`
+  - `call_to_action`
+  - `is_generic_campaign`
+  - `generic_topics`
+  - `remarketing_setup_fee`
+  - `remarketing_budget`
+
+#### `OrderLineLandingpageSerializer`
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
 * Change constant value from 3 to 4, to prevent clashes with `NEW_LANDINGPAGE` constant.
```

### Comparing `easys-ordermanager-2.1.1/dev/management/commands/i18n.py` & `easys-ordermanager-2.1.2/dev/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/dev/tests/v3/test_serializer.py` & `easys-ordermanager-2.1.2/dev/tests/v3/test_serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/__pycache__/__init__.cpython-311.pyc` & `easys-ordermanager-2.1.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xddbd1964 (Tue Mar 21 14:23:25 2023 UTC)
+moddate:  0x38d93764 (Thu Apr 13 10:28:08 2023 UTC)
 files sz: 300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
@@ -13,15 +13,15 @@
    
      1           2 LOAD_CONST               0 ('easys-ordermanager')
                  4 STORE_NAME               0 (__title__)
    
      2           6 LOAD_CONST               1 ('API definition of RH order manager for EasyS')
                  8 STORE_NAME               1 (__description__)
    
-     3          10 LOAD_CONST               2 ('2.1.1')
+     3          10 LOAD_CONST               2 ('2.1.2')
                 12 STORE_NAME               2 (__version__)
    
      4          14 LOAD_CONST               3 ('https://gitlab.herocentral.de/development/easys-ordermanager')
                 16 STORE_NAME               3 (__url__)
    
      5          18 LOAD_CONST               4 ('RegioHelden developers')
                 20 STORE_NAME               4 (__author__)
@@ -32,15 +32,15 @@
      7          26 LOAD_CONST               6 ('GPL 3')
                 28 STORE_NAME               6 (__license__)
                 30 LOAD_CONST               7 (None)
                 32 RETURN_VALUE
    consts
       'easys-ordermanager'
       'API definition of RH order manager for EasyS'
-      '2.1.1'
+      '2.1.2'
       'https://gitlab.herocentral.de/development/easys-ordermanager'
       'RegioHelden developers'
       'opensource@regiohelden.de'
       'GPL 3'
       None
    names      ('__title__', '__description__', '__version__', '__url__', '__author__', '__author_email__', '__license__')
    varnames   ()
```

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/fields.py` & `easys-ordermanager-2.1.2/easys_ordermanager/fields.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/locale/de/LC_MESSAGES/django.po` & `easys-ordermanager-2.1.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/v1/serializer.py` & `easys-ordermanager-2.1.2/easys_ordermanager/v1/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/v2/serializer.py` & `easys-ordermanager-2.1.2/easys_ordermanager/v2/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/v3/serializer.py` & `easys-ordermanager-2.1.2/easys_ordermanager/v3/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from django_countries.serializer_fields import CountryField
 from internationalflavor.iban import IBANValidator
 from internationalflavor.vat_number import VATNumberValidator
 from model_utils.choices import Choices
 from rest_framework import serializers
 
 from easys_ordermanager.fields import PhoneNumberField
-from easys_ordermanager.validators import comma_separated_period_validatior, HexColorValidator, \
-    DomainNameValidator
+from easys_ordermanager.validators import comma_separated_period_validatior, HexColorValidator, DomainNameValidator
 
 PAYMENT_METHOD_TRANSFER = 1
 PAYMENT_METHOD_CHARGE = 2
 PAYMENT_METHOD_CHOICES = Choices(
     (PAYMENT_METHOD_TRANSFER, 'transfer', _('Transfer')),
     (PAYMENT_METHOD_CHARGE, 'charge', _('Charge')),
 )
@@ -91,15 +90,15 @@
     (PRODUCT_TYPE_LANDINGPAGE, 'landingpage', _('Landingpage')),
     (PRODUCT_TYPE_FACEBOOK, 'facebook', _('Facebook')),
     (PRODUCT_TYPE_CUSTOMER_WEBSITE, 'customer_website', _('Customer website')),
     (PRODUCT_TYPE_EMAIL, 'email', _('Email')),
     (PRODUCT_TYPE_CONVERSION_TRACKING, 'conversion_tracking', _('Conversion tracking')),
     (PRODUCT_TYPE_TONLINE, 'tonline', _('T-Online')),
     (PRODUCT_TYPE_DISPLAY_NATIVE, 'display_native', _('Display Native advertisement')),
-    (PRODUCT_TYPE_DOMAIN, 'domain', _('Domain'))
+    (PRODUCT_TYPE_DOMAIN, 'domain', _('Domain')),
 )
 
 PRODUCT_PAYMENT_CYCLE_1 = 1
 PRODUCT_PAYMENT_CYCLE_3 = 3
 PRODUCT_PAYMENT_CYCLE_6 = 6
 PRODUCT_PAYMENT_CYCLE_12 = 12
 PRODUCT_PAYMENT_CYCLE_CHOICES = Choices(
@@ -209,26 +208,26 @@
 OPENING_HOURS_WEEK_DAY_CHOICES = Choices(
     (OPENING_HOURS_WEEK_DAY_MONDAY, 'monday', _('Monday')),
     (OPENING_HOURS_WEEK_DAY_TUESDAY, 'tuesday', _('Tuesday')),
     (OPENING_HOURS_WEEK_DAY_WEDNESDAY, 'wednesday', _('Wednesday')),
     (OPENING_HOURS_WEEK_DAY_THURSDAY, 'thursday', _('Thursday')),
     (OPENING_HOURS_WEEK_DAY_FRIDAY, 'friday', _('Friday')),
     (OPENING_HOURS_WEEK_DAY_SATURDAY, 'saturday', _('Saturday')),
-    (OPENING_HOURS_WEEK_DAY_SUNDAY, 'sunday', _('Sunday'))
+    (OPENING_HOURS_WEEK_DAY_SUNDAY, 'sunday', _('Sunday')),
 )
 
 OPENING_HOURS_MODE_OPEN = 1
 OPENING_HOURS_MODE_OPEN_MORNING_AFTERNOON = 2
 OPENING_HOURS_MODE_OPEN_24_HOURS = 3
 OPENING_HOURS_MODE_CLOSED = 4
 OPENING_HOURS_MODE_CHOICES = Choices(
     (OPENING_HOURS_MODE_OPEN, 'open', _('Open')),
     (OPENING_HOURS_MODE_OPEN_MORNING_AFTERNOON, 'open_morning_afternoon', _('Morning and afternoon')),
     (OPENING_HOURS_MODE_OPEN_24_HOURS, 'open_24_hours', _('Open 24 hours')),
-    (OPENING_HOURS_MODE_CLOSED, 'closed', pgettext_lazy('opening hours', 'Closed'))
+    (OPENING_HOURS_MODE_CLOSED, 'closed', pgettext_lazy('opening hours', 'Closed')),
 )
 
 SEO_TEXT_STYLE_ADVERTISING = 1
 SEO_TEXT_STYLE_FACTUAL = 2
 SEO_TEXT_STYLE_CUSTOMER_RELATED = 3
 SEO_TEXT_STYLE_CHOICES = Choices(
     (SEO_TEXT_STYLE_ADVERTISING, 'advertising', _('Advertising')),
@@ -363,24 +362,24 @@
     (DISPLAY_BANNER_IMAGE_SOURCE_REGIOHELDEN, 'regiohelden', _('Regiohelden photos')),
 )
 
 DISPLAY_BANNER_COLOR_SELECT_WEBSITE = 1
 DISPLAY_BANNER_COLOR_SELECT_PICKER = 2
 DISPLAY_BANNER_COLOR_SELECTION_CHOICES = Choices(
     (DISPLAY_BANNER_COLOR_SELECT_WEBSITE, 'website', _('Color from Logo/Website')),
-    (DISPLAY_BANNER_COLOR_SELECT_PICKER, 'color_picker', _('Set color'))
+    (DISPLAY_BANNER_COLOR_SELECT_PICKER, 'color_picker', _('Set color')),
 )
 
 DISPLAY_IMPRESSIONS_PER_MONTH_20 = 20000
 DISPLAY_IMPRESSIONS_PER_MONTH_40 = 40000
 DISPLAY_IMPRESSIONS_PER_MONTH_80 = 80000
 DISPLAY_IMPRESSIONS_PER_MONTH_CHOICES = Choices(
     (DISPLAY_IMPRESSIONS_PER_MONTH_20, 'impressions_20', _('20.000 Impressions')),
     (DISPLAY_IMPRESSIONS_PER_MONTH_40, 'impressions_40', _('40.000 Impressions')),
-    (DISPLAY_IMPRESSIONS_PER_MONTH_80, 'impressions_80', _('80.000 Impressions'))
+    (DISPLAY_IMPRESSIONS_PER_MONTH_80, 'impressions_80', _('80.000 Impressions')),
 )
 
 DISPLAY_BASIC_CREATIVE_OPTION_CHOICES = Choices(
     (CREATIVE_OPTION_CUSTOMER, 'customer', _('Customer provided')),
     (CREATIVE_OPTION_CREATE_ANIMATED, 'create_animated', _('Create animated')),
 )
 
@@ -390,39 +389,75 @@
 DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_299 = 4
 DISPLAY_CREATIVES_FORMAT_ADBUNDLE_MOBILE_599 = 5
 DISPLAY_CREATIVES_FORMAT_BILLBOARD_MEDIUM_RECTANGLE_599 = 6
 DISPLAY_CREATIVES_FORMAT_DYNAMIC_SITEBAR = 7
 DISPLAY_CREATIVES_FORMAT_HALFPAGE_599 = 8
 DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_399 = 9
 DISPLAY_CREATIVES_FORMAT_CHOICES = Choices(
-    (DISPLAY_CREATIVES_FORMAT_ADBUNDLE_MOBILE_399, 'adbundle_mobile_banner_399', _(
-        'AdBundle + Mobile Banner (includes the following formats: 160x600, 300x250, 728x90, 320x50) - %(price)d €'
-    ) % {'price': 399}),
-    (DISPLAY_CREATIVES_FORMAT_BILLBOARD_MEDIUM_RECTANGLE_399, 'billboard_medium_rectangle_399', _(
-        'Billboard + Medium Rectangle Presenter (includes the following formats: 800x250, 970x250, 770x250, 300x250)'
-        ' - %(price)d €') % {'price': 399}),
-    (DISPLAY_CREATIVES_FORMAT_HALFPAGE_399, 'halfpage_ad_399', _(
-        'Halfpage Ad (includes the following formats: 300x600, for desktop + mobile) - %(price)d €') % {'price': 399}),
-    (DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_299, 'medium_rectangle_mobile_299', _(
-        'Medium Rectangle + Mobile Banner (includes the following formats: 300x250, 320x50) - %(price)d €'
-    ) % {'price': 299}),
-    (DISPLAY_CREATIVES_FORMAT_ADBUNDLE_MOBILE_599, 'adbundle_mobile_banner_599', _(
-        'AdBundle + Mobile Banner (includes the following formats: 160x600, 300x250, 728x90, 320x50) - %(price)d €'
-    ) % {'price': 599}),
-    (DISPLAY_CREATIVES_FORMAT_BILLBOARD_MEDIUM_RECTANGLE_599, 'billboard_medium_rectangle_599', _(
-        'Billboard + Medium Rectangle Presenter (includes the following formats: 800x250, 970x250, 770x250, 300x250)'
-        ' - %(price)d €') % {'price': 599}),
-    (DISPLAY_CREATIVES_FORMAT_DYNAMIC_SITEBAR, 'dynamic_site_bar_599', _(
-        'Dynamic Sitebar + Medium Rectangle Presenter (includes the following formats: 301x601, 300x250) - %(price)d €'
-    ) % {'price': 599}),
-    (DISPLAY_CREATIVES_FORMAT_HALFPAGE_599, 'halfpage_ad_599', _(
-        'Halfpage Ad (includes the following formats: 300x600, for desktop + mobile) - %(price)d €') % {'price': 599}),
-    (DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_399, 'medium_rectangle_mobile_399', _(
-        'Medium Rectangle + Mobile Banner (includes the following formats: 300x250, 320x50) - %(price)d €'
-    ) % {'price': 399}),
+    (
+        DISPLAY_CREATIVES_FORMAT_ADBUNDLE_MOBILE_399,
+        'adbundle_mobile_banner_399',
+        _('AdBundle + Mobile Banner (includes the following formats: 160x600, 300x250, 728x90, 320x50) - %(price)d €')
+        % {'price': 399},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_BILLBOARD_MEDIUM_RECTANGLE_399,
+        'billboard_medium_rectangle_399',
+        _(
+            'Billboard + Medium Rectangle Presenter (includes the following formats: 800x250, 970x250, 770x250, '
+            '300x250) - %(price)d €'
+        )
+        % {'price': 399},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_HALFPAGE_399,
+        'halfpage_ad_399',
+        _('Halfpage Ad (includes the following formats: 300x600, for desktop + mobile) - %(price)d €') % {'price': 399},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_299,
+        'medium_rectangle_mobile_299',
+        _('Medium Rectangle + Mobile Banner (includes the following formats: 300x250, 320x50) - %(price)d €')
+        % {'price': 299},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_ADBUNDLE_MOBILE_599,
+        'adbundle_mobile_banner_599',
+        _('AdBundle + Mobile Banner (includes the following formats: 160x600, 300x250, 728x90, 320x50) - %(price)d €')
+        % {'price': 599},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_BILLBOARD_MEDIUM_RECTANGLE_599,
+        'billboard_medium_rectangle_599',
+        _(
+            'Billboard + Medium Rectangle Presenter (includes the following formats: 800x250, 970x250, 770x250, '
+            '300x250) - %(price)d €'
+        )
+        % {'price': 599},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_DYNAMIC_SITEBAR,
+        'dynamic_site_bar_599',
+        _(
+            'Dynamic Sitebar + Medium Rectangle Presenter (includes the following formats: 301x601, '
+            '300x250) - %(price)d €'
+        )
+        % {'price': 599},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_HALFPAGE_599,
+        'halfpage_ad_599',
+        _('Halfpage Ad (includes the following formats: 300x600, for desktop + mobile) - %(price)d €') % {'price': 599},
+    ),
+    (
+        DISPLAY_CREATIVES_FORMAT_MEDIUM_RECTANGLE_MOBILE_399,
+        'medium_rectangle_mobile_399',
+        _('Medium Rectangle + Mobile Banner (includes the following formats: 300x250, 320x50) - %(price)d €')
+        % {'price': 399},
+    ),
 )
 
 DISPLAY_AGE_14_29 = 7
 DISPLAY_AGE_30_39 = 3
 DISPLAY_AGE_40_49 = 4
 DISPLAY_AGE_50_59 = 5
 DISPLAY_AGE_60_PLUS = 6
@@ -545,16 +580,19 @@
     (INAPP_AUDIENCE_AUTOBESITZER, 'autobesitzer', _('Car owners')),
     (INAPP_AUDIENCE_SERIENJUNKIES, 'serienjunkies', _('Series junkies')),
     (INAPP_AUDIENCE_HEAVY_STREAMER, 'heavy_streamer', _('Heavy streamers')),
     (INAPP_AUDIENCE_MOVIE_LOVER, 'movie_lover', _('Movie lovers')),
     (INAPP_AUDIENCE_ENTERTAINMENT_LOVER, 'entertainment_lover', _('Entertainment lovers')),
     (INAPP_AUDIENCE_CASUAL_GAMER, 'casual_gamer', _('Casual gamer')),
     (INAPP_AUDIENCE_ECOMMERCE_SHOPPER, 'ecommerce_shopper', _('ecommerce shoppers')),
-    (INAPP_AUDIENCE_SMART_SHOPPER_SPARFUCHS_ANGEBOT, 'smart_shopper_sparfuchs_angebot',
-     _('Smart shoppers / scrimpers')),
+    (
+        INAPP_AUDIENCE_SMART_SHOPPER_SPARFUCHS_ANGEBOT,
+        'smart_shopper_sparfuchs_angebot',
+        _('Smart shoppers / scrimpers'),
+    ),
     (INAPP_AUDIENCE_STYLISH_MEN, 'stylish_men', _('Stylish men')),
     (INAPP_AUDIENCE_HIGH_END_FASHIONISTA, 'high_end_fashionista', _('High end fashionista')),
     (INAPP_AUDIENCE_LOW_BUDGET_FASHIONISTAS, 'low_budget_fashionistas', _('Low budget fashionista')),
     (INAPP_AUDIENCE_MOBELFREAKS, 'mobelfreaks', _('Furniture freaks')),
     (INAPP_AUDIENCE_DIY, 'diy', _('DIY')),
     (INAPP_AUDIENCE_AZUBIS_AKTUELLE_AZUBIS, 'azubis_aktuelle_azubis', _('Apprentices')),
     (INAPP_AUDIENCE_STUDENTEN_UND_ABSOLVENTEN, 'studenten_und_absolventen', _('Students and alumni')),
@@ -565,21 +603,23 @@
     (INAPP_AUDIENCE_FOTOKUNSTLER, 'fotokunstler', _('Photo artists')),
     (INAPP_AUDIENCE_REISENDE_REISEAFFINE, 'reisende_reiseaffine', _('Travelers / Travel afficionados')),
     (INAPP_AUDIENCE_FREQUENT_FLYER, 'frequent_flyer', _('Frequent flyer')),
     (INAPP_AUDIENCE_SPORTSKANONEN, 'sportskanonen', _('Sporting aces')),
     (INAPP_AUDIENCE_OUTDOOR_LIEBHABER, 'outdoor_liebhaber', _('Outdoor enthusiasts')),
     (INAPP_AUDIENCE_MOTORSPORT_FANS, 'motorsport_fans', _('Motorsport fans')),
     (INAPP_AUDIENCE_SMARTHOME, 'smarthome', _('Smart home')),
-    (INAPP_AUDIENCE_HAUSBESITZER_VLL_ANGEHENDE_HB, 'hausbesitzer_vll_angehende_hb',
-     _('House owners (or future ones)')),
+    (INAPP_AUDIENCE_HAUSBESITZER_VLL_ANGEHENDE_HB, 'hausbesitzer_vll_angehende_hb', _('House owners (or future ones)')),
     (INAPP_AUDIENCE_JOBSUCHENDE, 'jobsuchende', _('Job seakers')),
     (INAPP_AUDIENCE_YOUNG_PROFESSIONALS, 'young_professionals', _('Young professionals')),
     (INAPP_AUDIENCE_KULTURINTERESSIERTE, 'kulturinteressierte', _('Cultural interested')),
-    (INAPP_AUDIENCE_TECHNIKSOFTWARE_INTERESSIERTE, 'techniksoftware_interessierte',
-     _('Technology/software interested')),
+    (
+        INAPP_AUDIENCE_TECHNIKSOFTWARE_INTERESSIERTE,
+        'techniksoftware_interessierte',
+        _('Technology/software interested'),
+    ),
     (INAPP_AUDIENCE_TECHNIK_LOVER, 'technik_lover', _('Tech lovers')),
     (INAPP_AUDIENCE_HIGH_INCOME_RICH_PEOPLE, 'high_income_rich_people', _('High income / rich people')),
     (INAPP_AUDIENCE_MILLENIALS, 'millenials', _('Millenials')),
     (INAPP_AUDIENCE_MOMS_KIDS, 'moms_kids', _('Moms & kids')),
     (INAPP_AUDIENCE_FAMILIENVATER, 'familienvater', _('Dads')),
     (INAPP_AUDIENCE_BEST_AGER, 'best_ager', _('Best ager')),
     (INAPP_AUDIENCE_BOSSHOME, 'bosshome', _('Boss@Home')),
@@ -612,53 +652,53 @@
 DISPLAY_NATIVE_SPORT = 24
 DISPLAY_NATIVE_STYLE_AND_FASHION = 25
 DISPLAY_NATIVE_TECHNOLOGY_AND_COMPUTER = 26
 DISPLAY_NATIVE_EVENTS_AND_ATTRACTIONS = 27
 DISPLAY_NATIVE_VIDEO_GAMES = 28
 DISPLAY_NATIVE_SCIENCE = 29
 DISPLAY_NATIVE_INTERESTS_TYPES = Choices(
-        (DISPLAY_NATIVE_AUTOMOTIVE, 'automotive', _('Automotive')),
-        (DISPLAY_NATIVE_EDUCATION, 'education', _('Education')),
-        (DISPLAY_NATIVE_BOOKS_AND_LITERATURE, 'books_and_literature', _('Books & Literature')),
-        (DISPLAY_NATIVE_EAT_AND_DRINK, 'eat_and_drink', _('Eat & Drink')),
-        (DISPLAY_NATIVE_FAMILY_AND_RELATIONSHIP, 'family_and_relationship', _('Family & Relationship')),
-        (DISPLAY_NATIVE_TELEVISION, 'television', _('Television')),
-        (DISPLAY_NATIVE_FILMS, 'films', _('Films')),
-        (DISPLAY_NATIVE_BUSINESS_AND_FINANCE, 'business_and_finance', _('Business & Finance')),
-        (DISPLAY_NATIVE_HEALTHY_LIFE, 'healthy_life', _('Healthy life')),
-        (DISPLAY_NATIVE_PROPERTY, 'property', _('Property')),
-        (DISPLAY_NATIVE_HOUSE_AND_GARDEN, 'house_and_garden', _('House & Garden')),
-        (DISPLAY_NATIVE_ANIMALS, 'animals', _('Animals')),
-        (DISPLAY_NATIVE_HOBBIES_AND_INTERESTS, 'hobbies_and_interests', _('Hobbies & Interests')),
-        (DISPLAY_NATIVE_CAREER, 'career', _('Career')),
-        (DISPLAY_NATIVE_ART, 'art', _('Art')),
-        (DISPLAY_NATIVE_MEDICAL_HEALTHMENT, 'medical_healthment', _('Medical healthment')),
-        (DISPLAY_NATIVE_MUSIC_AND_AUDIO, 'music_and_audio', _('Music & Audio')),
-        (DISPLAY_NATIVE_NEWS_AND_POLITICS, 'news_and_politics', _('News & Politics')),
-        (DISPLAY_NATIVE_PERSONAL_FINANCE, 'personal_finance', _('Personal finance')),
-        (DISPLAY_NATIVE_POP_CULTURE, 'pop_culture', _('Pop culture')),
-        (DISPLAY_NATIVE_TRAVEL, 'travel', _('Travel')),
-        (DISPLAY_NATIVE_RELIGION_AND_SPIRITUALITY, 'religion_and_spirituality', _('Religion & Spirituality')),
-        (DISPLAY_NATIVE_SHOPPING, 'shopping', _('Shopping')),
-        (DISPLAY_NATIVE_SPORT, 'sport', _('Sport')),
-        (DISPLAY_NATIVE_STYLE_AND_FASHION, 'style_and_fashion', _('Style & Fashion')),
-        (DISPLAY_NATIVE_TECHNOLOGY_AND_COMPUTER, 'technology_and_computer', _('Technology & Computer')),
-        (DISPLAY_NATIVE_EVENTS_AND_ATTRACTIONS, 'events_and_attractions', _('Events & Attractions')),
-        (DISPLAY_NATIVE_VIDEO_GAMES, 'video_games', _('Video games')),
-        (DISPLAY_NATIVE_SCIENCE, 'science', _('Science')),
-    )
+    (DISPLAY_NATIVE_AUTOMOTIVE, 'automotive', _('Automotive')),
+    (DISPLAY_NATIVE_EDUCATION, 'education', _('Education')),
+    (DISPLAY_NATIVE_BOOKS_AND_LITERATURE, 'books_and_literature', _('Books & Literature')),
+    (DISPLAY_NATIVE_EAT_AND_DRINK, 'eat_and_drink', _('Eat & Drink')),
+    (DISPLAY_NATIVE_FAMILY_AND_RELATIONSHIP, 'family_and_relationship', _('Family & Relationship')),
+    (DISPLAY_NATIVE_TELEVISION, 'television', _('Television')),
+    (DISPLAY_NATIVE_FILMS, 'films', _('Films')),
+    (DISPLAY_NATIVE_BUSINESS_AND_FINANCE, 'business_and_finance', _('Business & Finance')),
+    (DISPLAY_NATIVE_HEALTHY_LIFE, 'healthy_life', _('Healthy life')),
+    (DISPLAY_NATIVE_PROPERTY, 'property', _('Property')),
+    (DISPLAY_NATIVE_HOUSE_AND_GARDEN, 'house_and_garden', _('House & Garden')),
+    (DISPLAY_NATIVE_ANIMALS, 'animals', _('Animals')),
+    (DISPLAY_NATIVE_HOBBIES_AND_INTERESTS, 'hobbies_and_interests', _('Hobbies & Interests')),
+    (DISPLAY_NATIVE_CAREER, 'career', _('Career')),
+    (DISPLAY_NATIVE_ART, 'art', _('Art')),
+    (DISPLAY_NATIVE_MEDICAL_HEALTHMENT, 'medical_healthment', _('Medical healthment')),
+    (DISPLAY_NATIVE_MUSIC_AND_AUDIO, 'music_and_audio', _('Music & Audio')),
+    (DISPLAY_NATIVE_NEWS_AND_POLITICS, 'news_and_politics', _('News & Politics')),
+    (DISPLAY_NATIVE_PERSONAL_FINANCE, 'personal_finance', _('Personal finance')),
+    (DISPLAY_NATIVE_POP_CULTURE, 'pop_culture', _('Pop culture')),
+    (DISPLAY_NATIVE_TRAVEL, 'travel', _('Travel')),
+    (DISPLAY_NATIVE_RELIGION_AND_SPIRITUALITY, 'religion_and_spirituality', _('Religion & Spirituality')),
+    (DISPLAY_NATIVE_SHOPPING, 'shopping', _('Shopping')),
+    (DISPLAY_NATIVE_SPORT, 'sport', _('Sport')),
+    (DISPLAY_NATIVE_STYLE_AND_FASHION, 'style_and_fashion', _('Style & Fashion')),
+    (DISPLAY_NATIVE_TECHNOLOGY_AND_COMPUTER, 'technology_and_computer', _('Technology & Computer')),
+    (DISPLAY_NATIVE_EVENTS_AND_ATTRACTIONS, 'events_and_attractions', _('Events & Attractions')),
+    (DISPLAY_NATIVE_VIDEO_GAMES, 'video_games', _('Video games')),
+    (DISPLAY_NATIVE_SCIENCE, 'science', _('Science')),
+)
 
 CPM = 1
 CPV = 2
 CPC = 3
 BILLING_TYPES = Choices(
-        (CPM, 'cpm', _('CPM')),
-        (CPV, 'cpv', _('CPV')),
-        (CPC, 'cpc', _('CPC')),
-    )
+    (CPM, 'cpm', _('CPM')),
+    (CPV, 'cpv', _('CPV')),
+    (CPC, 'cpc', _('CPC')),
+)
 
 REGIOHELDEN = 1
 CUSTOMER = 2
 CREATIVE_CREATORS = Choices(
     (REGIOHELDEN, 'regiohelden', _('by RegioHelden')),
     (CUSTOMER, 'customer', _('by customer')),
 )
@@ -680,14 +720,15 @@
 
 
 class FileSerializer(serializers.Serializer):
     """
     proof of offer file, e.g. pdf with signature, file scan, etc
 
     """
+
     filename = serializers.CharField()
     content = serializers.CharField()
 
 
 class AccountSerializer(serializers.Serializer):
     """
     represents a customer
@@ -707,15 +748,16 @@
 
     """
     list of industry topic codes, e.g.
     "011100_3" for "Dienstleistung / Handwerk / Baugewerbe / Ladenbau / Maßmöbel"
 
     """
     branch_codes = serializers.ListField(
-        child=serializers.CharField(max_length=16, required=True), required=True, allow_empty=False)
+        child=serializers.CharField(max_length=16, required=True), required=True, allow_empty=False
+    )
 
     """
     generic comment on the customer
 
     """
     comment = serializers.CharField(max_length=200, allow_blank=True, required=False)
 
@@ -1035,15 +1077,16 @@
     billing_no_tax = serializers.BooleanField(required=True)
 
     """
     customer vat number to be added to the invoice for input tax deduction
 
     """
     billing_vat_number = serializers.CharField(
-        max_length=16, allow_blank=True, required=False, validators=[VATNumberValidator()])
+        max_length=16, allow_blank=True, required=False, validators=[VATNumberValidator()]
+    )
 
     """
     payment method of the customer, currently charge and transfer are supported
 
     """
     payment_type = serializers.ChoiceField(choices=PAYMENT_METHOD_CHOICES, required=True)
 
@@ -1052,15 +1095,16 @@
 
     data must be provided if payment_type == PAYMENT_METHOD_CHARGE
     let blank for all other payment methods
 
         orders.billing_contact_id)
     """
     payment_debit_account_iban = serializers.CharField(
-        max_length=34, allow_blank=True, required=False, validators=[IBANValidator()])
+        max_length=34, allow_blank=True, required=False, validators=[IBANValidator()]
+    )
 
     """
     owner of the customers bank account that will be charged
 
     data must be provided if payment_type == PAYMENT_METHOD_CHARGE
     let blank for all other payment methods
 
@@ -1081,70 +1125,43 @@
 
 class OrderLineGoogleAdsPremiumSerializer(serializers.Serializer):
     """
     detailed specifications and briefing information for a google ads premium product - "adwords" product subtype
     """
 
     """
-    call to action text, e.g. "Need help? Call us now"
-    """
-    call_to_action = serializers.CharField(max_length=200, allow_blank=True, required=False)
-
-    """
     what goals should be reached with the advertisement campaign?
     e.g. get new customers, spread word about a product, etc.
     """
     campaign_goal = serializers.CharField(max_length=200, allow_blank=True, required=False)
 
     """
-    the expected clicks when the campaign budget is initially calculated
-    """
-    expected_clicks = serializers.IntegerField(required=True)
-
-    """
-    the expected conversions when the campaign budget is initially calculated
-    """
-    expected_conversions = serializers.IntegerField(required=True)
-
-    """
     which cities/regions should the ad be targeted on?
     """
     regions = serializers.ListField(child=serializers.CharField(max_length=100, required=True), required=True)
 
     """
     customer preferred keywords to be found on with his campaign
     """
     keywords = serializers.ListField(child=serializers.CharField(max_length=100, required=True), required=True)
 
     """
-    customer preferred topics (branch_codes) from which the keywords will be used to build his campaigns
-    """
-    branch_codes = serializers.ListField(child=serializers.CharField(max_length=100, required=True), required=False)
-
-    """
-    list of keywords that resulted in zero search volume on campaign calculation
-    these keywords will not be guaranteed to be included in the campaign
-    """
-    keywords_with_zero_search_volume = serializers.ListField(child=serializers.CharField(max_length=100, required=True),
-                                                             required=True)
-
-    """
     definition of the target group this google ads campaign should be focused on
     """
     target_audience = serializers.CharField(max_length=1000, required=True)
 
     """
     usp describing the customers competitive advantage that should get a focus in the campaign texts
     """
     usp = serializers.CharField(max_length=1000, required=True)
 
     """
     chose which type of target page should be used in the ad? new or existing website
     """
-    target_page_type = serializers.ChoiceField(choices=GOOGLE_ADS_LANDING_PAGE_CHOICES, required=False)
+    target_page_type = serializers.ChoiceField(choices=GOOGLE_ADS_LANDING_PAGE_CHOICES, required=True)
 
     """
     url of the ads target website if CUSTOMER_WEBSITE is chosen in target_page_type
     """
     target_url = serializers.URLField(allow_blank=True, required=False)
 
     """
@@ -1162,62 +1179,24 @@
 
     """
     does the customer want to have a remarketing campaign included?
     """
     include_remarketing = serializers.BooleanField(required=False)
 
     """
-    if remarketing campaign is booked (include_remarketing=True) this id its own separate setup fee
-    """
-    remarketing_setup_fee = serializers.DecimalField(decimal_places=2, max_digits=10, allow_null=True, required=False)
-
-    """
-    if remarketing campaign is booked (include_remarketing=True) this id its own separate budget
-    """
-    remarketing_budget = serializers.DecimalField(decimal_places=2, max_digits=10, allow_null=True, required=False)
-
-    """
-    the expected impression share when the campaign budget is initially calculated
-    """
-    expected_impression_share = serializers.DecimalField(
-        decimal_places=2, max_digits=5, allow_null=True, required=False)
-
-    """
-    the expected impressions when the campaign budget is initially calculated
-    """
-    expected_impressions = serializers.CharField(max_length=50, allow_blank=True, required=False)
-    """
-    indicates if the campaign is generic
-    """
-    is_generic_campaign = serializers.BooleanField(required=False)
-    """
-    the topics related of the generic campaign
-    """
-    generic_topics = serializers.ListField(child=serializers.CharField(max_length=250), required=False)
-    """
     zammad ticket id of the original google ads offer inquiry
     """
     ticket_id = serializers.CharField(max_length=20, required=False)
 
-    def validate(self, data):
-        if data.get('include_remarketing') and data.get('remarketing_setup_fee') is None:
-            raise serializers.ValidationError(
-                {'remarketing_setup_fee': 'value >= 0 must be provided when include_remarketing is true'}
-            )
-        if data.get('include_remarketing') and not data.get('remarketing_budget'):
-            raise serializers.ValidationError(
-                {'remarketing_budget': 'value > 0 must be provided when include_remarketing is true'}
-            )
-        return data
-
 
 class DisplayNativeCreativeSerializer(serializers.Serializer):
     '''
     creative advertisement type
     '''
+
     ad_type = serializers.ChoiceField(choices=NATIVE_AD_TYPES, required=True)
     '''
     who will create teaser? - regiohelden or customer
     '''
     teaser = serializers.ChoiceField(choices=CREATIVE_CREATORS, allow_null=True, required=True)
     '''
     who will create advertorial? - regiohelden or customer.
@@ -1244,14 +1223,15 @@
         return data
 
 
 class OrderLineDisplayNativeSerializer(serializers.Serializer):
     '''
     billing model
     '''
+
     billing_type = serializers.ChoiceField(choices=BILLING_TYPES, required=True)
 
     '''
     unit can be impressions count, views or clicks, depends of billing type
     '''
     unit = serializers.IntegerField(min_value=0, required=True)
 
@@ -1313,17 +1293,15 @@
     '''
     age_group_to = serializers.IntegerField(min_value=0, allow_null=True, required=False)
 
     '''
     list of interests the ad will be targeted on
     '''
     interests = serializers.MultipleChoiceField(
-        choices=DISPLAY_NATIVE_INTERESTS_TYPES,
-        required=False,
-        allow_empty=True
+        choices=DISPLAY_NATIVE_INTERESTS_TYPES, required=False, allow_empty=True
     )
 
     '''
     miscellaneous should be targeted on
     '''
     miscellaneous = serializers.CharField(allow_blank=True, required=False)
 
@@ -1429,28 +1407,31 @@
 
     """
     list of german zip codes used for geographical targeting
     RH: must be converted to our geo targeting format
 
     HC: the zip code list must be converted to our targeting json format
     """
-    geo_targeting = serializers.ListField(child=serializers.CharField(max_length=10, required=True),
-                                          allow_empty=True, required=True)
+    geo_targeting = serializers.ListField(
+        child=serializers.CharField(max_length=10, required=True), allow_empty=True, required=True
+    )
 
     """
     list of channel names the ad will be targeted on
     """
     channel_targeting = serializers.MultipleChoiceField(
-        choices=DISPLAY_CHANNEL_CHOICES, required=True, allow_empty=True)
+        choices=DISPLAY_CHANNEL_CHOICES, required=True, allow_empty=True
+    )
 
     """
     list of interests the ad will be targeted on
     """
     interest_targeting = serializers.MultipleChoiceField(
-        choices=DISPLAY_TARGETING_CHOICES, required=False, allow_empty=True)
+        choices=DISPLAY_TARGETING_CHOICES, required=False, allow_empty=True
+    )
 
     """
     what goals should be reached with the advertisement campaign?
     e.g. get new customers, spread word about a product, etc.
     """
     campaign_goal = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
@@ -1472,18 +1453,20 @@
     HC: ProductDisplay.premium_for_html5 (true if CREATIVE_OPTION_CREATE_ANIMATED, false otherwise)
     """
     creative_options = serializers.ChoiceField(choices=CREATIVE_OPTION_CHOICES, required=True)
 
     def validate(self, data):
         if data.get('booking_type') == BOOKING_TYPE_FIXED and not data.get('impressions_one_time'):
             raise serializers.ValidationError(
-                {'impressions_one_time': 'If booking type is fixed, impressions_one_time is required'})
+                {'impressions_one_time': 'If booking type is fixed, impressions_one_time is required'}
+            )
         if data.get('booking_type') == BOOKING_TYPE_CONTINUOUS and not data.get('impressions_per_month'):
             raise serializers.ValidationError(
-                {'impressions_per_month': 'If booking type is continuous, impressions_per_month is required'})
+                {'impressions_per_month': 'If booking type is continuous, impressions_per_month is required'}
+            )
 
         return data
 
 
 class OrderLineFacebookDetailedTargetingSerializer(serializers.Serializer):
     """
     definition of a facebook ad detail targeting
@@ -1823,16 +1806,17 @@
     """
     opening_hours_description = serializers.CharField(max_length=140, allow_blank=True, required=False)
 
     """
     list of keywords that will be submitted to directories to classify the company
 
     """
-    keywords = serializers.ListField(child=serializers.CharField(max_length=55, required=True), allow_empty=True,
-                                     required=True)
+    keywords = serializers.ListField(
+        child=serializers.CharField(max_length=55, required=True), allow_empty=True, required=True
+    )
 
     """
     costs for t-online product
     if this number not a 0 than will be created a t-online product on the same location
 
     """
     tonline_costs = serializers.DecimalField(decimal_places=2, max_digits=10, required=False)
@@ -1895,22 +1879,22 @@
     target_page_credentials = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
     """
     topics to optimize for
 
     """
     topics = serializers.ListField(
-        child=serializers.CharField(max_length=100, required=True), required=True, allow_empty=False)
+        child=serializers.CharField(max_length=100, required=True), required=True, allow_empty=False
+    )
 
     """
     regions to optimize for
 
     """
-    regions = serializers.ListField(
-        child=serializers.CharField(max_length=100, required=True), required=False)
+    regions = serializers.ListField(child=serializers.CharField(max_length=100, required=True), required=False)
 
     """
     main focus of the seo optimization, which of the customers products/services is the most important?
 
     """
     focus = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
@@ -1955,14 +1939,19 @@
     additional_subpages = serializers.IntegerField(required=True, min_value=0)
 
     """
     should a new logo be created for the customer?
     """
     logo_creation = serializers.ChoiceField(choices=LOGO_CREATION_CHOICES, required=True)
 
+    """
+    easys system id of the related order line
+    """
+    easys_related_orderline_id = serializers.IntegerField(required=True)
+
 
 class OrderLineWebsiteSerializer(serializers.Serializer):
     """
     detailed specifications and briefing information for a website product
     """
 
     """
@@ -1990,29 +1979,32 @@
     briefing = serializers.CharField(max_length=200, required=True)
 
     """
     color code to be used when designing the creative (priority 1)
 
     """
     color_code_1 = serializers.CharField(
-        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()])
+        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()]
+    )
 
     """
     color code to be used when designing the creative (priority 2)
 
     """
     color_code_2 = serializers.CharField(
-        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()])
+        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()]
+    )
 
     """
     color code to be used when designing the creative (priority 3)
 
     """
     color_code_3 = serializers.CharField(
-        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()])
+        max_length=7, allow_blank=True, required=False, validators=[HexColorValidator()]
+    )
 
     """
     should a new logo be created for the customer?
 
     """
     logo_creation = serializers.ChoiceField(choices=LOGO_CREATION_CHOICES, required=True)
 
@@ -2029,36 +2021,40 @@
     logo_description = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
     """
     website design choice between minimalistic and embellished
 
     """
     design_preference_minimalistic_embellished = serializers.ChoiceField(
-        choices=WEBSITE_DESIGN_PREFERENCE_MINIMALISTIC_EMBELLISHED, allow_null=True, required=False)
+        choices=WEBSITE_DESIGN_PREFERENCE_MINIMALISTIC_EMBELLISHED, allow_null=True, required=False
+    )
 
     """
     website design choice between modern and classic
 
     """
     design_preference_modern_classic = serializers.ChoiceField(
-        choices=WEBSITE_DESIGN_PREFERENCE_MODERN_CLASSIC, allow_null=True, required=False)
+        choices=WEBSITE_DESIGN_PREFERENCE_MODERN_CLASSIC, allow_null=True, required=False
+    )
 
     """
     website design choice between simple and striking
 
     """
     design_preference_simple_striking = serializers.ChoiceField(
-        choices=WEBSITE_DESIGN_PREFERENCE_SIMPLE_STRIKING, allow_null=True, required=False)
+        choices=WEBSITE_DESIGN_PREFERENCE_SIMPLE_STRIKING, allow_null=True, required=False
+    )
 
     """
     website design choice between text and picture
 
     """
     design_preference_text_picture = serializers.ChoiceField(
-        choices=WEBSITE_DESIGN_PREFERENCE_TEXT_PICTURE, allow_null=True, required=False)
+        choices=WEBSITE_DESIGN_PREFERENCE_TEXT_PICTURE, allow_null=True, required=False
+    )
 
     """
     textual description of wishes and requirements for the website design
 
     """
     design_preferences = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
@@ -2290,38 +2286,44 @@
     """
     initial_term_months = serializers.IntegerField(min_value=1, required=True)
 
     """
     notice period during the initial contract term as months,days (e.g. 2,14)
 
     """
-    first_cancellation_period = serializers.CharField(max_length=5, validators=[validate_comma_separated_integer_list,
-                                                                                comma_separated_period_validatior],
-                                                      allow_blank=True,
-                                                      required=False)
+    first_cancellation_period = serializers.CharField(
+        max_length=5,
+        validators=[validate_comma_separated_integer_list, comma_separated_period_validatior],
+        allow_blank=True,
+        required=False,
+    )
 
     """
     notice period during extended contract terms as months,days (e.g. 2,14)
 
     """
-    cancellation_period = serializers.CharField(max_length=5, validators=[validate_comma_separated_integer_list,
-                                                                          comma_separated_period_validatior],
-                                                allow_blank=True,
-                                                required=False)
+    cancellation_period = serializers.CharField(
+        max_length=5,
+        validators=[validate_comma_separated_integer_list, comma_separated_period_validatior],
+        allow_blank=True,
+        required=False,
+    )
 
     """
     contract revocation period after product has been started, only valid for MDS customers as months,days (e.g. 2,14)
 
     ONE: will not be provided in the beginning and default has to be calculated on HC side
     """
     # this is a special case for mds customers
-    early_cancellation_period = serializers.CharField(max_length=5, validators=[validate_comma_separated_integer_list,
-                                                                                comma_separated_period_validatior],
-                                                      allow_blank=True,
-                                                      required=False)
+    early_cancellation_period = serializers.CharField(
+        max_length=5,
+        validators=[validate_comma_separated_integer_list, comma_separated_period_validatior],
+        allow_blank=True,
+        required=False,
+    )
 
     """
     invoicing period of the product (in months)
     """
     payment_cycle = serializers.ChoiceField(choices=PRODUCT_PAYMENT_CYCLE_CHOICES, required=False)
 
     """
@@ -2401,18 +2403,15 @@
     """
     is_pre_briefing_necessary = serializers.BooleanField(default=False)
 
     """
     salesforce opportunity line item id
     """
     salesforce_opportunity_line_item_id = serializers.CharField(
-        min_length=15,
-        max_length=18,
-        allow_blank=True,
-        required=False
+        min_length=15, max_length=18, allow_blank=True, required=False
     )
 
 
 class SellerSerializer(serializers.Serializer):
     """
     represents a selling user
     """
@@ -2545,128 +2544,192 @@
     orderlines = OrderLineSerializer(many=True, required=True)
 
     """
     sub-serializer for offer proof files
     """
     files = FileSerializer(many=True, required=True)
 
+    def _get_orderline_details(self, orderline):
+        product_type = orderline['product_type']
+        detail_key = PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING[product_type].intersection(orderline.keys()).pop()
+        return orderline[detail_key]
+
     def validate(self, data):
         self.validate_easys_ids(data=data)
         self.validate_seller_shares(data=data)
         self.validate_productdetail_exists(data=data)
         self.validate_productfee_commissions(data=data)
         self.validate_deferred_payments(data=data)
         self.validate_website_and_landingpage_exists(data=data)
         self.validate_domain_products_exist(data=data)
+        self.validate_landingpages_related_orderline_exists(data=data)
         return data
 
     def validate_productfee_commissions(self, data):
         for orderline in data['orderlines']:
-            if orderline['product_type'] in [PRODUCT_TYPE_GOOGLE_ADS] and \
-                    orderline['product_level'] in [PRODUCT_LEVEL_BASIC]:
+            if orderline['product_type'] in [PRODUCT_TYPE_GOOGLE_ADS] and orderline['product_level'] in [
+                PRODUCT_LEVEL_BASIC
+            ]:
                 if orderline.get('commission') != Decimal('40'):
-                    raise serializers.ValidationError('commission value for orderline {} is fixed to 40'.format(
-                        orderline['easys_id']
-                    ))
+                    raise serializers.ValidationError(
+                        'commission value for orderline {} is fixed to 40'.format(orderline['easys_id'])
+                    )
 
     def validate_deferred_payments(self, data):
         for orderline in data['orderlines']:
             if orderline.get('deferred_payment_sum', False) and not orderline.get('deferred_payment_months'):
-                raise serializers.ValidationError('deferred payment months is required for orderline {}'.format(
-                    orderline['easys_id']
-                ))
+                raise serializers.ValidationError(
+                    'deferred payment months is required for orderline {}'.format(orderline['easys_id'])
+                )
 
     def validate_seller_shares(self, data):
         # verify that all accounts of orders are known
         for order in data['orders']:
             # verify that the sum of all seller shares is exactly 100
             sellershare_sum = 0
             for sellershare in order['sellershares']:
                 sellershare_sum += sellershare['share']
             if sellershare_sum != 100:
                 raise serializers.ValidationError(
                     'summed up seller shares of order {} are {}, must be exactly 100'.format(
-                        order['easys_id'], sellershare_sum))
+                        order['easys_id'], sellershare_sum
+                    )
+                )
 
     def validate_productdetail_exists(self, data):
         for orderline in data['orderlines']:
             if orderline['product_type'] in PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING:
                 if not PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING[orderline['product_type']].intersection(orderline.keys()):
-                    raise serializers.ValidationError('orderline {} is missing the product detail data'.format(
-                        orderline['easys_id']))
+                    raise serializers.ValidationError(
+                        'orderline {} is missing the product detail data'.format(orderline['easys_id'])
+                    )
 
     def validate_website_and_landingpage_exists(self, data):
-        # if one products has a its target urls chosen to be a HC website or landingpage,
+        # if one product has its target urls chosen to be a HC website or landingpage,
         # validate that an order for it was delivered
         needs_website = False
         has_website = False
-        needs_landingpage = False
-        has_landingpage = False
+
+        missing_landingpages = []
+        lp_related_ids = (
+            self._get_orderline_details(o)['easys_related_orderline_id']
+            for o in data['orderlines']
+            if o['product_type'] == PRODUCT_TYPE_LANDINGPAGE
+        )
+
         for orderline in data['orderlines']:
-            if orderline['product_type'] in PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING:
-                detail_attribute = PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING[orderline['product_type']].intersection(
-                    orderline.keys()).pop()
-                if orderline[detail_attribute].get('target_page_type') == NEW_WEBSITE:
-                    needs_website = True
-                if orderline[detail_attribute].get('target_page_type') == NEW_LANDINGPAGE:
-                    needs_landingpage = True
-                if orderline['product_type'] == PRODUCT_TYPE_LANDINGPAGE:
-                    has_landingpage = True
-                if orderline['product_type'] == PRODUCT_TYPE_WEBSITE:
-                    has_website = True
-        if needs_landingpage and not has_landingpage:
-            raise serializers.ValidationError('orderline for Landingpage product has to be provided since it was a '
-                                              'selected option in target_page_type in other product.')
+            if (product_type := orderline['product_type']) not in PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING:
+                continue
+
+            target_page_type = self._get_orderline_details(orderline).get('target_page_type')
+            needs_website = needs_website or (target_page_type == NEW_WEBSITE)
+
+            if (target_page_type == NEW_LANDINGPAGE) and orderline['easys_id'] not in lp_related_ids:
+                missing_landingpages.append(orderline['easys_id'])
+
+            has_website = has_website or (product_type == PRODUCT_TYPE_WEBSITE)
+
+        if missing_landingpages:
+            raise serializers.ValidationError(
+                f'orderlines {", ".join(map(str, missing_landingpages))} are missing an associated Landingpage product'
+            )
         if needs_website and not has_website:
-            raise serializers.ValidationError('orderline for Website product has to be provided since it was a '
-                                              'selected option in target_page_type in other product.')
+            raise serializers.ValidationError(
+                'orderline for Website product has to be provided since it was a selected option in target_page_type '
+                'in other product.'
+            )
 
     def validate_easys_ids(self, data):
         # get ids to validate against
         account_id = data['account']['easys_id']
         account_location_ids = [d['easys_id'] for d in data['account_locations']]
         order_ids = [d['easys_id'] for d in data['orders']]
 
         # verify that all accounts on account locations are known
         for account_location in data['account_locations']:
             if account_location['easys_account_id'] != account_id:
-                raise serializers.ValidationError('account id {} of account location {} is not known'.format(
-                    account_location['easys_account_id'], account_location['easys_id']))
+                raise serializers.ValidationError(
+                    'account id {} of account location {} is not known'.format(
+                        account_location['easys_account_id'], account_location['easys_id']
+                    )
+                )
 
         # verify that all accounts of contacts are known
         for contact in data['contacts']:
             if contact['easys_account_id'] != account_id:
-                raise serializers.ValidationError('account id {} of contact {} is not known'.format(
-                    contact['easys_account_id'], contact['easys_id']))
+                raise serializers.ValidationError(
+                    'account id {} of contact {} is not known'.format(contact['easys_account_id'], contact['easys_id'])
+                )
 
         # verify that all accounts of orders are known
         for order in data['orders']:
             if order['easys_account_id'] != account_id:
-                raise serializers.ValidationError('account id {} of order {} is not known'.format(
-                    order['easys_account_id'], order['easys_id']))
+                raise serializers.ValidationError(
+                    'account id {} of order {} is not known'.format(order['easys_account_id'], order['easys_id'])
+                )
 
         # verify that all orders and account locations of orderlines are known
         for orderline in data['orderlines']:
             if orderline['easys_order_id'] not in order_ids:
-                raise serializers.ValidationError('order id {} of orderline {} is not known'.format(
-                    orderline['easys_order_id'], orderline['easys_id']))
+                raise serializers.ValidationError(
+                    'order id {} of orderline {} is not known'.format(
+                        orderline['easys_order_id'], orderline['easys_id']
+                    )
+                )
             if orderline['easys_account_location_id'] not in account_location_ids:
-                raise serializers.ValidationError('account location id {} of orderline {} is not known'.format(
-                    orderline['easys_account_location_id'], orderline['easys_id']))
+                raise serializers.ValidationError(
+                    'account location id {} of orderline {} is not known'.format(
+                        orderline['easys_account_location_id'], orderline['easys_id']
+                    )
+                )
 
     def validate_domain_products_exist(self, data):
         # verify all referenced domain products are seen in the same order
         domain_ids = {
             orderline['easys_id']
             for orderline in data['orderlines']
             if orderline['product_type'] == PRODUCT_TYPE_CHOICES.domain
         }
         for orderline in data['orderlines']:
             if orderline['product_type'] not in PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING:
                 continue
 
-            detail_attribute = PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING[orderline['product_type']].intersection(
-                orderline.keys()).pop()
+            detail_attribute = (
+                PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING[orderline['product_type']].intersection(orderline.keys()).pop()
+            )
             details = orderline[detail_attribute]
             if 'easys_orderline_domain_id' in details and not details['easys_orderline_domain_id'] in domain_ids:
-                raise serializers.ValidationError('domain id {} of orderline {} is not known'.format(
-                    details['easys_orderline_domain_id'], orderline['easys_id']))
+                raise serializers.ValidationError(
+                    'domain id {} of orderline {} is not known'.format(
+                        details['easys_orderline_domain_id'], orderline['easys_id']
+                    )
+                )
+
+    def validate_landingpages_related_orderline_exists(self, data):
+        """
+        check landingpage's `easys_related_orderline_id` is referencing to ID that is present in the payload
+        """
+        easys_ids = []
+        easys_related_orderline_ids = []
+
+        for orderline in data['orderlines']:
+            if (product_type := orderline['product_type']) not in PRODUCT_TYPE_ORDER_ATTRIBUTES_MAPPING:
+                continue
+
+            if product_type == PRODUCT_TYPE_LANDINGPAGE:
+                easys_related_orderline_ids.append(self._get_orderline_details(orderline)['easys_related_orderline_id'])
+            else:
+                easys_ids.append(orderline['easys_id'])
+
+        errors = []
+
+        for orderline_id in easys_related_orderline_ids:
+            if orderline_id in easys_ids:
+                easys_ids.remove(orderline_id)
+            else:
+                errors.append(
+                    f'Landingpage "easys_related_orderline_id" is invalid. '
+                    f'Order line ID {orderline_id} is not present in the payload or used multiple times.'
+                )
+
+        if errors:
+            raise serializers.ValidationError(errors)
```

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager/validators.py` & `easys-ordermanager-2.1.2/easys_ordermanager/validators.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager.egg-info/PKG-INFO` & `easys-ordermanager-2.1.2/easys_ordermanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.1.1
+Version: 2.1.2
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -30,14 +30,18 @@
 ### Django 4.1
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.1.2 (2023-04-12)
+* Updates to Serializer v3, see serializer changelog
+* Fixed missing development dependency
+
 ## 2.1.1 (2023-03-21)
 * Updates to Serializer v3, see serializer changelog
 * New test to validate payloads including EXISTING_STROER_LANDINGPAGE, and only a SEO product orderline.
 
 ## 2.1.0 (2023-03-16)
 * Introduction of serializer v3, see serializer changelog
 * `easys-ordermanager/easys_ordermanager/v3/serializer.Serializer` is considered WIP until integration in EasyS starts
@@ -422,14 +426,34 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.1.2
+
+#### `OrderLineGoogleAdsPremiumSerializer`
+* Made `target_page_type` required.
+* Removed fields:
+  - `expected_clicks`
+  - `expected_conversions`
+  - `expected_impression_share`
+  - `expected_impressions`
+  - `keywords_with_zero_search_volume`
+  - `branch_codes`
+  - `call_to_action`
+  - `is_generic_campaign`
+  - `generic_topics`
+  - `remarketing_setup_fee`
+  - `remarketing_budget`
+
+#### `OrderLineLandingpageSerializer`
+* Added field `easys_related_orderline_id`, referencing the easys ID of a product in the same payload, required. 
+
 ## 2.1.1
 
 ### v2/v3
 
 #### `EXISTING_STROER_LANDINGPAGE`
 
 * Change constant value from 3 to 4, to prevent clashes with `NEW_LANDINGPAGE` constant.
```

### Comparing `easys-ordermanager-2.1.1/easys_ordermanager.egg-info/SOURCES.txt` & `easys-ordermanager-2.1.2/easys_ordermanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.1.1/setup.py` & `easys-ordermanager-2.1.2/setup.py`

 * *Files identical despite different names*

