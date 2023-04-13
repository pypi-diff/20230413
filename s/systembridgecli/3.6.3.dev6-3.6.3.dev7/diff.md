# Comparing `tmp/systembridgecli-3.6.3.dev6.tar.gz` & `tmp/systembridgecli-3.6.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-3.6.3.dev6.tar", last modified: Mon Apr 10 15:37:24 2023, max compression
+gzip compressed data, was "systembridgecli-3.6.3.dev7.tar", last modified: Thu Apr 13 20:20:15 2023, max compression
```

## Comparing `systembridgecli-3.6.3.dev6.tar` & `systembridgecli-3.6.3.dev7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:24.468515 systembridgecli-3.6.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 15:37:24.468515 systembridgecli-3.6.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-10 15:37:06.000000 systembridgecli-3.6.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:37:24.468515 systembridgecli-3.6.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-10 15:37:06.000000 systembridgecli-3.6.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:24.468515 systembridgecli-3.6.3.dev6/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 15:37:06.000000 systembridgecli-3.6.3.dev6/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-10 15:37:06.000000 systembridgecli-3.6.3.dev6/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 15:37:22.000000 systembridgecli-3.6.3.dev6/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:24.468515 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 15:37:24.000000 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 15:37:24.000000 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:37:24.000000 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 15:37:24.000000 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 15:37:24.000000 systembridgecli-3.6.3.dev6/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:20:15.324780 systembridgecli-3.6.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 20:20:15.324780 systembridgecli-3.6.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 20:19:55.000000 systembridgecli-3.6.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:20:15.324780 systembridgecli-3.6.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 20:19:55.000000 systembridgecli-3.6.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:20:15.324780 systembridgecli-3.6.3.dev7/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 20:19:55.000000 systembridgecli-3.6.3.dev7/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-13 20:19:55.000000 systembridgecli-3.6.3.dev7/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 20:20:13.000000 systembridgecli-3.6.3.dev7/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:20:15.324780 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 20:20:15.000000 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 20:20:15.000000 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:20:15.000000 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 20:20:15.000000 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 20:20:15.000000 systembridgecli-3.6.3.dev7/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-3.6.3.dev6/pyproject.toml` & `systembridgecli-3.6.3.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.6.3.dev6/setup.py` & `systembridgecli-3.6.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.6.3.dev6/systembridgecli/__main__.py` & `systembridgecli-3.6.3.dev7/systembridgecli/__main__.py`

 * *Files identical despite different names*

