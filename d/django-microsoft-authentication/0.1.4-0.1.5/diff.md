# Comparing `tmp/django-microsoft-authentication-0.1.4.tar.gz` & `tmp/django-microsoft-authentication-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-microsoft-authentication-0.1.4.tar", last modified: Thu Feb 16 21:39:32 2023, max compression
+gzip compressed data, was "django-microsoft-authentication-0.1.5.tar", last modified: Wed Apr 12 22:51:53 2023, max compression
```

## Comparing `django-microsoft-authentication-0.1.4.tar` & `django-microsoft-authentication-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 21:39:32.575477 django-microsoft-authentication-0.1.4/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1072 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/LICENSE
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-02-16 21:39:32.575311 django-microsoft-authentication-0.1.4/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     3584 2023-02-16 21:39:07.000000 django-microsoft-authentication-0.1.4/README.md
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 21:39:32.573287 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-02-16 21:39:32.000000 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      723 2023-02-16 21:39:32.000000 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2023-02-16 21:39:32.000000 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       21 2023-02-16 21:39:32.000000 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/requires.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       25 2023-02-16 21:39:32.000000 django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 21:39:32.574470 django-microsoft-authentication-0.1.4/microsoft_authentication/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/admin.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      122 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/apps.py
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 21:39:32.574909 django-microsoft-authentication-0.1.4/microsoft_authentication/auth/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/auth/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1002 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/auth/auth_decorators.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     2812 2023-02-16 21:38:43.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/auth/auth_utils.py
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 21:39:32.575130 django-microsoft-authentication-0.1.4/microsoft_authentication/migrations/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/migrations/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/models.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       60 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/tests.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      425 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/urls.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      975 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.4/microsoft_authentication/views.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2023-02-16 21:39:32.575522 django-microsoft-authentication-0.1.4/setup.cfg
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1646 2023-02-16 21:39:15.000000 django-microsoft-authentication-0.1.4/setup.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.752261 django-microsoft-authentication-0.1.5/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1072 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/LICENSE
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-04-12 22:51:53.752014 django-microsoft-authentication-0.1.5/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     3584 2023-02-16 21:39:07.000000 django-microsoft-authentication-0.1.5/README.md
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.750145 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4136 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      723 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       21 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/requires.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       25 2023-04-12 22:51:53.000000 django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751163 django-microsoft-authentication-0.1.5/microsoft_authentication/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/admin.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      122 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/apps.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751610 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1002 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_decorators.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     2812 2023-02-16 21:38:43.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_utils.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-04-12 22:51:53.751855 django-microsoft-authentication-0.1.5/microsoft_authentication/migrations/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/migrations/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        0 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/models.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       60 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/tests.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      425 2023-02-16 20:07:23.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/urls.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1243 2023-04-12 22:49:57.000000 django-microsoft-authentication-0.1.5/microsoft_authentication/views.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2023-04-12 22:51:53.752330 django-microsoft-authentication-0.1.5/setup.cfg
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1646 2023-04-12 22:50:48.000000 django-microsoft-authentication-0.1.5/setup.py
```

### Comparing `django-microsoft-authentication-0.1.4/LICENSE` & `django-microsoft-authentication-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.4/PKG-INFO` & `django-microsoft-authentication-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-authentication
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django based app for Microsoft authentication of users.
 Home-page: https://github.com/shubhamdipt/django-microsoft-authentication
 Author: Shubham Dipt
 Author-email: shubham.dipt@gmail.com
 License: MIT
 Keywords: django,microsoft,authentication
 Platform: any
```

### Comparing `django-microsoft-authentication-0.1.4/README.md` & `django-microsoft-authentication-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/PKG-INFO` & `django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-authentication
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django based app for Microsoft authentication of users.
 Home-page: https://github.com/shubhamdipt/django-microsoft-authentication
 Author: Shubham Dipt
 Author-email: shubham.dipt@gmail.com
 License: MIT
 Keywords: django,microsoft,authentication
 Platform: any
```

### Comparing `django-microsoft-authentication-0.1.4/django_microsoft_authentication.egg-info/SOURCES.txt` & `django-microsoft-authentication-0.1.5/django_microsoft_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.4/microsoft_authentication/auth/auth_decorators.py` & `django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_decorators.py`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.4/microsoft_authentication/auth/auth_utils.py` & `django-microsoft-authentication-0.1.5/microsoft_authentication/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `django-microsoft-authentication-0.1.4/setup.py` & `django-microsoft-authentication-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools import setup
 
 # Usage: python setup.py sdist bdist_wheel
 
 links = []  # for repo urls (dependency_links)
 
 DESCRIPTION = "Django based app for Microsoft authentication of users."
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 setup(
     name="django-microsoft-authentication",
     version=VERSION,
     author="Shubham Dipt",
     author_email="shubham.dipt@gmail.com",
     description=DESCRIPTION,
```

