# Comparing `tmp/bazingo-0.0.1.tar.gz` & `tmp/bazingo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bazingo-0.0.1.tar", last modified: Thu Apr 13 00:27:10 2023, max compression
+gzip compressed data, was "bazingo-0.0.2.tar", last modified: Thu Apr 13 00:27:59 2023, max compression
```

## Comparing `bazingo-0.0.1.tar` & `bazingo-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:10.241472 bazingo-0.0.1/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      627 2023-04-13 00:27:10.241223 bazingo-0.0.1/PKG-INFO
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:10.239928 bazingo-0.0.1/bazingo/
--rw-r--r--   0 joshyacktman   (501) staff       (20)       28 2023-04-13 00:23:36.000000 bazingo-0.0.1/bazingo/__init__.py
--rw-r--r--   0 joshyacktman   (501) staff       (20)       23 2023-04-13 00:23:11.000000 bazingo-0.0.1/bazingo/bazingo.py
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:10.240911 bazingo-0.0.1/bazingo.egg-info/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      627 2023-04-13 00:27:10.000000 bazingo-0.0.1/bazingo.egg-info/PKG-INFO
--rw-r--r--   0 joshyacktman   (501) staff       (20)      171 2023-04-13 00:27:10.000000 bazingo-0.0.1/bazingo.egg-info/SOURCES.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)        1 2023-04-13 00:27:10.000000 bazingo-0.0.1/bazingo.egg-info/dependency_links.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)        8 2023-04-13 00:27:10.000000 bazingo-0.0.1/bazingo.egg-info/top_level.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-13 00:27:10.241535 bazingo-0.0.1/setup.cfg
--rw-r--r--   0 joshyacktman   (501) staff       (20)      437 2023-04-13 00:17:29.000000 bazingo-0.0.1/setup.py
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:59.312835 bazingo-0.0.2/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      627 2023-04-13 00:27:59.312586 bazingo-0.0.2/PKG-INFO
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      392 2023-04-13 00:27:34.000000 bazingo-0.0.2/README.md
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:59.311251 bazingo-0.0.2/bazingo/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       28 2023-04-13 00:23:36.000000 bazingo-0.0.2/bazingo/__init__.py
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       23 2023-04-13 00:23:11.000000 bazingo-0.0.2/bazingo/bazingo.py
+drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-13 00:27:59.312226 bazingo-0.0.2/bazingo.egg-info/
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      627 2023-04-13 00:27:59.000000 bazingo-0.0.2/bazingo.egg-info/PKG-INFO
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      181 2023-04-13 00:27:59.000000 bazingo-0.0.2/bazingo.egg-info/SOURCES.txt
+-rw-r--r--   0 joshyacktman   (501) staff       (20)        1 2023-04-13 00:27:59.000000 bazingo-0.0.2/bazingo.egg-info/dependency_links.txt
+-rw-r--r--   0 joshyacktman   (501) staff       (20)        8 2023-04-13 00:27:59.000000 bazingo-0.0.2/bazingo.egg-info/top_level.txt
+-rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-13 00:27:59.312898 bazingo-0.0.2/setup.cfg
+-rw-r--r--   0 joshyacktman   (501) staff       (20)      437 2023-04-13 00:27:37.000000 bazingo-0.0.2/setup.py
```

### Comparing `bazingo-0.0.1/PKG-INFO` & `bazingo-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bazingo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A `Notebook` replacement for tkinter
 Home-page: https://github.com/Moosems/bazingo
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# Bazingo 0.0.1
+# Bazingo 0.0.2
 
 Bazingo aims to replace the conventional `Notebook` widget with a less buggy and more customizable alternative.
 
 The following is planned to be implemented:
 - [ ] Put custom widgets to tabbar -->
 - [ ] Tabs can have a close button and an icon at the same time
 - [ ] Tabs can be pinned
```

### Comparing `bazingo-0.0.1/bazingo.egg-info/PKG-INFO` & `bazingo-0.0.2/bazingo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bazingo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A `Notebook` replacement for tkinter
 Home-page: https://github.com/Moosems/bazingo
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# Bazingo 0.0.1
+# Bazingo 0.0.2
 
 Bazingo aims to replace the conventional `Notebook` widget with a less buggy and more customizable alternative.
 
 The following is planned to be implemented:
 - [ ] Put custom widgets to tabbar -->
 - [ ] Tabs can have a close button and an icon at the same time
 - [ ] Tabs can be pinned
```

