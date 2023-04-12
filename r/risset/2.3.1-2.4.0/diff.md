# Comparing `tmp/risset-2.3.1.tar.gz` & `tmp/risset-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.3.1.tar", last modified: Wed Apr 12 23:44:11 2023, max compression
+gzip compressed data, was "risset-2.4.0.tar", last modified: Wed Apr 12 23:58:15 2023, max compression
```

## Comparing `risset-2.3.1.tar` & `risset-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:44:11.933999 risset-2.3.1/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:44:11.933999 risset-2.3.1/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.3.1/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:44:11.933999 risset-2.3.1/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 23:44:11.000000 risset-2.3.1/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107887 2023-04-12 23:43:44.000000 risset-2.3.1/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 23:44:11.933999 risset-2.3.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.3.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:58:15.449814 risset-2.4.0/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:58:15.449814 risset-2.4.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.4.0/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:58:15.448814 risset-2.4.0/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107887 2023-04-12 23:58:06.000000 risset-2.4.0/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 23:58:15.449814 risset-2.4.0/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.0/setup.py
```

### Comparing `risset-2.3.1/PKG-INFO` & `risset-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.3.1
+Version: 2.4.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.3.1/README.md` & `risset-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `risset-2.3.1/risset.egg-info/PKG-INFO` & `risset-2.4.0/risset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.3.1
+Version: 2.4.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.3.1/risset.py` & `risset-2.4.0/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
```

### Comparing `risset-2.3.1/setup.py` & `risset-2.4.0/setup.py`

 * *Files identical despite different names*

