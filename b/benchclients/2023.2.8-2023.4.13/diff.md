# Comparing `tmp/benchclients-2023.2.8.tar.gz` & `tmp/benchclients-2023.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchclients-2023.2.8.tar", last modified: Wed Feb  8 21:32:54 2023, max compression
+gzip compressed data, was "benchclients-2023.4.13.tar", last modified: Thu Apr 13 13:38:08 2023, max compression
```

## Comparing `benchclients-2023.2.8.tar` & `benchclients-2023.4.13.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:32:54.754996 benchclients-2023.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-08 21:32:40.000000 benchclients-2023.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-08 21:32:54.754996 benchclients-2023.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-08 21:32:40.000000 benchclients-2023.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:32:54.754996 benchclients-2023.2.8/benchclients/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-08 21:32:40.000000 benchclients-2023.2.8/benchclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 21:32:40.000000 benchclients-2023.2.8/benchclients/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-02-08 21:32:40.000000 benchclients-2023.2.8/benchclients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-08 21:32:40.000000 benchclients-2023.2.8/benchclients/conbench.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-08 21:32:40.000000 benchclients-2023.2.8/benchclients/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:32:54.754996 benchclients-2023.2.8/benchclients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-08 21:32:54.000000 benchclients-2023.2.8/benchclients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-08 21:32:54.000000 benchclients-2023.2.8/benchclients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:32:54.000000 benchclients-2023.2.8/benchclients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-08 21:32:54.000000 benchclients-2023.2.8/benchclients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-08 21:32:54.000000 benchclients-2023.2.8/benchclients.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 21:32:40.000000 benchclients-2023.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-08 21:32:40.000000 benchclients-2023.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:32:54.754996 benchclients-2023.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-08 21:32:40.000000 benchclients-2023.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:07.994566 benchclients-2023.4.13/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 13:37:38.000000 benchclients-2023.4.13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-13 13:38:07.994566 benchclients-2023.4.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-13 13:37:38.000000 benchclients-2023.4.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:07.994566 benchclients-2023.4.13/benchclients/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 13:37:38.000000 benchclients-2023.4.13/benchclients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 13:37:44.000000 benchclients-2023.4.13/benchclients/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-13 13:37:38.000000 benchclients-2023.4.13/benchclients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 13:37:38.000000 benchclients-2023.4.13/benchclients/conbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 13:37:38.000000 benchclients-2023.4.13/benchclients/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:07.994566 benchclients-2023.4.13/benchclients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-13 13:38:07.000000 benchclients-2023.4.13/benchclients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 13:38:07.000000 benchclients-2023.4.13/benchclients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:38:07.000000 benchclients-2023.4.13/benchclients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 13:38:07.000000 benchclients-2023.4.13/benchclients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 13:38:07.000000 benchclients-2023.4.13/benchclients.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 13:37:38.000000 benchclients-2023.4.13/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 13:37:38.000000 benchclients-2023.4.13/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:38:07.994566 benchclients-2023.4.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-13 13:37:38.000000 benchclients-2023.4.13/setup.py
```

### Comparing `benchclients-2023.2.8/benchclients/conbench.py` & `benchclients-2023.4.13/benchclients/conbench.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     """A client to interact with a Conbench server.
 
     Parameters
     ----------
     adapter
         A requests adapter to mount to the requests session. If not given, one will be
         created with a backoff retry strategy.
+
     Environment variables
     ---------------------
     CONBENCH_URL
         The URL of the Conbench server. Required.
     CONBENCH_EMAIL
-        The email to use for Conbench login. Only required if the server is private.
+        The email to use for Conbench login. Only required for GETting if the server is private.
     CONBENCH_PASSWORD
-        The password to use for Conbench login. Only required if the server is private.
+        The password to use for Conbench login. Only required for GETting if the server is private.
     """
 
     def __init__(self, adapter: Optional[HTTPAdapter] = None):
         url = os.getenv("CONBENCH_URL")
         if not url:
             fatal_and_log("Environment variable CONBENCH_URL not found")
```

### Comparing `benchclients-2023.2.8/setup.py` & `benchclients-2023.4.13/setup.py`

 * *Files identical despite different names*

