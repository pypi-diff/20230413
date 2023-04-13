# Comparing `tmp/retrofix-0.8.tar.gz` & `tmp/retrofix-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/retrofix-0.8.tar", last modified: Tue Sep 23 08:33:57 2014, max compression
+gzip compressed data, was "dist/retrofix-0.9.tar", last modified: Mon Feb 16 20:47:08 2015, max compression
```

## Comparing `retrofix-0.8.tar` & `retrofix-0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 guillem   (1000) guillem   (1000)        0 2014-09-23 08:33:57.000000 retrofix-0.8/
-drwxrwxr-x   0 guillem   (1000) guillem   (1000)        0 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/
--rw-r--r--   0 guillem   (1000) guillem   (1000)        9 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/top_level.txt
--rw-r--r--   0 guillem   (1000) guillem   (1000)        1 2014-02-25 16:21:50.000000 retrofix-0.8/retrofix.egg-info/not-zip-safe
--rw-r--r--   0 guillem   (1000) guillem   (1000)        1 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/dependency_links.txt
--rw-r--r--   0 guillem   (1000) guillem   (1000)       17 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/requires.txt
--rw-r--r--   0 guillem   (1000) guillem   (1000)      554 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/SOURCES.txt
--rw-r--r--   0 guillem   (1000) guillem   (1000)     1579 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix.egg-info/PKG-INFO
--rw-r--r--   0 guillem   (1000) guillem   (1000)      595 2014-02-25 16:19:46.000000 retrofix-0.8/README
-drwxrwxr-x   0 guillem   (1000) guillem   (1000)        0 2014-09-23 08:33:57.000000 retrofix-0.8/retrofix/
--rw-rw-r--   0 guillem   (1000) guillem   (1000)     6954 2014-09-23 08:24:10.000000 retrofix-0.8/retrofix/aeat303.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     7425 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c34_01.py
--rw-rw-r--   0 guillem   (1000) guillem   (1000)     3307 2014-02-27 18:57:22.000000 retrofix-0.8/retrofix/aeat349.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     6373 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c58.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     4801 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/aeat347.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     5255 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c43.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)    10382 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c34.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     7451 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/aeat340.py
--rwxr-xr-x   0 guillem   (1000) guillem   (1000)     4521 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/record.py
--rw-rw-r--   0 guillem   (1000) guillem   (1000)     1042 2014-09-23 08:31:43.000000 retrofix-0.8/retrofix/version.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     8421 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c19.py
--rw-rw-r--   0 guillem   (1000) guillem   (1000)     8771 2014-09-23 08:24:10.000000 retrofix-0.8/retrofix/fields.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     1814 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/formatting.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)      984 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/__init__.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)    14361 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c34_1_la_caixa.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)      995 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/exception.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     7575 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c32.py
--rw-r--r--   0 guillem   (1000) guillem   (1000)     9431 2014-02-25 16:19:46.000000 retrofix-0.8/retrofix/c34_11.py
--rw-rw-r--   0 guillem   (1000) guillem   (1000)       59 2014-09-23 08:33:57.000000 retrofix-0.8/setup.cfg
--rw-r--r--   0 guillem   (1000) guillem   (1000)     2222 2014-02-25 16:20:11.000000 retrofix-0.8/setup.py
--rw-rw-r--   0 guillem   (1000) guillem   (1000)     1579 2014-09-23 08:33:57.000000 retrofix-0.8/PKG-INFO
+drwxr-xr-x   0 albert    (1000) albert    (1000)        0 2015-02-16 20:47:08.000000 retrofix-0.9/
+-rw-r--r--   0 albert    (1000) albert    (1000)       59 2015-02-16 20:47:08.000000 retrofix-0.9/setup.cfg
+-rw-r--r--   0 albert    (1000) albert    (1000)     1579 2015-02-16 20:47:08.000000 retrofix-0.9/PKG-INFO
+-rw-r--r--   0 albert    (1000) albert    (1000)      595 2015-02-16 20:36:17.000000 retrofix-0.9/README
+drwxr-xr-x   0 albert    (1000) albert    (1000)        0 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/
+-rw-r--r--   0 albert    (1000) albert    (1000)        9 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/top_level.txt
+-rw-r--r--   0 albert    (1000) albert    (1000)     1579 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/PKG-INFO
+-rw-r--r--   0 albert    (1000) albert    (1000)      554 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/SOURCES.txt
+-rw-r--r--   0 albert    (1000) albert    (1000)        1 2015-02-16 20:38:44.000000 retrofix-0.9/retrofix.egg-info/not-zip-safe
+-rw-r--r--   0 albert    (1000) albert    (1000)       17 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/requires.txt
+-rw-r--r--   0 albert    (1000) albert    (1000)        1 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix.egg-info/dependency_links.txt
+-rw-r--r--   0 albert    (1000) albert    (1000)     2222 2015-02-16 20:36:17.000000 retrofix-0.9/setup.py
+drwxr-xr-x   0 albert    (1000) albert    (1000)        0 2015-02-16 20:47:08.000000 retrofix-0.9/retrofix/
+-rwxr-xr-x   0 albert    (1000) albert    (1000)     4521 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/record.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     5184 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/aeat347.py
+-rw-r--r--   0 albert    (1000) albert    (1000)    10382 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c34.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     8421 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c19.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     6373 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c58.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     8771 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/fields.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     7575 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c32.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     9431 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c34_11.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     6954 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/aeat303.py
+-rw-r--r--   0 albert    (1000) albert    (1000)      984 2013-08-14 22:02:51.000000 retrofix-0.9/retrofix/__init__.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     3307 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/aeat349.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     1042 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/version.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     7451 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/aeat340.py
+-rw-r--r--   0 albert    (1000) albert    (1000)    14361 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c34_1_la_caixa.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     1814 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/formatting.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     5255 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c43.py
+-rw-r--r--   0 albert    (1000) albert    (1000)      995 2013-08-14 15:00:16.000000 retrofix-0.9/retrofix/exception.py
+-rw-r--r--   0 albert    (1000) albert    (1000)     7425 2015-02-16 20:36:17.000000 retrofix-0.9/retrofix/c34_01.py
```

### Comparing `retrofix-0.8/retrofix.egg-info/SOURCES.txt` & `retrofix-0.9/retrofix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix.egg-info/PKG-INFO` & `retrofix-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: retrofix
-Version: 0.8
+Version: 0.9
 Summary: retrofix
 Home-page: http://www.NaN-tic.com/
 Author: NaN·tic
 Author-email: info@nan-tic.com
 License: GPL-3
-Download-URL: https://pypi.python.org/pypi/retrofix/0.8
+Download-URL: https://pypi.python.org/pypi/retrofix/0.9
 Description: retrofix
         ========
         
         RetroFix is a python library for reading and writing fixed-size field text file
         and more specifically for managing files from Spanish banks and public
         institutions, including:
```

### Comparing `retrofix-0.8/README` & `retrofix-0.9/README`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/aeat303.py` & `retrofix-0.9/retrofix/aeat303.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c34_01.py` & `retrofix-0.9/retrofix/c34_01.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/aeat349.py` & `retrofix-0.9/retrofix/aeat349.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c58.py` & `retrofix-0.9/retrofix/c58.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/aeat347.py` & `retrofix-0.9/retrofix/aeat347.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # encoding: utf8
 ##############################################################################
 #
 #    Copyright (C) 2013 NaN Projectes de Programari Lliure, S.L.
 #                           http://www.NaN-tic.com
+#    Copyright (C) 2015 Zikzakmedia S.L.
+#                           http://www.zikzakmedia.com
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -35,15 +37,15 @@
     (108, 13, 'declaration_number', Number(align='right')),
     (121,  1, 'complementary', Char),
     (122,  1, 'replacement', Char),
     (123, 13, 'previous_declaration_number', Number(align='right')),
     (136,  9, 'party_count', Integer),
     (145, 16, 'party_amount', Numeric(sign=SIGN_N)),
     (161,  9, 'property_count', Integer),
-    (170, 15, 'property_amount', Numeric),
+    (170, 16, 'property_amount', Numeric(sign=SIGN_N)),
     (391,  9, 'representative_nif', Char),
     (488, 13, 'digital_signature', Char),
     )
 
 PARTY_RECORD = (
     (  1,  1, 'record_code', Const('2')),
     (  2,  3, 'model', Const('347')),
@@ -66,15 +68,20 @@
     (152, 16, 'first_quarter_property_amount', Numeric(sign=SIGN_N)),
     (168, 16, 'second_quarter_amount', Numeric(sign=SIGN_N)),
     (184, 16, 'second_quarter_property_amount', Numeric(sign=SIGN_N)),
     (200, 16, 'third_quarter_amount', Numeric(sign=SIGN_N)),
     (216, 16, 'third_quarter_property_amount', Numeric(sign=SIGN_N)),
     (232, 16, 'fourth_quarter_amount', Numeric(sign=SIGN_N)),
     (248, 16, 'fourth_quarter_property_amount', Numeric(sign=SIGN_N)),
-    (264, 237, 'blank', Char),
+    (264, 17, 'community_vat', Char),
+    (281,  1, 'cash_vat_operation', Boolean(BOOLEAN_X)),
+    (282,  1, 'tax_person_operation', Boolean(BOOLEAN_X)),
+    (283,  1, 'related_goods_operation', Boolean(BOOLEAN_X)),
+    (284, 16, 'cash_vat_criteria', Numeric(sign=SIGN_N)),
+    (300, 201, 'blank', Char),
     )
 
 PROPERTY_RECORD = (
     (  1,  1, 'record_code', Const('2')),
     (  2,  3, 'model', Const('347')),
     (  5,  4, 'fiscalyear', Number),
     (  9,  9, 'nif', Char),
```

### Comparing `retrofix-0.8/retrofix/c43.py` & `retrofix-0.9/retrofix/c43.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c34.py` & `retrofix-0.9/retrofix/c34.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/aeat340.py` & `retrofix-0.9/retrofix/aeat340.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/record.py` & `retrofix-0.9/retrofix/record.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/version.py` & `retrofix-0.9/retrofix/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ##############################################################################
 
 PACKAGE = 'retrofix'
-VERSION = '0.8'
+VERSION = '0.9'
 LICENSE = 'GPL-3'
 WEBSITE = 'http://www.NaN-tic.com/'
```

### Comparing `retrofix-0.8/retrofix/c19.py` & `retrofix-0.9/retrofix/c19.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/fields.py` & `retrofix-0.9/retrofix/fields.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/formatting.py` & `retrofix-0.9/retrofix/formatting.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/__init__.py` & `retrofix-0.9/retrofix/__init__.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c34_1_la_caixa.py` & `retrofix-0.9/retrofix/c34_1_la_caixa.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/exception.py` & `retrofix-0.9/retrofix/exception.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c32.py` & `retrofix-0.9/retrofix/c32.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/retrofix/c34_11.py` & `retrofix-0.9/retrofix/c34_11.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/setup.py` & `retrofix-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `retrofix-0.8/PKG-INFO` & `retrofix-0.9/retrofix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: retrofix
-Version: 0.8
+Version: 0.9
 Summary: retrofix
 Home-page: http://www.NaN-tic.com/
 Author: NaN·tic
 Author-email: info@nan-tic.com
 License: GPL-3
-Download-URL: https://pypi.python.org/pypi/retrofix/0.8
+Download-URL: https://pypi.python.org/pypi/retrofix/0.9
 Description: retrofix
         ========
         
         RetroFix is a python library for reading and writing fixed-size field text file
         and more specifically for managing files from Spanish banks and public
         institutions, including:
```

