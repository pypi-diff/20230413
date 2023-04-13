# Comparing `tmp/django-computedfields-0.2.1.tar.gz` & `tmp/django-computedfields-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-computedfields-0.2.1.tar", last modified: Wed Aug  3 15:48:44 2022, max compression
+gzip compressed data, was "dist/django-computedfields-0.2.2.tar", last modified: Thu Apr 13 14:26:14 2023, max compression
```

## Comparing `django-computedfields-0.2.1.tar` & `django-computedfields-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.387729 django-computedfields-0.2.1/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1023 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/LICENSE.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      150 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/MANIFEST.in
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     6878 2022-08-03 15:48:44.387729 django-computedfields-0.2.1/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5753 2022-08-03 15:44:26.000000 django-computedfields-0.2.1/README.md
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.379729 django-computedfields-0.2.1/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2022-08-03 15:44:26.000000 django-computedfields-0.2.1/computedfields/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     9123 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/admin.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1880 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/apps.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    35588 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/graph.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8597 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/handlers.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2751 2022-04-18 09:39:28.000000 django-computedfields-0.2.1/computedfields/helper.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.379729 django-computedfields-0.2.1/computedfields/management/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/computedfields/management/__init__.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.379729 django-computedfields-0.2.1/computedfields/management/commands/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/computedfields/management/commands/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2063 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/management/commands/_helpers.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8414 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/management/commands/checkdata.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2367 2022-04-15 08:50:44.000000 django-computedfields-0.2.1/computedfields/management/commands/rendergraph.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1900 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/management/commands/showdependencies.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     9711 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/management/commands/updatedata.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.383729 django-computedfields-0.2.1/computedfields/migrations/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      656 2020-04-24 12:52:14.000000 django-computedfields-0.2.1/computedfields/migrations/0001_initial.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      703 2020-04-24 12:52:14.000000 django-computedfields-0.2.1/computedfields/migrations/0002_contributingmodelsmodel.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      537 2020-07-14 19:41:57.000000 django-computedfields-0.2.1/computedfields/migrations/0003_auto_20200713_2212.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/computedfields/migrations/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5505 2022-04-15 08:50:44.000000 django-computedfields-0.2.1/computedfields/models.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    40894 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/resolver.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      902 2022-04-17 14:52:45.000000 django-computedfields-0.2.1/computedfields/settings.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.375729 django-computedfields-0.2.1/computedfields/static/
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.383729 django-computedfields-0.2.1/computedfields/static/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)  1441964 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/computedfields/static/computedfields/viz-lite.js
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.375729 django-computedfields-0.2.1/computedfields/templates/
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.383729 django-computedfields-0.2.1/computedfields/templates/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      991 2020-05-22 18:15:10.000000 django-computedfields-0.2.1/computedfields/templates/computedfields/change_list.html
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      750 2020-05-22 18:15:10.000000 django-computedfields-0.2.1/computedfields/templates/computedfields/graph.html
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.387729 django-computedfields-0.2.1/django_computedfields.egg-info/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     6878 2022-08-03 15:48:44.000000 django-computedfields-0.2.1/django_computedfields.egg-info/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1296 2022-08-03 15:48:44.000000 django-computedfields-0.2.1/django_computedfields.egg-info/SOURCES.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2022-08-03 15:48:44.000000 django-computedfields-0.2.1/django_computedfields.egg-info/dependency_links.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       61 2022-08-03 15:48:44.000000 django-computedfields-0.2.1/django_computedfields.egg-info/requires.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       15 2022-08-03 15:48:44.000000 django-computedfields-0.2.1/django_computedfields.egg-info/top_level.txt
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 15:48:44.387729 django-computedfields-0.2.1/docs/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      618 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/docs/Makefile
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5517 2022-01-26 15:45:25.000000 django-computedfields-0.2.1/docs/conf.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    54109 2022-04-18 12:52:27.000000 django-computedfields-0.2.1/docs/examples.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2020-05-29 20:53:10.000000 django-computedfields-0.2.1/docs/index.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      789 2019-03-10 14:07:26.000000 django-computedfields-0.2.1/docs/make.bat
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    30903 2022-08-03 15:44:26.000000 django-computedfields-0.2.1/docs/manual.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2022-04-15 08:50:44.000000 django-computedfields-0.2.1/docs/reference.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2022-08-03 15:48:44.387729 django-computedfields-0.2.1/setup.cfg
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1820 2022-08-03 15:44:26.000000 django-computedfields-0.2.1/setup.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    40930 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/resolver.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/migrations/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      656 2020-04-24 12:52:14.000000 django-computedfields-0.2.2/computedfields/migrations/0001_initial.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      703 2020-04-24 12:52:14.000000 django-computedfields-0.2.2/computedfields/migrations/0002_contributingmodelsmodel.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/migrations/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      537 2020-07-14 19:41:57.000000 django-computedfields-0.2.2/computedfields/migrations/0003_auto_20200713_2212.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/management/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/management/__init__.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/management/commands/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/management/commands/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     9735 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/management/commands/updatedata.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1900 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/management/commands/showdependencies.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2063 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/management/commands/_helpers.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8420 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/management/commands/checkdata.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2367 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/computedfields/management/commands/rendergraph.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     9129 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/admin.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/templates/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      991 2020-05-22 18:15:10.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/change_list.html
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      750 2020-05-22 18:15:10.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/graph.html
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/static/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/static/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)  1441964 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/static/computedfields/viz-lite.js
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    35600 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/graph.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      902 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/settings.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5505 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/computedfields/models.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8633 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/handlers.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2751 2022-04-18 09:39:28.000000 django-computedfields-0.2.2/computedfields/helper.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1880 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/apps.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1834 2023-04-13 14:19:50.000000 django-computedfields-0.2.2/setup.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/setup.cfg
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/docs/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    30903 2022-08-03 15:44:26.000000 django-computedfields-0.2.2/docs/manual.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    54109 2022-04-18 12:52:27.000000 django-computedfields-0.2.2/docs/examples.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      618 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/docs/Makefile
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/docs/reference.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2020-05-29 20:53:10.000000 django-computedfields-0.2.2/docs/index.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5517 2022-01-26 15:45:25.000000 django-computedfields-0.2.2/docs/conf.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      789 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/docs/make.bat
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1296 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8366 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       59 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/requires.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       15 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/top_level.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      150 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/MANIFEST.in
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1023 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/LICENSE.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8366 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5912 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-computedfields-0.2.1/LICENSE.txt` & `django-computedfields-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/PKG-INFO` & `django-computedfields-0.2.2/django_computedfields.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,195 @@
 Metadata-Version: 2.1
 Name: django-computedfields
-Version: 0.2.1
+Version: 0.2.2
 Summary: autoupdated database fields for model methods
 Home-page: https://github.com/netzkolchose/django-computedfields
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.1.tar.gz
+Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz
+Description: [![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
+        
+        
+        ### django-computedfields ###
+        
+        django-computedfields provides autoupdated database fields
+        for model methods.
+        
+        Tested with Django 3.2 and 4.2 (Python 3.7 to 3.10).
+        
+        
+        #### Example ####
+        
+        Just derive your model from `ComputedFieldsModel` and place
+        the `@computed` decorator at a method:
+        
+        ```python
+        from django.db import models
+        from computedfields.models import ComputedFieldsModel, computed
+        
+        class MyModel(ComputedFieldsModel):
+            name = models.CharField(max_length=32)
+        
+            @computed(models.CharField(max_length=32), depends=[('self', ['name'])])
+            def computed_field(self):
+                return self.name.upper()
+        ```
+        
+        `computed_field` will be turned into a real database field
+        and can be accessed and searched like any other database field.
+        During saving the associated method gets called and it’s result
+        written to the database.
+        
+        
+        #### How to recalculate without saving the model record ####
+        
+        If you need to recalculate the computed field but without saving it, use
+        `from computedfields.models import compute`
+        
+        ```python
+        >>> from computedfields.models import compute
+        >>> person = MyModel.objects.get(id=1)  # this is to retrieve existing record
+        >>> person.computed_field               # outputs 'BERTY'
+        >>> person.name = 'nina'                # changing the dependent field `name` to nina
+        >>> compute(person, 'computed_field')   # outputs 'NINA'
+        >>> person.computed_field               # outputs 'BERTY' because the `person` is not yet saved
+        >>> person.save()                       # alters the database record for `name` and `computed_field`
+        >>> person.computed_field               # outputs 'NINA'
+        ```
+        
+        #### `depends` keyword
+        
+        The  `depends` keyword argument can be used with any relation to indicate dependencies to fields on other models as well:
+        
+        ```python
+        from django.db import models
+        from computedfields.models import ComputedFieldsModel, computed
+        
+        class MyModel(ComputedFieldsModel):
+            name = models.CharField(max_length=32)
+            fk = models.ForeignKey(SomeModel)
+        
+            @computed(
+                models.CharField(max_length=32),
+                depends=[
+                    ('self', ['name']),
+                    ('fk', ['fieldname'])
+                ]
+            )
+            def computed_field(self):
+                return self.name.upper() + self.fk.fieldname
+        ```
+        
+        Now changes to `self.name`, `fk` or `fk.fieldname` will update `computed_field`.
+        
+        
+        #### Documentation ####
+        
+        The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
+        
+        
+        #### Changelog ####
+        
+        - 0.2.2
+            - Django 4.2 support
+            - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
+        
+        - 0.2.1
+            - Django 4.1 support
+        
+        - 0.2.0 - next beta release
+            - new features:
+                - better memory control for the update resolver via
+                  ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
+                - update optimization - early update-tree exit
+                - faster updates with ``COMPUTEDFIELDS_FASTUPDATE``
+                - `checkdata` command
+                - `showdependencies` command
+                - typing support for computed fields
+        
+            - enhancements:
+                - better `updatedata` command
+        
+            - removed features:
+                - transitive reduction on intermodel graph (due to negative impact)
+                - pickled resolver map (due to showing low benefit)
+                - `update_dependent_multi` and `preupdate_dependent_multi`
+                  (due to showing low benefit and being a code nuisance)
+                - Django 2.2 shims removed
+        
+            - bug fixes:
+                - regression on proxy models fixed
+                - sliced querset support for mysql fixed
+        
+        - 0.1.7
+            - add list type support for `update_fields` in signal handlers
+        
+        - 0.1.6
+            - maintenace version with CI test dependencies changes:
+                - removed Python 3.6
+                - removed Django 2.2
+                - added Python 3.10
+                - added Django 4.0
+                - move dev environment to Python 3.10 and Django 3.2
+        
+              Note that Django 2.2 will keep working until real incompatible code changes occur.
+              This may happen by any later release, thus treat 0.1.6 as last compatible version.
+        
+        - 0.1.5
+            - fix error on model instance cloning
+        - 0.1.4
+            - Django 3.2 support
+        - 0.1.3
+            - better multi table inheritance support and test cases
+            - explicit docs for multi table inheritance
+        - 0.1.2
+            - bugfix: o2o reverse name access
+            - add docs about model inheritance support
+        - 0.1.1
+            - bugfix: add missing migration
+        - 0.1.0
+            - fix recursion on empty queryset
+            - dependency expansion on M2M fields
+            - `m2m_changed` handler with filtering on m2m fields
+            - remove custom metaclass, introducing *Resolver* class
+            - new decorator `@precomputed` for custom save methods
+            - old *depends* syntax removed
+            - docs update
+        - 0.0.23:
+            - Bugfix: Fixing leaking computed fields in model inheritance.
+        - 0.0.22:
+            - Automatic dependency expansion on reverse relations.
+            - Example documentation.
+        - 0.0.21:
+            - Bugfix: Fixing undefined _batchsize for pickled map usage.
+        - 0.0.20
+            - Use `bulk_update` for computed field updates.
+            - Allow custom update optimizations with *select_related* and *prefetch_related*.
+            - Respect computed field MRO in `compute`.
+            - Allow updates on local computed fields from `update_dependent` simplifying bulk actions on `ComputedFieldsModel`.
+        - 0.0.19
+            - Better graph expansion on relation paths with support for *update_fields*.
+        - 0.0.18
+            - New *depends* syntax deprecating the old one.
+            - MRO of local computed field methods implemented.
+        - 0.0.17
+            - Dropped Python 2.7 and Django 1.11 support.
+        
 Keywords: django,method,decorator,autoupdate,persistent,field
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
-[![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
-
-
-### django-computedfields ###
-
-django-computedfields provides autoupdated database fields
-for model methods.
-
-Tested with Django 3.2 and 4.0 (Python 3.7 to 3.10).
-
-
-#### Example ####
-
-Just derive your model from `ComputedFieldsModel` and place
-the `@computed` decorator at a method:
-
-```python
-from django.db import models
-from computedfields.models import ComputedFieldsModel, computed
-
-class MyModel(ComputedFieldsModel):
-    name = models.CharField(max_length=32)
-
-    @computed(models.CharField(max_length=32), depends=[('self', ['name'])])
-    def computed_field(self):
-        return self.name.upper()
-```
-
-`computed_field` will be turned into a real database field
-and can be accessed and searched like any other database field.
-During saving the associated method gets called and it’s result
-written to the database. 
-
-
-#### How to recalculate without saving the model record ####
-
-If you need to recalculate the computed field but without saving it, use
-`from computedfields.models import compute`
-
-```python
->>> from computedfields.models import compute
->>> person = MyModel.objects.get(id=1)  # this is to retrieve existing record
->>> person.computed_field               # outputs 'BERTY'
->>> person.name = 'nina'                # changing the dependent field `name` to nina
->>> compute(person, 'computed_field')   # outputs 'NINA'
->>> person.computed_field               # outputs 'BERTY' because the `person` is not yet saved
->>> person.save()                       # alters the database record for `name` and `computed_field`
->>> person.computed_field               # outputs 'NINA'
-```
-
-#### `depends` keyword
-
-The  `depends` keyword argument can be used with any relation to indicate dependencies to fields on other models as well:
-
-```python
-from django.db import models
-from computedfields.models import ComputedFieldsModel, computed
-
-class MyModel(ComputedFieldsModel):
-    name = models.CharField(max_length=32)
-    fk = models.ForeignKey(SomeModel)
-
-    @computed(
-        models.CharField(max_length=32),
-        depends=[
-            ('self', ['name']),
-            ('fk', ['fieldname'])
-        ]
-    )
-    def computed_field(self):
-        return self.name.upper() + self.fk.fieldname
-```
-
-Now changes to `self.name`, `fk` or `fk.fieldname` will update `computed_field`.
-
-
-#### Documentation ####
-
-The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
-
-
-#### Changelog ####
-
-- 0.2.1
-    - Django 4.1 support
-
-- 0.2.0 - next beta release
-    - new features:
-        - better memory control for the update resolver via
-          ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
-        - update optimization - early update-tree exit
-        - faster updates with ``COMPUTEDFIELDS_FASTUPDATE``
-        - `checkdata` command
-        - `showdependencies` command
-        - typing support for computed fields
-
-    - enhancements:
-        - better `updatedata` command
-
-    - removed features:
-        - transitive reduction on intermodel graph (due to negative impact)
-        - pickled resolver map (due to showing low benefit)
-        - `update_dependent_multi` and `preupdate_dependent_multi`
-          (due to showing low benefit and being a code nuisance)
-        - Django 2.2 shims removed
-
-    - bug fixes:
-        - regression on proxy models fixed
-        - sliced querset support for mysql fixed
-
-- 0.1.7
-    - add list type support for `update_fields` in signal handlers
-
-- 0.1.6
-    - maintenace version with CI test dependencies changes:
-        - removed Python 3.6
-        - removed Django 2.2
-        - added Python 3.10
-        - added Django 4.0
-        - move dev environment to Python 3.10 and Django 3.2
-
-      Note that Django 2.2 will keep working until real incompatible code changes occur.
-      This may happen by any later release, thus treat 0.1.6 as last compatible version.
-
-- 0.1.5
-    - fix error on model instance cloning
-- 0.1.4
-    - Django 3.2 support
-- 0.1.3
-    - better multi table inheritance support and test cases
-    - explicit docs for multi table inheritance
-- 0.1.2
-    - bugfix: o2o reverse name access
-    - add docs about model inheritance support
-- 0.1.1
-    - bugfix: add missing migration
-- 0.1.0
-    - fix recursion on empty queryset
-    - dependency expansion on M2M fields
-    - `m2m_changed` handler with filtering on m2m fields
-    - remove custom metaclass, introducing *Resolver* class
-    - new decorator `@precomputed` for custom save methods
-    - old *depends* syntax removed
-    - docs update
-- 0.0.23:
-    - Bugfix: Fixing leaking computed fields in model inheritance.
-- 0.0.22:
-    - Automatic dependency expansion on reverse relations.
-    - Example documentation.
-- 0.0.21:
-    - Bugfix: Fixing undefined _batchsize for pickled map usage.
-- 0.0.20
-    - Use `bulk_update` for computed field updates.
-    - Allow custom update optimizations with *select_related* and *prefetch_related*.
-    - Respect computed field MRO in `compute`.
-    - Allow updates on local computed fields from `update_dependent` simplifying bulk actions on `ComputedFieldsModel`.
-- 0.0.19
-    - Better graph expansion on relation paths with support for *update_fields*.
-- 0.0.18
-    - New *depends* syntax deprecating the old one.
-    - MRO of local computed field methods implemented.
-- 0.0.17
-    - Dropped Python 2.7 and Django 1.11 support.
-
-
```

### Comparing `django-computedfields-0.2.1/README.md` & `django-computedfields-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 ### django-computedfields ###
 
 django-computedfields provides autoupdated database fields
 for model methods.
 
-Tested with Django 3.2 and 4.0 (Python 3.7 to 3.10).
+Tested with Django 3.2 and 4.2 (Python 3.7 to 3.10).
 
 
 #### Example ####
 
 Just derive your model from `ComputedFieldsModel` and place
 the `@computed` decorator at a method:
 
@@ -26,15 +26,15 @@
     def computed_field(self):
         return self.name.upper()
 ```
 
 `computed_field` will be turned into a real database field
 and can be accessed and searched like any other database field.
 During saving the associated method gets called and it’s result
-written to the database. 
+written to the database.
 
 
 #### How to recalculate without saving the model record ####
 
 If you need to recalculate the computed field but without saving it, use
 `from computedfields.models import compute`
 
@@ -78,14 +78,18 @@
 #### Documentation ####
 
 The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
 
 
 #### Changelog ####
 
+- 0.2.2
+    - Django 4.2 support
+    - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
+
 - 0.2.1
     - Django 4.1 support
 
 - 0.2.0 - next beta release
     - new features:
         - better memory control for the update resolver via
           ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
```

### Comparing `django-computedfields-0.2.1/computedfields/admin.py` & `django-computedfields-0.2.2/computedfields/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         return render(request, 'computedfields/graph.html', {'error': error, 'dot': dot})
 
     def render_modelgraph(self, request, modelid, extra_context=None):
         """
         Render modelgraph view.
         """
         try:
-            inst = self.model.objects.get(pk=modelid)
+            inst = self.model._base_manager.get(pk=modelid)
             model = apps.get_model(inst.app_label, inst.model)
         except ObjectDoesNotExist:
             error = 'illegal value for model'
             return render(request, 'computedfields/graph.html', {'error': error, 'dot': ''})
         error = 'graphviz must be installed to use this feature.'
         dot = ''
         if Digraph:
```

### Comparing `django-computedfields-0.2.1/computedfields/apps.py` & `django-computedfields-0.2.2/computedfields/apps.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/graph.py` & `django-computedfields-0.2.2/computedfields/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,16 +646,16 @@
             src_model:[src_field, ...] --> target_model:[(cf_field, filter_string), ...]
 
         During runtime ``update_dependent`` will use the the information to create
         select querysets on the target_models (roughly):
 
         .. code:: python
 
-            qs = target_model.objects.filter(filter_string=src_model.instance)
-            qs |= target_model.objects.filter(filter_string2=src_model.instance)
+            qs = target_model._base_manager.filter(filter_string=src_model.instance)
+            qs |= target_model._base_manager.filter(filter_string2=src_model.instance)
             ...
             bulk_updater(qs, cf_fields)
 
         The fk map list all models with fk fieldnames, that contribute to computed fields.
 
         Returns a tuple of (lookup_map, fk_map).
         """
```

### Comparing `django-computedfields-0.2.1/computedfields/handlers.py` & `django-computedfields-0.2.2/computedfields/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """
     # after deletion we can update the associated computed fields
     updates = DELETES.pop(instance, None)
     if updates:
         with transaction.atomic():
             for model, [pks, fields] in updates.items():
                 active_resolver.bulk_updater(
-                    model.objects.filter(pk__in=pks),
+                    model._base_manager.filter(pk__in=pks),
                     fields,
                     querysize=settings.COMPUTEDFIELDS_QUERYSIZE
                 )
 
 
 def merge_pk_maps(
     obj1: Dict[Type[Model], List[Any]],
@@ -142,15 +142,15 @@
     obj2: Dict[Type[Model], List[Any]]
 ) -> Dict[Type[Model], List[Any]]:
     """
     Merge queryset map in `obj2` on `obj1`.
     Updates obj1 inplace and also returns it.
     """
     for model, [qs2, fields2] in obj2.items():
-        query_field = obj1.setdefault(model, [model.objects.none(), set()])
+        query_field = obj1.setdefault(model, [model._base_manager.none(), set()])
         query_field[0] |= qs2            # or'ed querysets
         query_field[1].update(fields2)   # add fields
     return obj1
 
 
 def m2m_handler(sender: Type[Model], instance: Model, **kwargs) -> None:
     """
@@ -177,15 +177,15 @@
     model = kwargs['model']
 
     if action == 'post_add':
         pks_add: Set[Any] = kwargs['pk_set']
         data_add: Dict[Type[Model], List[Any]] = active_resolver._querysets_for_update(
             type(instance), instance, update_fields={left})
         other_add: Dict[Type[Model], List[Any]] = active_resolver._querysets_for_update(
-            model, model.objects.filter(pk__in=pks_add), update_fields={right})
+            model, model._base_manager.filter(pk__in=pks_add), update_fields={right})
         if other_add:
             merge_qs_maps(data_add, other_add)
         if data_add:
             with transaction.atomic():
                 for queryset, update_fields in data_add.values():
                     active_resolver.bulk_updater(
                         queryset,
@@ -194,27 +194,27 @@
                     )
 
     elif action == 'pre_remove':
         pks_remove: Set[Any] = kwargs['pk_set']
         data_remove: Dict[Type[Model], List[Any]] = active_resolver._querysets_for_update(
             type(instance), instance, update_fields={left}, pk_list=True)
         other_remove: Dict[Type[Model], List[Any]] = active_resolver._querysets_for_update(
-            model, model.objects.filter(pk__in=pks_remove), update_fields={right}, pk_list=True)
+            model, model._base_manager.filter(pk__in=pks_remove), update_fields={right}, pk_list=True)
         if other_remove:
             merge_pk_maps(data_remove, other_remove)
         if data_remove:
             M2M_REMOVE[instance] = data_remove
 
     elif action == 'post_remove':
         updates_remove: Dict[Type[Model], List[Any]] = M2M_REMOVE.pop(instance, None)
         if updates_remove:
             with transaction.atomic():
                 for _model, [pks, update_fields] in updates_remove.items():
                     active_resolver.bulk_updater(
-                        _model.objects.filter(pk__in=pks),
+                        _model._base_manager.filter(pk__in=pks),
                         update_fields,
                         querysize=settings.COMPUTEDFIELDS_QUERYSIZE
                     )
 
     elif action == 'pre_clear':
         data: Dict[Type[Model], List[Any]] = active_resolver._querysets_for_update(
             type(instance), instance, update_fields={left}, pk_list=True)
@@ -227,11 +227,11 @@
 
     elif action == 'post_clear':
         updates_clear: Dict[Type[Model], List[Any]] = M2M_CLEAR.pop(instance, None)
         if updates_clear:
             with transaction.atomic():
                 for _model, [pks, update_fields] in updates_clear.items():
                     active_resolver.bulk_updater(
-                        _model.objects.filter(pk__in=pks),
+                        _model._base_manager.filter(pk__in=pks),
                         update_fields,
                         querysize=settings.COMPUTEDFIELDS_QUERYSIZE
                     )
```

### Comparing `django-computedfields-0.2.1/computedfields/helper.py` & `django-computedfields-0.2.2/computedfields/helper.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/management/commands/_helpers.py` & `django-computedfields-0.2.2/computedfields/management/commands/_helpers.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/management/commands/checkdata.py` & `django-computedfields-0.2.2/computedfields/management/commands/checkdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.eprint(f'\nTotal check time: {timedelta(seconds=duration)}')
         sys.exit(1 if has_desync else 0)
     
     @transaction.atomic
     def action_check(self, models, progress, size, json_out):
         has_desync = False
         for model in models:
-            qs = model.objects.all()
+            qs = model._base_manager.all()
             amount = qs.count()
             fields = set(active_resolver.computed_models[model].keys())
             qsize = active_resolver.get_querysize(model, fields, size)
             self.eprint(f'- {self.style.MIGRATE_LABEL(modelname(model))}')
             self.eprint(f'  Fields: {", ".join(fields)}')
             self.eprint(f'  Records: {amount}')
             if not amount:
```

### Comparing `django-computedfields-0.2.1/computedfields/management/commands/rendergraph.py` & `django-computedfields-0.2.2/computedfields/management/commands/rendergraph.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/management/commands/showdependencies.py` & `django-computedfields-0.2.2/computedfields/management/commands/showdependencies.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/management/commands/updatedata.py` & `django-computedfields-0.2.2/computedfields/management/commands/updatedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,34 +95,34 @@
             if progress:
                 qsize = size
                 if qsize > amount/100:
                     qsize = amount // 100 or 1
                 with tqdm(total=amount, desc='  Update', unit=' rec') as bar:
                     pos = 0
                     while pos < amount:
-                        active_resolver.update_dependent(model.objects.filter(pk__in=desync[pos:pos+qsize]))
+                        active_resolver.update_dependent(model._base_manager.filter(pk__in=desync[pos:pos+qsize]))
                         progressed = min(pos+qsize, amount) - pos
                         bar.update(progressed)
                         pos += qsize
             else:
-                active_resolver.update_dependent(model.objects.filter(pk__in=desync))
+                active_resolver.update_dependent(model._base_manager.filter(pk__in=desync))
 
     @transaction.atomic
     def action_default(self, models, size, show_progress, mode=''):
         """
         Runs either in fast or bulk mode, whatever was set in settings.
         """
         if not mode:
             mode = 'fast' if settings.COMPUTEDFIELDS_FASTUPDATE else 'bulk'
             print(f'Update mode: settings.py --> {mode}')
 
         print(f'Default querysize: {size}')
         print('Models:')
         for model in models:
-            qs = model.objects.all()
+            qs = model._base_manager.all()
             amount = qs.count()
             fields = set(active_resolver.computed_models[model].keys())
             print(f'- {self.style.MIGRATE_LABEL(modelname(model))}')
             print(f'  Fields: {", ".join(fields)}')
             print(f'  Records: {amount}')
             print(f'  Querysize: {active_resolver.get_querysize(model, fields, size)}')
 
@@ -175,15 +175,15 @@
         print('Models:')
         if size != settings.COMPUTEDFIELDS_QUERYSIZE:
             # patch django settings in case querysize was explicitly given
             # needed here, as we have no other API to announce the changed value
             from django.conf import settings as ds
             ds.COMPUTEDFIELDS_QUERYSIZE = size
         for model in models:
-            qs = model.objects.all()
+            qs = model._base_manager.all()
             amount = qs.count()
             fields = list(active_resolver.computed_models[model].keys())
             qsize = active_resolver.get_querysize(model, fields, size)
             print(f'- {self.style.MIGRATE_LABEL(modelname(model))}')
             print(f'  Fields: {", ".join(fields)}')
             print(f'  Records: {amount}')
             print(f'  Querysize: {qsize}')
```

### Comparing `django-computedfields-0.2.1/computedfields/migrations/0001_initial.py` & `django-computedfields-0.2.2/computedfields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/migrations/0002_contributingmodelsmodel.py` & `django-computedfields-0.2.2/computedfields/migrations/0002_contributingmodelsmodel.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/migrations/0003_auto_20200713_2212.py` & `django-computedfields-0.2.2/computedfields/migrations/0003_auto_20200713_2212.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/models.py` & `django-computedfields-0.2.2/computedfields/models.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/resolver.py` & `django-computedfields-0.2.2/computedfields/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,17 +347,17 @@
             for model, resolver in modeldata[update].items():
                 fields, paths = resolver
                 m_fields, m_paths = model_updates.setdefault(model, (set(), set()))
                 m_fields.update(fields)
                 m_paths.update(paths)
         for model, data in model_updates.items():
             fields, paths = data
-            queryset: Any = model.objects.none()
+            queryset: Any = model._base_manager.none()
             for path in paths:
-                queryset |= model.objects.filter(**{path+subquery: instance})
+                queryset |= model._base_manager.filter(**{path+subquery: instance})
             if pk_list:
                 # need pks for post_delete since the real queryset will be empty
                 # after deleting the instance in question
                 # since we need to interact with the db anyways
                 # we can already drop empty results here
                 queryset = set(queryset.values_list('pk', flat=True).iterator())
                 if not queryset:
@@ -460,15 +460,15 @@
 
         # Note: update_local is always off for updates triggered from the resolver
         # but True by default to avoid accidentally skipping updates called by user
         if update_local and self.has_computedfields(_model):
             # We skip a transaction here in the same sense,
             # as local cf updates are not guarded either.
             queryset = instance if isinstance(instance, QuerySet) \
-                else _model.objects.filter(pk__in=[instance.pk])
+                else _model._base_manager.filter(pk__in=[instance.pk])
             self.bulk_updater(queryset, _update_fields, local_only=True, querysize=querysize)
 
         updates = self._querysets_for_update(_model, instance, _update_fields).values()
         if updates:
             with transaction.atomic():  # FIXME: place transaction only once in tree descent
                 pks_updated: Dict[Type[Model], Set[Any]] = {}
                 for queryset, fields in updates:
@@ -514,15 +514,15 @@
         # TODO: distinct is a major query perf smell, and is in fact only needed on back relations
         #       may need some rework in _querysets_for_update
         #       ideally we find a way to avoid it for forward relations
         #       also see #101
         if queryset.query.can_filter() and not queryset.query.distinct_fields:
             queryset = queryset.distinct()
         else:
-            queryset = model.objects.filter(pk__in=subquery_pk(queryset, queryset.db))
+            queryset = model._base_manager.filter(pk__in=subquery_pk(queryset, queryset.db))
 
         # correct update_fields by local mro
         mro = self.get_local_mro(model, update_fields)
         fields: Any = set(mro)  # FIXME: narrow type once issue in django-stubs is resolved
         if update_fields:
             update_fields.update(fields)
 
@@ -555,22 +555,22 @@
             if change:
                 self._update(queryset, change, fields)
 
         # trigger dependent comp field updates from changed records
         # other than before we exit the update tree early, if we have no changes at all
         # also cuts the update tree for recursive deps (tree-like)
         if not local_only and pks:
-            self.update_dependent(model.objects.filter(pk__in=pks), model, fields, update_local=False)
+            self.update_dependent(model._base_manager.filter(pk__in=pks), model, fields, update_local=False)
         return set(pks) if return_pks else None
     
     def _update(self, queryset: QuerySet, change: Sequence[Any], fields: Sequence[str]) -> Union[int, None]:
         # we can skip batch_size here, as it already was batched in bulk_updater
         if self.use_fastupdate:
             return fast_update(queryset, change, fields, None)
-        return queryset.model.objects.bulk_update(change, fields)
+        return queryset.model._base_manager.bulk_update(change, fields)
 
     def _compute(self, instance: Model, model: Type[Model], fieldname: str) -> Any:
         """
         Returns the computed field value for ``fieldname``.
         Note that this is just a shorthand method for calling the underlying computed
         field method and does not deal with local MRO, thus should only be used,
         if the MRO is respected by other means.
```

### Comparing `django-computedfields-0.2.1/computedfields/settings.py` & `django-computedfields-0.2.2/computedfields/settings.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/static/computedfields/viz-lite.js` & `django-computedfields-0.2.2/computedfields/static/computedfields/viz-lite.js`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/templates/computedfields/change_list.html` & `django-computedfields-0.2.2/computedfields/templates/computedfields/change_list.html`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/computedfields/templates/computedfields/graph.html` & `django-computedfields-0.2.2/computedfields/templates/computedfields/graph.html`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/django_computedfields.egg-info/PKG-INFO` & `django-computedfields-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,195 @@
 Metadata-Version: 2.1
 Name: django-computedfields
-Version: 0.2.1
+Version: 0.2.2
 Summary: autoupdated database fields for model methods
 Home-page: https://github.com/netzkolchose/django-computedfields
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.1.tar.gz
+Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz
+Description: [![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
+        
+        
+        ### django-computedfields ###
+        
+        django-computedfields provides autoupdated database fields
+        for model methods.
+        
+        Tested with Django 3.2 and 4.2 (Python 3.7 to 3.10).
+        
+        
+        #### Example ####
+        
+        Just derive your model from `ComputedFieldsModel` and place
+        the `@computed` decorator at a method:
+        
+        ```python
+        from django.db import models
+        from computedfields.models import ComputedFieldsModel, computed
+        
+        class MyModel(ComputedFieldsModel):
+            name = models.CharField(max_length=32)
+        
+            @computed(models.CharField(max_length=32), depends=[('self', ['name'])])
+            def computed_field(self):
+                return self.name.upper()
+        ```
+        
+        `computed_field` will be turned into a real database field
+        and can be accessed and searched like any other database field.
+        During saving the associated method gets called and it’s result
+        written to the database.
+        
+        
+        #### How to recalculate without saving the model record ####
+        
+        If you need to recalculate the computed field but without saving it, use
+        `from computedfields.models import compute`
+        
+        ```python
+        >>> from computedfields.models import compute
+        >>> person = MyModel.objects.get(id=1)  # this is to retrieve existing record
+        >>> person.computed_field               # outputs 'BERTY'
+        >>> person.name = 'nina'                # changing the dependent field `name` to nina
+        >>> compute(person, 'computed_field')   # outputs 'NINA'
+        >>> person.computed_field               # outputs 'BERTY' because the `person` is not yet saved
+        >>> person.save()                       # alters the database record for `name` and `computed_field`
+        >>> person.computed_field               # outputs 'NINA'
+        ```
+        
+        #### `depends` keyword
+        
+        The  `depends` keyword argument can be used with any relation to indicate dependencies to fields on other models as well:
+        
+        ```python
+        from django.db import models
+        from computedfields.models import ComputedFieldsModel, computed
+        
+        class MyModel(ComputedFieldsModel):
+            name = models.CharField(max_length=32)
+            fk = models.ForeignKey(SomeModel)
+        
+            @computed(
+                models.CharField(max_length=32),
+                depends=[
+                    ('self', ['name']),
+                    ('fk', ['fieldname'])
+                ]
+            )
+            def computed_field(self):
+                return self.name.upper() + self.fk.fieldname
+        ```
+        
+        Now changes to `self.name`, `fk` or `fk.fieldname` will update `computed_field`.
+        
+        
+        #### Documentation ####
+        
+        The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
+        
+        
+        #### Changelog ####
+        
+        - 0.2.2
+            - Django 4.2 support
+            - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
+        
+        - 0.2.1
+            - Django 4.1 support
+        
+        - 0.2.0 - next beta release
+            - new features:
+                - better memory control for the update resolver via
+                  ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
+                - update optimization - early update-tree exit
+                - faster updates with ``COMPUTEDFIELDS_FASTUPDATE``
+                - `checkdata` command
+                - `showdependencies` command
+                - typing support for computed fields
+        
+            - enhancements:
+                - better `updatedata` command
+        
+            - removed features:
+                - transitive reduction on intermodel graph (due to negative impact)
+                - pickled resolver map (due to showing low benefit)
+                - `update_dependent_multi` and `preupdate_dependent_multi`
+                  (due to showing low benefit and being a code nuisance)
+                - Django 2.2 shims removed
+        
+            - bug fixes:
+                - regression on proxy models fixed
+                - sliced querset support for mysql fixed
+        
+        - 0.1.7
+            - add list type support for `update_fields` in signal handlers
+        
+        - 0.1.6
+            - maintenace version with CI test dependencies changes:
+                - removed Python 3.6
+                - removed Django 2.2
+                - added Python 3.10
+                - added Django 4.0
+                - move dev environment to Python 3.10 and Django 3.2
+        
+              Note that Django 2.2 will keep working until real incompatible code changes occur.
+              This may happen by any later release, thus treat 0.1.6 as last compatible version.
+        
+        - 0.1.5
+            - fix error on model instance cloning
+        - 0.1.4
+            - Django 3.2 support
+        - 0.1.3
+            - better multi table inheritance support and test cases
+            - explicit docs for multi table inheritance
+        - 0.1.2
+            - bugfix: o2o reverse name access
+            - add docs about model inheritance support
+        - 0.1.1
+            - bugfix: add missing migration
+        - 0.1.0
+            - fix recursion on empty queryset
+            - dependency expansion on M2M fields
+            - `m2m_changed` handler with filtering on m2m fields
+            - remove custom metaclass, introducing *Resolver* class
+            - new decorator `@precomputed` for custom save methods
+            - old *depends* syntax removed
+            - docs update
+        - 0.0.23:
+            - Bugfix: Fixing leaking computed fields in model inheritance.
+        - 0.0.22:
+            - Automatic dependency expansion on reverse relations.
+            - Example documentation.
+        - 0.0.21:
+            - Bugfix: Fixing undefined _batchsize for pickled map usage.
+        - 0.0.20
+            - Use `bulk_update` for computed field updates.
+            - Allow custom update optimizations with *select_related* and *prefetch_related*.
+            - Respect computed field MRO in `compute`.
+            - Allow updates on local computed fields from `update_dependent` simplifying bulk actions on `ComputedFieldsModel`.
+        - 0.0.19
+            - Better graph expansion on relation paths with support for *update_fields*.
+        - 0.0.18
+            - New *depends* syntax deprecating the old one.
+            - MRO of local computed field methods implemented.
+        - 0.0.17
+            - Dropped Python 2.7 and Django 1.11 support.
+        
 Keywords: django,method,decorator,autoupdate,persistent,field
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
-[![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
-
-
-### django-computedfields ###
-
-django-computedfields provides autoupdated database fields
-for model methods.
-
-Tested with Django 3.2 and 4.0 (Python 3.7 to 3.10).
-
-
-#### Example ####
-
-Just derive your model from `ComputedFieldsModel` and place
-the `@computed` decorator at a method:
-
-```python
-from django.db import models
-from computedfields.models import ComputedFieldsModel, computed
-
-class MyModel(ComputedFieldsModel):
-    name = models.CharField(max_length=32)
-
-    @computed(models.CharField(max_length=32), depends=[('self', ['name'])])
-    def computed_field(self):
-        return self.name.upper()
-```
-
-`computed_field` will be turned into a real database field
-and can be accessed and searched like any other database field.
-During saving the associated method gets called and it’s result
-written to the database. 
-
-
-#### How to recalculate without saving the model record ####
-
-If you need to recalculate the computed field but without saving it, use
-`from computedfields.models import compute`
-
-```python
->>> from computedfields.models import compute
->>> person = MyModel.objects.get(id=1)  # this is to retrieve existing record
->>> person.computed_field               # outputs 'BERTY'
->>> person.name = 'nina'                # changing the dependent field `name` to nina
->>> compute(person, 'computed_field')   # outputs 'NINA'
->>> person.computed_field               # outputs 'BERTY' because the `person` is not yet saved
->>> person.save()                       # alters the database record for `name` and `computed_field`
->>> person.computed_field               # outputs 'NINA'
-```
-
-#### `depends` keyword
-
-The  `depends` keyword argument can be used with any relation to indicate dependencies to fields on other models as well:
-
-```python
-from django.db import models
-from computedfields.models import ComputedFieldsModel, computed
-
-class MyModel(ComputedFieldsModel):
-    name = models.CharField(max_length=32)
-    fk = models.ForeignKey(SomeModel)
-
-    @computed(
-        models.CharField(max_length=32),
-        depends=[
-            ('self', ['name']),
-            ('fk', ['fieldname'])
-        ]
-    )
-    def computed_field(self):
-        return self.name.upper() + self.fk.fieldname
-```
-
-Now changes to `self.name`, `fk` or `fk.fieldname` will update `computed_field`.
-
-
-#### Documentation ####
-
-The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
-
-
-#### Changelog ####
-
-- 0.2.1
-    - Django 4.1 support
-
-- 0.2.0 - next beta release
-    - new features:
-        - better memory control for the update resolver via
-          ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
-        - update optimization - early update-tree exit
-        - faster updates with ``COMPUTEDFIELDS_FASTUPDATE``
-        - `checkdata` command
-        - `showdependencies` command
-        - typing support for computed fields
-
-    - enhancements:
-        - better `updatedata` command
-
-    - removed features:
-        - transitive reduction on intermodel graph (due to negative impact)
-        - pickled resolver map (due to showing low benefit)
-        - `update_dependent_multi` and `preupdate_dependent_multi`
-          (due to showing low benefit and being a code nuisance)
-        - Django 2.2 shims removed
-
-    - bug fixes:
-        - regression on proxy models fixed
-        - sliced querset support for mysql fixed
-
-- 0.1.7
-    - add list type support for `update_fields` in signal handlers
-
-- 0.1.6
-    - maintenace version with CI test dependencies changes:
-        - removed Python 3.6
-        - removed Django 2.2
-        - added Python 3.10
-        - added Django 4.0
-        - move dev environment to Python 3.10 and Django 3.2
-
-      Note that Django 2.2 will keep working until real incompatible code changes occur.
-      This may happen by any later release, thus treat 0.1.6 as last compatible version.
-
-- 0.1.5
-    - fix error on model instance cloning
-- 0.1.4
-    - Django 3.2 support
-- 0.1.3
-    - better multi table inheritance support and test cases
-    - explicit docs for multi table inheritance
-- 0.1.2
-    - bugfix: o2o reverse name access
-    - add docs about model inheritance support
-- 0.1.1
-    - bugfix: add missing migration
-- 0.1.0
-    - fix recursion on empty queryset
-    - dependency expansion on M2M fields
-    - `m2m_changed` handler with filtering on m2m fields
-    - remove custom metaclass, introducing *Resolver* class
-    - new decorator `@precomputed` for custom save methods
-    - old *depends* syntax removed
-    - docs update
-- 0.0.23:
-    - Bugfix: Fixing leaking computed fields in model inheritance.
-- 0.0.22:
-    - Automatic dependency expansion on reverse relations.
-    - Example documentation.
-- 0.0.21:
-    - Bugfix: Fixing undefined _batchsize for pickled map usage.
-- 0.0.20
-    - Use `bulk_update` for computed field updates.
-    - Allow custom update optimizations with *select_related* and *prefetch_related*.
-    - Respect computed field MRO in `compute`.
-    - Allow updates on local computed fields from `update_dependent` simplifying bulk actions on `ComputedFieldsModel`.
-- 0.0.19
-    - Better graph expansion on relation paths with support for *update_fields*.
-- 0.0.18
-    - New *depends* syntax deprecating the old one.
-    - MRO of local computed field methods implemented.
-- 0.0.17
-    - Dropped Python 2.7 and Django 1.11 support.
-
-
```

### Comparing `django-computedfields-0.2.1/django_computedfields.egg-info/SOURCES.txt` & `django-computedfields-0.2.2/django_computedfields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/Makefile` & `django-computedfields-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/conf.py` & `django-computedfields-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/examples.rst` & `django-computedfields-0.2.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/index.rst` & `django-computedfields-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/make.bat` & `django-computedfields-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/manual.rst` & `django-computedfields-0.2.2/docs/manual.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/docs/reference.rst` & `django-computedfields-0.2.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.1/setup.py` & `django-computedfields-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
+
 def get_version(path):
     with open(path) as f:
         for line in f:
             if line.startswith('__version__'):
                 delim = '"' if '"' in line else "'"
                 return line.split(delim)[1]
         raise RuntimeError('Unable to find version string.')
 
+
 setup(
     name='django-computedfields',
     packages=find_packages(exclude=['example']),
     include_package_data=True,
     install_requires=[
-        'Django>=2.2,<4.2',
-        'typing_extensions>=4.0.1',
+        'Django>=2.2,<5.0',
+        'typing_extensions>=4.1',
         'django-fast-update'
     ],
     version=get_version('computedfields/__init__.py'),
     license='MIT',
     description='autoupdated database fields for model methods',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='netzkolchose',
     author_email='j.breitbart@netzkolchose.de',
     url='https://github.com/netzkolchose/django-computedfields',
-    download_url='https://github.com/netzkolchose/django-computedfields/archive/0.2.1.tar.gz',
-    keywords=['django', 'method', 'decorator', 'autoupdate', 'persistent', 'field'],
+    download_url='https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz',
+    keywords=['django', 'method', 'decorator',
+              'autoupdate', 'persistent', 'field'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Database',
         'Topic :: Database :: Front-Ends',
         'Topic :: Software Development :: Libraries',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
```

