# Comparing `tmp/devpi-client-6.0.3.tar.gz` & `tmp/devpi-client-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-client-6.0.3.tar", last modified: Mon Feb 20 09:11:16 2023, max compression
+gzip compressed data, was "devpi-client-6.0.4.tar", last modified: Thu Apr 13 05:14:10 2023, max compression
```

## Comparing `devpi-client-6.0.3.tar` & `devpi-client-6.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:16.122377 devpi-client-6.0.3/
--rw-r--r--   0 fschulze   (501) staff       (20)      192 2023-02-20 09:11:07.000000 devpi-client-6.0.3/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    26050 2023-02-20 09:11:07.000000 devpi-client-6.0.3/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-02-20 09:11:07.000000 devpi-client-6.0.3/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      147 2023-02-20 09:11:07.000000 devpi-client-6.0.3/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     6349 2023-02-20 09:11:16.122493 devpi-client-6.0.3/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      930 2023-02-20 09:11:07.000000 devpi-client-6.0.3/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:16.115060 devpi-client-6.0.3/devpi/
--rw-r--r--   0 fschulze   (501) staff       (20)       23 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       70 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/__main__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1540 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/getjson.py
--rw-r--r--   0 fschulze   (501) staff       (20)      679 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3772 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/index.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2177 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/install.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7711 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/list_remove.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1430 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/login.py
--rw-r--r--   0 fschulze   (501) staff       (20)    44026 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3565 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/push.py
--rw-r--r--   0 fschulze   (501) staff       (20)      536 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/pypirc.py
--rw-r--r--   0 fschulze   (501) staff       (20)      550 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/refresh.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9930 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/test.py
--rw-r--r--   0 fschulze   (501) staff       (20)    20340 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/upload.py
--rw-r--r--   0 fschulze   (501) staff       (20)    28348 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/use.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3290 2023-02-20 09:11:07.000000 devpi-client-6.0.3/devpi/user.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:16.116747 devpi-client-6.0.3/devpi_client.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     6349 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      987 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      129 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      125 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        6 2023-02-20 09:11:16.000000 devpi-client-6.0.3/devpi_client.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      542 2023-02-20 09:11:07.000000 devpi-client-6.0.3/pyproject.toml
--rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-02-20 09:11:16.122932 devpi-client-6.0.3/setup.cfg
--rwxr-xr-x   0 fschulze   (501) staff       (20)     2540 2023-02-20 09:11:07.000000 devpi-client-6.0.3/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:16.121846 devpi-client-6.0.3/testing/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    25680 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/conftest.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-02-20 09:11:16.122140 devpi-client-6.0.3/testing/data/
--rw-r--r--   0 fschulze   (501) staff       (20)     1846 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/data/dddttt-0.1.dev45-py27-none-any.whl
--rw-r--r--   0 fschulze   (501) staff       (20)    20813 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3040 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6106 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/simpypi.py
--rw-r--r--   0 fschulze   (501) staff       (20)    18203 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4556 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4245 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_install.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13592 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_list_remove.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2167 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_login.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3757 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9700 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_push.py
--rw-r--r--   0 fschulze   (501) staff       (20)      979 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_pypirc.py
--rw-r--r--   0 fschulze   (501) staff       (20)    20033 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_test.py
--rw-r--r--   0 fschulze   (501) staff       (20)    27607 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_upload.py
--rw-r--r--   0 fschulze   (501) staff       (20)    40391 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_use.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1905 2023-02-20 09:11:07.000000 devpi-client-6.0.3/testing/test_user.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1190 2023-02-20 09:11:07.000000 devpi-client-6.0.3/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172940 devpi-client-6.0.4/
+-rw-r--r--   0 fschulze   (501) staff       (20)      192 2023-04-13 05:14:01.000000 devpi-client-6.0.4/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    26534 2023-04-13 05:14:01.000000 devpi-client-6.0.4/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-04-13 05:14:01.000000 devpi-client-6.0.4/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      147 2023-04-13 05:14:01.000000 devpi-client-6.0.4/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     6725 2023-04-13 05:14:10.173057 devpi-client-6.0.4/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      930 2023-04-13 05:14:01.000000 devpi-client-6.0.4/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.161411 devpi-client-6.0.4/devpi/
+-rw-r--r--   0 fschulze   (501) staff       (20)       23 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       70 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/__main__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1540 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/getjson.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      679 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3772 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2177 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/install.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7711 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/list_remove.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1430 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/login.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    45869 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3565 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/push.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      536 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/pypirc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      550 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/refresh.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9930 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/test.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    20388 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/upload.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    28791 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/use.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3290 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/user.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.163096 devpi-client-6.0.4/devpi_client.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     6725 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      987 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      129 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      125 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        6 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      510 2023-04-13 05:14:01.000000 devpi-client-6.0.4/pyproject.toml
+-rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-04-13 05:14:10.173506 devpi-client-6.0.4/setup.cfg
+-rwxr-xr-x   0 fschulze   (501) staff       (20)     2540 2023-04-13 05:14:01.000000 devpi-client-6.0.4/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172242 devpi-client-6.0.4/testing/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    25605 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/conftest.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172678 devpi-client-6.0.4/testing/data/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1846 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/data/dddttt-0.1.dev45-py27-none-any.whl
+-rw-r--r--   0 fschulze   (501) staff       (20)    21019 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/simpypi.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    18203 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4556 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4245 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_install.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13592 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_list_remove.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3811 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_login.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7466 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    10817 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_push.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      979 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_pypirc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    20033 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_test.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    31200 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_upload.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    47698 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_use.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1905 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_user.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1253 2023-04-13 05:14:01.000000 devpi-client-6.0.4/tox.ini
```

### Comparing `devpi-client-6.0.3/CHANGELOG` & `devpi-client-6.0.4/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 
 
 .. towncrier release notes start
 
+6.0.4 (2023-04-13)
+==================
+
+Bug Fixes
+---------
+
+- Fix precedence of URL from command line over DEVPI_INDEX environment variable for ``devpi use``.
+
+- Fix relative DEVPI_INDEX environment variable with user and index causing an invalid URL in some cases.
+
+- Fix persistence of username when DEVPI_INDEX environment variable is used with ``devpi login``.
+
+- Fix precedence of ``--sdist`` and ``--wheel`` over ``formats`` setting from setup.cfg ``[devpi:upload]`` section.
+
+
 6.0.3 (2023-02-20)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #919: Retry 3 times and wait a moment on PermissionError during file removal to fix race condition after running tox.
```

### Comparing `devpi-client-6.0.3/LICENSE` & `devpi-client-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/PKG-INFO` & `devpi-client-6.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-client
-Version: 6.0.3
+Version: 6.0.4
 Summary: devpi upload/install/... workflow commands for Python developers
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/client/CHANGELOG
@@ -57,14 +57,29 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.0.4 (2023-04-13)
+==================
+
+Bug Fixes
+---------
+
+- Fix precedence of URL from command line over DEVPI_INDEX environment variable for ``devpi use``.
+
+- Fix relative DEVPI_INDEX environment variable with user and index causing an invalid URL in some cases.
+
+- Fix persistence of username when DEVPI_INDEX environment variable is used with ``devpi login``.
+
+- Fix precedence of ``--sdist`` and ``--wheel`` over ``formats`` setting from setup.cfg ``[devpi:upload]`` section.
+
+
 6.0.3 (2023-02-20)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #919: Retry 3 times and wait a moment on PermissionError during file removal to fix race condition after running tox.
@@ -162,16 +177,7 @@
 
 
 Other Changes
 -------------
 
 - When there is no json error message only the HTML error code and reason is printed now, to get the full HTML output use the ``--debug`` flag.
 
-
-5.2.3 (2021-11-15)
-==================
-
-Bug Fixes
----------
-
-- Bump upper version limit on pluggy to <2.0.
-
```

### Comparing `devpi-client-6.0.3/README.rst` & `devpi-client-6.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/getjson.py` & `devpi-client-6.0.4/devpi/getjson.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/hookspecs.py` & `devpi-client-6.0.4/devpi/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/index.py` & `devpi-client-6.0.4/devpi/index.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/install.py` & `devpi-client-6.0.4/devpi/install.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/list_remove.py` & `devpi-client-6.0.4/devpi/list_remove.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/login.py` & `devpi-client-6.0.4/devpi/login.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/main.py` & `devpi-client-6.0.4/devpi/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,38 +254,73 @@
 
         self.info("using workdir", workdir)
         try:
             yield workdir
         finally:
             rmtree(workdir.strpath, onerror=remove_readonly)
 
-    @cached_property
-    def current(self):
+    def get_current(self, args_url=None):
         self.clientdir.ensure(dir=1)
         current = PersistentCurrent(self.auth_path, self.current_path)
-        url = getattr(self.args, "index", None)
+        index_url = getattr(self.args, "index", None)
         if "DEVPI_INDEX" in os.environ:
-            if url is None:
-                if current.index is None:
+            devpi_index = os.environ["DEVPI_INDEX"]
+            self.debug("Got DEVPI_INDEX from environment: %s", devpi_index)
+            if args_url is not None:
+                self.info(
+                    "Using index URL from command line instead of "
+                    "DEVPI_INDEX (%s) from environment." % devpi_index)
+                # cache in case get_current was called directly
+                self.__dict__['current'] = current
+                return current
+            if URL(devpi_index).is_valid_http_url():
+                # switch to full DEVPI_INDEX URL, so possible relative
+                # --index switches work
+                current.persist_index = False
+                current.configure_fromurl(self, devpi_index)
+            if index_url is None:
+                if current.index is None or '/' in devpi_index:
                     url = current.root_url
                 else:
                     url = current.index_url
+                url = url.joinpath(devpi_index)
+                if not current.root_url.is_valid_http_url() and not url.is_valid_http_url():
+                    self.fatal(
+                        "No server set and DEVPI_INDEX from environment is not a "
+                        "full valid URL: %s" % devpi_index)
+                self.info("Using DEVPI_INDEX from environment: %s" % devpi_index)
             else:
-                url = URL(url)
-            devpi_index = os.environ["DEVPI_INDEX"]
-            url = url.joinpath(devpi_index)
-            if not current.root_url.is_valid_http_url() and not url.is_valid_http_url():
-                self.fatal(
-                    "No server set and DEVPI_INDEX from environment is not a "
-                    "full valid URL: %s" % devpi_index)
-            self.info("Using DEVPI_INDEX from environment: %s" % devpi_index)
+                url = URL(index_url)
+                if not url.is_valid_http_url():
+                    if not current.root_url.is_valid_http_url():
+                        if not URL(devpi_index).is_valid_http_url():
+                            self.fatal(
+                                "No server set and neither the --index URL (%s) "
+                                "nor the DEVPI_INDEX from environment (%s) is a "
+                                "full valid URL." % (index_url, devpi_index))
+                        url = URL(devpi_index)
+                        self.info("Using DEVPI_INDEX from environment: %s" % devpi_index)
+                    elif current.index is None or '/' in index_url:
+                        url = current.root_url
+                    else:
+                        url = current.index_url
+                    url = url.joinpath(index_url)
+        else:
+            url = index_url
         if url is not None:
-            current = current.switch_to_local(self, URL(url).url, None)
+            current.persist_index = False
+            current.configure_fromurl(self, URL(url).url)
+        # cache in case get_current was called directly
+        self.__dict__['current'] = current
         return current
 
+    @cached_property
+    def current(self):
+        return self.get_current()
+
     def get_existing_file(self, arg):
         p = py.path.local(arg, expanduser=True)
         if not p.exists():
             self.fatal("file does not exist: %s" % p)
         elif not p.isfile():
             self.fatal("is not a file: %s" % p)
         return p
@@ -1147,29 +1182,29 @@
     parser.add_argument(
         "--venv", action="store", metavar="DIR",
         help="install into specified virtualenv.")
     parser.add_argument("-r", "--requirement", action="store_true",
         help="Install from the given requirements file.")
     parser.add_argument("pkgspecs", metavar="pkg", type=str,
         action="store", default=None, nargs="*",
-        help="uri or package file for installation from current index. """)
+        help="uri or package file for installation from current index. ")
 
 
 @subcommand("devpi.refresh")
 def refresh(parser):
     """ invalidates the mirror caches for the specified package(s).
 
     In case your devpi server hasn't updated the list of latest releases, this
     forces a reload of the them (EXPERIMENTAL).
     """
     parser.add_argument("--index", default=None,
         help="index to refresh (defaults to current index)")
     parser.add_argument(
         "pkgnames", metavar="pkg", type=str, action="store", nargs="+",
-        help="package name to refresh.""")
+        help="package name to refresh.")
 
 
 def verify_reply_version(hub, reply):
     acceptable_api_version = ("2",)
     version = reply.headers.get("X-DEVPI-API-VERSION", None)
     if version is None:
         if not hasattr(hub, "_WARNAPI_DELIVERED"):
```

### Comparing `devpi-client-6.0.3/devpi/push.py` & `devpi-client-6.0.4/devpi/push.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/pypirc.py` & `devpi-client-6.0.4/devpi/pypirc.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/refresh.py` & `devpi-client-6.0.4/devpi/refresh.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/test.py` & `devpi-client-6.0.4/devpi/test.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi/upload.py` & `devpi-client-6.0.4/devpi/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     def post(self, action, path, meta):
         hub = self.hub
         assert "name" in meta and "version" in meta, meta
         dic = meta.copy()
         pypi_action = action
         dic[":action"] = pypi_action
-        dic["protocol_version"] = "1",
+        dic["protocol_version"] = "1"
         headers = {}
         auth = hub.current.get_auth()
         if auth:
             auth = (auth[0], hub.derive_token(auth[1], meta['name']))
             set_devpi_auth_header(headers, auth)
         if path:
             files = {"content": (path.basename, path.open("rb"))}
@@ -401,18 +401,20 @@
                 return setup_format == "zip"
             else:
                 return setup_format == "gztar"
         return False
 
     def setup_build(self, default_formats=None):
         deprecated_formats = []
+        sdist = self.args.sdist
+        wheel = self.args.wheel
         formats = self.args.formats
         if formats is None:
             formats = default_formats
-        if formats:
+        if formats and not sdist and not wheel:
             sdist = None
             wheel = None
             for format in formats.split(","):
                 format = format.strip()
                 if not format:
                     continue
                 if self.is_default_sdist(format):
@@ -443,17 +445,14 @@
                     "replace it with --wheel to only get wheel release "
                     "as with your currently specified format.")
             else:
                 self.hub.warn(
                     "The --formats option is deprecated, "
                     "you can remove it to get the default sdist and wheel "
                     "releases you get with your currently specified formats.")
-        else:
-            sdist = self.args.sdist
-            wheel = self.args.wheel
 
         cmds = []
         if sdist is not None or wheel is not None:
             cmd = [self.python, "-m", "build"]
             if sdist:
                 cmd.append("--sdist")
             if wheel:
@@ -555,10 +554,11 @@
     return res
 
 
 def read_setupcfg(hub, path):
     setup_cfg = path.join("setup.cfg")
     if setup_cfg.exists():
         cfg = iniconfig.IniConfig(setup_cfg)
-        hub.line("detected devpi:upload section in %s" % setup_cfg, bold=True)
-        return cfg.sections.get("devpi:upload", {})
+        if 'devpi:upload' in cfg.sections:
+            hub.line("detected devpi:upload section in %s" % setup_cfg, bold=True)
+            return cfg.sections["devpi:upload"]
     return {}
```

### Comparing `devpi-client-6.0.3/devpi/use.py` & `devpi-client-6.0.4/devpi/use.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,39 +15,44 @@
 else:
     vbin = "bin"
 
 devpi_endpoints = "index simpleindex pypisubmit login".split()
 devpi_data_keys = ["features"]
 
 
-def currentproperty(name):
-    def propget(self):
-        return self._currentdict.get(name, None)
+class baseproperty(object):
+    def __init__(self, name):
+        self.name = name
 
-    def propset(self, val):
-        self._currentdict[name] = val
+    def __get__(self, inst, owner=None):
+        if inst is None:
+            return self
+        return getattr(inst, self.dict_name).get(self.name)
 
-    return property(propget, propset)
+    def __set__(self, inst, value):
+        getattr(inst, self.dict_name)[self.name] = value
 
 
-def authproperty(name):
-    def propget(self):
-        return self._authdict.get(name, None)
+class authproperty(baseproperty):
+    dict_name = '_authdict'
 
-    def propset(self, val):
-        self._authdict[name] = val
 
-    return property(propget, propset)
+class currentproperty(baseproperty):
+    dict_name = '_currentdict'
+
+
+class indexproperty(baseproperty):
+    dict_name = '_currentdict'
 
 
 class Current(object):
-    index = currentproperty("index")
-    simpleindex = currentproperty("simpleindex")
-    pypisubmit = currentproperty("pypisubmit")
-    login = currentproperty("login")
+    index = indexproperty("index")
+    simpleindex = indexproperty("simpleindex")
+    pypisubmit = indexproperty("pypisubmit")
+    login = indexproperty("login")
     username = currentproperty("username")
     venvdir = currentproperty("venvdir")
     _auth = authproperty("auth")
     _basic_auth = authproperty("basic_auth")
     _client_cert = authproperty("client_cert")
     always_setcfg = currentproperty("always_setcfg")
     settrusted = currentproperty("settrusted")
@@ -377,27 +382,37 @@
             indexname=indexname).addpath('+simple', asdir=1)
 
     def get_simpleproject_url(self, name, indexname=None):
         return self.get_simpleindex_url(
             indexname=indexname).addpath(name, asdir=1)
 
 
+def _load_json(path, dest):
+    if path is None:
+        return
+    if not path.check():
+        return
+    raw = path.read().strip()
+    if not raw:
+        return
+    data = json.loads(raw)
+    if not isinstance(data, dict):
+        return
+    dest.update(data)
+
+
 class PersistentCurrent(Current):
+    persist_index = True
+
     def __init__(self, auth_path, current_path):
         Current.__init__(self)
         self.auth_path = auth_path
         self.current_path = current_path
-        if self.auth_path.check():
-            auth_data = self.auth_path.read().strip()
-            if auth_data:
-                self._authdict.update(json.loads(auth_data))
-        if self.current_path and self.current_path.check():
-            current_data = self.current_path.read().strip()
-            if current_data:
-                self._currentdict.update(json.loads(current_data))
+        _load_json(self.auth_path, self._authdict)
+        _load_json(self.current_path, self._currentdict)
 
     def exists(self):
         return self.current_path and self.current_path.check()
 
     def _persist(self, data, path, force_write=False):
         if path is None:
             return
@@ -412,17 +427,24 @@
                     json.dumps(data, indent=2, sort_keys=True))
             finally:
                 os.umask(oldumask)
 
     def reconfigure(self, data, force_write=False):
         Current.reconfigure(self, data)
         self._persist(self._authdict, self.auth_path, force_write=force_write)
+        currentdict = {}
+        _load_json(self.current_path, currentdict)
+        for key, value in self._currentdict.items():
+            prop = getattr(self.__class__, key)
+            if isinstance(prop, indexproperty) and not self.persist_index:
+                continue
+            currentdict[key] = value
         # we make sure to remove legacy auth data
-        self._currentdict.pop("auth", None)
-        self._persist(self._currentdict, self.current_path, force_write=force_write)
+        currentdict.pop("auth", None)
+        self._persist(currentdict, self.current_path, force_write=force_write)
 
 
 def out_index_list(hub, data):
     for user in sorted(data):
         indexes = data[user].get("indexes", {})
         for index, ixconfig in sorted(indexes.items()):
             ixname = "%s/%s" % (user, index)
@@ -441,15 +463,15 @@
             current = hub.current
             hub.info("Creating local configuration at %s" % hub.local_current_path)
             hub.local_current_path.ensure()
             current = current.switch_to_local(
                 hub, current.index, hub.local_current_path)
             # now store existing data in new location
             current.reconfigure({}, force_write=True)
-    current = hub.current
+    current = hub.get_current(args.url)
 
     if args.delete:
         if not hub.current.exists():
             hub.error_and_out("NO configuration found")
         hub.current.current_path.remove()
         hub.info("REMOVED configuration at", hub.current.current_path)
         return
```

### Comparing `devpi-client-6.0.3/devpi/user.py` & `devpi-client-6.0.4/devpi/user.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/devpi_client.egg-info/PKG-INFO` & `devpi-client-6.0.4/devpi_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-client
-Version: 6.0.3
+Version: 6.0.4
 Summary: devpi upload/install/... workflow commands for Python developers
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/client/CHANGELOG
@@ -57,14 +57,29 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.0.4 (2023-04-13)
+==================
+
+Bug Fixes
+---------
+
+- Fix precedence of URL from command line over DEVPI_INDEX environment variable for ``devpi use``.
+
+- Fix relative DEVPI_INDEX environment variable with user and index causing an invalid URL in some cases.
+
+- Fix persistence of username when DEVPI_INDEX environment variable is used with ``devpi login``.
+
+- Fix precedence of ``--sdist`` and ``--wheel`` over ``formats`` setting from setup.cfg ``[devpi:upload]`` section.
+
+
 6.0.3 (2023-02-20)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #919: Retry 3 times and wait a moment on PermissionError during file removal to fix race condition after running tox.
@@ -162,16 +177,7 @@
 
 
 Other Changes
 -------------
 
 - When there is no json error message only the HTML error code and reason is printed now, to get the full HTML output use the ``--debug`` flag.
 
-
-5.2.3 (2021-11-15)
-==================
-
-Bug Fixes
----------
-
-- Bump upper version limit on pluggy to <2.0.
-
```

### Comparing `devpi-client-6.0.3/devpi_client.egg-info/SOURCES.txt` & `devpi-client-6.0.4/devpi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/setup.py` & `devpi-client-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     extras_require = {}
 
     setup(
       name="devpi-client",
       description="devpi upload/install/... workflow commands for Python "
                   "developers",
       long_description="\n\n".join([README, CHANGELOG]),
-      version='6.0.3',
+      version='6.0.4',
       packages=['devpi'],
       install_requires=install_requires,
       extras_require=extras_require,
       python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
       url="https://devpi.net",
       project_urls={
           'Bug Tracker': 'https://github.com/devpi/devpi/issues',
```

### Comparing `devpi-client-6.0.3/testing/conftest.py` & `devpi-client-6.0.4/testing/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -738,20 +738,18 @@
         args = parse_args(["devpi_"] + arglist, pm)
         with tmp.as_cwd():
             return Hub(args)
     return mkhub
 
 
 @pytest.fixture
-def mock_http_api(monkeypatch):
+def mock_http_api(monkeypatch, reqmock):  # noqa
     """ mock out all Hub.http_api calls and return an object
     offering 'set' and 'add' to fake replies. """
     from devpi import main
-    from requests.sessions import Session
-    monkeypatch.setattr(Session, "request", None)
 
     class MockHTTPAPI:
         def __init__(self):
             self.called = []
             self._json_responses = {}
 
         def __call__(self, method, url, kvdict=None, quiet=False,
```

### Comparing `devpi-client-6.0.3/testing/data/dddttt-0.1.dev45-py27-none-any.whl` & `devpi-client-6.0.4/testing/data/dddttt-0.1.dev45-py27-none-any.whl`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/functional.py` & `devpi-client-6.0.4/testing/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     from urllib import quote as url_quote  # type: ignore
 
 
 class API:
     def __init__(self, d):
         self.__dict__ = d
 
+    def __repr__(self):
+        cls = self.__class__
+        name = "%s.%s" % (cls.__module__, cls.__name__)
+        return "<%s %r>" % (
+            name, self.__dict__.get('stagename', 'uninitialized'))
+
 
 class MappMixin:
     _usercount = 0
 
     def create_and_use(self, stagename=None, password="123", indexconfig=None):
         if stagename is None:
             stagename = self.get_new_stagename()
```

### Comparing `devpi-client-6.0.3/testing/reqmock.py` & `devpi-client-6.0.4/testing/reqmock.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             response = self.url2reply.get((url, None))
             if response is None:
                 for (name, method), response in self.url2reply.items():
                     if method is None or method == request.method:
                         if fnmatch.fnmatch(request.url, name):
                             break
                 else:
-                    raise Exception("not mocked call to %s" % url)
+                    raise Exception("not mocked call to %s" % url)  # noqa: TRY002
         response.add_request(request)
         r = HTTPAdapter().build_response(request, response)
         return r
 
     def mockresponse(self, url, code, method=None, data=None, headers=None,
                      on_request=None, reason=None):
         if not url:
```

### Comparing `devpi-client-6.0.3/testing/simpypi.py` & `devpi-client-6.0.4/testing/simpypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
 class SimPyPI:
     def __init__(self, address):
         self.baseurl = "http://%s:%s" % address
         self.simpleurl = "%s/simple" % self.baseurl
         self.projects = {}
         self.files = {}
+        self.clear()
+
+    def clear(self):
         self.clear_log()
         self.clear_requests()
 
     def clear_log(self):
         self.log = []
 
     def clear_requests(self):
```

### Comparing `devpi-client-6.0.3/testing/test_functional.py` & `devpi-client-6.0.4/testing/test_functional.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_index.py` & `devpi-client-6.0.4/testing/test_index.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_install.py` & `devpi-client-6.0.4/testing/test_install.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_list_remove.py` & `devpi-client-6.0.4/testing/test_list_remove.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_push.py` & `devpi-client-6.0.4/testing/test_push.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,14 +86,39 @@
     pusher = parse_target(loghub, args)
     mock_http_api.set("src/dev", 200, result={})
     pusher.execute(loghub, "pytest", "2.3.5")
     dict(name="pytest", version="2.3.5", targetindex="user/name")
     assert len(mock_http_api.called) == 1
 
 
+def test_push_devpi_index_option_with_environment(loghub, monkeypatch, mock_http_api):
+    loghub.args.target = "user/name"
+    loghub.args.index = "src/dev"
+    monkeypatch.setenv("DEVPI_INDEX", "http://devpi/user/dev")
+    mock_http_api.set(
+        "http://devpi/user/dev/+api", 200, result=dict(
+            pypisubmit="http://devpi/user/dev/",
+            simpleindex="http://devpi/user/dev/+simple/",
+            index="http://devpi/user/dev",
+            login="http://devpi/+login",
+            authstatus=["noauth", "", []]))
+    mock_http_api.set(
+        "http://devpi/src/dev/+api", 200, result=dict(
+            pypisubmit="http://devpi/src/dev/",
+            simpleindex="http://devpi/src/dev/+simple/",
+            index="http://devpi/src/dev",
+            login="http://devpi/+login",
+            authstatus=["noauth", "", []]))
+    pusher = parse_target(loghub, loghub.args)
+    mock_http_api.set("http://devpi/src/dev", 200, result={})
+    pusher.execute(loghub, "pytest", "2.3.5")
+    dict(name="pytest", version="2.3.5", targetindex="user/name")
+    assert len(mock_http_api.called) == 3
+
+
 @pytest.mark.parametrize("spec", ("pkg==1.0", "pkg-1.0"))
 def test_main_push_pypi(capsys, monkeypatch, tmpdir, spec):
     from devpi.push import main
     l = []
 
     def mypost(method, url, data, headers, auth=None, cert=None, verify=None):
         l.append((method, url, data))
@@ -240,15 +265,15 @@
         def info(self, msg):
             msgs.append(msg)
 
         def warn(self, msg):
             msgs.append(msg)
     hub = MockHub()
     hub.derive_token = Hub.derive_token.__get__(hub)
-    hub.derive_token("%s-foo" % prefix, None) == "%s-foo" % prefix
+    assert hub.derive_token("%s-foo" % prefix, None) == "%s-foo" % prefix
     (msg,) = msgs
     assert "can not parse it" in msg
 
 
 @pytest.mark.skipif("sys.version_info < (3, 7)")
 def test_derive_token():
     import pypitoken
```

### Comparing `devpi-client-6.0.3/testing/test_pypirc.py` & `devpi-client-6.0.4/testing/test_pypirc.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_test.py` & `devpi-client-6.0.4/testing/test_test.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/testing/test_upload.py` & `devpi-client-6.0.4/testing/test_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             runproc("git config user.name 'you'")
             runproc("git add {0}/file {0}/link {0}/setup.py".format(setupdir_rel))
             runproc("git add {0}/file {0}/{1}".format(setupdir_rel,
                                                       unicode_fn))
             runproc("git commit -m message")
         return repo
 
-    def test_vcs_export(self, uploadhub, repo, setupdir, tmpdir, monkeypatch):
+    def test_vcs_export(self, uploadhub, repo, setupdir, tmpdir):
         checkout = Checkout(uploadhub, uploadhub.args, setupdir)
         assert checkout.rootpath == repo
         newrepo = tmpdir.mkdir("newrepo")
         result = checkout.export(newrepo)
         assert result.rootpath.join("file").check()
         assert result.rootpath.join("link").check()
         if not sys.platform.startswith("win"):
@@ -141,37 +141,36 @@
                                       tmpdir, monkeypatch):
         monkeypatch.setattr(uploadhub.args, "novcs", True)
         checkout = Checkout(uploadhub, uploadhub.args, setupdir)
         assert not checkout.hasvcs
         exported = checkout.export(tmpdir)
         assert exported.rootpath == checkout.setupdir
 
-    def test_vcs_export_verify_setup(self, uploadhub, setupdir,
-                                          tmpdir, monkeypatch):
+    def test_vcs_export_verify_setup(self, uploadhub, setupdir, tmpdir):
         subdir = setupdir.mkdir("subdir")
         subdir.ensure("setup.py")
         checkout = Checkout(uploadhub, uploadhub.args, subdir)
         wc = tmpdir.mkdir("wc")
         exported = checkout.export(wc)
         assert not exported.rootpath.join("setup.py").check()
 
-    def test_export_attributes(self, uploadhub, setupdir, tmpdir, monkeypatch):
+    def test_export_attributes(self, uploadhub, setupdir, tmpdir):
         checkout = Checkout(uploadhub, uploadhub.args, setupdir)
         setupdir.join("setup.py").write(dedent("""
             from setuptools import setup
             # some packages like numpy produce output during build, simulate:
             print("* foo, bar")
             setup(name="xyz", version="1.2.3")
         """))
         exported = checkout.export(tmpdir)
         name, version = exported.setup_name_and_version()
         assert name == "xyz"
         assert version == "1.2.3"
 
-    def test_setup_build_docs(self, uploadhub, setupdir, tmpdir, monkeypatch):
+    def test_setup_build_docs(self, uploadhub, setupdir, tmpdir):
         checkout = Checkout(uploadhub, uploadhub.args, setupdir)
         setupdir.join("setup.py").write(dedent("""
             from setuptools import setup
             setup(name="xyz", version="1.2.3")
         """))
         exported = checkout.export(tmpdir)
         assert exported.rootpath != exported.origrepo
@@ -225,27 +224,29 @@
     assert find_parent_subpath(tmpdir.mkdir("a"), "xyz") == s
     assert find_parent_subpath(tmpdir.ensure("a", "b"), "xyz") == s
     assert find_parent_subpath(s, "xyz") == s
     pytest.raises(ValueError, lambda: find_parent_subpath(tmpdir, "poiqel123"))
 
 
 @pytest.mark.skipif("config.option.fast")
-def test_post_includes_auth_info(initproj, monkeypatch, uploadhub):
+def test_post_includes_auth_info(initproj, uploadhub):
     class Session:
         posts = []
 
         def post(self, *args, **kwargs):
             class reply:
                 status_code = 200
             self.posts.append((args, kwargs))
             return reply
 
     class args:
         dryrun = None
-        formats = "sdist,bdist_wheel"
+        sdist = False
+        wheel = False
+        formats = None
         index = None
         no_isolation = True
         novcs = None
         only_latest = None
         onlydocs = None
         path = None
         python = None
@@ -273,17 +274,71 @@
     assert "X-Devpi-Auth" in upload1[1]["headers"]
     assert upload2[0][1][":action"] == "file_upload"
     assert upload2[1]["auth"] == ("basic", "auth")
     assert upload2[1]["cert"] == certpath
     assert "X-Devpi-Auth" in upload2[1]["headers"]
 
 
+@pytest.mark.skipif("sys.version_info < (3,)")
+@pytest.mark.skipif("config.option.fast")
+def test_post_data(initproj, monkeypatch, reqmock, uploadhub):
+    import email
+
+    class args:
+        dryrun = None
+        sdist = False
+        wheel = False
+        formats = None
+        index = None
+        no_isolation = True
+        novcs = None
+        only_latest = None
+        onlydocs = None
+        path = None
+        python = None
+        setupdironly = None
+        verbose = 0
+        withdocs = None
+
+    class Response:
+        status_code = 200
+
+    sent = []
+
+    def send(req, **kw):
+        sent.append((req, kw))
+        return Response()
+
+    initproj("pkg-1.0")
+    tmpdir = py.path.local()
+    uploadhub.cwd = tmpdir
+    uploadhub.current.reconfigure(dict(
+        index="http://devpi/foo/bar",
+        login="http://devpi/+login",
+        pypisubmit="http://devpi/foo/bar"))
+    monkeypatch.setattr(uploadhub.http, "send", send)
+    main(uploadhub, args)
+    # convert POST data to Message
+    msg = email.message_from_bytes(
+        b"MIME-Version: 1.0\nContent-Type: %s\n\n%s" % (
+            sent[0][0].headers['Content-Type'].encode('ascii'),
+            sent[0][0].body))
+    # get the data
+    data = {
+        x.get_param("name", header="Content-Disposition"): x.get_payload()
+        for x in msg.get_payload()}
+    assert data[":action"] == "file_upload"
+    assert data["name"] == "pkg"
+    assert data["protocol_version"] == "1"
+    assert data["version"] == "1.0"
+
+
 @pytest.mark.skipif("sys.version_info < (3, 7)")
 @pytest.mark.skipif("config.option.fast")
-def test_post_derived_devpi_token(initproj, monkeypatch, uploadhub):
+def test_post_derived_devpi_token(initproj, uploadhub):
     from base64 import b64decode
     import pypitoken
 
     class Session:
         posts = []
 
         def post(self, *args, **kwargs):
@@ -583,29 +638,50 @@
         # go to other index
         out = out_devpi("use", other_index)
 
         # --index option
         out = out_devpi("upload", "--no-isolation", "--index", "%s/dev" % user, "--dry-run")
         out.stdout.fnmatch_lines_random("skipped: file_upload*to*/%s/dev*" % user)
 
+    @pytest.mark.parametrize("other_index", ["root/pypi", "/"])
+    def test_index_option_with_environment_relative(
+            self, devpi, initproj, monkeypatch, out_devpi,
+            other_index, projname_version):
+        initproj(projname_version.rsplit("-", 1), {"doc": {
+            "conf.py": "#nothing",
+            "contents.rst": "",
+            "index.html": "<html/>"}})
+        assert py.path.local("setup.py").check()
+        # remember username
+        out = out_devpi("use")
+        user = re.search(r'\(logged in as (.+?)\)', out.stdout.str()).group(1)
+
+        # go to other index
+        out = out_devpi("use", other_index)
+
+        monkeypatch.setenv("DEVPI_INDEX", "user/dev")
+        # --index option
+        out = out_devpi("upload", "--no-isolation", "--index", "%s/dev" % user, "--dry-run")
+        out.stdout.fnmatch_lines_random("skipped: file_upload*to*/%s/dev*" % user)
+
     def test_logout(self, capfd, devpi, out_devpi, projname_version):
         # logoff then upload
         out = out_devpi("logoff")
         out.stdout.fnmatch_lines_random("login information deleted")
 
         # see if we get an error return code
         (out, err) = capfd.readouterr()
         res = devpi("upload", "--no-isolation")
         (out, err) = capfd.readouterr()
         assert "401 FAIL file_upload" in out
         assert "Unauthorized" in out
         assert isinstance(res.sysex, SystemExit)
         assert res.sysex.args == (1,)
 
-    def test_fromdir(self, initproj, devpi, out_devpi, runproc, monkeypatch):
+    def test_fromdir(self, initproj, devpi, out_devpi, runproc):
         initproj("hello-1.1", {"doc": {
             "conf.py": "",
             "index.html": "<html/>"}})
         tmpdir = py.path.local()
         runproc(tmpdir, "python setup.py sdist --format=zip".split())
         initproj("hello-1.2")
         runproc(tmpdir, "python setup.py sdist --format=zip".split())
@@ -649,14 +725,44 @@
         data = json.loads(out.stdout.str())
         vv = ViewLinkStore(url, data["result"])
         assert len(vv.get_links()) == 2
         links = dict((x.rel, x.basename.lower()) for x in vv.get_links())
         assert links["releasefile"] == "%s.zip" % name_version_str
         assert links["doczip"] == "%s.doc.zip" % name_version_str
 
+    def test_cli_sdist_precedence(self, initproj, devpi, out_devpi):
+        initproj("pkg-1.0")
+        tmpdir = py.path.local()
+        tmpdir.join("setup.cfg").write(dedent("""
+            [devpi:upload]
+            formats=bdist_wheel,sdist.zip"""))
+        hub = devpi("upload", "--sdist", "--no-isolation")
+        url = hub.current.get_index_url().url + 'pkg/1.0/'
+        out = out_devpi("getjson", url)
+        data = json.loads(out.stdout.str())
+        vv = ViewLinkStore(url, data["result"])
+        assert len(vv.get_links()) == 1
+        assert vv.get_links()[0].basename in ('pkg-1.0.tar.gz', 'pkg-1.0.zip')
+
+    def test_cli_wheel_precedence(self, initproj, devpi, out_devpi):
+        initproj("pkg-1.0")
+        tmpdir = py.path.local()
+        tmpdir.join("setup.cfg").write(dedent("""
+            [devpi:upload]
+            formats=bdist_wheel,sdist.zip"""))
+        hub = devpi("upload", "--wheel", "--no-isolation")
+        url = hub.current.get_index_url().url + 'pkg/1.0/'
+        out = out_devpi("getjson", url)
+        data = json.loads(out.stdout.str())
+        vv = ViewLinkStore(url, data["result"])
+        assert len(vv.get_links()) == 1
+        assert vv.get_links()[0].basename in (
+            'pkg-1.0-py2-none-any.whl',
+            'pkg-1.0-py3-none-any.whl')
+
 
 def test_getpkginfo(datadir):
     info = get_pkginfo(datadir.join("dddttt-0.1.dev45-py27-none-any.whl"))
     assert info.name == "dddttt"
     assert info.metadata_version == "2.0"
     info = get_pkginfo(datadir.join("ddd-1.0.doc.zip"))
     assert info.name == "ddd"
```

### Comparing `devpi-client-6.0.3/testing/test_use.py` & `devpi-client-6.0.4/testing/test_use.py`

 * *Files 12% similar despite different names*

```diff
@@ -798,14 +798,78 @@
         assert "Using DEVPI_INDEX from environment: http://devpi/user/dev\n" in out
         assert "index: http://devpi/user/dev" in out
         assert "simpleindex: http://devpi/user/dev/+simple/" in out
         assert "pypisubmit: http://devpi/user/dev/" in out
         assert "login: http://devpi/+login" in out
 
     @pytest.mark.parametrize("devpi_index", ["user/dev", "/user/dev"])
+    def test_environment_relative_with_current(
+            self, capfd, cmd_devpi, devpi_index, mock_http_api, monkeypatch):
+        mock_http_api.set(
+            "http://world/user/dev/+api", 200, result=dict(
+                pypisubmit="http://world/user/dev/",
+                simpleindex="http://world/user/dev/+simple/",
+                index="http://world/user/dev",
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://world/user/dev?no_projects=", 200, result=dict())
+        cmd_devpi("use", "http://world/user/dev")
+        (out, err) = capfd.readouterr()
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "index: http://world/user/dev" in out
+        assert "simpleindex: http://world/user/dev/+simple/" in out
+        assert "pypisubmit: http://world/user/dev/" in out
+        assert "login: http://world/+login" in out
+        monkeypatch.setenv("DEVPI_INDEX", devpi_index)
+        mock_http_api.set(
+            "http://world/user/dev/+api", 200, result=dict(
+                pypisubmit="http://world/user/dev/",
+                simpleindex="http://world/user/dev/+simple/",
+                index="http://world/user/dev",
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://world/user/dev?no_projects=", 200, result=dict())
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using DEVPI_INDEX from environment: %s\n" % devpi_index in out
+        assert "index: http://world/user/dev" in out
+        assert "simpleindex: http://world/user/dev/+simple/" in out
+        assert "pypisubmit: http://world/user/dev/" in out
+        assert "login: http://world/+login" in out
+
+    def test_environment_with_root_current(self, capfd, cmd_devpi, mock_http_api, monkeypatch):
+        mock_http_api.set(
+            "http://world/+api", 200, result=dict(
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        cmd_devpi("use", "http://world/")
+        (out, err) = capfd.readouterr()
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "using server: http://world/ (not logged in)" in out
+        assert "no current index" in out
+        monkeypatch.setenv("DEVPI_INDEX", "http://devpi/user/dev")
+        mock_http_api.set(
+            "http://devpi/user/dev/+api", 200, result=dict(
+                pypisubmit="http://devpi/user/dev/",
+                simpleindex="http://devpi/user/dev/+simple/",
+                index="http://devpi/user/dev",
+                login="http://devpi/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://devpi/user/dev?no_projects=", 200, result=dict())
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using DEVPI_INDEX from environment: http://devpi/user/dev\n" in out
+        assert "index: http://devpi/user/dev" in out
+        assert "simpleindex: http://devpi/user/dev/+simple/" in out
+        assert "pypisubmit: http://devpi/user/dev/" in out
+        assert "login: http://devpi/+login" in out
+
+    @pytest.mark.parametrize("devpi_index", ["user/dev", "/user/dev"])
     def test_environment_relative_with_root_current(
             self, capfd, cmd_devpi, devpi_index, mock_http_api, monkeypatch):
         mock_http_api.set(
             "http://world/+api", 200, result=dict(
                 login="http://world/+login",
                 authstatus=["noauth", "", []]))
         cmd_devpi("use", "http://world/")
@@ -827,14 +891,89 @@
         (out, err) = capfd.readouterr()
         assert "Using DEVPI_INDEX from environment: %s\n" % devpi_index in out
         assert "index: http://world/user/dev" in out
         assert "simpleindex: http://world/user/dev/+simple/" in out
         assert "pypisubmit: http://world/user/dev/" in out
         assert "login: http://world/+login" in out
 
+    def test_environment_with_url_from_commandline(
+            self, capfd, cmd_devpi, mock_http_api, monkeypatch):
+        monkeypatch.setenv("DEVPI_INDEX", "http://devpi/user/dev")
+        mock_http_api.set(
+            "http://world/user/foo/+api", 200, result=dict(
+                pypisubmit="http://world/user/foo/",
+                simpleindex="http://world/user/foo/+simple/",
+                index="http://world/user/foo",
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://world/user/foo?no_projects=", 200, result=dict())
+        cmd_devpi("use", "http://world/user/foo")
+        (out, err) = capfd.readouterr()
+        assert "Using index URL from command line" in out
+        mock_http_api.set(
+            "http://devpi/user/dev/+api", 200, result=dict(
+                pypisubmit="http://devpi/user/dev/",
+                simpleindex="http://devpi/user/dev/+simple/",
+                index="http://devpi/user/dev",
+                login="http://devpi/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://devpi/user/dev?no_projects=", 200, result=dict())
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using DEVPI_INDEX from environment: http://devpi/user/dev\n" in out
+        assert "index: http://devpi/user/dev" in out
+        assert "simpleindex: http://devpi/user/dev/+simple/" in out
+        assert "pypisubmit: http://devpi/user/dev/" in out
+        assert "login: http://devpi/+login" in out
+        cmd_devpi("use", "http://world/user/foo", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using index URL from command line" in out
+        assert "index: http://world/user/foo" in out
+        assert "simpleindex: http://world/user/foo/+simple/" in out
+        assert "pypisubmit: http://world/user/foo/" in out
+        assert "login: http://world/+login" in out
+
+    @pytest.mark.parametrize("devpi_index", ["user/dev", "/user/dev"])
+    def test_environment_relative_with_url_from_commandline(
+            self, capfd, cmd_devpi, devpi_index, mock_http_api, monkeypatch):
+        monkeypatch.setenv("DEVPI_INDEX", devpi_index)
+        mock_http_api.set(
+            "http://world/user/foo/+api", 200, result=dict(
+                pypisubmit="http://world/user/foo/",
+                simpleindex="http://world/user/foo/+simple/",
+                index="http://world/user/foo",
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://world/user/foo?no_projects=", 200, result=dict())
+        cmd_devpi("use", "http://world/user/foo")
+        (out, err) = capfd.readouterr()
+        assert "Using index URL from command line" in out
+        mock_http_api.set(
+            "http://world/user/dev/+api", 200, result=dict(
+                pypisubmit="http://world/user/dev/",
+                simpleindex="http://world/user/dev/+simple/",
+                index="http://world/user/dev",
+                login="http://world/+login",
+                authstatus=["noauth", "", []]))
+        mock_http_api.set("http://world/user/dev?no_projects=", 200, result=dict())
+        cmd_devpi("use", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using DEVPI_INDEX from environment: %s\n" % devpi_index in out
+        assert "index: http://world/user/dev" in out
+        assert "simpleindex: http://world/user/dev/+simple/" in out
+        assert "pypisubmit: http://world/user/dev/" in out
+        assert "login: http://world/+login" in out
+        cmd_devpi("use", "http://world/user/foo", "--urls")
+        (out, err) = capfd.readouterr()
+        assert "Using index URL from command line" in out
+        assert "index: http://world/user/foo" in out
+        assert "simpleindex: http://world/user/foo/+simple/" in out
+        assert "pypisubmit: http://world/user/foo/" in out
+        assert "login: http://world/+login" in out
+
 
 def test_getparse_keyvalues_invalid():
     with pytest.raises(ValueError):
         get_keyvalues(["hello123"])
 
 
 @pytest.mark.parametrize("input expected".split(), [
```

### Comparing `devpi-client-6.0.3/testing/test_user.py` & `devpi-client-6.0.4/testing/test_user.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.3/tox.ini` & `devpi-client-6.0.4/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 timeout = 60
 
 
 [tox]
 envlist = py27-server520,py27-version,py27,py35,py38,pypy,pypy3
 
 [testenv]
-passenv = LANG, PIP_INDEX_URL
+passenv = GITHUB_ACTIONS, LANG, PIP_INDEX_URL
 deps =
        pytest
        pytest-flake8 < 1.1.0;python_version=="2.7"
        pytest-flake8;python_version!="2.7"
        flake8<5
+       pytest-github-actions-annotate-failures
        pytest-instafail
        pytest-timeout
        devpi-server;python_version!="2.7"
        pypitoken;python_version>="3.7"
        importlib.metadata;python_version<"3.8"
        py35: ruamel.yaml
        py35: pyparsing<3
```

