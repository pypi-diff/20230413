# Comparing `tmp/hagis-0.1.tar.gz` & `tmp/hagis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.1.tar", last modified: Thu Apr 13 02:51:41 2023, max compression
+gzip compressed data, was "hagis-0.1.1.tar", last modified: Thu Apr 13 11:47:55 2023, max compression
```

## Comparing `hagis-0.1.tar` & `hagis-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:51:41.570726 hagis-0.1/
--rw-rw-rw-   0        0        0      207 2023-04-13 02:51:41.553917 hagis-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-04-12 12:05:00.000000 hagis-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:51:41.526322 hagis-0.1/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 02:48:13.000000 hagis-0.1/hagis/__init__.py
--rw-rw-rw-   0        0        0     8706 2023-04-12 12:19:11.000000 hagis-0.1/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:51:41.553917 hagis-0.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      207 2023-04-13 02:51:41.000000 hagis-0.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-13 02:51:41.000000 hagis-0.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:51:41.000000 hagis-0.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 02:33:39.000000 hagis-0.1/hagis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-13 02:51:41.000000 hagis-0.1/hagis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 02:51:41.000000 hagis-0.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 02:51:41.570726 hagis-0.1/setup.cfg
--rw-rw-rw-   0        0        0      358 2023-04-13 02:48:02.000000 hagis-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.259671 hagis-0.1.1/
+-rw-rw-rw-   0        0        0      958 2023-04-13 11:47:55.245970 hagis-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-13 11:35:45.000000 hagis-0.1.1/README.md
+-rw-rw-rw-   0        0        0      589 2023-04-13 11:44:46.000000 hagis-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:47:55.259671 hagis-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.178067 hagis-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.211055 hagis-0.1.1/src/hagis/
+-rw-rw-rw-   0        0        0        0 2023-04-13 11:39:40.000000 hagis-0.1.1/src/hagis/__init__.py
+-rw-rw-rw-   0        0        0     8706 2023-04-12 12:19:11.000000 hagis-0.1.1/src/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:47:55.245970 hagis-0.1.1/src/hagis.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 11:47:55.000000 hagis-0.1.1/src/hagis.egg-info/top_level.txt
```

### Comparing `hagis-0.1/hagis/hagis.py` & `hagis-0.1.1/src/hagis/hagis.py`

 * *Files identical despite different names*

