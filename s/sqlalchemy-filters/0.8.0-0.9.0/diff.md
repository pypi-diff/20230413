# Comparing `tmp/sqlalchemy-filters-0.8.0.tar.gz` & `tmp/sqlalchemy-filters-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlalchemy-filters-0.8.0.tar", last modified: Mon Jun 25 07:36:43 2018, max compression
+gzip compressed data, was "dist/sqlalchemy-filters-0.9.0.tar", last modified: Thu Mar  7 12:11:33 2019, max compression
```

## Comparing `sqlalchemy-filters-0.8.0.tar` & `sqlalchemy-filters-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/
--rw-r--r--   0 travis    (2000) travis    (2000)      220 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      314 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/exceptions.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7130 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/filters.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2707 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/loads.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3717 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/models.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2529 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/pagination.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2827 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters/sorting.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    14130 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      479 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      150 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       19 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)    10532 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1547 2018-06-25 07:36:22.000000 sqlalchemy-filters-0.8.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)    14130 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-06-25 07:36:43.000000 sqlalchemy-filters-0.8.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1778 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/CHANGELOG.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      550 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      106 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16195 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11860 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      314 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7406 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/loads.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3717 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/pagination.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2827 2019-03-07 12:10:49.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters/sorting.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16195 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-07 12:11:33.000000 sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/zip-safe
```

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters/filters.py` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # -*- coding: utf-8 -*-
 from collections import Iterable, namedtuple
-from inspect import signature
+try:
+    from inspect import signature
+except ImportError:  # pragma: no cover
+    # For python2 capability. NOTE: This is in not handled in install_requires
+    # but rather in extras_require. You can install with
+    # 'pip install sqlalchemy-filters[python2]'
+    from funcsigs import signature
 from itertools import chain
 
 from six import string_types
 from sqlalchemy import and_, or_, not_
 
 from .exceptions import BadFilterFormat
 from .models import Field, auto_join, get_model_from_spec, get_default_model
@@ -100,15 +106,15 @@
         if arity == 1:
             return function(sqlalchemy_field)
 
         if arity == 2:
             return function(sqlalchemy_field, value)
 
 
-class BooleanFilter:
+class BooleanFilter(object):
 
     def __init__(self, function, *filters):
         self.function = function
         self.filters = filters
 
     def get_named_models(self):
         models = set()
```

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters/loads.py` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters/loads.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters/models.py` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters/pagination.py` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters/pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,8 @@
     return query
 
 
 def _calculate_num_pages(page_number, page_size, total_results):
     if page_size == 0:
         return 0
 
-    return math.ceil(total_results / page_size)
+    return math.ceil(float(total_results) / float(page_size))
```

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters/sorting.py` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters/sorting.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-filters-0.8.0/sqlalchemy_filters.egg-info/PKG-INFO` & `sqlalchemy-filters-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-filters
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library to filter SQLAlchemy queries.
-Home-page: https://github.com/Overseas-Student-Living/sqlalchemy-filters
+Home-page: https://github.com/juliotrigo/sqlalchemy-filters
 Author: Student.com
 Author-email: wearehiring@student.com
 License: Apache License, Version 2.0
 Description: SQLAlchemy-filters
         ==================
         
         .. pull-quote::
         
             Filter, sort and paginate SQLAlchemy query objects.
             Ideal for exposing these actions over a REST API.
         
+        
+        .. image:: https://img.shields.io/pypi/v/sqlalchemy-filters.svg
+            :target: https://pypi.org/project/sqlalchemy-filters/
+        
+        .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-filters.svg
+            :target: https://pypi.org/project/sqlalchemy-filters/
+        
+        .. image:: https://travis-ci.org/juliotrigo/sqlalchemy-filters.svg?branch=master
+            :target: https://travis-ci.org/juliotrigo/sqlalchemy-filters
+        
+        
         Filtering
         ---------
         
-        Assuming that we have a SQLAlchemy `query` object:
+        Assuming that we have a SQLAlchemy ``query`` object:
         
         .. code-block:: python
         
             from sqlalchemy import Column, Integer, String
             from sqlalchemy.ext.declarative import declarative_base
         
         
@@ -54,15 +65,16 @@
             filtered_query = apply_filters(query, filter_spec)
         
             more_filters = [{'field': 'foo_id', 'op': 'is_not_null'}]
             filtered_query = apply_filters(filtered_query, more_filters)
         
             result = filtered_query.all()
         
-        It is also possible to filter queries that contain multiple models, including joins:
+        It is also possible to filter queries that contain multiple models,
+        including joins:
         
         .. code-block:: python
         
             class Bar(Base):
         
                 __tablename__ = 'bar'
                 foo_id = Column(Integer, ForeignKey('foo.id'))
@@ -77,15 +89,18 @@
                 {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
             ]
             filtered_query = apply_filters(query, filter_spec)
         
             result = filtered_query.all()
         
         
-        `apply_filters` will attempt to automatically join models to `query` if they're not already present and a model-specific filter is supplied. For example, the value of `filtered_query` in the following two code blocks is identical:
+        ``apply_filters`` will attempt to automatically join models to ``query``
+        if they're not already present and a model-specific filter is supplied.
+        For example, the value of ``filtered_query`` in the following two code
+        blocks is identical:
         
         .. code-block:: python
         
             query = session.query(Foo).join(Bar)  # join pre-applied to query
         
             filter_spec = [
                 {'model': 'Foo', field': 'name', 'op': '==', 'value': 'name_1'},
@@ -99,81 +114,102 @@
         
             filter_spec = [
                 {field': 'name', 'op': '==', 'value': 'name_1'},
                 {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
             ]
             filtered_query = apply_filters(query, filter_spec)
         
-        The automatic join is only possible if sqlalchemy can implictly determine the condition for the join, for example because of a foreign key relationship.
-        
-        Automatic joins allow flexibility for clients to filter and sort by related objects without specifying all possible joins on the server beforehand.
-        
-        Note that first filter of the second block does not specify a model. It is implictly applied to the `Foo` model because that is the only model in the original query passed to `apply_filters`.
+        The automatic join is only possible if sqlalchemy can implictly
+        determine the condition for the join, for example because of a foreign
+        key relationship.
+        
+        Automatic joins allow flexibility for clients to filter and sort by
+        related objects without specifying all possible joins on the server
+        beforehand.
+        
+        Note that first filter of the second block does not specify a model.
+        It is implictly applied to the ``Foo`` model because that is the only
+        model in the original query passed to ``apply_filters``.
         
-        It is also possible to apply filters to queries defined by fields or functions:
+        It is also possible to apply filters to queries defined by fields or
+        functions:
         
         .. code-block:: python
         
             query_alt_1 = session.query(Foo.id, Foo.name)
             query_alt_2 = session.query(func.count(Foo.id))
         
         
         Restricted Loads
         ----------------
         
-        You can restrict the fields that SQLAlchemy loads from the database by using
-        the `apply_loads` function:
+        You can restrict the fields that SQLAlchemy loads from the database by
+        using the ``apply_loads`` function:
         
         .. code-block:: python
         
             query = session.query(Foo, Bar).join(Bar)
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']},
                 {'model': 'Bar', 'fields': ['count']}
             ]
             query = apply_loads(query, load_spec)  # will load only Foo.name and Bar.count
         
         
-        The effect of the `apply_loads` function is to _defer_ the load of any other fields to when/if they're accessed, rather than loading them when the query is executed. It only applies to fields that would be loaded during normal query execution.
+        The effect of the ``apply_loads`` function is to ``_defer_`` the load
+        of any other fields to when/if they're accessed, rather than loading
+        them when the query is executed. It only applies to fields that would be
+        loaded during normal query execution.
         
         
         Effect on joined queries
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
-        The default SQLAlchemy join is lazy, meaning that columns from the joined table are loaded only when required. Therefore `apply_loads` has limited effect in the following scenario:
+        The default SQLAlchemy join is lazy, meaning that columns from the
+        joined table are loaded only when required. Therefore ``apply_loads``
+        has limited effect in the following scenario:
         
         .. code-block:: python
         
             query = session.query(Foo).join(Bar)
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
                 {'model': 'Bar', 'fields': ['count']}  # ignored
             ]
             query = apply_loads(query, load_spec)  # will load only Foo.name
         
         
-        `apply_loads` cannot be applied to columns that are loaded as `joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_. This is because a joined eager load does not add the joined model to the original query, as explained `here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
+        ``apply_loads`` cannot be applied to columns that are loaded as
+        `joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_.
+        This is because a joined eager load does not add the joined model to the
+        original query, as explained
+        `here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
         
-        The following would not prevent all columns from Bar being eagerly loaded:
+        The following would not prevent all columns from ``Bar`` being eagerly
+        loaded:
         
         .. code-block:: python
         
             query = session.query(Foo).options(joinedload(Foo.bar))
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
                 {'model': 'Bar', 'fields': ['count']}
             ]
             query = apply_loads(query, load_spec)
         
         .. sidebar:: Automatic Join
         
-            In fact, what happens here is that `Bar` is automatically joined to `query`, because it is determined that `Bar` is not part of the original query. The `load_spec` therefore has no effect because the automatic join
-            results in lazy evaluation.
-        
-        If you wish to perform a joined load with restricted columns, you must specify the columns as part of the joined load, rather than with `apply_loads`:
+            In fact, what happens here is that ``Bar`` is automatically joined
+            to ``query``, because it is determined that ``Bar`` is not part of
+            the original query. The ``load_spec`` therefore has no effect
+            because the automatic join results in lazy evaluation.
+        
+        If you wish to perform a joined load with restricted columns, you must
+        specify the columns as part of the joined load, rather than with
+        ``apply_loads``:
         
         .. code-block:: python
         
             query = session.query(Foo).options(joinedload(Bar).load_only('count'))
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
             ]
@@ -194,17 +230,20 @@
                 {'model': 'Bar', field': 'id', 'direction': 'desc'},
             ]
             sorted_query = apply_sort(query, sort_spec)
         
             result = sorted_query.all()
         
         
-        `apply_sort` will attempt to automatically join models to `query` if they're not already present and a model-specific sort is supplied. The behaviour is the same as in `apply_filters`.
+        ``apply_sort`` will attempt to automatically join models to ``query`` if
+        they're not already present and a model-specific sort is supplied.
+        The behaviour is the same as in ``apply_filters``.
         
-        This allows flexibility for clients to sort by fields on related objects without specifying all possible joins on the server beforehand.
+        This allows flexibility for clients to sort by fields on related objects
+        without specifying all possible joins on the server beforehand.
         
         
         Pagination
         ----------
         
         .. code-block:: python
         
@@ -233,24 +272,25 @@
         
             filter_spec = [
                 {'model': 'model_name', 'field': 'field_name', 'op': '==', 'value': 'field_value'},
                 {'model': 'model_name', 'field': 'field_2_name', 'op': '!=', 'value': 'field_2_value'},
                 # ...
             ]
         
-        The `model` key is optional if the original query being filtered only applies to one model.
+        The ``model`` key is optional if the original query being filtered only
+        applies to one model.
         
         If there is only one filter, the containing list may be omitted:
         
         .. code-block:: python
         
             filter_spec = {'field': 'field_name', 'op': '==', 'value': 'field_value'}
         
         Where ``field`` is the name of the field that will be filtered using the
-        operator provided in ``op`` (optional, defaults to `==`) and the
+        operator provided in ``op`` (optional, defaults to ``==``) and the
         provided ``value`` (optional, depending on the operator).
         
         This is the list of operators that can be used:
         
         - ``is_null``
         - ``is_not_null``
         - ``==``, ``eq``
@@ -261,16 +301,17 @@
         - ``<=``, ``le``
         - ``like``
         - ``ilike``
         - ``in``
         - ``not_in``
         
         Boolean Functions
-        *****************
-        ``and``, ``or``, and ``not`` functions can be used and nested within the filter specification:
+        ^^^^^^^^^^^^^^^^^
+        ``and``, ``or``, and ``not`` functions can be used and nested within the
+        filter specification:
         
         .. code-block:: python
         
             filter_spec = [
                 {
                     'or': [
                         {
@@ -285,15 +326,16 @@
                             ]
                         },
                     ],
                 }
             ]
         
         
-        Note: ``or`` and ``and`` must reference a list of at least one element. ``not`` must reference a list of exactly one element.
+        Note: ``or`` and ``and`` must reference a list of at least one element.
+        ``not`` must reference a list of exactly one element.
         
         Sort format
         -----------
         
         Sort elements must be provided as dictionaries in a list and will be
         applied sequentially:
         
@@ -304,33 +346,52 @@
                 {'model': 'Bar', 'field': 'id', 'direction': 'desc'},
                 # ...
             ]
         
         Where ``field`` is the name of the field that will be sorted using the
         provided ``direction``.
         
-        The `model` key is optional if the original query being sorted only applies to one model.
+        The ``model`` key is optional if the original query being sorted only
+        applies to one model.
         
         
         Running tests
         -------------
         
-        There are some Makefile targets that can be used to run the tests. A
-        test database will be created, used during the tests and destroyed
-        afterwards.
-        
-        The default configuration uses both SQLite and MySQL (if the driver is
-        installed) to run the tests, with the following URIs:
+        The default configuration uses **SQLite**, **MySQL** (if the driver is
+        installed, which is the case when ``tox`` is used) and **PostgreSQL**
+        (if the driver is installed, which is the case when ``tox`` is used) to
+        run the tests, with the following URIs:
         
         .. code-block:: shell
         
             sqlite+pysqlite:///test_sqlalchemy_filters.db
             mysql+mysqlconnector://root:@localhost:3306/test_sqlalchemy_filters
+            postgresql+psycopg2://postgres:@localhost:5432/test_sqlalchemy_filters?client_encoding=utf8'
+        
+        A test database will be created, used during the tests and destroyed
+        afterwards for each RDBMS configured.
+        
+        There are Makefile targets to run docker containers locally for both
+        **MySQL** and **PostgreSQL**, using the default ports and configuration:
+        
+        .. code-block:: shell
+        
+            $ make docker-mysql-run
+            $ make docker-postgres-run
         
-        Example of usage:
+        To run the tests locally:
+        
+        .. code-block:: shell
+        
+            $ # Create/activate a virtual environment
+            $ pip install tox
+            $ tox
+        
+        There are some other Makefile targets that can be used to run the tests:
         
         .. code-block:: shell
         
             $ # using default settings
             $ make test
             $ make coverage
         
@@ -338,26 +399,47 @@
             $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make test
             $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make test
         
             $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make coverage
             $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make coverage
         
         
+        
+        Database management systems
+        ---------------------------
+        
+        The following RDBMS are supported (tested):
+        
+        - SQLite
+        - MySQL
+        - PostgreSQL
+        
+        
+        Python 2
+        --------
+        
+        There is no active support for python 2, however it is compatible as of
+        February 2019, if you install ``funcsigs``.
+        
+        
         License
         -------
         
         Apache 2.0. See LICENSE for details.
         
 Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Internet
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
 Provides-Extra: dev
+Provides-Extra: python2
 Provides-Extra: mysql
+Provides-Extra: postgresql
```

### Comparing `sqlalchemy-filters-0.8.0/README.rst` & `sqlalchemy-filters-0.9.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,29 @@
 ==================
 
 .. pull-quote::
 
     Filter, sort and paginate SQLAlchemy query objects.
     Ideal for exposing these actions over a REST API.
 
+
+.. image:: https://img.shields.io/pypi/v/sqlalchemy-filters.svg
+    :target: https://pypi.org/project/sqlalchemy-filters/
+
+.. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-filters.svg
+    :target: https://pypi.org/project/sqlalchemy-filters/
+
+.. image:: https://travis-ci.org/juliotrigo/sqlalchemy-filters.svg?branch=master
+    :target: https://travis-ci.org/juliotrigo/sqlalchemy-filters
+
+
 Filtering
 ---------
 
-Assuming that we have a SQLAlchemy `query` object:
+Assuming that we have a SQLAlchemy ``query`` object:
 
 .. code-block:: python
 
     from sqlalchemy import Column, Integer, String
     from sqlalchemy.ext.declarative import declarative_base
 
 
@@ -46,15 +57,16 @@
     filtered_query = apply_filters(query, filter_spec)
 
     more_filters = [{'field': 'foo_id', 'op': 'is_not_null'}]
     filtered_query = apply_filters(filtered_query, more_filters)
 
     result = filtered_query.all()
 
-It is also possible to filter queries that contain multiple models, including joins:
+It is also possible to filter queries that contain multiple models,
+including joins:
 
 .. code-block:: python
 
     class Bar(Base):
 
         __tablename__ = 'bar'
         foo_id = Column(Integer, ForeignKey('foo.id'))
@@ -69,15 +81,18 @@
         {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
     ]
     filtered_query = apply_filters(query, filter_spec)
 
     result = filtered_query.all()
 
 
-`apply_filters` will attempt to automatically join models to `query` if they're not already present and a model-specific filter is supplied. For example, the value of `filtered_query` in the following two code blocks is identical:
+``apply_filters`` will attempt to automatically join models to ``query``
+if they're not already present and a model-specific filter is supplied.
+For example, the value of ``filtered_query`` in the following two code
+blocks is identical:
 
 .. code-block:: python
 
     query = session.query(Foo).join(Bar)  # join pre-applied to query
 
     filter_spec = [
         {'model': 'Foo', field': 'name', 'op': '==', 'value': 'name_1'},
@@ -91,81 +106,102 @@
 
     filter_spec = [
         {field': 'name', 'op': '==', 'value': 'name_1'},
         {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
     ]
     filtered_query = apply_filters(query, filter_spec)
 
-The automatic join is only possible if sqlalchemy can implictly determine the condition for the join, for example because of a foreign key relationship.
-
-Automatic joins allow flexibility for clients to filter and sort by related objects without specifying all possible joins on the server beforehand.
-
-Note that first filter of the second block does not specify a model. It is implictly applied to the `Foo` model because that is the only model in the original query passed to `apply_filters`.
+The automatic join is only possible if sqlalchemy can implictly
+determine the condition for the join, for example because of a foreign
+key relationship.
+
+Automatic joins allow flexibility for clients to filter and sort by
+related objects without specifying all possible joins on the server
+beforehand.
+
+Note that first filter of the second block does not specify a model.
+It is implictly applied to the ``Foo`` model because that is the only
+model in the original query passed to ``apply_filters``.
 
-It is also possible to apply filters to queries defined by fields or functions:
+It is also possible to apply filters to queries defined by fields or
+functions:
 
 .. code-block:: python
 
     query_alt_1 = session.query(Foo.id, Foo.name)
     query_alt_2 = session.query(func.count(Foo.id))
 
 
 Restricted Loads
 ----------------
 
-You can restrict the fields that SQLAlchemy loads from the database by using
-the `apply_loads` function:
+You can restrict the fields that SQLAlchemy loads from the database by
+using the ``apply_loads`` function:
 
 .. code-block:: python
 
     query = session.query(Foo, Bar).join(Bar)
     load_spec = [
         {'model': 'Foo', 'fields': ['name']},
         {'model': 'Bar', 'fields': ['count']}
     ]
     query = apply_loads(query, load_spec)  # will load only Foo.name and Bar.count
 
 
-The effect of the `apply_loads` function is to _defer_ the load of any other fields to when/if they're accessed, rather than loading them when the query is executed. It only applies to fields that would be loaded during normal query execution.
+The effect of the ``apply_loads`` function is to ``_defer_`` the load
+of any other fields to when/if they're accessed, rather than loading
+them when the query is executed. It only applies to fields that would be
+loaded during normal query execution.
 
 
 Effect on joined queries
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
-The default SQLAlchemy join is lazy, meaning that columns from the joined table are loaded only when required. Therefore `apply_loads` has limited effect in the following scenario:
+The default SQLAlchemy join is lazy, meaning that columns from the
+joined table are loaded only when required. Therefore ``apply_loads``
+has limited effect in the following scenario:
 
 .. code-block:: python
 
     query = session.query(Foo).join(Bar)
     load_spec = [
         {'model': 'Foo', 'fields': ['name']}
         {'model': 'Bar', 'fields': ['count']}  # ignored
     ]
     query = apply_loads(query, load_spec)  # will load only Foo.name
 
 
-`apply_loads` cannot be applied to columns that are loaded as `joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_. This is because a joined eager load does not add the joined model to the original query, as explained `here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
+``apply_loads`` cannot be applied to columns that are loaded as
+`joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_.
+This is because a joined eager load does not add the joined model to the
+original query, as explained
+`here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
 
-The following would not prevent all columns from Bar being eagerly loaded:
+The following would not prevent all columns from ``Bar`` being eagerly
+loaded:
 
 .. code-block:: python
 
     query = session.query(Foo).options(joinedload(Foo.bar))
     load_spec = [
         {'model': 'Foo', 'fields': ['name']}
         {'model': 'Bar', 'fields': ['count']}
     ]
     query = apply_loads(query, load_spec)
 
 .. sidebar:: Automatic Join
 
-    In fact, what happens here is that `Bar` is automatically joined to `query`, because it is determined that `Bar` is not part of the original query. The `load_spec` therefore has no effect because the automatic join
-    results in lazy evaluation.
-
-If you wish to perform a joined load with restricted columns, you must specify the columns as part of the joined load, rather than with `apply_loads`:
+    In fact, what happens here is that ``Bar`` is automatically joined
+    to ``query``, because it is determined that ``Bar`` is not part of
+    the original query. The ``load_spec`` therefore has no effect
+    because the automatic join results in lazy evaluation.
+
+If you wish to perform a joined load with restricted columns, you must
+specify the columns as part of the joined load, rather than with
+``apply_loads``:
 
 .. code-block:: python
 
     query = session.query(Foo).options(joinedload(Bar).load_only('count'))
     load_spec = [
         {'model': 'Foo', 'fields': ['name']}
     ]
@@ -186,17 +222,20 @@
         {'model': 'Bar', field': 'id', 'direction': 'desc'},
     ]
     sorted_query = apply_sort(query, sort_spec)
 
     result = sorted_query.all()
 
 
-`apply_sort` will attempt to automatically join models to `query` if they're not already present and a model-specific sort is supplied. The behaviour is the same as in `apply_filters`.
+``apply_sort`` will attempt to automatically join models to ``query`` if
+they're not already present and a model-specific sort is supplied.
+The behaviour is the same as in ``apply_filters``.
 
-This allows flexibility for clients to sort by fields on related objects without specifying all possible joins on the server beforehand.
+This allows flexibility for clients to sort by fields on related objects
+without specifying all possible joins on the server beforehand.
 
 
 Pagination
 ----------
 
 .. code-block:: python
 
@@ -225,24 +264,25 @@
 
     filter_spec = [
         {'model': 'model_name', 'field': 'field_name', 'op': '==', 'value': 'field_value'},
         {'model': 'model_name', 'field': 'field_2_name', 'op': '!=', 'value': 'field_2_value'},
         # ...
     ]
 
-The `model` key is optional if the original query being filtered only applies to one model.
+The ``model`` key is optional if the original query being filtered only
+applies to one model.
 
 If there is only one filter, the containing list may be omitted:
 
 .. code-block:: python
 
     filter_spec = {'field': 'field_name', 'op': '==', 'value': 'field_value'}
 
 Where ``field`` is the name of the field that will be filtered using the
-operator provided in ``op`` (optional, defaults to `==`) and the
+operator provided in ``op`` (optional, defaults to ``==``) and the
 provided ``value`` (optional, depending on the operator).
 
 This is the list of operators that can be used:
 
 - ``is_null``
 - ``is_not_null``
 - ``==``, ``eq``
@@ -253,16 +293,17 @@
 - ``<=``, ``le``
 - ``like``
 - ``ilike``
 - ``in``
 - ``not_in``
 
 Boolean Functions
-*****************
-``and``, ``or``, and ``not`` functions can be used and nested within the filter specification:
+^^^^^^^^^^^^^^^^^
+``and``, ``or``, and ``not`` functions can be used and nested within the
+filter specification:
 
 .. code-block:: python
 
     filter_spec = [
         {
             'or': [
                 {
@@ -277,15 +318,16 @@
                     ]
                 },
             ],
         }
     ]
 
 
-Note: ``or`` and ``and`` must reference a list of at least one element. ``not`` must reference a list of exactly one element.
+Note: ``or`` and ``and`` must reference a list of at least one element.
+``not`` must reference a list of exactly one element.
 
 Sort format
 -----------
 
 Sort elements must be provided as dictionaries in a list and will be
 applied sequentially:
 
@@ -296,33 +338,52 @@
         {'model': 'Bar', 'field': 'id', 'direction': 'desc'},
         # ...
     ]
 
 Where ``field`` is the name of the field that will be sorted using the
 provided ``direction``.
 
-The `model` key is optional if the original query being sorted only applies to one model.
+The ``model`` key is optional if the original query being sorted only
+applies to one model.
 
 
 Running tests
 -------------
 
-There are some Makefile targets that can be used to run the tests. A
-test database will be created, used during the tests and destroyed
-afterwards.
-
-The default configuration uses both SQLite and MySQL (if the driver is
-installed) to run the tests, with the following URIs:
+The default configuration uses **SQLite**, **MySQL** (if the driver is
+installed, which is the case when ``tox`` is used) and **PostgreSQL**
+(if the driver is installed, which is the case when ``tox`` is used) to
+run the tests, with the following URIs:
 
 .. code-block:: shell
 
     sqlite+pysqlite:///test_sqlalchemy_filters.db
     mysql+mysqlconnector://root:@localhost:3306/test_sqlalchemy_filters
+    postgresql+psycopg2://postgres:@localhost:5432/test_sqlalchemy_filters?client_encoding=utf8'
+
+A test database will be created, used during the tests and destroyed
+afterwards for each RDBMS configured.
+
+There are Makefile targets to run docker containers locally for both
+**MySQL** and **PostgreSQL**, using the default ports and configuration:
+
+.. code-block:: shell
 
-Example of usage:
+    $ make docker-mysql-run
+    $ make docker-postgres-run
+
+To run the tests locally:
+
+.. code-block:: shell
+
+    $ # Create/activate a virtual environment
+    $ pip install tox
+    $ tox
+
+There are some other Makefile targets that can be used to run the tests:
 
 .. code-block:: shell
 
     $ # using default settings
     $ make test
     $ make coverage
 
@@ -330,11 +391,29 @@
     $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make test
     $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make test
 
     $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make coverage
     $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make coverage
 
 
+
+Database management systems
+---------------------------
+
+The following RDBMS are supported (tested):
+
+- SQLite
+- MySQL
+- PostgreSQL
+
+
+Python 2
+--------
+
+There is no active support for python 2, however it is compatible as of
+February 2019, if you install ``funcsigs``.
+
+
 License
 -------
 
 Apache 2.0. See LICENSE for details.
```

### Comparing `sqlalchemy-filters-0.8.0/setup.py` & `sqlalchemy-filters-0.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,45 +8,54 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'README.rst'), 'r', 'utf-8') as handle:
     readme = handle.read()
 
 setup(
     name='sqlalchemy-filters',
-    version='0.8.0',
+    version='0.9.0',
     description='A library to filter SQLAlchemy queries.',
     long_description=readme,
     author='Student.com',
     author_email='wearehiring@student.com',
-    url='https://github.com/Overseas-Student-Living/sqlalchemy-filters',
+    url='https://github.com/juliotrigo/sqlalchemy-filters',
     packages=find_packages(exclude=['test', 'test.*']),
     install_requires=[
         'sqlalchemy>=1.0.16',
         'six>=1.10.0',
     ],
     extras_require={
         'dev': [
-            'pytest==3.0.5',
-            'flake8==3.2.1',
-            'coverage==4.3.1',
-            'sqlalchemy-utils==0.32.12',
+            'pytest==4.3.0',
+            'flake8==3.7.7',
+            'coverage==4.5.2',
+            'sqlalchemy-utils==0.33.11',
+            'restructuredtext-lint==1.2.2',
+            'Pygments==2.3.1',
         ],
         'mysql': [
-            'mysql-connector-python-rf==2.1.3',
+            'mysql-connector-python-rf==2.2.2',
+        ],
+        'postgresql': [
+            'psycopg2==2.7.7'
+        ],
+        'python2': [
+            "funcsigs>=1.0.2"
         ]
     },
     zip_safe=True,
     license='Apache License, Version 2.0',
     classifiers=[
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Operating System :: POSIX",
-        "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
-        "Topic :: Internet",
+        "Programming Language :: Python :: 3.7",
+        "Topic :: Database",
+        "Topic :: Database :: Front-Ends",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Intended Audience :: Developers",
     ]
 )
```

### Comparing `sqlalchemy-filters-0.8.0/PKG-INFO` & `sqlalchemy-filters-0.9.0/sqlalchemy_filters.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-filters
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library to filter SQLAlchemy queries.
-Home-page: https://github.com/Overseas-Student-Living/sqlalchemy-filters
+Home-page: https://github.com/juliotrigo/sqlalchemy-filters
 Author: Student.com
 Author-email: wearehiring@student.com
 License: Apache License, Version 2.0
 Description: SQLAlchemy-filters
         ==================
         
         .. pull-quote::
         
             Filter, sort and paginate SQLAlchemy query objects.
             Ideal for exposing these actions over a REST API.
         
+        
+        .. image:: https://img.shields.io/pypi/v/sqlalchemy-filters.svg
+            :target: https://pypi.org/project/sqlalchemy-filters/
+        
+        .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-filters.svg
+            :target: https://pypi.org/project/sqlalchemy-filters/
+        
+        .. image:: https://travis-ci.org/juliotrigo/sqlalchemy-filters.svg?branch=master
+            :target: https://travis-ci.org/juliotrigo/sqlalchemy-filters
+        
+        
         Filtering
         ---------
         
-        Assuming that we have a SQLAlchemy `query` object:
+        Assuming that we have a SQLAlchemy ``query`` object:
         
         .. code-block:: python
         
             from sqlalchemy import Column, Integer, String
             from sqlalchemy.ext.declarative import declarative_base
         
         
@@ -54,15 +65,16 @@
             filtered_query = apply_filters(query, filter_spec)
         
             more_filters = [{'field': 'foo_id', 'op': 'is_not_null'}]
             filtered_query = apply_filters(filtered_query, more_filters)
         
             result = filtered_query.all()
         
-        It is also possible to filter queries that contain multiple models, including joins:
+        It is also possible to filter queries that contain multiple models,
+        including joins:
         
         .. code-block:: python
         
             class Bar(Base):
         
                 __tablename__ = 'bar'
                 foo_id = Column(Integer, ForeignKey('foo.id'))
@@ -77,15 +89,18 @@
                 {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
             ]
             filtered_query = apply_filters(query, filter_spec)
         
             result = filtered_query.all()
         
         
-        `apply_filters` will attempt to automatically join models to `query` if they're not already present and a model-specific filter is supplied. For example, the value of `filtered_query` in the following two code blocks is identical:
+        ``apply_filters`` will attempt to automatically join models to ``query``
+        if they're not already present and a model-specific filter is supplied.
+        For example, the value of ``filtered_query`` in the following two code
+        blocks is identical:
         
         .. code-block:: python
         
             query = session.query(Foo).join(Bar)  # join pre-applied to query
         
             filter_spec = [
                 {'model': 'Foo', field': 'name', 'op': '==', 'value': 'name_1'},
@@ -99,81 +114,102 @@
         
             filter_spec = [
                 {field': 'name', 'op': '==', 'value': 'name_1'},
                 {'model': 'Bar', field': 'count', 'op': '>=', 'value': 5},
             ]
             filtered_query = apply_filters(query, filter_spec)
         
-        The automatic join is only possible if sqlalchemy can implictly determine the condition for the join, for example because of a foreign key relationship.
-        
-        Automatic joins allow flexibility for clients to filter and sort by related objects without specifying all possible joins on the server beforehand.
-        
-        Note that first filter of the second block does not specify a model. It is implictly applied to the `Foo` model because that is the only model in the original query passed to `apply_filters`.
+        The automatic join is only possible if sqlalchemy can implictly
+        determine the condition for the join, for example because of a foreign
+        key relationship.
+        
+        Automatic joins allow flexibility for clients to filter and sort by
+        related objects without specifying all possible joins on the server
+        beforehand.
+        
+        Note that first filter of the second block does not specify a model.
+        It is implictly applied to the ``Foo`` model because that is the only
+        model in the original query passed to ``apply_filters``.
         
-        It is also possible to apply filters to queries defined by fields or functions:
+        It is also possible to apply filters to queries defined by fields or
+        functions:
         
         .. code-block:: python
         
             query_alt_1 = session.query(Foo.id, Foo.name)
             query_alt_2 = session.query(func.count(Foo.id))
         
         
         Restricted Loads
         ----------------
         
-        You can restrict the fields that SQLAlchemy loads from the database by using
-        the `apply_loads` function:
+        You can restrict the fields that SQLAlchemy loads from the database by
+        using the ``apply_loads`` function:
         
         .. code-block:: python
         
             query = session.query(Foo, Bar).join(Bar)
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']},
                 {'model': 'Bar', 'fields': ['count']}
             ]
             query = apply_loads(query, load_spec)  # will load only Foo.name and Bar.count
         
         
-        The effect of the `apply_loads` function is to _defer_ the load of any other fields to when/if they're accessed, rather than loading them when the query is executed. It only applies to fields that would be loaded during normal query execution.
+        The effect of the ``apply_loads`` function is to ``_defer_`` the load
+        of any other fields to when/if they're accessed, rather than loading
+        them when the query is executed. It only applies to fields that would be
+        loaded during normal query execution.
         
         
         Effect on joined queries
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
-        The default SQLAlchemy join is lazy, meaning that columns from the joined table are loaded only when required. Therefore `apply_loads` has limited effect in the following scenario:
+        The default SQLAlchemy join is lazy, meaning that columns from the
+        joined table are loaded only when required. Therefore ``apply_loads``
+        has limited effect in the following scenario:
         
         .. code-block:: python
         
             query = session.query(Foo).join(Bar)
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
                 {'model': 'Bar', 'fields': ['count']}  # ignored
             ]
             query = apply_loads(query, load_spec)  # will load only Foo.name
         
         
-        `apply_loads` cannot be applied to columns that are loaded as `joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_. This is because a joined eager load does not add the joined model to the original query, as explained `here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
+        ``apply_loads`` cannot be applied to columns that are loaded as
+        `joined eager loads <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#joined-eager-loading>`_.
+        This is because a joined eager load does not add the joined model to the
+        original query, as explained
+        `here <http://docs.sqlalchemy.org/en/latest/orm/loading_relationships.html#the-zen-of-joined-eager-loading>`_
         
-        The following would not prevent all columns from Bar being eagerly loaded:
+        The following would not prevent all columns from ``Bar`` being eagerly
+        loaded:
         
         .. code-block:: python
         
             query = session.query(Foo).options(joinedload(Foo.bar))
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
                 {'model': 'Bar', 'fields': ['count']}
             ]
             query = apply_loads(query, load_spec)
         
         .. sidebar:: Automatic Join
         
-            In fact, what happens here is that `Bar` is automatically joined to `query`, because it is determined that `Bar` is not part of the original query. The `load_spec` therefore has no effect because the automatic join
-            results in lazy evaluation.
-        
-        If you wish to perform a joined load with restricted columns, you must specify the columns as part of the joined load, rather than with `apply_loads`:
+            In fact, what happens here is that ``Bar`` is automatically joined
+            to ``query``, because it is determined that ``Bar`` is not part of
+            the original query. The ``load_spec`` therefore has no effect
+            because the automatic join results in lazy evaluation.
+        
+        If you wish to perform a joined load with restricted columns, you must
+        specify the columns as part of the joined load, rather than with
+        ``apply_loads``:
         
         .. code-block:: python
         
             query = session.query(Foo).options(joinedload(Bar).load_only('count'))
             load_spec = [
                 {'model': 'Foo', 'fields': ['name']}
             ]
@@ -194,17 +230,20 @@
                 {'model': 'Bar', field': 'id', 'direction': 'desc'},
             ]
             sorted_query = apply_sort(query, sort_spec)
         
             result = sorted_query.all()
         
         
-        `apply_sort` will attempt to automatically join models to `query` if they're not already present and a model-specific sort is supplied. The behaviour is the same as in `apply_filters`.
+        ``apply_sort`` will attempt to automatically join models to ``query`` if
+        they're not already present and a model-specific sort is supplied.
+        The behaviour is the same as in ``apply_filters``.
         
-        This allows flexibility for clients to sort by fields on related objects without specifying all possible joins on the server beforehand.
+        This allows flexibility for clients to sort by fields on related objects
+        without specifying all possible joins on the server beforehand.
         
         
         Pagination
         ----------
         
         .. code-block:: python
         
@@ -233,24 +272,25 @@
         
             filter_spec = [
                 {'model': 'model_name', 'field': 'field_name', 'op': '==', 'value': 'field_value'},
                 {'model': 'model_name', 'field': 'field_2_name', 'op': '!=', 'value': 'field_2_value'},
                 # ...
             ]
         
-        The `model` key is optional if the original query being filtered only applies to one model.
+        The ``model`` key is optional if the original query being filtered only
+        applies to one model.
         
         If there is only one filter, the containing list may be omitted:
         
         .. code-block:: python
         
             filter_spec = {'field': 'field_name', 'op': '==', 'value': 'field_value'}
         
         Where ``field`` is the name of the field that will be filtered using the
-        operator provided in ``op`` (optional, defaults to `==`) and the
+        operator provided in ``op`` (optional, defaults to ``==``) and the
         provided ``value`` (optional, depending on the operator).
         
         This is the list of operators that can be used:
         
         - ``is_null``
         - ``is_not_null``
         - ``==``, ``eq``
@@ -261,16 +301,17 @@
         - ``<=``, ``le``
         - ``like``
         - ``ilike``
         - ``in``
         - ``not_in``
         
         Boolean Functions
-        *****************
-        ``and``, ``or``, and ``not`` functions can be used and nested within the filter specification:
+        ^^^^^^^^^^^^^^^^^
+        ``and``, ``or``, and ``not`` functions can be used and nested within the
+        filter specification:
         
         .. code-block:: python
         
             filter_spec = [
                 {
                     'or': [
                         {
@@ -285,15 +326,16 @@
                             ]
                         },
                     ],
                 }
             ]
         
         
-        Note: ``or`` and ``and`` must reference a list of at least one element. ``not`` must reference a list of exactly one element.
+        Note: ``or`` and ``and`` must reference a list of at least one element.
+        ``not`` must reference a list of exactly one element.
         
         Sort format
         -----------
         
         Sort elements must be provided as dictionaries in a list and will be
         applied sequentially:
         
@@ -304,33 +346,52 @@
                 {'model': 'Bar', 'field': 'id', 'direction': 'desc'},
                 # ...
             ]
         
         Where ``field`` is the name of the field that will be sorted using the
         provided ``direction``.
         
-        The `model` key is optional if the original query being sorted only applies to one model.
+        The ``model`` key is optional if the original query being sorted only
+        applies to one model.
         
         
         Running tests
         -------------
         
-        There are some Makefile targets that can be used to run the tests. A
-        test database will be created, used during the tests and destroyed
-        afterwards.
-        
-        The default configuration uses both SQLite and MySQL (if the driver is
-        installed) to run the tests, with the following URIs:
+        The default configuration uses **SQLite**, **MySQL** (if the driver is
+        installed, which is the case when ``tox`` is used) and **PostgreSQL**
+        (if the driver is installed, which is the case when ``tox`` is used) to
+        run the tests, with the following URIs:
         
         .. code-block:: shell
         
             sqlite+pysqlite:///test_sqlalchemy_filters.db
             mysql+mysqlconnector://root:@localhost:3306/test_sqlalchemy_filters
+            postgresql+psycopg2://postgres:@localhost:5432/test_sqlalchemy_filters?client_encoding=utf8'
+        
+        A test database will be created, used during the tests and destroyed
+        afterwards for each RDBMS configured.
+        
+        There are Makefile targets to run docker containers locally for both
+        **MySQL** and **PostgreSQL**, using the default ports and configuration:
+        
+        .. code-block:: shell
+        
+            $ make docker-mysql-run
+            $ make docker-postgres-run
         
-        Example of usage:
+        To run the tests locally:
+        
+        .. code-block:: shell
+        
+            $ # Create/activate a virtual environment
+            $ pip install tox
+            $ tox
+        
+        There are some other Makefile targets that can be used to run the tests:
         
         .. code-block:: shell
         
             $ # using default settings
             $ make test
             $ make coverage
         
@@ -338,26 +399,47 @@
             $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make test
             $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make test
         
             $ ARGS='--mysql-test-db-uri mysql+mysqlconnector://root:@192.168.99.100:3340/test_sqlalchemy_filters' make coverage
             $ ARGS='--sqlite-test-db-uri sqlite+pysqlite:///test_sqlalchemy_filters.db' make coverage
         
         
+        
+        Database management systems
+        ---------------------------
+        
+        The following RDBMS are supported (tested):
+        
+        - SQLite
+        - MySQL
+        - PostgreSQL
+        
+        
+        Python 2
+        --------
+        
+        There is no active support for python 2, however it is compatible as of
+        February 2019, if you install ``funcsigs``.
+        
+        
         License
         -------
         
         Apache 2.0. See LICENSE for details.
         
 Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Internet
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
 Provides-Extra: dev
+Provides-Extra: python2
 Provides-Extra: mysql
+Provides-Extra: postgresql
```

