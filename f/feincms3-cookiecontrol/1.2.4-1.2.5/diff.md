# Comparing `tmp/feincms3_cookiecontrol-1.2.4.tar.gz` & `tmp/feincms3_cookiecontrol-1.2.5.tar.gz`

## Comparing `feincms3_cookiecontrol-1.2.4.tar` & `feincms3_cookiecontrol-1.2.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/admin.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/apps.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/embedding.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/models.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/views.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/migrations/0001_rework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/migrations/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/templatetags/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/LICENSE
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/README.rst
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/admin.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/apps.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/embedding.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/models.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/views.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/0001_rework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/__init__.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/README.rst
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.2.5/PKG-INFO
```

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/embedding.py` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/models.py` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/views.py` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/views.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/migrations/0001_rework.py` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/migrations/0001_rework.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/static/feincms3_cookiecontrol/build.js`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py` & `feincms3_cookiecontrol-1.2.5/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/LICENSE` & `feincms3_cookiecontrol-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/README.rst` & `feincms3_cookiecontrol-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/pyproject.toml` & `feincms3_cookiecontrol-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.2.4/PKG-INFO` & `feincms3_cookiecontrol-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feincms3-cookiecontrol
-Version: 1.2.4
+Version: 1.2.5
 Summary: Cookie Control Panel for GDPR compliant feincms3 websites
 Project-URL: Homepage, https://github.com/feinheit/feincms3-cookiecontrol/
 Author-email: York Schickl <ys@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

