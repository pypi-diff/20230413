# Comparing `tmp/loxprox-0.1.0.tar.gz` & `tmp/loxprox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loxprox-0.1.0.tar", last modified: Thu Apr 13 10:39:38 2023, max compression
+gzip compressed data, was "loxprox-0.1.1.tar", last modified: Thu Apr 13 17:10:27 2023, max compression
```

## Comparing `loxprox-0.1.0.tar` & `loxprox-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 10:39:38.464711 loxprox-0.1.0/
--rw-r--r--   0 kab        (501) staff       (20)     1079 2023-04-12 07:05:30.000000 loxprox-0.1.0/LICENSE
--rw-r--r--   0 kab        (501) staff       (20)      153 2023-04-13 10:39:38.464580 loxprox-0.1.0/PKG-INFO
--rw-r--r--   0 kab        (501) staff       (20)      514 2023-04-13 10:36:15.000000 loxprox-0.1.0/README.md
-drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 10:39:38.463570 loxprox-0.1.0/loxprox/
--rw-r--r--   0 kab        (501) staff       (20)        1 2023-04-12 09:32:30.000000 loxprox-0.1.0/loxprox/__init__.py
--rw-r--r--   0 kab        (501) staff       (20)     2798 2023-04-12 07:05:30.000000 loxprox-0.1.0/loxprox/colors.py
--rw-r--r--   0 kab        (501) staff       (20)      149 2023-04-12 10:53:31.000000 loxprox-0.1.0/loxprox/config.py
--rw-r--r--   0 kab        (501) staff       (20)     1685 2023-04-12 07:05:30.000000 loxprox-0.1.0/loxprox/converter.py
--rw-r--r--   0 kab        (501) staff       (20)     4652 2023-04-12 11:35:41.000000 loxprox-0.1.0/loxprox/main.py
-drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 10:39:38.464404 loxprox-0.1.0/loxprox.egg-info/
--rw-r--r--   0 kab        (501) staff       (20)      153 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/PKG-INFO
--rw-r--r--   0 kab        (501) staff       (20)      307 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/SOURCES.txt
--rw-r--r--   0 kab        (501) staff       (20)        1 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/dependency_links.txt
--rw-r--r--   0 kab        (501) staff       (20)       46 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/entry_points.txt
--rw-r--r--   0 kab        (501) staff       (20)       39 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/requires.txt
--rw-r--r--   0 kab        (501) staff       (20)        8 2023-04-13 10:39:38.000000 loxprox-0.1.0/loxprox.egg-info/top_level.txt
--rw-r--r--   0 kab        (501) staff       (20)       38 2023-04-13 10:39:38.464743 loxprox-0.1.0/setup.cfg
--rw-r--r--   0 kab        (501) staff       (20)      448 2023-04-12 10:05:38.000000 loxprox-0.1.0/setup.py
+drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 17:10:27.519627 loxprox-0.1.1/
+-rwxr-xr-x   0 kab        (501) staff       (20)     1079 2023-04-13 16:41:21.000000 loxprox-0.1.1/LICENSE
+-rw-r--r--   0 kab        (501) staff       (20)      461 2023-04-13 17:10:27.519514 loxprox-0.1.1/PKG-INFO
+-rwxr-xr-x   0 kab        (501) staff       (20)     1318 2023-04-13 17:04:37.000000 loxprox-0.1.1/README.md
+drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 17:10:27.518618 loxprox-0.1.1/loxprox/
+-rwxr-xr-x   0 kab        (501) staff       (20)        1 2023-04-13 16:41:21.000000 loxprox-0.1.1/loxprox/__init__.py
+-rwxr-xr-x   0 kab        (501) staff       (20)     2798 2023-04-13 16:41:21.000000 loxprox-0.1.1/loxprox/colors.py
+-rwxr-xr-x   0 kab        (501) staff       (20)      149 2023-04-13 16:41:21.000000 loxprox-0.1.1/loxprox/config.py
+-rwxr-xr-x   0 kab        (501) staff       (20)     1685 2023-04-13 16:41:21.000000 loxprox-0.1.1/loxprox/converter.py
+-rwxr-xr-x   0 kab        (501) staff       (20)     4652 2023-04-13 16:41:21.000000 loxprox-0.1.1/loxprox/main.py
+drwxr-xr-x   0 kab        (501) staff       (20)        0 2023-04-13 17:10:27.519332 loxprox-0.1.1/loxprox.egg-info/
+-rw-r--r--   0 kab        (501) staff       (20)      461 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/PKG-INFO
+-rw-r--r--   0 kab        (501) staff       (20)      307 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/SOURCES.txt
+-rw-r--r--   0 kab        (501) staff       (20)        1 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/dependency_links.txt
+-rw-r--r--   0 kab        (501) staff       (20)       46 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/entry_points.txt
+-rw-r--r--   0 kab        (501) staff       (20)       39 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/requires.txt
+-rw-r--r--   0 kab        (501) staff       (20)        8 2023-04-13 17:10:27.000000 loxprox-0.1.1/loxprox.egg-info/top_level.txt
+-rw-r--r--   0 kab        (501) staff       (20)       38 2023-04-13 17:10:27.519673 loxprox-0.1.1/setup.cfg
+-rwxr-xr-x   0 kab        (501) staff       (20)      782 2023-04-13 17:10:07.000000 loxprox-0.1.1/setup.py
```

### Comparing `loxprox-0.1.0/LICENSE` & `loxprox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loxprox-0.1.0/loxprox/colors.py` & `loxprox-0.1.1/loxprox/colors.py`

 * *Files identical despite different names*

### Comparing `loxprox-0.1.0/loxprox/converter.py` & `loxprox-0.1.1/loxprox/converter.py`

 * *Files identical despite different names*

### Comparing `loxprox-0.1.0/loxprox/main.py` & `loxprox-0.1.1/loxprox/main.py`

 * *Files identical despite different names*

