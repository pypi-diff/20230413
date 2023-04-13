# Comparing `tmp/graphal-1.0.0.tar.gz` & `tmp/graphal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphal-1.0.0.tar", last modified: Thu Apr 13 17:52:27 2023, max compression
+gzip compressed data, was "graphal-1.0.1.tar", last modified: Thu Apr 13 21:44:05 2023, max compression
```

## Comparing `graphal-1.0.0.tar` & `graphal-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:52:26.779660 graphal-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-04-13 17:41:21.000000 graphal-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      359 2023-04-13 17:52:26.908638 graphal-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-13 17:51:12.000000 graphal-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:52:25.614884 graphal-1.0.0/graphal/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:25:59.000000 graphal-1.0.0/graphal/__init__.py
--rw-rw-rw-   0        0        0      259 2023-04-13 17:45:38.000000 graphal-1.0.0/graphal/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:52:26.718660 graphal-1.0.0/graphal.egg-info/
--rw-rw-rw-   0        0        0      359 2023-04-13 17:52:24.000000 graphal-1.0.0/graphal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-13 17:52:24.000000 graphal-1.0.0/graphal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:52:24.000000 graphal-1.0.0/graphal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 17:52:24.000000 graphal-1.0.0/graphal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 17:52:24.000000 graphal-1.0.0/graphal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:52:27.052519 graphal-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-04-13 17:39:24.000000 graphal-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:44:05.944999 graphal-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-04-13 17:41:21.000000 graphal-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      326 2023-04-13 21:44:05.946147 graphal-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-13 17:51:12.000000 graphal-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 21:44:05.910212 graphal-1.0.1/graphal/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:25:59.000000 graphal-1.0.1/graphal/__init__.py
+-rw-rw-rw-   0        0        0     2817 2023-04-13 21:27:22.000000 graphal-1.0.1/graphal/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:44:05.941968 graphal-1.0.1/graphal.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-04-13 21:44:05.000000 graphal-1.0.1/graphal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-13 21:44:05.000000 graphal-1.0.1/graphal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 21:44:05.000000 graphal-1.0.1/graphal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 21:44:05.000000 graphal-1.0.1/graphal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 21:44:05.000000 graphal-1.0.1/graphal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 21:44:05.949553 graphal-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-04-13 21:44:00.000000 graphal-1.0.1/setup.py
```

### Comparing `graphal-1.0.0/LICENSE` & `graphal-1.0.1/LICENSE`

 * *Files identical despite different names*

