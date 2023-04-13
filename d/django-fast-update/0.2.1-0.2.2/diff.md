# Comparing `tmp/django-fast-update-0.2.1.tar.gz` & `tmp/django-fast-update-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-fast-update-0.2.1.tar", last modified: Wed Aug  3 13:53:03 2022, max compression
+gzip compressed data, was "dist/django-fast-update-0.2.2.tar", last modified: Thu Apr 13 13:57:55 2023, max compression
```

## Comparing `django-fast-update-0.2.1.tar` & `django-fast-update-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 13:53:03.000000 django-fast-update-0.2.1/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1690 2022-08-03 13:49:36.000000 django-fast-update-0.2.1/setup.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2022-08-03 13:53:03.000000 django-fast-update-0.2.1/setup.cfg
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      120 2022-04-03 19:37:07.000000 django-fast-update-0.2.1/MANIFEST.in
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 13:53:03.000000 django-fast-update-0.2.1/fast_update/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    32883 2022-04-11 14:35:12.000000 django-fast-update-0.2.1/fast_update/copy.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2022-08-03 13:50:03.000000 django-fast-update-0.2.1/fast_update/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5369 2022-04-30 18:22:51.000000 django-fast-update-0.2.1/fast_update/query.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    13548 2022-04-30 18:22:51.000000 django-fast-update-0.2.1/fast_update/fast.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1024 2022-04-03 19:35:58.000000 django-fast-update-0.2.1/LICENSE.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5720 2022-08-03 13:53:03.000000 django-fast-update-0.2.1/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     3919 2022-04-30 19:00:58.000000 django-fast-update-0.2.1/README.md
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2022-08-03 13:53:03.000000 django-fast-update-0.2.1/django_fast_update.egg-info/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2022-08-03 13:53:02.000000 django-fast-update-0.2.1/django_fast_update.egg-info/dependency_links.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      346 2022-08-03 13:53:02.000000 django-fast-update-0.2.1/django_fast_update.egg-info/SOURCES.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5720 2022-08-03 13:53:02.000000 django-fast-update-0.2.1/django_fast_update.egg-info/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       17 2022-08-03 13:53:02.000000 django-fast-update-0.2.1/django_fast_update.egg-info/requires.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       12 2022-08-03 13:53:02.000000 django-fast-update-0.2.1/django_fast_update.egg-info/top_level.txt
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1741 2023-04-13 12:40:03.000000 django-fast-update-0.2.2/setup.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/setup.cfg
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      120 2022-04-03 19:37:07.000000 django-fast-update-0.2.2/MANIFEST.in
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/fast_update/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    33274 2023-04-13 12:36:18.000000 django-fast-update-0.2.2/fast_update/copy.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-04-13 12:40:13.000000 django-fast-update-0.2.2/fast_update/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5411 2023-04-13 13:06:11.000000 django-fast-update-0.2.2/fast_update/query.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    13548 2022-04-30 18:22:51.000000 django-fast-update-0.2.2/fast_update/fast.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1024 2022-04-03 19:35:58.000000 django-fast-update-0.2.2/LICENSE.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     4141 2023-04-13 13:36:58.000000 django-fast-update-0.2.2/README.md
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      346 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     6017 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       18 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/requires.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       12 2023-04-13 13:57:55.000000 django-fast-update-0.2.2/django_fast_update.egg-info/top_level.txt
```

### Comparing `django-fast-update-0.2.1/setup.py` & `django-fast-update-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,35 @@
                 return line.split(delim)[1]
         raise RuntimeError('Unable to find version string.')
 
 setup(
     name='django-fast-update',
     packages=find_packages(exclude=['example']),
     include_package_data=True,
-    install_requires=['Django>=3.2,<4.2'],
+    install_requires=['Django>=3.2,<=4.2'],
     version=get_version('fast_update/__init__.py'),
     license='MIT',
     description='Faster db updates for Django using UPDATE FROM VALUES sql variants.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='netzkolchose',
     author_email='j.breitbart@netzkolchose.de',
     url='https://github.com/netzkolchose/django-fast-update',
-    download_url='https://github.com/netzkolchose/django-fast-update/archive/v0.2.1.tar.gz',
+    download_url='https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz',
     keywords=['django', 'bulk_update', 'fast', 'update', 'fast_update'],
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
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
 )
```

### Comparing `django-fast-update-0.2.1/fast_update/copy.py` & `django-fast-update-0.2.2/fast_update/copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,15 +902,22 @@
     rows_updated = 0
     with transaction.atomic(using=conn.alias, savepoint=False), conn.cursor() as c:
         temp = f'temp_cu_{model._meta.db_table}'
         c.execute(f'DROP TABLE IF EXISTS "{temp}"')
         c.execute(f'CREATE TEMPORARY TABLE "{temp}" ({create_columns(column_def)})')
         copy_from(c, temp, objs, attnames, colnames, get, encs,
             encoding or CONNECTION_ENCODINGS[c.connection.encoding])
-        c.execute(f'ANALYZE "{temp}" ({pk_field.column})')
+        # optimization (~6x speedup in ./manage.py perf for 10 instances):
+        # for small changesets ANALYZE is much more expensive than
+        # a sequential scan of the temp table
+        # tipping point is 150+-80 records (higher for less fields)
+        # --> enable ANALYZE for >100 only (assuming rather big records
+        #     for copy_update)
+        if len(objs) > 100:
+            c.execute(f'ANALYZE "{temp}" ({pk_field.column})')
         c.execute(update_sql(model._meta.db_table, temp, pk_field.column, fields))
         rows_updated = c.rowcount
         c.execute(f'DROP TABLE "{temp}"')
 
         # handle remaining non local fields (done by bulk_update for now)
         if non_local_fieldnames:
             _rows_updated = qs.bulk_update(objs, non_local_fieldnames)
```

### Comparing `django-fast-update-0.2.1/fast_update/query.py` & `django-fast-update-0.2.2/fast_update/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         Returns the number of affected rows.
 
         NOTE: The underlying implementation is only a PoC and probably will be replaced
         soon by the much safer and superior COPY support of psycopg3.
         """
         self._for_write = True
         connection = connections[self.db]
-        if connection.vendor != 'postgresql':
+        if connection.vendor != 'postgresql' or connection.Database.__version__ > '3':
             raise NotSupportedError(
-                f'copy_update() is not supported on "{connection.vendor}" backend')
+                f'copy_update() only supported on "postgres" backend with psycopg2')
         from .copy import copy_update   # TODO: better in conditional import?
         if not objs:
             return 0
         objs = tuple(objs)
         fields_ = set(fields or [])
         sanity_check(self.model, objs, fields_, 'copy_update()')
         return copy_update(self, objs, fields_, field_encoders, encoding)
```

### Comparing `django-fast-update-0.2.1/fast_update/fast.py` & `django-fast-update-0.2.2/fast_update/fast.py`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.1/LICENSE.txt` & `django-fast-update-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-fast-update-0.2.1/PKG-INFO` & `django-fast-update-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-fast-update
-Version: 0.2.1
+Version: 0.2.2
 Summary: Faster db updates for Django using UPDATE FROM VALUES sql variants.
 Home-page: https://github.com/netzkolchose/django-fast-update
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.1.tar.gz
+Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz
 Description: [![test](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml/badge.svg?branch=master)](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-fast-update/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-fast-update?branch=master)
         
         
         ## django-fast-update ##
         
         Faster db updates using `UPDATE FROM VALUES` sql variants.
@@ -73,20 +73,23 @@
         `copy_update` follows the same interface idea as `bulk_update` and `fast_update`, minus a `batch_size`
         argument (data is always transferred in one big batch). It can be used likewise from the `FastUpdateManager`.
         `copy_update` also has no support for f-expressions, also duplicates will raise.
         
         **Note** `copy_update` will probably never leave the alpha/PoC-state, as psycopg3 brings great COPY support,
         which does a more secure value conversion and has a very fast C-version.
         
+        **Note** Django 4.2 brings psycopg3 support, which is currently not yet supported by `copy_update`.
+        While psycopg2 will keep working as before, psycopg3 will raise on attempts to use `copy_update` until #16 got resolved.
+        
         
         ### Status ###
         
         Currently beta, still some TODOs left.
         
-        The whole package is tested with Django 3.2 & 4.0 on Python 3.8 & 3.10.
+        The whole package is tested with Django 3.2 & 4.2 on Python 3.8 & 3.11.
         
         
         ### Performance ###
         
         There is a management command in the example app testing performance of updates on the `FieldUpdate`
         model (`./manage.py perf`).
         
@@ -105,14 +108,15 @@
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `django-fast-update-0.2.1/README.md` & `django-fast-update-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,20 +64,23 @@
 `copy_update` follows the same interface idea as `bulk_update` and `fast_update`, minus a `batch_size`
 argument (data is always transferred in one big batch). It can be used likewise from the `FastUpdateManager`.
 `copy_update` also has no support for f-expressions, also duplicates will raise.
 
 **Note** `copy_update` will probably never leave the alpha/PoC-state, as psycopg3 brings great COPY support,
 which does a more secure value conversion and has a very fast C-version.
 
+**Note** Django 4.2 brings psycopg3 support, which is currently not yet supported by `copy_update`.
+While psycopg2 will keep working as before, psycopg3 will raise on attempts to use `copy_update` until #16 got resolved.
+
 
 ### Status ###
 
 Currently beta, still some TODOs left.
 
-The whole package is tested with Django 3.2 & 4.0 on Python 3.8 & 3.10.
+The whole package is tested with Django 3.2 & 4.2 on Python 3.8 & 3.11.
 
 
 ### Performance ###
 
 There is a management command in the example app testing performance of updates on the `FieldUpdate`
 model (`./manage.py perf`).
```

### Comparing `django-fast-update-0.2.1/django_fast_update.egg-info/PKG-INFO` & `django-fast-update-0.2.2/django_fast_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-fast-update
-Version: 0.2.1
+Version: 0.2.2
 Summary: Faster db updates for Django using UPDATE FROM VALUES sql variants.
 Home-page: https://github.com/netzkolchose/django-fast-update
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.1.tar.gz
+Download-URL: https://github.com/netzkolchose/django-fast-update/archive/v0.2.2.tar.gz
 Description: [![test](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml/badge.svg?branch=master)](https://github.com/netzkolchose/django-fast-update/actions/workflows/django.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-fast-update/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-fast-update?branch=master)
         
         
         ## django-fast-update ##
         
         Faster db updates using `UPDATE FROM VALUES` sql variants.
@@ -73,20 +73,23 @@
         `copy_update` follows the same interface idea as `bulk_update` and `fast_update`, minus a `batch_size`
         argument (data is always transferred in one big batch). It can be used likewise from the `FastUpdateManager`.
         `copy_update` also has no support for f-expressions, also duplicates will raise.
         
         **Note** `copy_update` will probably never leave the alpha/PoC-state, as psycopg3 brings great COPY support,
         which does a more secure value conversion and has a very fast C-version.
         
+        **Note** Django 4.2 brings psycopg3 support, which is currently not yet supported by `copy_update`.
+        While psycopg2 will keep working as before, psycopg3 will raise on attempts to use `copy_update` until #16 got resolved.
+        
         
         ### Status ###
         
         Currently beta, still some TODOs left.
         
-        The whole package is tested with Django 3.2 & 4.0 on Python 3.8 & 3.10.
+        The whole package is tested with Django 3.2 & 4.2 on Python 3.8 & 3.11.
         
         
         ### Performance ###
         
         There is a management command in the example app testing performance of updates on the `FieldUpdate`
         model (`./manage.py perf`).
         
@@ -105,14 +108,15 @@
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

