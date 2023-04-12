# Comparing `tmp/kt-legacy-1.0.4.tar.gz` & `tmp/kt-legacy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/haifengj/git/kt-legacy/dist/tmpavvdkl0j/kt-legacy-1.0.4.tar", last modified: Tue Aug 10 21:48:21 2021, max compression
+gzip compressed data, was "kt-legacy-1.0.5.tar", last modified: Wed Apr 12 23:01:32 2023, max compression
```

## Comparing `kt-legacy-1.0.4.tar` & `kt-legacy-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/
--rw-r--r--   0 haifengj  (1000) haifengj  (1000)    11357 2021-06-10 19:38:52.000000 kt-legacy-1.0.4/LICENSE
--rw-r--r--   0 haifengj  (1000) haifengj  (1000)      248 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/PKG-INFO
--rw-r--r--   0 haifengj  (1000) haifengj  (1000)      232 2021-06-10 19:38:52.000000 kt-legacy-1.0.4/README.md
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)      200 2021-08-10 21:43:25.000000 kt-legacy-1.0.4/kerastuner/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/applications/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       39 2021-06-11 17:03:53.000000 kt-legacy-1.0.4/kerastuner/applications/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/distribute/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       37 2021-06-11 17:04:14.000000 kt-legacy-1.0.4/kerastuner/distribute/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/engine/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       33 2021-06-11 17:04:36.000000 kt-legacy-1.0.4/kerastuner/engine/__init__.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       44 2021-06-11 21:01:39.000000 kt-legacy-1.0.4/kerastuner/engine/base_tuner.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       44 2021-06-11 21:02:00.000000 kt-legacy-1.0.4/kerastuner/engine/conditions.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       44 2021-06-11 20:58:20.000000 kt-legacy-1.0.4/kerastuner/engine/hypermodel.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       49 2021-06-11 21:00:06.000000 kt-legacy-1.0.4/kerastuner/engine/hyperparameters.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       40 2021-06-11 21:00:33.000000 kt-legacy-1.0.4/kerastuner/engine/logger.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       50 2021-06-11 21:03:26.000000 kt-legacy-1.0.4/kerastuner/engine/metrics_tracking.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       55 2021-06-11 21:04:01.000000 kt-legacy-1.0.4/kerastuner/engine/multi_execution_tuner.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       40 2021-06-11 20:57:22.000000 kt-legacy-1.0.4/kerastuner/engine/oracle.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       42 2021-06-11 21:11:20.000000 kt-legacy-1.0.4/kerastuner/engine/stateful.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       39 2021-06-11 21:11:38.000000 kt-legacy-1.0.4/kerastuner/engine/trial.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       39 2021-06-11 20:57:11.000000 kt-legacy-1.0.4/kerastuner/engine/tuner.py
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       45 2021-06-11 21:11:59.000000 kt-legacy-1.0.4/kerastuner/engine/tuner_utils.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/oracles/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       34 2021-06-11 17:04:57.000000 kt-legacy-1.0.4/kerastuner/oracles/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/protos/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       33 2021-06-11 17:05:22.000000 kt-legacy-1.0.4/kerastuner/protos/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kerastuner/tuners/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       33 2021-06-11 17:05:40.000000 kt-legacy-1.0.4/kerastuner/tuners/__init__.py
-drwxr-xr-x   0 haifengj  (1000) haifengj  (1000)        0 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kt_legacy.egg-info/
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)      248 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kt_legacy.egg-info/PKG-INFO
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)      759 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kt_legacy.egg-info/SOURCES.txt
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)        1 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kt_legacy.egg-info/dependency_links.txt
--rw-rw-r--   0 haifengj  (1000) haifengj  (1000)       11 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/kt_legacy.egg-info/top_level.txt
--rw-r--r--   0 haifengj  (1000) haifengj  (1000)       38 2021-08-10 21:48:21.000000 kt-legacy-1.0.4/setup.cfg
--rw-r--r--   0 haifengj  (1000) haifengj  (1000)      985 2021-08-10 21:45:38.000000 kt-legacy-1.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.738225 kt-legacy-1.0.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      220 2023-04-12 23:01:32.738225 kt-legacy-1.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      232 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.710225 kt-legacy-1.0.5/kerastuner/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      200 2023-04-12 22:58:47.000000 kt-legacy-1.0.5/kerastuner/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.710225 kt-legacy-1.0.5/kerastuner/applications/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/applications/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.710225 kt-legacy-1.0.5/kerastuner/distribute/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       37 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/distribute/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.718225 kt-legacy-1.0.5/kerastuner/engine/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/base_tuner.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/conditions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/hypermodel.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/hyperparameters.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/metrics_tracking.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      154 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/multi_execution_tuner.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/oracle.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/stateful.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/trial.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/tuner.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       45 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/engine/tuner_utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.722225 kt-legacy-1.0.5/kerastuner/oracles/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       34 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/oracles/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.722225 kt-legacy-1.0.5/kerastuner/protos/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/protos/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.722225 kt-legacy-1.0.5/kerastuner/tuners/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-04-12 22:58:00.000000 kt-legacy-1.0.5/kerastuner/tuners/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 23:01:32.734225 kt-legacy-1.0.5/kt_legacy.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      220 2023-04-12 23:01:32.000000 kt-legacy-1.0.5/kt_legacy.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-04-12 23:01:32.000000 kt-legacy-1.0.5/kt_legacy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 23:01:32.000000 kt-legacy-1.0.5/kt_legacy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-04-12 23:01:32.000000 kt-legacy-1.0.5/kt_legacy.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 23:01:32.738225 kt-legacy-1.0.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      985 2023-04-12 22:59:00.000000 kt-legacy-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kt-legacy-1.0.4/LICENSE` & `kt-legacy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kt-legacy-1.0.4/kt_legacy.egg-info/SOURCES.txt` & `kt-legacy-1.0.5/kt_legacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kt-legacy-1.0.4/setup.py` & `kt-legacy-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Setup script."""
 
 from __future__ import absolute_import
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = "1.0.4"
+version = "1.0.5"
 
 setup(
     name="kt-legacy",
     version=version,
     description="Legacy import names for Keras Tuner",
     url="https://github.com/haifeng-jin/kt-legacy",
     author="Haifeng Jin",
```

