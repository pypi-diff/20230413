# Comparing `tmp/awsenergylabelercli-3.2.2.tar.gz` & `tmp/awsenergylabelercli-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsenergylabelercli-3.2.2.tar", last modified: Tue Apr 11 15:06:10 2023, max compression
+gzip compressed data, was "awsenergylabelercli-3.2.3.tar", last modified: Thu Apr 13 15:01:15 2023, max compression
```

## Comparing `awsenergylabelercli-3.2.2.tar` & `awsenergylabelercli-3.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2556 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/USAGE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/aws_energy_labeler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/awsenergylabelercli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2556 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2327 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33423 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/awsenergylabelercli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/awsenergylabelercliexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/awsenergylabelercli/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/conf/logging.json-example
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     8899 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/awsenergylabelercli/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 15:06:10.000000 awsenergylabelercli-3.2.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:10.656591 awsenergylabelercli-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    75400 2023-04-11 15:04:47.000000 awsenergylabelercli-3.2.2/tests/test_awsenergylabelercli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.222700 awsenergylabelercli-3.2.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2650 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-13 15:01:15.222700 awsenergylabelercli-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/USAGE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/aws_energy_labeler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.218700 awsenergylabelercli-3.2.3/awsenergylabelercli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2650 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74016 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2327 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33423 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/awsenergylabelercli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/awsenergylabelercliexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.218700 awsenergylabelercli-3.2.3/awsenergylabelercli/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/conf/logging.json-example
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8899 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/awsenergylabelercli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.218700 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 15:01:15.000000 awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.222700 awsenergylabelercli-3.2.3/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-13 15:01:14.000000 awsenergylabelercli-3.2.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-13 15:01:15.222700 awsenergylabelercli-3.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:01:15.222700 awsenergylabelercli-3.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    75400 2023-04-13 14:59:42.000000 awsenergylabelercli-3.2.3/tests/test_awsenergylabelercli.py
```

### Comparing `awsenergylabelercli-3.2.2/CONTRIBUTING.rst` & `awsenergylabelercli-3.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/HISTORY.rst` & `awsenergylabelercli-3.2.3/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -157,7 +157,13 @@
 * Bump dependencies.
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Added support for Python3.11
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Bumped library - Changed dataclass to normal class
```

### Comparing `awsenergylabelercli-3.2.2/LICENSE` & `awsenergylabelercli-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/PKG-INFO` & `awsenergylabelercli-3.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelercli
-Version: 3.2.2
+Version: 3.2.3
 Summary: A cli to label accounts and landing zones with energy labels based on Security Hub finding.
 Home-page: https://github.com/schubergphilis/awsenergylabelercli.git
 Author: Theodoor Scholte
 Author-email: tscholte@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelercli energy labeler aws security hub
 Classifier: Development Status :: 4 - Beta
@@ -237,7 +237,13 @@
 * Bump dependencies.
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Added support for Python3.11
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Bumped library - Changed dataclass to normal class
```

### Comparing `awsenergylabelercli-3.2.2/Pipfile.lock` & `awsenergylabelercli-3.2.3/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843689083820664%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'07f8e18c5951b8b181a95cf802f6469bc0ba7f899d532902ef9b41044fe99c7a'}}",*

 * * "'default'": "{'awsenergylabelerlib': {'hashes': "*

 * *              "['sha256:9bccf51d81bc56ac1e5b94c5ff9191715e4b2f460dc898c277c87b8b1fdd61cf', "*

 * *              "'sha256:d22a7fe8d703abab191aa39e6edc71441cf4393bfd50e2c6c980bed4a2418ae6'], "*

 * *              "'version': '==3.2.3'}, 'boto3': {'hashes': "*

 * *              "['sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f', "*

 * *   […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1ab88e138ae8adb7b47045ad44d28cc53a5e521563d413534d4fb8d5c8d3135c"
+            "sha256": "07f8e18c5951b8b181a95cf802f6469bc0ba7f899d532902ef9b41044fe99c7a"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -22,35 +22,35 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "awsenergylabelerlib": {
             "hashes": [
-                "sha256:15b05d392c8be56788fae8de4745848f32180e2b865af67cf1b89255599cb192",
-                "sha256:78215206f3822b396ebca0a70a26f2b1c55338b47c650ccb5c4241a1e1c52da7"
+                "sha256:9bccf51d81bc56ac1e5b94c5ff9191715e4b2f460dc898c277c87b8b1fdd61cf",
+                "sha256:d22a7fe8d703abab191aa39e6edc71441cf4393bfd50e2c6c980bed4a2418ae6"
             ],
             "index": "pypi",
-            "version": "==3.2.2"
+            "version": "==3.2.3"
         },
         "boto3": {
             "hashes": [
-                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
-                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
+                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
+                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
             ],
             "markers": "python_version >= '3.7'",
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
             "markers": "python_version ~= '3.7'",
@@ -782,19 +782,19 @@
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
@@ -1005,19 +1005,19 @@
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

### Comparing `awsenergylabelercli-3.2.2/README.rst` & `awsenergylabelercli-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/USAGE.rst` & `awsenergylabelercli-3.2.3/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/aws_energy_labeler_cli.py` & `awsenergylabelercli-3.2.3/aws_energy_labeler_cli.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/CONTRIBUTING.rst` & `awsenergylabelercli-3.2.3/awsenergylabelercli/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/HISTORY.rst` & `awsenergylabelercli-3.2.3/awsenergylabelercli/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -157,7 +157,13 @@
 * Bump dependencies.
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Added support for Python3.11
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Bumped library - Changed dataclass to normal class
```

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/LICENSE` & `awsenergylabelercli-3.2.3/awsenergylabelercli/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/Pipfile.lock` & `awsenergylabelercli-3.2.3/awsenergylabelercli/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843689083820664%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'07f8e18c5951b8b181a95cf802f6469bc0ba7f899d532902ef9b41044fe99c7a'}}",*

 * * "'default'": "{'awsenergylabelerlib': {'hashes': "*

 * *              "['sha256:9bccf51d81bc56ac1e5b94c5ff9191715e4b2f460dc898c277c87b8b1fdd61cf', "*

 * *              "'sha256:d22a7fe8d703abab191aa39e6edc71441cf4393bfd50e2c6c980bed4a2418ae6'], "*

 * *              "'version': '==3.2.3'}, 'boto3': {'hashes': "*

 * *              "['sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f', "*

 * *   […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "1ab88e138ae8adb7b47045ad44d28cc53a5e521563d413534d4fb8d5c8d3135c"
+            "sha256": "07f8e18c5951b8b181a95cf802f6469bc0ba7f899d532902ef9b41044fe99c7a"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -22,35 +22,35 @@
                 "sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1"
             ],
             "index": "pypi",
             "version": "==5.9"
         },
         "awsenergylabelerlib": {
             "hashes": [
-                "sha256:15b05d392c8be56788fae8de4745848f32180e2b865af67cf1b89255599cb192",
-                "sha256:78215206f3822b396ebca0a70a26f2b1c55338b47c650ccb5c4241a1e1c52da7"
+                "sha256:9bccf51d81bc56ac1e5b94c5ff9191715e4b2f460dc898c277c87b8b1fdd61cf",
+                "sha256:d22a7fe8d703abab191aa39e6edc71441cf4393bfd50e2c6c980bed4a2418ae6"
             ],
             "index": "pypi",
-            "version": "==3.2.2"
+            "version": "==3.2.3"
         },
         "boto3": {
             "hashes": [
-                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
-                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
+                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
+                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
             ],
             "markers": "python_version >= '3.7'",
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
             "markers": "python_version ~= '3.7'",
@@ -782,19 +782,19 @@
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
@@ -1005,19 +1005,19 @@
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

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/README.rst` & `awsenergylabelercli-3.2.3/awsenergylabelercli/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/USAGE.rst` & `awsenergylabelercli-3.2.3/awsenergylabelercli/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/__init__.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/__init__.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/_version.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/_version.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/awsenergylabelercli.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/awsenergylabelercli.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/awsenergylabelercliexceptions.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/awsenergylabelercliexceptions.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/conf/logging.json-example` & `awsenergylabelercli-3.2.3/awsenergylabelercli/conf/logging.json-example`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/dev-requirements.txt` & `awsenergylabelercli-3.2.3/awsenergylabelercli/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/entities.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/entities.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli/validators.py` & `awsenergylabelercli-3.2.3/awsenergylabelercli/validators.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/PKG-INFO` & `awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelercli
-Version: 3.2.2
+Version: 3.2.3
 Summary: A cli to label accounts and landing zones with energy labels based on Security Hub finding.
 Home-page: https://github.com/schubergphilis/awsenergylabelercli.git
 Author: Theodoor Scholte
 Author-email: tscholte@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelercli energy labeler aws security hub
 Classifier: Development Status :: 4 - Beta
@@ -237,7 +237,13 @@
 * Bump dependencies.
 
 
 3.2.2 (11-04-2023)
 ------------------
 
 * Added support for Python3.11
+
+
+3.2.3 (13-04-2023)
+------------------
+
+* Bumped library - Changed dataclass to normal class
```

### Comparing `awsenergylabelercli-3.2.2/awsenergylabelercli.egg-info/SOURCES.txt` & `awsenergylabelercli-3.2.3/awsenergylabelercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/dev-requirements.txt` & `awsenergylabelercli-3.2.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/docs/Makefile` & `awsenergylabelercli-3.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/docs/conf.py` & `awsenergylabelercli-3.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/docs/index.rst` & `awsenergylabelercli-3.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/setup.py` & `awsenergylabelercli-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelercli-3.2.2/tests/test_awsenergylabelercli.py` & `awsenergylabelercli-3.2.3/tests/test_awsenergylabelercli.py`

 * *Files identical despite different names*

