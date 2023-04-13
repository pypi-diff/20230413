# Comparing `tmp/django_hell_auth-0.0.2.tar.gz` & `tmp/django_hell_auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hell_auth-0.0.2.tar", max compression
+gzip compressed data, was "django_hell_auth-0.0.3.tar", max compression
```

## Comparing `django_hell_auth-0.0.2.tar` & `django_hell_auth-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-04-12 17:27:29.487511 django_hell_auth-0.0.2/LICENSE
--rw-r--r--   0        0        0      381 2023-04-13 12:12:44.301970 django_hell_auth-0.0.2/README.md
--rw-r--r--   0        0        0     1982 2023-04-13 12:08:12.987931 django_hell_auth-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-09 18:46:03.161079 django_hell_auth-0.0.2/src/django_hell_auth/__init__.py
--rw-r--r--   0        0        0     2240 2023-04-12 20:36:35.183743 django_hell_auth-0.0.2/src/django_hell_auth/oidc.py
--rw-r--r--   0        0        0      215 2023-04-12 20:36:35.167076 django_hell_auth-0.0.2/src/django_hell_auth/settings.py
--rw-r--r--   0        0        0      246 2023-04-12 20:36:35.167076 django_hell_auth-0.0.2/src/django_hell_auth/urls.py
--rw-r--r--   0        0        0     1621 2023-04-12 20:36:35.177076 django_hell_auth-0.0.2/src/django_hell_auth/views.py
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 django_hell_auth-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/LICENSE
+-rw-r--r--   0        0        0      381 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/README.md
+-rw-r--r--   0        0        0     1982 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/src/django_hell_auth/__init__.py
+-rw-r--r--   0        0        0     2240 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/src/django_hell_auth/oidc.py
+-rw-r--r--   0        0        0      215 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/src/django_hell_auth/settings.py
+-rw-r--r--   0        0        0      246 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/src/django_hell_auth/urls.py
+-rw-r--r--   0        0        0     1621 2023-04-13 12:19:03.893260 django_hell_auth-0.0.3/src/django_hell_auth/views.py
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 django_hell_auth-0.0.3/setup.py
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 django_hell_auth-0.0.3/PKG-INFO
```

### Comparing `django_hell_auth-0.0.2/LICENSE` & `django_hell_auth-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hell_auth-0.0.2/pyproject.toml` & `django_hell_auth-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-hell-auth"
-version = "0.0.2"
+version = "0.0.3"
 description = "hell gitlab auth for django"
 authors = [
     "David Bauer <hausprojekt@debauer.de>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `django_hell_auth-0.0.2/src/django_hell_auth/oidc.py` & `django_hell_auth-0.0.3/src/django_hell_auth/oidc.py`

 * *Files identical despite different names*

### Comparing `django_hell_auth-0.0.2/src/django_hell_auth/views.py` & `django_hell_auth-0.0.3/src/django_hell_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_hell_auth-0.0.2/PKG-INFO` & `django_hell_auth-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hell-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: hell gitlab auth for django
 License: MIT
 Author: David Bauer
 Author-email: hausprojekt@debauer.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

