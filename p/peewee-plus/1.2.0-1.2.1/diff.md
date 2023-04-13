# Comparing `tmp/peewee_plus-1.2.0.tar.gz` & `tmp/peewee_plus-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_plus-1.2.0.tar", max compression
+gzip compressed data, was "peewee_plus-1.2.1.tar", max compression
```

## Comparing `peewee_plus-1.2.0.tar` & `peewee_plus-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1053 2022-11-15 15:19:44.471867 peewee_plus-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     4655 2022-11-15 15:19:44.539867 peewee_plus-1.2.0/README.md
--rw-r--r--   0        0        0    14354 2022-11-15 15:18:41.051376 peewee_plus-1.2.0/peewee_plus.py
--rw-r--r--   0        0        0     1540 2022-11-15 15:18:41.055376 peewee_plus-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      348 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/fixtures.py
--rw-r--r--   0        0        0      999 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_about.py
--rw-r--r--   0        0        0     1266 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_calc_batch_size.py
--rw-r--r--   0        0        0     1218 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_enumfield.py
--rw-r--r--   0        0        0      794 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_jsonfield.py
--rw-r--r--   0        0        0     1899 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_pathfield.py
--rw-r--r--   0        0        0      985 2022-11-15 12:56:40.995229 peewee_plus-1.2.0/tests/test_precision_float_field.py
--rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 peewee_plus-1.2.0/setup.py
--rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 peewee_plus-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-13 19:01:56.883362 peewee_plus-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4516 2023-04-13 19:01:56.907362 peewee_plus-1.2.1/README.md
+-rw-r--r--   0        0        0    15314 2023-04-13 18:59:55.010556 peewee_plus-1.2.1/peewee_plus.py
+-rw-r--r--   0        0        0     2521 2023-04-13 18:59:46.222493 peewee_plus-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      348 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/fixtures.py
+-rw-r--r--   0        0        0      999 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_about.py
+-rw-r--r--   0        0        0     1443 2023-04-13 18:59:35.226414 peewee_plus-1.2.1/tests/test_calc_batch_size.py
+-rw-r--r--   0        0        0     1218 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_enumfield.py
+-rw-r--r--   0        0        0      794 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_jsonfield.py
+-rw-r--r--   0        0        0     1899 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_pathfield.py
+-rw-r--r--   0        0        0      985 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_precision_float_field.py
+-rw-r--r--   0        0        0     5859 1970-01-01 00:00:00.000000 peewee_plus-1.2.1/PKG-INFO
```

### Comparing `peewee_plus-1.2.0/LICENSE.md` & `peewee_plus-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/README.md` & `peewee_plus-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 - [Installing](#installing)
 - [Features](#features)
 - [For Developers](#for-developers)
 
 ## Installing
 
-Peewee+ is [available on PyPI](https://pypi.org/project/peewee-plus/) and can be installed
+peewee+ is [available on PyPI](https://pypi.org/project/peewee-plus/) and can be installed
 using Poetry, Pipenv, or Pip:
 
 ```bash
 # Using poetry
 poetry add peewee-plus
 
 # Using pipenv
@@ -53,38 +53,37 @@
 [Peewee docs](http://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings).
 
 `SQLITE_DEFAULT_VARIABLE_LIMIT` - The maximum number of variables an SQL query can use
 when using SQLite
 
 ### Functions
 
-[`calc_batch_size`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L71) -
-Helper function for determining how to batch a create/update query with SQLite
+[`calc_batch_size`](blob/devel/peewee_plus.py#L93) - Helper function for writing
+backend-agnostic batch queries while accounting for the
+[SQLite max variable limit](https://www.sqlite.org/limits.html#max_variable_number).
 
-[`flat_transaction`](https://github.com/enpaul/peewee-plus/blob/devel/peewee_plus.py#L137)
-\- Decorator function for wrapping callables in a database transaction without creating
-nested transactions
+[`flat_transaction`](blob/devel/peewee_plus.py#L159) - Decorator function for wrapping
+callables in a database transaction without creating nested transactions
 
 ### Classes
 
-[`PathField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#179) - A
-Peewee database field for storing
+[`PathField`](blob/devel/peewee_plus.py#204) - A Peewee database field for storing
 [Pathlib](https://docs.python.org/3/library/pathlib.html) objects, optionally relative to
 a runtime value.
 
-[`PrecisionFloatField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L237)
-\- A Peewee database field for storing floats while specifying the
+[`PrecisionFloatField`](blob/devel/peewee_plus.py#L262) - A Peewee database field for
+storing floats while specifying the
 [MySQL precision parameters](https://dev.mysql.com/doc/refman/8.0/en/floating-point-types.html)
 `M` and `D`
 
-[`JSONField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L267) - A
-Peewee database field for storing arbitrary JSON-serializable data
+[`JSONField`](blob/devel/peewee_plus.py#L293) - A Peewee database field for storing
+arbitrary JSON-serializable data
 
-[`EnumField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L322) - A
-Peewee database field for storing Enums by name
+[`EnumField`](blob/devel/peewee_plus.py#L348) - A Peewee database field for storing Enums
+by name
 
 ## For Developers
 
 All project contributors and participants are expected to adhere to the
 [Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
 
 The `devel` branch has the latest (and potentially unstable) changes. The stable releases
@@ -96,16 +95,16 @@
   [open an issue on the Github repository](https://github.com/enpaul/peewee-plus/issues/new).
 - To report a security concern or code of conduct violation, please contact the project
   author directly at **‌me \[at‌\] enp dot‎ ‌one**.
 - To submit an update, please
   [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
   and [open a pull request](https://github.com/enpaul/peewee-plus/compare).
 
-Developing this project requires at least [Python 3.7](https://www.python.org/downloads/)
-and at least [Poetry 1.0](https://python-poetry.org/docs/#installation). GNU Make can
+Developing this project requires [Python 3.10](https://www.python.org/downloads/) or later
+and [Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can
 optionally be used to quickly setup a local development environment, but this is not
 required.
 
 To setup a local development environment:
 
 ```bash
 # Clone the repository...
```

### Comparing `peewee_plus-1.2.0/peewee_plus.py` & `peewee_plus-1.2.1/peewee_plus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-"""Peewee+
+"""peewee+
+
+Various extensions, helpers, and utilities for `Peewee`_
 
 :constant SQLITE_DEFAULT_VARIABLE_LIMIT: The default number of variables that a single SQL query
                                          can contain when interfacing with SQLite. The actual
                                          number is set at compile time and is not easily
                                          discoverable from within Python. This default value will
                                          be correct for the vast majority of applications.
 
 :constant SQLITE_DEFAULT_PRAGMAS: The default pragmas that should be used when instantiating an
                                   SQLite database connection. The value for this constant is taken
                                   directly from the `Peewee documentation`_
 
-.. _`Peewee documentation`: http://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings
+.. _`Peewee`: https://docs.peewee-orm.com/en/latest/
+
+.. _`Peewee documentation`: https://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings
 """
 import contextlib
 import enum
 import functools
 import json
 from pathlib import Path
 from typing import Any
@@ -24,15 +28,15 @@
 from typing import Type
 from typing import TypeVar
 
 import peewee
 
 
 __title__ = "peewee-plus"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __license__ = "MIT"
 __summary__ = "Various extensions, helpers, and utilities for Peewee"
 __url__ = "https://github.com/enpaul/peewee-plus/"
 __authors__ = ["Ethan Paul <24588726+enpaul@users.noreply.github.com>"]
 
 
 __all__ = [
@@ -58,15 +62,33 @@
     "cache_size": -1 * 64000,
     "foreign_keys": 1,
     "ignore_check_constraints": 0,
     "synchronous": 0,
 }
 
 
-SQLITE_DEFAULT_VARIABLE_LIMIT: int = 999
+SQLITE_DEFAULT_VARIABLE_LIMIT: int
+
+# With SQLite 3.32 (2020-05-22) the devs bumped the default variable limit to
+# 32766. This logic attemps to import the sqlite3 bindings and determine whether
+# the version of the installed SQLite version is greater or equal to 3.32. If
+# the sqlite3 bindings cannot be imported (either because they aren't installed)
+# or because the platform is using SQLite 1 or 2 then it falls back to the
+# 999 value.
+try:
+    import sqlite3
+except ImportError:
+    SQLITE_DEFAULT_VARIABLE_LIMIT = 999
+else:
+    if sqlite3.sqlite_version_info[0] >= 3 or (
+        sqlite3.sqlite_version_info[0] == 3 and sqlite3.sqlite_version_info[1] >= 32
+    ):
+        SQLITE_DEFAULT_VARIABLE_LIMIT = 32766
+    else:
+        SQLITE_DEFAULT_VARIABLE_LIMIT = 999
 
 
 T = TypeVar("T", bound=peewee.Model)
 
 
 def calc_batch_size(
     models: Sequence[T], sqlite_variable_limit: int = SQLITE_DEFAULT_VARIABLE_LIMIT
@@ -250,31 +272,32 @@
 
     .. note:: This field's implementation was adapted from here_
 
     .. _`MySQL documentation`: https://dev.mysql.com/doc/refman/8.0/en/floating-point-types.html
     .. _here: https://stackoverflow.com/a/67476045/5361209
 
     :param max_digits: Maximum number of digits, combined from left and right of the decimal place,
-                       to store for the value.
-    :param decimal_places: Maximum number of digits that will be stored after the decimal place
+                       to store for the value; corresponds to the ``M`` MySQL precision parameter.
+    :param decimal_places: Maximum number of digits that will be stored after the decimal place;
+                           corresponds to the ``D`` MySQL precision parameter.
     """
 
     def __init__(self, *args, max_digits: int = 10, decimal_places: int = 4, **kwargs):
         super().__init__(*args, **kwargs)
         self.max_digits = max_digits
         self.decimal_places = decimal_places
 
     def get_modifiers(self):
         return [self.max_digits, self.decimal_places]
 
 
 class JSONField(peewee.TextField):  # pylint: disable=abstract-method
     """Field class for storing JSON-serializable data
 
-    This field can be used to store a dictionary of data directly in the database without needing
+    This field can be used to store a dictionary of data directly in the database
     without needing to call :func:`json.dumps` and :func:`json.loads` directly.
 
     ::
 
         >>> class MyModel(peewee.Model):
         ...    some_data = JSONField()
         ...
```

### Comparing `peewee_plus-1.2.0/tests/test_about.py` & `peewee_plus-1.2.1/tests/test_about.py`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/tests/test_calc_batch_size.py` & `peewee_plus-1.2.1/tests/test_calc_batch_size.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
     class TestModel(peewee.Model):
         class Meta:
             database = fakedb
 
         data = peewee.IntegerField()
 
-    models = [TestModel(item) for item in range(500)]
+    # Three is just chosen as an arbitrary multiplier to ensure the value is larger than the
+    # sqlite variable limit
+    models = [
+        TestModel(item) for item in range(peewee_plus.SQLITE_DEFAULT_VARIABLE_LIMIT * 3)
+    ]
     assert (
         peewee_plus.calc_batch_size(models) <= peewee_plus.SQLITE_DEFAULT_VARIABLE_LIMIT
     )
     assert peewee_plus.calc_batch_size(models) < len(models)
 
     assert peewee_plus.calc_batch_size([]) == 0
```

### Comparing `peewee_plus-1.2.0/tests/test_enumfield.py` & `peewee_plus-1.2.1/tests/test_enumfield.py`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/tests/test_jsonfield.py` & `peewee_plus-1.2.1/tests/test_jsonfield.py`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/tests/test_pathfield.py` & `peewee_plus-1.2.1/tests/test_pathfield.py`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/tests/test_precision_float_field.py` & `peewee_plus-1.2.1/tests/test_precision_float_field.py`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.0/PKG-INFO` & `peewee_plus-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-plus
-Version: 1.2.0
+Version: 1.2.1
 Summary: Various extensions, helpers, and utilities for Peewee
 Home-page: https://github.com/enpaul/peewee-plus/
 License: MIT
 Keywords: peewee,orm,extension,plguin,extra
 Author: Ethan Paul
 Author-email: 24588726+enpaul@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Typing :: Typed
 Requires-Dist: peewee (>=3.14.8,<4.0.0)
@@ -49,15 +50,15 @@
 
 - [Installing](#installing)
 - [Features](#features)
 - [For Developers](#for-developers)
 
 ## Installing
 
-Peewee+ is [available on PyPI](https://pypi.org/project/peewee-plus/) and can be installed
+peewee+ is [available on PyPI](https://pypi.org/project/peewee-plus/) and can be installed
 using Poetry, Pipenv, or Pip:
 
 ```bash
 # Using poetry
 poetry add peewee-plus
 
 # Using pipenv
@@ -84,38 +85,37 @@
 [Peewee docs](http://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings).
 
 `SQLITE_DEFAULT_VARIABLE_LIMIT` - The maximum number of variables an SQL query can use
 when using SQLite
 
 ### Functions
 
-[`calc_batch_size`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L71) -
-Helper function for determining how to batch a create/update query with SQLite
+[`calc_batch_size`](blob/devel/peewee_plus.py#L93) - Helper function for writing
+backend-agnostic batch queries while accounting for the
+[SQLite max variable limit](https://www.sqlite.org/limits.html#max_variable_number).
 
-[`flat_transaction`](https://github.com/enpaul/peewee-plus/blob/devel/peewee_plus.py#L137)
-\- Decorator function for wrapping callables in a database transaction without creating
-nested transactions
+[`flat_transaction`](blob/devel/peewee_plus.py#L159) - Decorator function for wrapping
+callables in a database transaction without creating nested transactions
 
 ### Classes
 
-[`PathField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#179) - A
-Peewee database field for storing
+[`PathField`](blob/devel/peewee_plus.py#204) - A Peewee database field for storing
 [Pathlib](https://docs.python.org/3/library/pathlib.html) objects, optionally relative to
 a runtime value.
 
-[`PrecisionFloatField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L237)
-\- A Peewee database field for storing floats while specifying the
+[`PrecisionFloatField`](blob/devel/peewee_plus.py#L262) - A Peewee database field for
+storing floats while specifying the
 [MySQL precision parameters](https://dev.mysql.com/doc/refman/8.0/en/floating-point-types.html)
 `M` and `D`
 
-[`JSONField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L267) - A
-Peewee database field for storing arbitrary JSON-serializable data
+[`JSONField`](blob/devel/peewee_plus.py#L293) - A Peewee database field for storing
+arbitrary JSON-serializable data
 
-[`EnumField`](https://github.com/enpaul/peewee-plus/blob/1.0.0/peewee_plus.py#L322) - A
-Peewee database field for storing Enums by name
+[`EnumField`](blob/devel/peewee_plus.py#L348) - A Peewee database field for storing Enums
+by name
 
 ## For Developers
 
 All project contributors and participants are expected to adhere to the
 [Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
 
 The `devel` branch has the latest (and potentially unstable) changes. The stable releases
@@ -127,16 +127,16 @@
   [open an issue on the Github repository](https://github.com/enpaul/peewee-plus/issues/new).
 - To report a security concern or code of conduct violation, please contact the project
   author directly at **‌me \[at‌\] enp dot‎ ‌one**.
 - To submit an update, please
   [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
   and [open a pull request](https://github.com/enpaul/peewee-plus/compare).
 
-Developing this project requires at least [Python 3.7](https://www.python.org/downloads/)
-and at least [Poetry 1.0](https://python-poetry.org/docs/#installation). GNU Make can
+Developing this project requires [Python 3.10](https://www.python.org/downloads/) or later
+and [Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can
 optionally be used to quickly setup a local development environment, but this is not
 required.
 
 To setup a local development environment:
 
 ```bash
 # Clone the repository...
```

