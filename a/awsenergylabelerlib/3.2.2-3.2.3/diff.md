# Comparing `tmp/awsenergylabelerlib-3.2.2.tar.gz` & `tmp/awsenergylabelerlib-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsenergylabelerlib-3.2.2.tar", last modified: Tue Apr 11 14:35:51 2023, max compression
+gzip compressed data, was "awsenergylabelerlib-3.2.3.tar", last modified: Thu Apr 13 14:51:20 2023, max compression
```

## Comparing `awsenergylabelerlib-3.2.2.tar` & `awsenergylabelerlib-3.2.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3529 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/USAGE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.015179 awsenergylabelerlib-3.2.2/awsenergylabelerlib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3529 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlibexceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/datamodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/dev-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    40854 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.015179 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/USAGE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.985839 awsenergylabelerlib-3.2.3/awsenergylabelerlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlibexceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/datamodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40747 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.985839 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_validations.py
```

### Comparing `awsenergylabelerlib-3.2.2/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/HISTORY.rst` & `awsenergylabelerlib-3.2.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -194,7 +194,13 @@
 * Updated dependencies
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Convert Dataclasses to Frozen for compatibility with latest python.
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Changed from dataclass to normal.
```

### Comparing `awsenergylabelerlib-3.2.2/LICENSE` & `awsenergylabelerlib-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/PKG-INFO` & `awsenergylabelerlib-3.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.2
+Version: 3.2.3
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -281,7 +281,13 @@
 * Updated dependencies
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Convert Dataclasses to Frozen for compatibility with latest python.
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Changed from dataclass to normal.
```

### Comparing `awsenergylabelerlib-3.2.2/Pipfile` & `awsenergylabelerlib-3.2.3/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/Pipfile.lock` & `awsenergylabelerlib-3.2.3/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943646996278576%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f', "*

 * *              "'sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69'], "*

 * *              "'version': '==1.26.112'}, 'botocore': {'hashes': "*

 * *              "['sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1', "*

 * *              "'sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
-                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
+                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
+                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
             ],
             "index": "pypi",
-            "version": "==1.26.110"
+            "version": "==1.26.112"
         },
         "botocore": {
             "hashes": [
-                "sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399",
-                "sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0"
+                "sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1",
+                "sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.110"
+            "version": "==1.29.112"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -725,19 +725,19 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
@@ -948,19 +948,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.3"
+            "version": "==13.3.4"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
```

### Comparing `awsenergylabelerlib-3.2.2/README.rst` & `awsenergylabelerlib-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/USAGE.rst` & `awsenergylabelerlib-3.2.3/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/HISTORY.rst` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -194,7 +194,13 @@
 * Updated dependencies
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Convert Dataclasses to Frozen for compatibility with latest python.
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Changed from dataclass to normal.
```

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/LICENSE` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile.lock` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943646996278576%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f', "*

 * *              "'sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69'], "*

 * *              "'version': '==1.26.112'}, 'botocore': {'hashes': "*

 * *              "['sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1', "*

 * *              "'sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
-                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
+                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
+                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
             ],
             "index": "pypi",
-            "version": "==1.26.110"
+            "version": "==1.26.112"
         },
         "botocore": {
             "hashes": [
-                "sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399",
-                "sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0"
+                "sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1",
+                "sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.110"
+            "version": "==1.29.112"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -725,19 +725,19 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
@@ -948,19 +948,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.3"
+            "version": "==13.3.4"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
```

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/README.rst` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/USAGE.rst` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/__init__.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/_version.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/_version.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlibexceptions.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlibexceptions.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/configuration.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/configuration.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/datamodels.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/datamodels.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/dev-requirements.txt` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/entities.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,20 @@
 entities package.
 
 Import all parts from entities here
 
 .. _Google Python Style Guide:
    http://google.github.io/styleguide/pyguide.html
 """
-# pylint: disable=too-many-lines
 
 import logging
 import tempfile
 from abc import ABC, abstractmethod
 from collections import Counter
 from copy import copy, deepcopy
-from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urlparse, urljoin
 
 import boto3
 import botocore.errorfactory
 import botocore.exceptions
@@ -379,26 +377,24 @@
         accounts = []
         for page in paginator.paginate():
             accounts.extend([AwsAccount(account.get('AccountId'), self.account_thresholds)
                              for account in page['Members']])
         return accounts
 
 
-@dataclass(frozen=True)
 class AwsAccount:
     """Models the aws account that can label itself."""
 
-    id: str  # pylint: disable=invalid-name
-    account_thresholds: field(default_factory=list)
-    name: str = 'NOT_RETRIEVED'
-    energy_label: AccountEnergyLabel = AccountEnergyLabel()
-    _alias: str = None
-
-    def __post_init__(self):
-        super().__setattr__('_logger', logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}'))
+    def __init__(self, id_: str, account_thresholds: list, name='NOT_RETRIEVED') -> None:
+        self.id = id_
+        self.account_thresholds = account_thresholds
+        self.name = name
+        self._alias = None
+        self.energy_label = AccountEnergyLabel()
+        self._logger = logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}')
 
     @property
     def alias(self):
         """Alias."""
         if self._alias is None:
             self._alias = ''
             try:
@@ -470,22 +466,20 @@
                                                        number_of_low_findings,
                                                        max_days_open)
         except Exception:  # pylint: disable=broad-except
             self._logger.warning(f'Could not calculate energy label for account {self.id}, using the default "F"')
         return self.energy_label
 
 
-@dataclass(frozen=True)
 class Finding:
     """Models a finding."""
 
-    _data: dict
-
-    def __post_init__(self):
-        super().__setattr__('_logger', logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}'))
+    def __init__(self, data: dict) -> None:
+        self._data = data
+        self._logger = logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}')
 
     def __hash__(self):
         return hash(self.id)
 
     def __eq__(self, other):
         """Override the default equals behavior."""
         if not isinstance(other, Finding):
```

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/labels.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/labels.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/schemas.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/schemas.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib/validations.py` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib/validations.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/PKG-INFO` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.2
+Version: 3.2.3
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -281,7 +281,13 @@
 * Updated dependencies
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Convert Dataclasses to Frozen for compatibility with latest python.
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Changed from dataclass to normal.
```

### Comparing `awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/SOURCES.txt` & `awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/dev-requirements.txt` & `awsenergylabelerlib-3.2.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/docs/Makefile` & `awsenergylabelerlib-3.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/docs/conf.py` & `awsenergylabelerlib-3.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/docs/index.rst` & `awsenergylabelerlib-3.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/setup.py` & `awsenergylabelerlib-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/tests/test_awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.3/tests/test_awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/tests/test_entities.py` & `awsenergylabelerlib-3.2.3/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.2/tests/test_validations.py` & `awsenergylabelerlib-3.2.3/tests/test_validations.py`

 * *Files identical despite different names*

