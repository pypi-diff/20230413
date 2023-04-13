# Comparing `tmp/pytest-invenio-2.1.2.tar.gz` & `tmp/pytest-invenio-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-invenio-2.1.2.tar", last modified: Fri Mar 24 18:01:01 2023, max compression
+gzip compressed data, was "pytest-invenio-2.1.3.tar", last modified: Thu Apr 13 14:55:09 2023, max compression
```

## Comparing `pytest-invenio-2.1.2.tar` & `pytest-invenio-2.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.592338 pytest-invenio-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.588338 pytest-invenio-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.588338 pytest-invenio-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5305 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9233 2023-03-24 18:01:01.592338 pytest-invenio-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/constraints-min.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.588338 pytest-invenio-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.588338 pytest-invenio-2.1.2/pytest_invenio/
--rw-r--r--   0 runner    (1001) docker     (122)    16246 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/pytest_invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26781 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/pytest_invenio/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/pytest_invenio/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5164 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/pytest_invenio/user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.592338 pytest-invenio-2.1.2/pytest_invenio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9233 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-24 18:01:01.000000 pytest-invenio-2.1.2/pytest_invenio.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      734 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-03-24 18:01:01.592338 pytest-invenio-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 18:01:01.592338 pytest-invenio-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    18451 2023-03-24 18:00:54.000000 pytest-invenio-2.1.2/tests/test_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.630480 pytest-invenio-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.622480 pytest-invenio-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.626480 pytest-invenio-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5374 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9334 2023-04-13 14:55:09.630480 pytest-invenio-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/constraints-min.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.626480 pytest-invenio-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.626480 pytest-invenio-2.1.3/pytest_invenio/
+-rw-r--r--   0 runner    (1001) docker     (122)    16246 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/pytest_invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26535 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/pytest_invenio/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/pytest_invenio/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5164 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/pytest_invenio/user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.630480 pytest-invenio-2.1.3/pytest_invenio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9334 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-13 14:55:09.000000 pytest-invenio-2.1.3/pytest_invenio.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      734 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-13 14:55:09.630480 pytest-invenio-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:55:09.630480 pytest-invenio-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18463 2023-04-13 14:55:00.000000 pytest-invenio-2.1.3/tests/test_fixtures.py
```

### Comparing `pytest-invenio-2.1.2/.editorconfig` & `pytest-invenio-2.1.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/.github/workflows/pypi-publish.yml` & `pytest-invenio-2.1.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/.github/workflows/tests.yml` & `pytest-invenio-2.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/CHANGES.rst` & `pytest-invenio-2.1.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     pytest-invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.3 (released 2023-04-13)
+
+- db: upgrade flask-sqlalchemy
+
 Version 2.1.2 (released 2023-03-20)
 
 - disable request rate-limiting
 
 Version 2.1.1 (released 2022-10-25)
 
 - pin pytest version
```

### Comparing `pytest-invenio-2.1.2/CONTRIBUTING.rst` & `pytest-invenio-2.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/INSTALL.rst` & `pytest-invenio-2.1.3/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/LICENSE` & `pytest-invenio-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/MANIFEST.in` & `pytest-invenio-2.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/PKG-INFO` & `pytest-invenio-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-invenio
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pytest fixtures for Invenio.
 Home-page: https://github.com/inveniosoftware/pytest-invenio
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of pytest-invenio.
@@ -52,14 +52,18 @@
         
             pytest-invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.3 (released 2023-04-13)
+        
+        - db: upgrade flask-sqlalchemy
+        
         Version 2.1.2 (released 2023-03-20)
         
         - disable request rate-limiting
         
         Version 2.1.1 (released 2022-10-25)
         
         - pin pytest version
```

### Comparing `pytest-invenio-2.1.2/README.rst` & `pytest-invenio-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/docs/Makefile` & `pytest-invenio-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/docs/conf.py` & `pytest-invenio-2.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/docs/index.rst` & `pytest-invenio-2.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/docs/make.bat` & `pytest-invenio-2.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/pytest_invenio/__init__.py` & `pytest-invenio-2.1.3/pytest_invenio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,10 +495,10 @@
     before_script:
       - "export DISPLAY=:99.0"
       - "sh -e /etc/init.d/xvfb start"
       - sleep 3 # give xvfb some time to start
 """
 
 
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 
 __all__ = ("__version__",)
```

### Comparing `pytest-invenio-2.1.2/pytest_invenio/fixtures.py` & `pytest-invenio-2.1.3/pytest_invenio/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,30 +484,21 @@
     fixture will set a save point and rollback all changes performed during
     the test (this is much faster than recreating the entire database).
     """
     import sqlalchemy as sa
 
     connection = database.engine.connect()
     transaction = connection.begin()
+    old_session = database.session
 
+    # Create a new session and assign it to the current db session.
+    # The new session is scoped and bound to the `connection`.
     options = dict(bind=connection, binds={})
-    session = database.create_scoped_session(options=options)
-
-    session.begin_nested()
-
-    # `session` is actually a scoped_session. For the `after_transaction_end`
-    # event, we need a session instance to listen for, hence the `session()`
-    # call.
-    @sa.event.listens_for(session(), "after_transaction_end")
-    def restart_savepoint(sess, trans):
-        if trans.nested and not trans._parent.nested:
-            session.expire_all()
-            session.begin_nested()
-
-    old_session = database.session
+    session_factory = sa.orm.sessionmaker(**options)
+    session = sa.orm.scoped_session(session_factory)
     database.session = session
 
     yield database
 
     session.remove()
     transaction.rollback()
     connection.close()
```

### Comparing `pytest-invenio-2.1.2/pytest_invenio/plugin.py` & `pytest-invenio-2.1.3/pytest_invenio/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/pytest_invenio/user.py` & `pytest-invenio-2.1.3/pytest_invenio/user.py`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/pytest_invenio.egg-info/PKG-INFO` & `pytest-invenio-2.1.3/pytest_invenio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-invenio
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pytest fixtures for Invenio.
 Home-page: https://github.com/inveniosoftware/pytest-invenio
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of pytest-invenio.
@@ -52,14 +52,18 @@
         
             pytest-invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.3 (released 2023-04-13)
+        
+        - db: upgrade flask-sqlalchemy
+        
         Version 2.1.2 (released 2023-03-20)
         
         - disable request rate-limiting
         
         Version 2.1.1 (released 2022-10-25)
         
         - pin pytest version
```

### Comparing `pytest-invenio-2.1.2/pytest_invenio.egg-info/SOURCES.txt` & `pytest-invenio-2.1.3/pytest_invenio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/pytest_invenio.egg-info/requires.txt` & `pytest-invenio-2.1.3/pytest_invenio.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 
 [opensearch2]
 invenio-search[opensearch2]<3.0.0,>=2.1.0
 
 [tests]
 pytest-black>=0.3.0
 invenio-celery<2.0.0,>=1.2.4
-invenio-db<2.0.0,>=1.0.12
+invenio-db<2.0.0,>=1.1.0
 invenio-files-rest<2.0.0,>=1.3.2
 invenio-mail<2.0.0,>=1.0.2
 invenio-search<3.0.0,>=2.1.0
 sphinx>=4.5
```

### Comparing `pytest-invenio-2.1.2/run-tests.sh` & `pytest-invenio-2.1.3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/setup.cfg` & `pytest-invenio-2.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	importlib-metadata>=4.4
 	importlib-resources>=5.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0
 	invenio-celery>=1.2.4,<2.0.0
-	invenio-db>=1.0.12,<2.0.0
+	invenio-db>=1.1.0,<2.0.0
 	invenio-files-rest>=1.3.2,<2.0.0
 	invenio-mail>=1.0.2,<2.0.0
 	invenio-search>=2.1.0,<3.0.0
 	sphinx>=4.5
 elasticsearch7 = 
 	invenio-search[elasticsearch7]>=2.1.0,<3.0.0
 opensearch1 =
```

### Comparing `pytest-invenio-2.1.2/setup.py` & `pytest-invenio-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/tests/conftest.py` & `pytest-invenio-2.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-invenio-2.1.2/tests/test_fixtures.py` & `pytest-invenio-2.1.3/tests/test_fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,19 +315,19 @@
     conftest_testdir.runpytest().assert_outcomes(passed=1)
 
 
 def test_db(conftest_testdir):
     """Test database creation and initialization."""
     conftest_testdir.makepyfile(
         """
-        from invenio_db import db
+        from invenio_db import db as _db
 
-        class UserA(db.Model):
-            id = db.Column(db.Integer, primary_key=True)
-            username = db.Column(db.String(80), unique=True)
+        class UserA(_db.Model):
+            id = _db.Column(_db.Integer, primary_key=True)
+            username = _db.Column(_db.String(80), unique=True)
 
         def test_db1(db):
             assert UserA.query.count() == 0
             db.session.add(UserA(username='alice'))
             db.session.commit()
             assert UserA.query.count() == 1
```

